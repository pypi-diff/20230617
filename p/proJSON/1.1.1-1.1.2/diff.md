# Comparing `tmp/proJSON-1.1.1.tar.gz` & `tmp/proJSON-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proJSON-1.1.1.tar", last modified: Sat Jun 17 20:49:09 2023, max compression
+gzip compressed data, was "proJSON-1.1.2.tar", last modified: Sat Jun 17 20:54:28 2023, max compression
```

## Comparing `proJSON-1.1.1.tar` & `proJSON-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-17 20:48:58.000000 proJSON-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-17 20:49:09.629624 proJSON-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-17 20:48:58.000000 proJSON-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 20:48:58.000000 proJSON-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 20:49:09.629624 proJSON-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/src/proJSON/
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-17 20:48:58.000000 proJSON-1.1.1/src/proJSON/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/src/proJSON.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-17 20:49:09.000000 proJSON-1.1.1/src/proJSON.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 20:49:09.000000 proJSON-1.1.1/src/proJSON.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 20:49:09.000000 proJSON-1.1.1/src/proJSON.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 20:49:09.000000 proJSON-1.1.1/src/proJSON.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-17 20:48:58.000000 proJSON-1.1.1/tests/test_projson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:54:28.863538 proJSON-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-17 20:54:19.000000 proJSON-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-17 20:54:28.863538 proJSON-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-17 20:54:19.000000 proJSON-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 20:54:19.000000 proJSON-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 20:54:28.863538 proJSON-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:54:28.859538 proJSON-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:54:28.859538 proJSON-1.1.2/src/proJSON/
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-17 20:54:19.000000 proJSON-1.1.2/src/proJSON/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:54:28.859538 proJSON-1.1.2/src/proJSON.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-17 20:54:28.000000 proJSON-1.1.2/src/proJSON.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 20:54:28.000000 proJSON-1.1.2/src/proJSON.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 20:54:28.000000 proJSON-1.1.2/src/proJSON.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 20:54:28.000000 proJSON-1.1.2/src/proJSON.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:54:28.863538 proJSON-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-17 20:54:19.000000 proJSON-1.1.2/tests/test_projson.py
```

### Comparing `proJSON-1.1.1/LICENSE` & `proJSON-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proJSON-1.1.1/PKG-INFO` & `proJSON-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,15 +63,15 @@
 
 ***Don't put a dir in another dir. It won't work***
 
 ### Init
 
 ``` python
 
-from projson import Crafter
+from proJSON import Crafter
 
 template = {
     # See the [types section](###Types) for how to make this.
     "intExample" : {
         "type": "int",
         "byte": 1
     },
```

### Comparing `proJSON-1.1.1/README.md` & `proJSON-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 ***Don't put a dir in another dir. It won't work***
 
 ### Init
 
 ``` python
 
-from projson import Crafter
+from proJSON import Crafter
 
 template = {
     # See the [types section](###Types) for how to make this.
     "intExample" : {
         "type": "int",
         "byte": 1
     },
```

### Comparing `proJSON-1.1.1/pyproject.toml` & `proJSON-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proJSON"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="JKinc", email="communications@jkinc.co.uk" },
 ]
 description = "A python library to compress a dict into a bytearray."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `proJSON-1.1.1/src/proJSON/__init__.py` & `proJSON-1.1.2/src/proJSON/__init__.py`

 * *Files identical despite different names*

### Comparing `proJSON-1.1.1/src/proJSON.egg-info/PKG-INFO` & `proJSON-1.1.2/src/proJSON.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.1.1
+Version: 1.1.2
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -63,15 +63,15 @@
 
 ***Don't put a dir in another dir. It won't work***
 
 ### Init
 
 ``` python
 
-from projson import Crafter
+from proJSON import Crafter
 
 template = {
     # See the [types section](###Types) for how to make this.
     "intExample" : {
         "type": "int",
         "byte": 1
     },
```

### Comparing `proJSON-1.1.1/tests/test_projson.py` & `proJSON-1.1.2/tests/test_projson.py`

 * *Files identical despite different names*

