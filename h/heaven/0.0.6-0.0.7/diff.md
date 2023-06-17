# Comparing `tmp/heaven-0.0.6.tar.gz` & `tmp/heaven-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.0.6.tar", max compression
+gzip compressed data, was "heaven-0.0.7.tar", max compression
```

## Comparing `heaven-0.0.6.tar` & `heaven-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.6/LICENSE
--rw-r--r--   0        0        0     1300 2023-06-16 18:27:00.893443 heaven-0.0.6/README.md
--rw-r--r--   0        0        0      216 2023-06-17 00:29:09.254197 heaven-0.0.6/heaven/__init__.py
--rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.6/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.6/heaven/context.py
--rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.6/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.6/heaven/form.py
--rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.6/heaven/mocks.py
--rw-r--r--   0        0        0     3511 2023-06-17 00:28:06.422331 heaven-0.0.6/heaven/request.py
--rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.6/heaven/response.py
--rw-r--r--   0        0        0    22029 2023-06-16 18:25:20.409409 heaven-0.0.6/heaven/router.py
--rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.6/heaven/server.py
--rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.6/heaven/tutorials.py
--rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.6/heaven/utils.py
--rw-r--r--   0        0        0      485 2023-06-17 00:29:48.990808 heaven-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 heaven-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1300 2023-06-16 18:27:00.893443 heaven-0.0.7/README.md
+-rw-r--r--   0        0        0      216 2023-06-17 01:41:51.330631 heaven-0.0.7/heaven/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.7/heaven/constants.py
+-rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.7/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.7/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.7/heaven/form.py
+-rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.7/heaven/mocks.py
+-rw-r--r--   0        0        0     3559 2023-06-17 01:35:55.170610 heaven-0.0.7/heaven/request.py
+-rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.7/heaven/response.py
+-rw-r--r--   0        0        0    22029 2023-06-16 18:25:20.409409 heaven-0.0.7/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.7/heaven/server.py
+-rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.7/heaven/tutorials.py
+-rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.7/heaven/utils.py
+-rw-r--r--   0        0        0      485 2023-06-17 01:41:31.794232 heaven-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 heaven-0.0.7/PKG-INFO
```

### Comparing `heaven-0.0.6/LICENSE` & `heaven-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.0.6/README.md` & `heaven-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `heaven-0.0.6/heaven/constants.py` & `heaven-0.0.7/heaven/constants.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.6/heaven/form.py` & `heaven-0.0.7/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.6/heaven/mocks.py` & `heaven-0.0.7/heaven/mocks.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.6/heaven/request.py` & `heaven-0.0.7/heaven/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._body = body
         self._cookies = None
         self._form = None
         self._receive = receive
         self._scope = scope
         self._subdomain, self._headers = metadata
         self._params = None
-        self._parameterized = False
+        self._dirty = False
         self._mounted_from_application = None
 
     def _parse_qs(self):
         qs = self._scope.get("query_string")
         qsd = {}
         if not qs:
             return qsd
@@ -92,17 +92,18 @@
 
     @mounted.setter
     def mounted(self, value: 'Router'):
         self._mounted_from_application
 
     @property
     def params(self):
-        if not self._parameterized:
-            self._params = self._parse_qs()
-            self._parameterized = True
+        if not self._dirty:
+            if not self._params: self._params = {}
+            self._params = {**self._params, **self._parse_qs()}
+            self._dirty = True
         return self._params
 
     @params.setter
     def params(self, pair):
         if not self._params:
             self._params = {}
         self._params[pair[0]] = pair[1]
```

### Comparing `heaven-0.0.6/heaven/response.py` & `heaven-0.0.7/heaven/response.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.6/heaven/router.py` & `heaven-0.0.7/heaven/router.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.6/heaven/tutorials.py` & `heaven-0.0.7/heaven/tutorials.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.6/heaven/utils.py` & `heaven-0.0.7/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.6/PKG-INFO` & `heaven-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

