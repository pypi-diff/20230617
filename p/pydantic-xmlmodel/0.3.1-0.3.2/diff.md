# Comparing `tmp/pydantic_xmlmodel-0.3.1.tar.gz` & `tmp/pydantic_xmlmodel-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xmlmodel-0.3.1.tar", max compression
+gzip compressed data, was "pydantic_xmlmodel-0.3.2.tar", max compression
```

## Comparing `pydantic_xmlmodel-0.3.1.tar` & `pydantic_xmlmodel-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.3.1/LICENSE
--rw-r--r--   0        0        0     2174 2023-06-14 18:50:15.256988 pydantic_xmlmodel-0.3.1/README.md
--rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.3.1/pydantic_xmlmodel/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.3.1/pydantic_xmlmodel/py.typed
--rw-r--r--   0        0        0    14379 2023-06-14 19:01:31.733595 pydantic_xmlmodel-0.3.1/pydantic_xmlmodel/xmlmodel.py
--rw-r--r--   0        0        0      613 2023-06-14 19:02:45.363532 pydantic_xmlmodel-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-17 13:32:22.273043 pydantic_xmlmodel-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2190 2023-06-15 14:01:43.476858 pydantic_xmlmodel-0.3.2/README.md
+-rw-r--r--   0        0        0       55 2023-05-17 13:44:08.514440 pydantic_xmlmodel-0.3.2/pydantic_xmlmodel/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 08:52:39.775359 pydantic_xmlmodel-0.3.2/pydantic_xmlmodel/py.typed
+-rw-r--r--   0        0        0    14980 2023-06-17 20:27:41.893387 pydantic_xmlmodel-0.3.2/pydantic_xmlmodel/xmlmodel.py
+-rw-r--r--   0        0        0      613 2023-06-17 20:28:05.134691 pydantic_xmlmodel-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2934 1970-01-01 00:00:00.000000 pydantic_xmlmodel-0.3.2/PKG-INFO
```

### Comparing `pydantic_xmlmodel-0.3.1/LICENSE` & `pydantic_xmlmodel-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xmlmodel-0.3.1/README.md` & `pydantic_xmlmodel-0.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 - Convert Pydantic models to XML and vice versa
 - Support for XML attributes, elements, content, **lists**.
 - Compatible with most Pydantic features (e.g. default values, validators, `Field` etc.)
 - Very easy to use. Extends Pydantic's API with only a few methods.
 - Has no dependencies other than Pydantic
 - Have a good docs in the source code
-- Fully tested
+- Fully tested (100% coverage)
 
 ## Installation
 
 You can install PydanticXML with pip:
 
 ```bash
 pip install pydantic-xmlmodel
```

### Comparing `pydantic_xmlmodel-0.3.1/pydantic_xmlmodel/xmlmodel.py` & `pydantic_xmlmodel-0.3.2/pydantic_xmlmodel/xmlmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 """A module that contains the XMLModel class."""
 
-from typing import Any, Callable, Dict, Optional, Type, TypeVar, no_type_check
+from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, no_type_check
 from xml.dom.minidom import parseString
 from xml.etree.ElementTree import Element, SubElement, fromstring, tostring
 
 from pydantic import BaseModel
+from pydantic.fields import ModelField
 from pydantic.main import ModelMetaclass
 
 T = TypeVar("T", bound="XMLModel")
 
 
+def _issubclass_safe(cls: Any, classinfo: Any) -> bool:
+    """Safe version of issubclass that doesn't raise an exception if the first argument is not a class."""
+    try:
+        return issubclass(cls, classinfo)
+    except TypeError:
+        return False
+
+
 class XMLModelMeta(ModelMetaclass):
     """A metaclass for XMLModel.
 
     It's a subclass of `ModelMetaclass` (the metaclass of `pydantic.BaseModel`).
 
     It adds the following class attributes to XMLModel:
         - `__xml_name__`: The name of the XML element. If not specified, the name of the class is used.
     """
 
-    @no_type_check
     def __new__(cls, name, bases, attrs, **kwargs):
         """Add the following class attributes to XMLModel.
 
         - xml_name: The name of the XML element. If not specified, the name of the class is used.
         """
         xml_name = kwargs.pop("xml_name", None)
         if xml_name is not None:
@@ -119,26 +127,31 @@
             for field, _ in obj.dict().items():
                 # We skip the xml_content field because we handle it separately
                 if field == "xml_content":
                     continue
                 # We get the value of the field using getattr() because the we need subclass of BaseModel, not just dict
                 value = getattr(obj, field)
                 # If the value is a BaseModel, we convert it to XML recursively
-                if isinstance(value, BaseModel):
+                if (
+                    _issubclass_safe(obj.__fields__[field].type_, BaseModel)
+                    and obj.__fields__[field].sub_fields is None
+                ):
+                    if obj.__fields__[field].allow_none and value is None:
+                        continue
                     # Get the name of the XML element
                     name = value.__class__.__name__
                     if isinstance(value, XMLModel):
                         name = value._get_xml_name()
                     # Create the XML element and add it to the parent element
                     sub = SubElement(e, name)
                     # Convert the BaseModel to XML recursively
                     to_xml_innner(sub, value)
                 elif obj.__fields__[field].sub_fields is not None:
                     # If the field is a list-like field but not a list of BaseModel, we raise an error
-                    if not issubclass(
+                    if not _issubclass_safe(
                         obj.__fields__[field].sub_fields[0].type_, BaseModel
                     ):
                         raise ValueError(
                             f"Field {field} is a list-like field but not a list of BaseModel"
                         )
                     # Iterate over the list and convert each item to XML recursively
                     for item in value:
@@ -160,26 +173,25 @@
                         name = pydantic_field.alias
                     # Add the attribute to the XML element
                     e.set(name, str(value))
             # If the model has content, we add it to the XML element
             if isinstance(obj, XMLModel) and obj.xml_content is not None:
                 xml_content_field = obj.__fields__["xml_content"]
                 # if field is a list-like field but not a list of BaseModel, we raise an error
-                if xml_content_field.sub_fields is not None and not issubclass(
+                if xml_content_field.sub_fields is not None and not _issubclass_safe(
                     xml_content_field.sub_fields[0].type_, BaseModel
                 ):
                     raise ValueError(
-                        f"xml_content field of {obj.__class__.__name__} must be a List[BaseModel] "
-                        f"but got {xml_content_field.sub_fields[0].type_.__name__}"
+                        f"xml_content field of {obj.__class__.__name__} must be a List[BaseModel]"
                     )
                 # if field is a list-like field, we add each item as a separate XML element
                 if xml_content_field.sub_fields is not None:
                     type_ = xml_content_field.sub_fields[0].type_
                     name = type_.__name__
-                    if issubclass(type_, XMLModel):
+                    if _issubclass_safe(type_, XMLModel):
                         name = type_._get_xml_name()
                     for item in obj.xml_content:
                         sub = SubElement(e, name)
                         to_xml_innner(sub, item)
                 # else, we add the content as a text
                 else:
                     e.text = str(obj.xml_content)
@@ -237,85 +249,87 @@
         """
 
         def from_element(element: Element, model: Type[BaseModel]) -> Any:
             data: Dict[str, Any] = {}
             for field in model.__fields__:
                 if field == "xml_content":
                     continue
-                field_type = model.__annotations__[field]
-                is_list_like = model.__fields__[field].sub_fields is not None
+                field_type = model.__fields__[field].type_
+                is_list_like = False
+                # mypy doesn't understand that sub_fields is not None if is_list_like is True
+                # so we use a typing and "or []" to tell mypy that sub_fields is not None
+                sub_fields: List[ModelField] = model.__fields__[field].sub_fields or []
+                if sub_fields:
+                    is_list_like = True
                 if is_list_like:
-                    sub_fields = model.__fields__[field].sub_fields
-                    if not sub_fields:
-                        raise ValueError(
-                            f"Field {field} is a list-like field but it's empty"
-                        )
                     type_ = sub_fields[0].type_
-                    field_info = sub_fields[0].field_info
-                    if not issubclass(type_, BaseModel):
+                    # See below for the explanation of this comment
+                    # field_info = sub_fields[0].field_info
+                    if not _issubclass_safe(type_, BaseModel):
                         raise ValueError(
                             f"Field {field} is a list-like field but not a list of BaseModel"
                         )
-                    if issubclass(type_, XMLModel):
+                    if _issubclass_safe(type_, XMLModel):
                         xml_name = type_._get_xml_name()
-                    else:
-                        xml_name = field_info.extra.get("__xml_name__")
-                elif issubclass(field_type, XMLModel):
+                    # This is needed if we load a model with BaseModel
+                    # But at the moment, it's not possible to load a model with BaseModel
+                    # So we comment this part
+                    # else:
+                    #     xml_name = field_info.extra.get("__xml_name__")
+                elif _issubclass_safe(field_type, XMLModel):
                     xml_name = field_type._get_xml_name()
                 else:
                     xml_name = (
                         model.__fields__[field].field_info.extra.get("__xml_name__")
                         or model.__fields__[field].alias
                     )
 
                 # Get the value of the field
-                if xml_name in element.attrib and not issubclass(field_type, BaseModel):
+                if xml_name in element.attrib and not _issubclass_safe(
+                    field_type, BaseModel
+                ):
                     data[xml_name] = element.attrib[xml_name]
                 # If the field is a list-like field, we convert each XML element to a BaseModel
                 elif is_list_like:
                     data[field] = []
                     for child in element.findall(xml_name):
                         data[field].append(from_element(child, type_))
                 # If the field is a subelement, we convert it to XML recursively
                 else:
                     child_find = element.find(xml_name)
                     if child_find is not None:
-                        if issubclass(field_type, BaseModel):
+                        if _issubclass_safe(field_type, BaseModel):
                             data[field] = from_element(child_find, field_type)
-                        else:
-                            data[field] = child_find.text or ""
 
             # Handle the xml_content field
             # Set the content of the XML element
-            xml_content_meta = model.__fields__.get("xml_content")
+            xml_content_meta = model.__fields__["xml_content"]
             xml_content_data: Any
             # if the field is a list-like field, we add each item as a separate XML element
             if xml_content_meta is not None and xml_content_meta.sub_fields is not None:
-                if not issubclass(xml_content_meta.sub_fields[0].type_, BaseModel):
+                if not _issubclass_safe(
+                    xml_content_meta.sub_fields[0].type_, BaseModel
+                ):
                     raise ValueError(
-                        f"xml_content field of {model.__name__} must be a List[BaseModel] "
-                        f"but got {xml_content_meta.sub_fields[0].type_.__name__}"
+                        f"xml_content field of {model.__name__} must be a List[BaseModel]"
                     )
                 xml_content_data = []
                 name = xml_content_meta.sub_fields[0].type_.__name__
-                if issubclass(xml_content_meta.sub_fields[0].type_, XMLModel):
+                if _issubclass_safe(xml_content_meta.sub_fields[0].type_, XMLModel):
                     name = xml_content_meta.sub_fields[0].type_._get_xml_name()
                 for child in element:
                     if child.tag != name:
                         continue
                     xml_content_data.append(
                         from_element(child, xml_content_meta.sub_fields[0].type_)
                     )
             # else, we add the content as a text
             else:
                 xml_content_data = element.text or ""
-            if xml_content_meta is not None:
-                data[xml_content_meta.alias] = xml_content_data
-            else:
-                data["xml_content"] = xml_content_data
+            data[xml_content_meta.alias] = xml_content_data
 
             # Convert the data to the model
             out = model(**data)
 
             return out
 
         root = fromstring(xml)
```

### Comparing `pydantic_xmlmodel-0.3.1/pyproject.toml` & `pydantic_xmlmodel-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xmlmodel"
-version = "0.3.1"
+version = "0.3.2"
 description = "PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa."
 authors = ["cofob <cofob@riseup.net>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/cofob/pydanticxml"
 homepage = "https://github.com/cofob/pydanticxml"
```

### Comparing `pydantic_xmlmodel-0.3.1/PKG-INFO` & `pydantic_xmlmodel-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xmlmodel
-Version: 0.3.1
+Version: 0.3.2
 Summary: PydanticXML is a Python library that provides a way to convert Pydantic models to XML and vice versa.
 Home-page: https://github.com/cofob/pydanticxml
 License: MIT
 Author: cofob
 Author-email: cofob@riseup.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -25,15 +25,15 @@
 
 - Convert Pydantic models to XML and vice versa
 - Support for XML attributes, elements, content, **lists**.
 - Compatible with most Pydantic features (e.g. default values, validators, `Field` etc.)
 - Very easy to use. Extends Pydantic's API with only a few methods.
 - Has no dependencies other than Pydantic
 - Have a good docs in the source code
-- Fully tested
+- Fully tested (100% coverage)
 
 ## Installation
 
 You can install PydanticXML with pip:
 
 ```bash
 pip install pydantic-xmlmodel
```

