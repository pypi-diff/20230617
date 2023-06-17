# Comparing `tmp/libsodium-2.4.1.tar.gz` & `tmp/libsodium-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libsodium-2.4.1.tar", last modified: Mon Mar 13 03:17:42 2023, max compression
+gzip compressed data, was "libsodium-2.5.0.tar", last modified: Sat Jun 17 19:49:13 2023, max compression
```

## Comparing `libsodium-2.4.1.tar` & `libsodium-2.5.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-03-13 03:17:42.679557 libsodium-2.4.1/
--rw-r--r--   0 ahsan      (502) staff       (20)      958 2023-03-13 03:17:42.679679 libsodium-2.4.1/PKG-INFO
--rw-r--r--   0 ahsan      (502) staff       (20)      485 2023-03-13 03:17:18.000000 libsodium-2.4.1/README.md
--rw-r--r--   0 ahsan      (502) staff       (20)      104 2022-12-07 01:00:09.000000 libsodium-2.4.1/pyproject.toml
--rw-r--r--   0 ahsan      (502) staff       (20)      620 2023-03-13 03:17:42.680220 libsodium-2.4.1/setup.cfg
-drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-03-13 03:17:42.635672 libsodium-2.4.1/src/
-drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-03-13 03:17:42.676868 libsodium-2.4.1/src/libsodium/
--rw-r--r--   0 ahsan      (502) staff       (20)      218 2022-12-15 15:41:32.000000 libsodium-2.4.1/src/libsodium/__init__.py
--rw-r--r--   0 ahsan      (502) staff       (20)    20178 2023-03-13 03:16:48.000000 libsodium-2.4.1/src/libsodium/__main__.py
--rw-r--r--   0 ahsan      (502) staff       (20)     3785 2023-03-12 17:31:56.000000 libsodium-2.4.1/src/libsodium/classes.py
-drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-03-13 03:17:42.679074 libsodium-2.4.1/src/libsodium/db/
--rw-r--r--   0 ahsan      (502) staff       (20)      487 2023-03-12 17:31:56.000000 libsodium-2.4.1/src/libsodium/db/__init__.py
--rw-r--r--   0 ahsan      (502) staff       (20)      302 2023-03-12 17:31:56.000000 libsodium-2.4.1/src/libsodium/db/connect.py
--rw-r--r--   0 ahsan      (502) staff       (20)     7198 2023-03-13 03:16:48.000000 libsodium-2.4.1/src/libsodium/wsgi.py
-drwxr-xr-x   0 ahsan      (502) staff       (20)        0 2023-03-13 03:17:42.678154 libsodium-2.4.1/src/libsodium.egg-info/
--rw-r--r--   0 ahsan      (502) staff       (20)      958 2023-03-13 03:17:42.000000 libsodium-2.4.1/src/libsodium.egg-info/PKG-INFO
--rw-r--r--   0 ahsan      (502) staff       (20)      338 2023-03-13 03:17:42.000000 libsodium-2.4.1/src/libsodium.egg-info/SOURCES.txt
--rw-r--r--   0 ahsan      (502) staff       (20)        1 2023-03-13 03:17:42.000000 libsodium-2.4.1/src/libsodium.egg-info/dependency_links.txt
--rw-r--r--   0 ahsan      (502) staff       (20)       10 2023-03-13 03:17:42.000000 libsodium-2.4.1/src/libsodium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.772675 libsodium-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-17 19:48:47.000000 libsodium-2.5.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-17 19:49:13.772675 libsodium-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-17 19:48:47.000000 libsodium-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-17 19:48:47.000000 libsodium-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-17 19:49:13.772675 libsodium-2.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.768675 libsodium-2.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.772675 libsodium-2.5.0/src/libsodium/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26876 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.772675 libsodium-2.5.0/src/libsodium/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/db/connect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-06-17 19:48:47.000000 libsodium-2.5.0/src/libsodium/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 19:49:13.772675 libsodium-2.5.0/src/libsodium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-17 19:49:13.000000 libsodium-2.5.0/src/libsodium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-17 19:49:13.000000 libsodium-2.5.0/src/libsodium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 19:49:13.000000 libsodium-2.5.0/src/libsodium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-17 19:49:13.000000 libsodium-2.5.0/src/libsodium.egg-info/top_level.txt
```

### Comparing `libsodium-2.4.1/PKG-INFO` & `libsodium-2.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.4.1
+Version: 2.5.0
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
 
-# Sodium v2.41
+# Sodium v2.50
 [![Documentation Status](https://readthedocs.org/projects/libsodium/badge/?version=latest)](https://libsodium.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/libsodium)
 
 Sodium is a WSGI web framework(like django) that is built for creating API's.
 # Instalation
-Linux/Mac OS:
+Linux/MacOS:
 ```
 pip3 install libsodium
 ```
 Windows:
 ```
 pip install libsodium
 ```
```

### Comparing `libsodium-2.4.1/setup.cfg` & `libsodium-2.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libsodium
-version = 2.4.1
+version = 2.5.0
 author = Ahsan Ahmed
 author_email = ahsan.ahmed3246@gmail.com
 description = A simple web framework
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://libsodium.readthedocs.io/en/latest/
 project_urls =
```

### Comparing `libsodium-2.4.1/src/libsodium/classes.py` & `libsodium-2.5.0/src/libsodium/classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+from datetime import datetime
+from datetime import timedelta
+from os import sync
 from .wsgi import WSGI
 from functools import wraps
+import typing as t
+
 
 class Runtime:
     def __init__(self):
         self.routes = []
     def addRoute(self, route):
         self.routes.append(route)
```

### Comparing `libsodium-2.4.1/src/libsodium/wsgi.py` & `libsodium-2.5.0/src/libsodium/wsgi.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,136 +1,193 @@
-from werkzeug.wrappers import Response, Request
+import json
 import re
+import base64
+from werkzeug.wrappers import Response, Request
 from routes import Mapper
+
+class Route:
+    def __init__(self, method, url, controler):
+        self.method = method
+        self.url = url
+        self.controler = controler
+
 class WSGI:
     def __init__(self):
         self.Routes = []
         self.Config = {}
+        self._secondary_map = {}
         self.map = Mapper()
 
     def wsgi_handler(self, environ, start_response):
         path = environ.get('PATH_INFO')
-        for route in self.Routes:
-            if not self.map.match(path) == None:
-                if not route.method == environ['REQUEST_METHOD']: 
-                    rsp = Response("<h1>405 Method Not Allowed</h1>")
-                    rsp.status_code = 405
-                    rsp.headers['Content-Type'] = 'text/html'
-                    return rsp(environ, start_response)
-                controler = route.controler()
-                request = Request(environ)
-                if hasattr(controler, "auth"):
-                    auth = controler.auth()
-                    verifier = auth[0]
-                    auth = auth[1]
-                    claims = auth.get('claims')
-                    location = auth.get('cookie') 
-                    if not location:
-                        location = "header"
-
-                    if location == "header":
-                        header = request.headers.get("Authorization")
-                        if not header:
-                            rsp = Response('{"error":"JWT not found"}')
-                            rsp.headers['Content-Type'] = "application/json"
-                            return rsp(environ, start_response)
-                        header = header.split(" ")
-                        if len(header) == 1:
-                            jwt = header[0]
-                        elif len(header) == 2 and header[0] == "Bearer":
-                            jwt = header[1]
-                        else:
-                            rsp = Response('{"error":"JWT is formated incorrectly"}')
-                            rsp.headers['Content-Type'] = "application/json"
-                            return rsp(environ, start_response)
-                    else:
-                        c = request.cookies.get(location)
-                        if not c:
-                            rsp = Response('{"error":"JWT not found"}')
-                            rsp.headers['Content-Type'] = "application/json"
-                            return rsp(environ, start_response)
-                        jwt = c
-
-                    #TODO: Check if the JWT is valid
-                    try:
-                        ans:bool = verifier.verify(jwt)
-                    except Exception as e:
-                        ans = False
-                    if ans:
-                        rsp = controler.onRequest(request)
+        if self.map.match(path):
+            route = self._secondary_map[self.map.match(path).get("controler")]
+            if not route.method == environ['REQUEST_METHOD']: 
+                rsp = Response("<h1>405 Method Not Allowed</h1>")
+                rsp.status_code = 405
+                rsp.headers['Content-Type'] = 'text/html'
+                return rsp(environ, start_response)
+            controler = route.controler()
+            request = Request(environ)
+            if hasattr(controler, "auth"):
+                auth = controler.auth()
+                verifier = auth[0]
+                extra = auth[1]
+                scopes = extra.get('scopes')
+                location = extra.get('cookie') 
+                if not location:
+                    location = "header"
+                if location == "header":
+                    header = request.headers.get("Authorization")
+                    if not header:
+                        rsp = Response('{"error":"JWT not found"}')
+                        rsp.headers['Content-Type'] = "application/json"
+                        return rsp(environ, start_response)
+                    header = header.split(" ")
+                    if len(header) == 1:
+                        jwt = header[0]
+                    elif len(header) == 2 and header[0] == "Bearer":
+                        jwt = header[1]
                     else:
-                        rsp = Response('{"error":"Invalid Jwt"}', status=403)
+                        rsp = Response('{"error":"JWT is formated incorrectly"}')
                         rsp.headers['Content-Type'] = "application/json"
                         return rsp(environ, start_response)
-
-                if hasattr(controler, "blueprint"):
-                    blueprint = controler.blueprint()
-                    targetMimetypes = blueprint[1]
-                    blueprint = blueprint[0]
-                    blueprint = blueprint.blueprint
-                    if not request.mimetype in targetMimetypes:
-                        rsp = Response("<h1>Incorrect mimetype.</h1><p>Sodium v2.41</p>")
-                        rsp.headers['Content-Type'] = 'text/html' 
+                else:
+                    c = request.cookies.get(location)
+                    if not c:
+                        rsp = Response('{"error":"JWT not found"}')
+                        rsp.headers['Content-Type'] = "application/json"
                         return rsp(environ, start_response)
-                    if request.mimetype == "application/x-www-form-urlencoded":
-                        target = request.form
-                    elif request.mimetype == "multipart/form":
+                    jwt = c
+
+                try:
+                    ans:bool = verifier.verify(jwt)
+                except Exception as e:
+                    ans = False
+                if ans:
+                    #Check for scopes
+                    if scopes:
+                        jwt = jwt.split(".")
+                        header = jwt[0]
+                        body = jwt[1]
+                        body = json.loads(base64.urlsafe_b64decode(body+"=="))
+                        found_scopes = body.get("scopes")
+                        if not found_scopes:
+                            rsp = Response('{"error":"Invalid Jwt", "detail":"No scopes specified"}', status=403)
+                            rsp.headers["Content-Type"] = "application/json"
+                            return rsp(environ, start_response)
+                        for scope in scopes:
+                            if not isinstance(scope, tuple) and not scope in found_scopes:
+                                rsp = Response('{"error":"Scope Error", "detail":"Scope ' + f"'{scope}'" + ' not found"}', status=403)
+                                rsp.headers["Content-Type"] = "application/json"
+                                return rsp(environ, start_response)
+                            elif isinstance(scope, tuple):
+                                found1scope = False
+                                for optional_scope in scope:
+                                    if optional_scope in found_scopes:
+                                        found1scope = True
+
+                                if not found1scope:
+                                    rsp = Response('{"error":"Scope Error", "detail":"Scope ' + f"'{scope}'" + ' not found(you need at least one of those scopes)"}', status=403)
+                                    rsp.headers["Content-Type"] = "application/json"
+                                    return rsp(environ, start_response)
+
+
+                    rsp = controler.onRequest(request)
+                else:
+                    rsp = Response('{"error":"Invalid Jwt"}', status=403)
+                    rsp.headers['Content-Type'] = "application/json"
+                    return rsp(environ, start_response)
+
+            if hasattr(controler, "blueprint"):
+                blueprint = controler.blueprint()
+                targetMimetypes = blueprint[1]
+                blueprint = blueprint[0]
+                blueprint = blueprint.blueprint
+                if not request.mimetype in targetMimetypes:
+                    rsp = Response("<h1>Incorrect mimetype.</h1><p>Sodium v2.50</p>")
+                    rsp.headers['Content-Type'] = 'text/html' 
+                    return rsp(environ, start_response)
+                if request.mimetype == "application/x-www-form-urlencoded":
+                    target = request.form
+                elif request.mimetype == "multipart/form":
                         target = request.form
-                    elif request.mimetype == "application/json":
+                elif request.mimetype == "application/json":
                         target = request.json
-                    else:
-                        target = request.raw
-                    for rule in blueprint:
-                        name = rule[0]
-                        targetType = rule[1]
+                else:
+                    target = None 
+                for rule in blueprint:
+                    name = rule[0]
+                    targetType = rule[1]
+                    try:
                         if not name in list(target.keys()):
                             if request.mimetype == "application/json":
                                 rsp = Response('{"status_code":"400", "error":"The route requires a '+ name + ' but it was not found"}')
                                 rsp.headers['Content-Type'] = 'application/json'
+                                return rsp(environ, start_response)
                             else:
                                 rsp = Response(f"<h1>400 Bad Request</h1><p>The route requires a {name} but it was not found</p>")
                                 rsp.headers['Content-Type'] = 'text/html'
-                            return rsp(environ, start_response)
+                                return rsp(environ, start_response)
+                    except:
+                        rsp = Response(f"<h1>400 Bad Request</h1><p>The route requires a {name} but it was not found</p>")
+                        rsp.headers['Content-Type'] = 'text/html'
+                        return rsp(environ, start_response)
+
+                    try:
                         value = target[name]
-                        clientType = type(value)
-                        if not clientType == targetType:
-                            if request.mimetype == "application/json":
-                                rsp = Response('{"status_code":"400", "error":"The route requires a the ' + name + ' parameter to be the data type ' + str(targetType) + ' but the ' + str(clientType) + ' type was provided"}')                                
-                                rsp.headers['Content-Type'] = 'application/json'
-                            else:
-                                rsp = Response(f"<h1>400 Bad Request</h1><p>The route requires a the {name} parameter to be the data type {targetType} but the {clientType} type was provided</p>")
-                                rsp.headers['Content-Type'] = 'text/html'
-                            return rsp(environ, start_response)
-                        regex = "."
-                        if len(rule) == 3:
-                            regex = rule[2] 
-                        if not re.search(regex, value):
-                            if request.mimetype == "application/json":
-                                rsp = Response('{"status_code":"400", "error":"The route requires a the ' + name + ' parameter to follow this regex: ' + str(regex) + '}')                                
-                                rsp.headers['Content-Type'] = 'application/json'
-                            else:
-                                rsp = Response(f"<h1>400 Bad Request</h1><p>The route requires a the {name} parameter to follow this regex {str(regex)}</p>")
-                                rsp.headers['Content-Type'] = 'text/html'
-                            return rsp(environ, start_response)
+                    except:
+                        rsp = Response(f"<h1>400 Bad Request</h1><p>The route requires a {name} but it was not found</p>")
+                        rsp.headers['Content-Type'] = 'text/html'
+                        return rsp(environ, start_response)
 
-                    rsp = controler.onRequest(request)
-                else:
-                    rsp = controler.onRequest(Request(environ))
-                if not isinstance(rsp, Response):
-                    rsp = Response(rsp) 
-                return rsp(environ, start_response)
+                    clientType = type(value)
+                    if not clientType == targetType:
+                        if request.mimetype == "application/json":
+                            rsp = Response('{"status_code":"400", "error":"The route requires a the ' + name + ' parameter to be the data type ' + str(targetType) + ' but the ' + str(clientType) + ' type was provided"}')                                
+                            rsp.headers['Content-Type'] = 'application/json'
+                        else:
+                            rsp = Response(f"<h1>400 Bad Request</h1><p>The route requires a the {name} parameter to be the data type {targetType} but the {clientType} type was provided</p>")
+                            rsp.headers['Content-Type'] = 'text/html'
+                        return rsp(environ, start_response)
+                    regex = "."
+                    if len(rule) == 3:
+                        regex = rule[2] 
+                    if not re.search(regex, str(value)):
+                        if request.mimetype == "application/json":
+                            rsp = Response('{"status_code":"400", "error":"The route requires a the ' + name + ' parameter to follow this regex: ' + str(regex) + '}')                                
+                            rsp.headers['Content-Type'] = 'application/json'
+                        else:
+                            rsp = Response(f"<h1>400 Bad Request</h1><p>The route requires a the {name} parameter to follow this regex {str(regex)}</p>")
+                            rsp.headers['Content-Type'] = 'text/html'
+                        return rsp(environ, start_response)
+
+                rsp = controler.onRequest(request)
+            else:
+                rsp = controler.onRequest(Request(environ))
+            if not isinstance(rsp, Response):
+                rsp = Response(rsp) 
+            return rsp(environ, start_response)
             
         rsp = Response("<h1>404 Not Found</h1>")
         rsp.status_code = 404
         rsp.headers['Content-Type'] = 'text/html'
         return rsp(environ, start_response)
 
     def onMount(self):
         temp = []
         for route in self.Routes:
             rt = route.route()
             temp.append(rt)
-            self.map.connect(None, rt.url)
+            if not rt.url[len(rt.url)-1] == "/":
+                self.map.connect(None, rt.url+"/", controler=rt)
+                self._secondary_map[str(rt)] = rt
+            else:
+                self.map.connect(None, rt.url[:len(rt.url)-1], controler=rt)
+                self._secondary_map[str(rt)] = rt
+                
+            self.map.connect(None, rt.url, controler=rt)
+            self._secondary_map[str(rt)] = rt
         self.Routes = temp
 
     def __call__(self, environ, start_response):
         return self.wsgi_handler(environ, start_response)
```

### Comparing `libsodium-2.4.1/src/libsodium.egg-info/PKG-INFO` & `libsodium-2.5.0/src/libsodium.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: libsodium
-Version: 2.4.1
+Version: 2.5.0
 Summary: A simple web framework
 Home-page: https://libsodium.readthedocs.io/en/latest/
 Author: Ahsan Ahmed
 Author-email: ahsan.ahmed3246@gmail.com
 Project-URL: Docs, https://libsodium.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENCE
 
-# Sodium v2.41
+# Sodium v2.50
 [![Documentation Status](https://readthedocs.org/projects/libsodium/badge/?version=latest)](https://libsodium.readthedocs.io/en/latest/?badge=latest)
 ![PyPI](https://img.shields.io/pypi/v/libsodium)
 
 Sodium is a WSGI web framework(like django) that is built for creating API's.
 # Instalation
-Linux/Mac OS:
+Linux/MacOS:
 ```
 pip3 install libsodium
 ```
 Windows:
 ```
 pip install libsodium
 ```
```

