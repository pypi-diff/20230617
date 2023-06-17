# Comparing `tmp/easy-flask-restful-1.1.3.tar.gz` & `tmp/easy-flask-restful-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-flask-restful-1.1.3.tar", last modified: Wed Nov 23 15:12:28 2022, max compression
+gzip compressed data, was "easy-flask-restful-1.1.5.tar", last modified: Sat Jun 17 02:13:45 2023, max compression
```

## Comparing `easy-flask-restful-1.1.3.tar` & `easy-flask-restful-1.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:28.438919 easy-flask-restful-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3619 2022-11-23 15:12:28.438919 easy-flask-restful-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3069 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:28.434919 easy-flask-restful-1.1.3/easy_flask/
--rw-r--r--   0 runner    (1001) docker     (121)     2323 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:28.434919 easy-flask-restful-1.1.3/easy_flask/api/
--rw-r--r--   0 runner    (1001) docker     (121)     3169 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:28.434919 easy-flask-restful-1.1.3/easy_flask/api/demo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/api/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/api/demo/demo_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:28.434919 easy-flask-restful-1.1.3/easy_flask/conf/
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/conf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:28.438919 easy-flask-restful-1.1.3/easy_flask/internal/
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      519 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/internal/error.py
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/start.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:28.438919 easy-flask-restful-1.1.3/easy_flask/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6738 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/easy_flask/utils/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 15:12:28.438919 easy-flask-restful-1.1.3/easy_flask_restful.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3619 2022-11-23 15:12:28.000000 easy-flask-restful-1.1.3/easy_flask_restful.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-11-23 15:12:28.000000 easy-flask-restful-1.1.3/easy_flask_restful.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 15:12:28.000000 easy-flask-restful-1.1.3/easy_flask_restful.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-23 15:12:28.000000 easy-flask-restful-1.1.3/easy_flask_restful.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 15:12:28.000000 easy-flask-restful-1.1.3/easy_flask_restful.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-23 15:12:28.000000 easy-flask-restful-1.1.3/easy_flask_restful.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-23 15:12:28.000000 easy-flask-restful-1.1.3/easy_flask_restful.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-23 15:12:28.438919 easy-flask-restful-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-11-23 15:12:19.000000 easy-flask-restful-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:45.877168 easy-flask-restful-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-17 02:13:45.877168 easy-flask-restful-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:45.873168 easy-flask-restful-1.1.5/easy_flask/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:45.873168 easy-flask-restful-1.1.5/easy_flask/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:45.873168 easy-flask-restful-1.1.5/easy_flask/api/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/api/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/api/demo/demo_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:45.873168 easy-flask-restful-1.1.5/easy_flask/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/conf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:45.873168 easy-flask-restful-1.1.5/easy_flask/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/internal/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:45.873168 easy-flask-restful-1.1.5/easy_flask/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/easy_flask/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:13:45.877168 easy-flask-restful-1.1.5/easy_flask_restful.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-17 02:13:45.000000 easy-flask-restful-1.1.5/easy_flask_restful.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-17 02:13:45.000000 easy-flask-restful-1.1.5/easy_flask_restful.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:13:45.000000 easy-flask-restful-1.1.5/easy_flask_restful.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-17 02:13:45.000000 easy-flask-restful-1.1.5/easy_flask_restful.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:13:45.000000 easy-flask-restful-1.1.5/easy_flask_restful.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 02:13:45.000000 easy-flask-restful-1.1.5/easy_flask_restful.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 02:13:45.000000 easy-flask-restful-1.1.5/easy_flask_restful.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 02:13:45.877168 easy-flask-restful-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-17 02:13:35.000000 easy-flask-restful-1.1.5/setup.py
```

### Comparing `easy-flask-restful-1.1.3/LICENSE` & `easy-flask-restful-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-flask-restful-1.1.3/PKG-INFO` & `easy-flask-restful-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-flask-restful
-Version: 1.1.3
+Version: 1.1.5
 Summary: Easy to Make Flask Server
 Home-page: https://github.com/GuoTengda1993/easy-flask
 Author: Guo Tengda
 Author-email: ttguotengda@foxmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `easy-flask-restful-1.1.3/README.md` & `easy-flask-restful-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `easy-flask-restful-1.1.3/easy_flask/__init__.py` & `easy-flask-restful-1.1.5/easy_flask/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 import os
 import sys
 from fnmatch import filter
 from os.path import isdir, join
 
 
-__version__ = '1.1.3'
+__version__ = '1.1.5'
 
 
 def init_args():
     """init args
 
     :return:
     """
```

### Comparing `easy-flask-restful-1.1.3/easy_flask/api/__init__.py` & `easy-flask-restful-1.1.5/easy_flask/api/__init__.py`

 * *Files identical despite different names*

### Comparing `easy-flask-restful-1.1.3/easy_flask/api/demo/demo_api.py` & `easy-flask-restful-1.1.5/easy_flask/api/demo/demo_api.py`

 * *Files identical despite different names*

### Comparing `easy-flask-restful-1.1.3/easy_flask/conf/__init__.py` & `easy-flask-restful-1.1.5/easy_flask/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `easy-flask-restful-1.1.3/easy_flask/internal/__init__.py` & `easy-flask-restful-1.1.5/easy_flask/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `easy-flask-restful-1.1.3/easy_flask/internal/error.py` & `easy-flask-restful-1.1.5/easy_flask/internal/error.py`

 * *Files identical despite different names*

### Comparing `easy-flask-restful-1.1.3/easy_flask/start.py` & `easy-flask-restful-1.1.5/easy_flask/start.py`

 * *Files identical despite different names*

### Comparing `easy-flask-restful-1.1.3/easy_flask/utils/parser.py` & `easy-flask-restful-1.1.5/easy_flask/utils/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 extra_pattern = {
     "class": {Type: str, Default: "a", In: ["a", "b", "c"]},
     "likes": {Type: list, Split: ","}
 }
 pattern = {
     "name": {Type: str, Required: True},
     "age": {Type: int, Required: True, Min: 1, Max: 200},
-    "extra": {Type: dict, Required: True}
+    "extra": {Type: dict, Required: True, Pattern=extra_pattern}
 }
 
 data, err = parser(data=request.args.to_dict(), pattern=pattern)
 ...
 """
 import json
 from json.decoder import JSONDecodeError
```

### Comparing `easy-flask-restful-1.1.3/easy_flask_restful.egg-info/PKG-INFO` & `easy-flask-restful-1.1.5/easy_flask_restful.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-flask-restful
-Version: 1.1.3
+Version: 1.1.5
 Summary: Easy to Make Flask Server
 Home-page: https://github.com/GuoTengda1993/easy-flask
 Author: Guo Tengda
 Author-email: ttguotengda@foxmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `easy-flask-restful-1.1.3/easy_flask_restful.egg-info/SOURCES.txt` & `easy-flask-restful-1.1.5/easy_flask_restful.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easy-flask-restful-1.1.3/setup.py` & `easy-flask-restful-1.1.5/setup.py`

 * *Files identical despite different names*

