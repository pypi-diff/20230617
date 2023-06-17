# Comparing `tmp/proJSON-1.0.0.tar.gz` & `tmp/proJSON-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proJSON-1.0.0.tar", last modified: Sat Jun 17 17:51:54 2023, max compression
+gzip compressed data, was "proJSON-1.1.1.tar", last modified: Sat Jun 17 20:49:09 2023, max compression
```

## Comparing `proJSON-1.0.0.tar` & `proJSON-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:51:54.669926 proJSON-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-17 17:51:42.000000 proJSON-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-17 17:51:54.669926 proJSON-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-17 17:51:42.000000 proJSON-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 17:51:42.000000 proJSON-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 17:51:54.669926 proJSON-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:51:54.669926 proJSON-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:51:54.669926 proJSON-1.0.0/src/proJSON/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-17 17:51:42.000000 proJSON-1.0.0/src/proJSON/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:51:54.669926 proJSON-1.0.0/src/proJSON.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-17 17:51:54.000000 proJSON-1.0.0/src/proJSON.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 17:51:54.000000 proJSON-1.0.0/src/proJSON.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:51:54.000000 proJSON-1.0.0/src/proJSON.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 17:51:54.000000 proJSON-1.0.0/src/proJSON.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:51:54.669926 proJSON-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-17 17:51:42.000000 proJSON-1.0.0/tests/test_projson.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-17 20:48:58.000000 proJSON-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-17 20:49:09.629624 proJSON-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-17 20:48:58.000000 proJSON-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 20:48:58.000000 proJSON-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 20:49:09.629624 proJSON-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/src/proJSON/
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-17 20:48:58.000000 proJSON-1.1.1/src/proJSON/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/src/proJSON.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-17 20:49:09.000000 proJSON-1.1.1/src/proJSON.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-17 20:49:09.000000 proJSON-1.1.1/src/proJSON.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 20:49:09.000000 proJSON-1.1.1/src/proJSON.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 20:49:09.000000 proJSON-1.1.1/src/proJSON.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 20:49:09.629624 proJSON-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-17 20:48:58.000000 proJSON-1.1.1/tests/test_projson.py
```

### Comparing `proJSON-1.0.0/LICENSE` & `proJSON-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `proJSON-1.0.0/PKG-INFO` & `proJSON-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.0.0
+Version: 1.1.1
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proJSON-1.0.0/README.md` & `proJSON-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `proJSON-1.0.0/pyproject.toml` & `proJSON-1.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proJSON"
-version = "1.0.0"
+version = "1.1.1"
 authors = [
   { name="JKinc", email="communications@jkinc.co.uk" },
 ]
 description = "A python library to compress a dict into a bytearray."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `proJSON-1.0.0/src/proJSON.egg-info/PKG-INFO` & `proJSON-1.1.1/src/proJSON.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proJSON
-Version: 1.0.0
+Version: 1.1.1
 Summary: A python library to compress a dict into a bytearray.
 Author-email: JKinc <communications@jkinc.co.uk>
 Project-URL: Homepage, https://github.com/The-Geiger-Network-Project/proJSON/tree/main
 Project-URL: Bug Tracker, https://github.com/The-Geiger-Network-Project/proJSON/tree/main/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proJSON-1.0.0/tests/test_projson.py` & `proJSON-1.1.1/tests/test_projson.py`

 * *Files identical despite different names*

