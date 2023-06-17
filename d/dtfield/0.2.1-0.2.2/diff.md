# Comparing `tmp/dtfield-0.2.1.tar.gz` & `tmp/dtfield-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtfield-0.2.1.tar", max compression
+gzip compressed data, was "dtfield-0.2.2.tar", max compression
```

## Comparing `dtfield-0.2.1.tar` & `dtfield-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.2.1/dtfield/__init__.py
--rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.2.1/dtfield/_imports.py
--rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.2.1/dtfield/base_enum.py
--rw-r--r--   0        0        0    23608 2023-06-16 23:43:38.638846 dtfield-0.2.1/dtfield/engine.py
--rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.2.1/dtfield/functions.py
--rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.2.1/dtfield/parse/__init__.py
--rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.2.1/dtfield/parse/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.2.1/dtfield/parse/__pycache__/_types.cpython-39.pyc
--rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.2.1/dtfield/parse/__pycache__/dates.cpython-39.pyc
--rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.2.1/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
--rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.2.1/dtfield/parse/__pycache__/null.cpython-39.pyc
--rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.2.1/dtfield/parse/__pycache__/number.cpython-39.pyc
--rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.2.1/dtfield/parse/__pycache__/string.cpython-39.pyc
--rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.2.1/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
--rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.2.1/dtfield/parse/_types.py
--rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.2.1/dtfield/parse/dates.py
--rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.2.1/dtfield/parse/json_encoder.py
--rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.2.1/dtfield/parse/null.py
--rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.2.1/dtfield/parse/number.py
--rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.2.1/dtfield/parse/string.py
--rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.2.1/dtfield/parse/type_hint.py
--rw-r--r--   0        0        0      457 2023-06-16 23:43:54.904891 dtfield-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      806 2023-06-16 23:44:01.126830 dtfield-0.2.1/setup.py
--rw-r--r--   0        0        0      636 2023-06-16 23:44:01.127222 dtfield-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-12 03:54:19.665800 dtfield-0.2.2/dtfield/__init__.py
+-rw-r--r--   0        0        0     2014 2023-06-12 14:04:46.335668 dtfield-0.2.2/dtfield/_imports.py
+-rw-r--r--   0        0        0     1389 2023-06-12 03:54:59.665860 dtfield-0.2.2/dtfield/base_enum.py
+-rw-r--r--   0        0        0    23631 2023-06-17 00:02:42.064522 dtfield-0.2.2/dtfield/engine.py
+-rw-r--r--   0        0        0     2526 2023-06-12 01:02:37.187182 dtfield-0.2.2/dtfield/functions.py
+-rw-r--r--   0        0        0      159 2023-06-11 22:28:46.644614 dtfield-0.2.2/dtfield/parse/__init__.py
+-rw-r--r--   0        0        0      340 2023-06-11 22:28:46.790548 dtfield-0.2.2/dtfield/parse/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      443 2023-06-11 22:28:46.791054 dtfield-0.2.2/dtfield/parse/__pycache__/_types.cpython-39.pyc
+-rw-r--r--   0        0        0      777 2023-06-11 19:47:04.574010 dtfield-0.2.2/dtfield/parse/__pycache__/dates.cpython-39.pyc
+-rw-r--r--   0        0        0     1728 2023-06-11 22:26:00.687944 dtfield-0.2.2/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc
+-rw-r--r--   0        0        0      526 2023-06-11 19:47:01.431654 dtfield-0.2.2/dtfield/parse/__pycache__/null.cpython-39.pyc
+-rw-r--r--   0        0        0     1280 2023-06-11 19:47:04.492588 dtfield-0.2.2/dtfield/parse/__pycache__/number.cpython-39.pyc
+-rw-r--r--   0        0        0      802 2023-06-11 19:47:04.487489 dtfield-0.2.2/dtfield/parse/__pycache__/string.cpython-39.pyc
+-rw-r--r--   0        0        0    11644 2023-06-12 05:40:54.569591 dtfield-0.2.2/dtfield/parse/__pycache__/type_hint.cpython-39.pyc
+-rw-r--r--   0        0        0      321 2023-06-11 22:28:46.640186 dtfield-0.2.2/dtfield/parse/_types.py
+-rw-r--r--   0        0        0      694 2023-06-11 02:28:20.159802 dtfield-0.2.2/dtfield/parse/dates.py
+-rw-r--r--   0        0        0     1543 2023-06-11 22:26:00.531404 dtfield-0.2.2/dtfield/parse/json_encoder.py
+-rw-r--r--   0        0        0      346 2023-06-11 02:36:40.384030 dtfield-0.2.2/dtfield/parse/null.py
+-rw-r--r--   0        0        0     1260 2023-06-11 02:29:46.320272 dtfield-0.2.2/dtfield/parse/number.py
+-rw-r--r--   0        0        0      627 2023-06-11 02:34:21.462547 dtfield-0.2.2/dtfield/parse/string.py
+-rw-r--r--   0        0        0    10839 2023-06-12 04:07:43.884069 dtfield-0.2.2/dtfield/parse/type_hint.py
+-rw-r--r--   0        0        0      457 2023-06-17 00:25:40.076770 dtfield-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      806 2023-06-17 00:25:44.005888 dtfield-0.2.2/setup.py
+-rw-r--r--   0        0        0      636 2023-06-17 00:25:44.006130 dtfield-0.2.2/PKG-INFO
```

### Comparing `dtfield-0.2.1/dtfield/_imports.py` & `dtfield-0.2.2/dtfield/_imports.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/base_enum.py` & `dtfield-0.2.2/dtfield/base_enum.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/engine.py` & `dtfield-0.2.2/dtfield/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         'display_repr',
         'eq_function',
         'get_attr_or_item',
         'filter_dict',
         'make_dict',
         'dict_items',
         'normalize_lower_if_string',
-        'exclude_keys_from_dict'
+        'exclude_keys_from_dict',
+        'TEMPLATES'
 ]
 
 import os.path
 
 from deta.base import FetchResponse
 from starlette.templating import Jinja2Templates
 from dtfield._imports import *
@@ -339,26 +340,26 @@
     @classmethod
     async def ordered_instances_list(cls) -> list[Self]:
         return ordered(await cls.instances_list())
     
     @classmethod
     async def html_list(cls, request: Request):
         return TEMPLATES.TemplateResponse(
-                'partial/instances_list.jj',
+                '/partial/instances_list.jj',
                 {
                         'request': request,
                         'instances': await cls.sorted_instances_list(),
                         'model': cls
                 }
         )
     
     @classmethod
     async def html_datalist(cls, request: Request):
         return TEMPLATES.TemplateResponse(
-                'partial/datalist.jj',
+                '/partial/datalist.jj',
                 {
                         'request': request,
                         'instances': await cls.sorted_instances_list(),
                         'model': cls
                 }
         )
```

### Comparing `dtfield-0.2.1/dtfield/functions.py` & `dtfield-0.2.2/dtfield/functions.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/__pycache__/dates.cpython-39.pyc` & `dtfield-0.2.2/dtfield/parse/__pycache__/dates.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc` & `dtfield-0.2.2/dtfield/parse/__pycache__/json_encoder.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/__pycache__/null.cpython-39.pyc` & `dtfield-0.2.2/dtfield/parse/__pycache__/null.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/__pycache__/number.cpython-39.pyc` & `dtfield-0.2.2/dtfield/parse/__pycache__/number.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/__pycache__/string.cpython-39.pyc` & `dtfield-0.2.2/dtfield/parse/__pycache__/string.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/__pycache__/type_hint.cpython-39.pyc` & `dtfield-0.2.2/dtfield/parse/__pycache__/type_hint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/dates.py` & `dtfield-0.2.2/dtfield/parse/dates.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/json_encoder.py` & `dtfield-0.2.2/dtfield/parse/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/number.py` & `dtfield-0.2.2/dtfield/parse/number.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/string.py` & `dtfield-0.2.2/dtfield/parse/string.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/dtfield/parse/type_hint.py` & `dtfield-0.2.2/dtfield/parse/type_hint.py`

 * *Files identical despite different names*

### Comparing `dtfield-0.2.1/setup.py` & `dtfield-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'itsdangerous>=2.1.2,<3.0.0',
  'python-multipart>=0.0.6,<0.0.7',
  'typing-extensions>=4.6.3,<5.0.0',
  'uvicorn>=0.22.0,<0.23.0']
 
 setup_kwargs = {
     'name': 'dtfield',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': '',
     'long_description': None,
     'author': 'Daniel Arantes',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dtfield-0.2.1/PKG-INFO` & `dtfield-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtfield
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Daniel Arantes
 Author-email: arantesdv@me.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

