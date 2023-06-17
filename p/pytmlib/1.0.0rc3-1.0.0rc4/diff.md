# Comparing `tmp/pytmlib-1.0.0rc3.tar.gz` & `tmp/pytmlib-1.0.0rc4.tar.gz`

## Comparing `pytmlib-1.0.0rc3.tar` & `pytmlib-1.0.0rc4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/abstract_exercise.py
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/api.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/archiver.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/context.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/create_app.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/handle_error.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/latex.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/method_call_exception.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/serializer.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/abstract.py
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/builder.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/button.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/field.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/field_attribute.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/field_type_enum.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/figure.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/image.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/option.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/option_group.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/paragraph.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/table.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pytmlib/output/table_cell.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/README.md
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/pyproject.toml
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc3/PKG-INFO
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/abstract_exercise.py
+-rw-r--r--   0        0        0     4852 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/api.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/archiver.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/context.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/create_app.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/handle_error.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/latex.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/method_call_exception.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/serializer.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/abstract.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/builder.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/button.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/field.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/field_attribute.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/field_type_enum.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/figure.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/image.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/option.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/option_group.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/paragraph.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/table.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pytmlib/output/table_cell.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/README.md
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc4/PKG-INFO
```

### Comparing `pytmlib-1.0.0rc3/pytmlib/abstract_exercise.py` & `pytmlib-1.0.0rc4/pytmlib/abstract_exercise.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/api.py` & `pytmlib-1.0.0rc4/pytmlib/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,31 +79,31 @@
         method_signature: Signature = signature(method)
         available_arguments: dict = envelop.pop('payload')
         additional_parameters: dict = self._get_additional_parameters(envelop)
         arguments: dict = {}
 
         for key in method_signature.parameters.keys():
             parameter: Parameter = method_signature.parameters[key]
-            self._apply_argument(parameter, arguments, available_arguments)
+            self._apply_argument(parameter, arguments, available_arguments, additional_parameters)
 
         return self._call_method(method, **arguments, **additional_parameters)
 
     def _get_additional_parameters(self, envelop: dict) -> dict:
         additional_parameters: dict = envelop.pop(ButtonOutput.PARAMETERS_FIELD)
         parameters_signature: str = additional_parameters.pop(ButtonOutput.SIGNATURE_FIELD)
         encoded_parameters: str = additional_parameters.pop(ButtonOutput.DATA_FIELD)
 
         return self._context.serializer.deserialize(parameters_signature, encoded_parameters)
 
     @staticmethod
-    def _apply_argument(parameter: Parameter, arguments: dict, available_arguments: dict):
+    def _apply_argument(parameter: Parameter, arguments: dict, available_arguments: dict, additional_parameters: dict):
         name: str = parameter.name
         is_positional_or_keyword: bool = parameter.kind is Parameter.POSITIONAL_OR_KEYWORD
         is_empty_default: bool = parameter.default is Parameter.empty
-        is_argument_available: bool = name in available_arguments
+        is_argument_available: bool = name in available_arguments or name in additional_parameters
 
         # ignore not present arguments with default value
         if is_positional_or_keyword and not is_empty_default and not is_argument_available:
             return
 
         # raise error on required arguments
         if is_positional_or_keyword and is_empty_default and not is_argument_available:
```

### Comparing `pytmlib-1.0.0rc3/pytmlib/archiver.py` & `pytmlib-1.0.0rc4/pytmlib/archiver.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/context.py` & `pytmlib-1.0.0rc4/pytmlib/context.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/create_app.py` & `pytmlib-1.0.0rc4/pytmlib/create_app.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/handle_error.py` & `pytmlib-1.0.0rc4/pytmlib/handle_error.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/serializer.py` & `pytmlib-1.0.0rc4/pytmlib/serializer.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/abstract.py` & `pytmlib-1.0.0rc4/pytmlib/output/abstract.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/builder.py` & `pytmlib-1.0.0rc4/pytmlib/output/builder.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/button.py` & `pytmlib-1.0.0rc4/pytmlib/output/button.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/field.py` & `pytmlib-1.0.0rc4/pytmlib/output/field.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/figure.py` & `pytmlib-1.0.0rc4/pytmlib/output/figure.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/image.py` & `pytmlib-1.0.0rc4/pytmlib/output/image.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/option.py` & `pytmlib-1.0.0rc4/pytmlib/output/option.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/option_group.py` & `pytmlib-1.0.0rc4/pytmlib/output/option_group.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/paragraph.py` & `pytmlib-1.0.0rc4/pytmlib/output/paragraph.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/table.py` & `pytmlib-1.0.0rc4/pytmlib/output/table.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pytmlib/output/table_cell.py` & `pytmlib-1.0.0rc4/pytmlib/output/table_cell.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/LICENSE` & `pytmlib-1.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc3/pyproject.toml` & `pytmlib-1.0.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytmlib"
-version = "1.0.0rc3"
+version = "1.0.0rc4"
 authors = [
     { name = "Oliver Fabel", email = "oliver.fabel@fhnw.ch" },
 ]
 description = "This is the base library for the Python Tool Manager."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `pytmlib-1.0.0rc3/PKG-INFO` & `pytmlib-1.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmlib
-Version: 1.0.0rc3
+Version: 1.0.0rc4
 Summary: This is the base library for the Python Tool Manager.
 Project-URL: Homepage, https://github.com/ofabel/pytm-bootstrap
 Project-URL: Bug Tracker, https://github.com/ofabel/pytm-bootstrap/issues
 Project-URL: Changelog, https://github.com/ofabel/pytm-bootstrap/blob/main/CHANGELOG.md
 Author-email: Oliver Fabel <oliver.fabel@fhnw.ch>
 License: MIT License
```

