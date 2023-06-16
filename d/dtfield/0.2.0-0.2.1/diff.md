# Comparing `tmp/dtfield-0.2.0.tar.gz` & `tmp/dtfield-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.2.0.tar", max compression
+gzip compressed data, was "dtfield-0.2.1.tar", max compression
```

## Comparing `dtfield-0.2.0.tar` & `dtfield-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.2.0/dtfield/__init__.py
--rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.2.0/dtfield/_imports.py
--rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.2.0/dtfield/base_enum.py
--rw-r--r--   0        0        0    22624 2023-06-14 00:41:24.943418 dtfield-0.2.0/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.2.0/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.2.0/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.2.0/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.2.0/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.2.0/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.2.0/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.2.0/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.2.0/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.2.0/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.2.0/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.2.0/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.2.0/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.2.0/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.2.0/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.2.0/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.2.0/dtfield/parse/string.py
--rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.2.0/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      387 2023-06-14 00:41:24.955878 dtfield-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      715 2023-06-14 00:41:32.063553 dtfield-0.2.0/setup.py
--rw-r--r--   0        0        0      503 2023-06-14 00:41:32.063788 dtfield-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.2.1/dtfield/__init__.py
+-rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.2.1/dtfield/_imports.py
+-rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.2.1/dtfield/base_enum.py
+-rw-r--r--   0        0        0    23608 2023-06-16 23:43:38.638846 dtfield-0.2.1/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.2.1/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.2.1/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.2.1/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.2.1/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.2.1/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.2.1/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.2.1/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.2.1/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.2.1/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.2.1/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.2.1/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.2.1/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.2.1/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.2.1/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.2.1/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.2.1/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.2.1/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      457 2023-06-16 23:43:54.904891 dtfield-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      806 2023-06-16 23:44:01.126830 dtfield-0.2.1/setup.py
+-rw-r--r--   0        0        0      636 2023-06-16 23:44:01.127222 dtfield-0.2.1/PKG-INFO
```

### Comparing `dtfield-0.2.0/dtfield/_imports.py` & `dtfield-0.2.1/dtfield/_imports.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/base_enum.py` & `dtfield-0.2.1/dtfield/base_enum.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/engine.py` & `dtfield-0.2.1/dtfield/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,29 @@
         'filter_dict',
         'make_dict',
         'dict_items',
         'normalize_lower_if_string',
         'exclude_keys_from_dict'
 ]
 
+import os.path
 
 from deta.base import FetchResponse
+from starlette.templating import Jinja2Templates
 from dtfield._imports import *
 from dtbase import *
 from .parse import *
 from .functions import *
 
+try:
+    TEMPLATES: Jinja2Templates = Jinja2Templates(directory=os.path.join(os.getcwd(), 'templates'))
+except:
+    TEMPLATES: Jinja2Templates
+
+
 
 context = copy_context()
 
 
 def exclude_keys_from_dict(data: Mapping, exclude: list[str]):
     return {k: v for k, v in data.items() if not k in exclude}
 
@@ -248,15 +256,15 @@
         else:
             return None
         
     async def update_instance(self, **kwargs):
         current = self.asjson()
         current.update(exclude_keys_from_dict(kwargs, exclude=['key']))
         key = current.pop('key')
-        updated = await DetaBase(self.table()).put(data=current, key=key)
+        await DetaBase(self.table()).put(data=current, key=key)
         await self.update_context()
         return self.from_context(key)
         
     
     @classmethod
     def singular(cls):
         return cls.SINGULAR or cls.clsname()
@@ -316,24 +324,48 @@
             for item in cls.model_dependants():
                 tks.start_soon(item.set_context)
                 
     def __lt__(self, other):
         return normalize_lower(str(self)) < normalize_lower(str(other))
     
     @classmethod
-    def instances_list(cls) -> list[Self]:
+    async def instances_list(cls) -> list[Self]:
+        await cls.update_context()
         return [cls.from_context(i) for i in cls.get_context().keys()]
     
     @classmethod
-    def sorted_instances_list(cls) -> list[Self]:
-        return sorted(cls.instances_list())
+    async def sorted_instances_list(cls) -> list[Self]:
+        return sorted(await cls.instances_list())
+    
+    @classmethod
+    async def ordered_instances_list(cls) -> list[Self]:
+        return ordered(await cls.instances_list())
     
     @classmethod
-    def ordered_instances_list(cls) -> list[Self]:
-        return ordered(cls.instances_list())
+    async def html_list(cls, request: Request):
+        return TEMPLATES.TemplateResponse(
+                'partial/instances_list.jj',
+                {
+                        'request': request,
+                        'instances': await cls.sorted_instances_list(),
+                        'model': cls
+                }
+        )
+    
+    @classmethod
+    async def html_datalist(cls, request: Request):
+        return TEMPLATES.TemplateResponse(
+                'partial/datalist.jj',
+                {
+                        'request': request,
+                        'instances': await cls.sorted_instances_list(),
+                        'model': cls
+                }
+        )
+        
     
 
 def model_dependants(obj: type[ContextBase], collection: list = None):
     collection = collection or list()
     for item in obj.dependant_descriptors().values():
         models = item.dependants
         for model in models:
@@ -350,15 +382,14 @@
 
 def context_model(cls: type[ContextBase]):
     @wraps(cls)
     def wrapper():
         cls.CTXVAR = ContextVar(f'{cls.__name__}Var')
         cls.__repr__ = partialmethod(repr_func)
         cls.__eq__ = partialmethod(eq_function)
-
         ModelMap[cls.__name__] = cls
         return cls
     
     return wrapper()
 
 
 class BaseDescriptor:
```

### Comparing `dtfield-0.2.0/dtfield/functions.py` & `dtfield-0.2.1/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.2.1/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.2.1/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.2.1/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.2.1/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.2.1/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtfield-0.2.1/dtfield/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/dates.py` & `dtfield-0.2.1/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/json_encoder.py` & `dtfield-0.2.1/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/number.py` & `dtfield-0.2.1/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/string.py` & `dtfield-0.2.1/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/dtfield/parse/type_hint.py` & `dtfield-0.2.1/dtfield/parse/type_hint.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.0/setup.py` & `dtfield-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 packages = \
 ['dtfield', 'dtfield.parse']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Unidecode>=1.3.6,<2.0.0',
+['Jinja2>=3.1.2,<4.0.0',
+ 'Unidecode>=1.3.6,<2.0.0',
  'anyio>=3.7.0,<4.0.0',
  'dtbase>=0.0.4,<0.0.5',
+ 'itsdangerous>=2.1.2,<3.0.0',
+ 'python-multipart>=0.0.6,<0.0.7',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

