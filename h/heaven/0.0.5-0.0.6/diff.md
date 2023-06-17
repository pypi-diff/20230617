# Comparing `tmp/heaven-0.0.5.tar.gz` & `tmp/heaven-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaven-0.0.5.tar", max compression
+gzip compressed data, was "heaven-0.0.6.tar", max compression
```

## Comparing `heaven-0.0.5.tar` & `heaven-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.5/LICENSE
--rw-r--r--   0        0        0     1312 2023-06-10 13:10:30.152074 heaven-0.0.5/README.md
--rw-r--r--   0        0        0      216 2023-06-11 00:42:20.272309 heaven-0.0.5/heaven/__init__.py
--rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.5/heaven/constants.py
--rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.5/heaven/context.py
--rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.5/heaven/errors.py
--rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.5/heaven/form.py
--rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.5/heaven/mocks.py
--rw-r--r--   0        0        0     3427 2023-06-10 23:16:34.082772 heaven-0.0.5/heaven/request.py
--rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.5/heaven/response.py
--rw-r--r--   0        0        0    21987 2023-06-11 00:41:32.757365 heaven-0.0.5/heaven/router.py
--rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.5/heaven/server.py
--rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.5/heaven/tutorials.py
--rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.5/heaven/utils.py
--rw-r--r--   0        0        0      485 2023-06-11 00:42:49.100375 heaven-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 heaven-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-04 16:11:34.728189 heaven-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1300 2023-06-16 18:27:00.893443 heaven-0.0.6/README.md
+-rw-r--r--   0        0        0      216 2023-06-17 00:29:09.254197 heaven-0.0.6/heaven/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-10 13:10:30.157056 heaven-0.0.6/heaven/constants.py
+-rw-r--r--   0        0        0      261 2023-06-10 13:10:30.157160 heaven-0.0.6/heaven/context.py
+-rw-r--r--   0        0        0      141 2023-06-10 13:10:30.157248 heaven-0.0.6/heaven/errors.py
+-rw-r--r--   0        0        0      977 2023-06-10 13:10:30.157442 heaven-0.0.6/heaven/form.py
+-rw-r--r--   0        0        0     2946 2023-06-10 13:10:30.157649 heaven-0.0.6/heaven/mocks.py
+-rw-r--r--   0        0        0     3511 2023-06-17 00:28:06.422331 heaven-0.0.6/heaven/request.py
+-rw-r--r--   0        0        0     4390 2023-06-10 23:36:48.661427 heaven-0.0.6/heaven/response.py
+-rw-r--r--   0        0        0    22029 2023-06-16 18:25:20.409409 heaven-0.0.6/heaven/router.py
+-rw-r--r--   0        0        0        0 2023-06-10 13:10:30.158385 heaven-0.0.6/heaven/server.py
+-rw-r--r--   0        0        0     1116 2023-06-10 13:10:30.158553 heaven-0.0.6/heaven/tutorials.py
+-rw-r--r--   0        0        0      926 2023-06-10 13:10:30.158643 heaven-0.0.6/heaven/utils.py
+-rw-r--r--   0        0        0      485 2023-06-17 00:29:48.990808 heaven-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 heaven-0.0.6/PKG-INFO
```

### Comparing `heaven-0.0.5/LICENSE` & `heaven-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `heaven-0.0.5/README.md` & `heaven-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Routerling : <img src="https://img.shields.io/badge/coverage-95%25-green" />
+# Heaven : <img src="https://img.shields.io/badge/coverage-95%25-green" />
 
-Routerling is a very very small, extremely tiny, and insanely fast [ASGI](https://asgi.readthedocs.io) web application framework. It was designed to facilitate productivity by allowing for complete mastery in 7 minutes or less.
+Heaven is a very very small, extremely tiny, and insanely fast [ASGI](https://asgi.readthedocs.io) web application framework. It was designed to facilitate productivity by allowing for complete mastery in 7 minutes or less.
 
-Routerling is a very light layer around ASGI with support for application mounting and is perhaps the simplest and one of the fastest python web frameworks (biased opinion of course).
+Heaven is a very light layer around ASGI with support for application mounting and is perhaps the simplest and one of the fastest python web frameworks (biased opinion of course).
 
 
 ## Installling
 Install with [pip](https://pip.pypa.io/en/stable/getting-started/)
 ```sh
 $ pip install heaven
 ```
```

### Comparing `heaven-0.0.5/heaven/constants.py` & `heaven-0.0.6/heaven/constants.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.5/heaven/form.py` & `heaven-0.0.6/heaven/form.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.5/heaven/mocks.py` & `heaven-0.0.6/heaven/mocks.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.5/heaven/request.py` & `heaven-0.0.6/heaven/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         self._body = body
         self._cookies = None
         self._form = None
         self._receive = receive
         self._scope = scope
         self._subdomain, self._headers = metadata
         self._params = None
+        self._parameterized = False
         self._mounted_from_application = None
 
     def _parse_qs(self):
         qs = self._scope.get("query_string")
         qsd = {}
         if not qs:
             return qsd
@@ -91,16 +92,17 @@
 
     @mounted.setter
     def mounted(self, value: 'Router'):
         self._mounted_from_application
 
     @property
     def params(self):
-        if not self._params:
+        if not self._parameterized:
             self._params = self._parse_qs()
+            self._parameterized = True
         return self._params
 
     @params.setter
     def params(self, pair):
         if not self._params:
             self._params = {}
         self._params[pair[0]] = pair[1]
```

### Comparing `heaven-0.0.5/heaven/response.py` & `heaven-0.0.6/heaven/response.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.5/heaven/router.py` & `heaven-0.0.6/heaven/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,34 +90,34 @@
         self.parameterized = False
         self.route = route
         self.handler = handler
         self.children = {}
 
     def match(self, routes: deque, r: Request):
         matched: str = None
-        route_at_deviation = None
-        deviation_point: Route = None
         node: Route = self
+        route_at_deviation = '/'.join(routes)
+        deviation_point: Route = node.children.get('*')
         while routes:
             route = routes.popleft()
             current_node = node.children.get(route)
             if not current_node:
                 # is there a parameterized child?
                 current_node = node.children.get(':')
                 if current_node:
-                    r.params = current_node.parameterized, route
                     """Store the label that immediately follows the ':' represented by paremeterized
                     and its value represented as route into request.params"""
+                    r.params = current_node.parameterized, route
 
                     if(node.children.get('*')):
+                        """If there was also a wildcard seeing as placeholder ':' takes precedence, then
+                        mark the point it deviated so it is possible to backtrack and use that point for
+                        matching if this path fumbles later"""
                         route_at_deviation = '/'.join([route, *routes])
                         deviation_point = node.children.get('*')
-                    """If there was also a wildcard seeing as placeholder ':' takes precedence, then
-                    mark the point it deviated so it is possible to backtrack and use that point for
-                    matching if this path fumbles later"""
 
                     node = current_node
                     continue
 
                 wildcard = node.children.get('*')
                 if wildcard:  #pragma: nocover
                     r.params = '*', '/'.join([route, *routes])
```

### Comparing `heaven-0.0.5/heaven/tutorials.py` & `heaven-0.0.6/heaven/tutorials.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.5/heaven/utils.py` & `heaven-0.0.6/heaven/utils.py`

 * *Files identical despite different names*

### Comparing `heaven-0.0.5/PKG-INFO` & `heaven-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaven
-Version: 0.0.5
+Version: 0.0.6
 Summary: Extremely Stupid Simple, Blazing Fast, Get Out of your way immediately Microframework for building Python Web Applications.
 License: MIT
 Author: Raymond Ortserga
 Author-email: ortserga@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,19 +14,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1.0,<4.0.0)
 Requires-Dist: uvicorn (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
-# Routerling : <img src="https://img.shields.io/badge/coverage-95%25-green" />
+# Heaven : <img src="https://img.shields.io/badge/coverage-95%25-green" />
 
-Routerling is a very very small, extremely tiny, and insanely fast [ASGI](https://asgi.readthedocs.io) web application framework. It was designed to facilitate productivity by allowing for complete mastery in 7 minutes or less.
+Heaven is a very very small, extremely tiny, and insanely fast [ASGI](https://asgi.readthedocs.io) web application framework. It was designed to facilitate productivity by allowing for complete mastery in 7 minutes or less.
 
-Routerling is a very light layer around ASGI with support for application mounting and is perhaps the simplest and one of the fastest python web frameworks (biased opinion of course).
+Heaven is a very light layer around ASGI with support for application mounting and is perhaps the simplest and one of the fastest python web frameworks (biased opinion of course).
 
 
 ## Installling
 Install with [pip](https://pip.pypa.io/en/stable/getting-started/)
 ```sh
 $ pip install heaven
 ```
```

