# Comparing `tmp/struid-0.0.2.tar.gz` & `tmp/struid-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struid-0.0.2.tar", last modified: Sat Jun 17 14:41:32 2023, max compression
+gzip compressed data, was "struid-0.0.3.tar", last modified: Sat Jun 17 14:58:07 2023, max compression
```

## Comparing `struid-0.0.2.tar` & `struid-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:41:32.507496 struid-0.0.2/
--rw-rw-r--   0 antisol   (1000) antisol   (1000)       48 2023-06-17 14:00:47.000000 struid-0.0.2/LICENSE
--rw-rw-r--   0 antisol   (1000) antisol   (1000)     2268 2023-06-17 14:41:32.507496 struid-0.0.2/PKG-INFO
--rw-rw-r--   0 antisol   (1000) antisol   (1000)     1668 2023-06-17 14:26:52.000000 struid-0.0.2/README.md
--rw-rw-r--   0 antisol   (1000) antisol   (1000)      659 2023-06-17 14:31:40.000000 struid-0.0.2/pyproject.toml
--rw-rw-r--   0 antisol   (1000) antisol   (1000)       38 2023-06-17 14:41:32.507496 struid-0.0.2/setup.cfg
-drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:41:32.507496 struid-0.0.2/src/
-drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:41:32.507496 struid-0.0.2/src/struid/
--rw-rw-r--   0 antisol   (1000) antisol   (1000)       40 2023-06-17 14:30:48.000000 struid-0.0.2/src/struid/__init__.py
--rw-rw-r--   0 antisol   (1000) antisol   (1000)     5912 2023-06-04 13:45:59.000000 struid-0.0.2/src/struid/struid.py
-drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:41:32.507496 struid-0.0.2/src/struid.egg-info/
--rw-rw-r--   0 antisol   (1000) antisol   (1000)     2268 2023-06-17 14:41:32.000000 struid-0.0.2/src/struid.egg-info/PKG-INFO
--rw-rw-r--   0 antisol   (1000) antisol   (1000)      212 2023-06-17 14:41:32.000000 struid-0.0.2/src/struid.egg-info/SOURCES.txt
--rw-rw-r--   0 antisol   (1000) antisol   (1000)        1 2023-06-17 14:41:32.000000 struid-0.0.2/src/struid.egg-info/dependency_links.txt
--rw-rw-r--   0 antisol   (1000) antisol   (1000)        7 2023-06-17 14:41:32.000000 struid-0.0.2/src/struid.egg-info/top_level.txt
+drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:58:07.577257 struid-0.0.3/
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)       48 2023-06-17 14:00:47.000000 struid-0.0.3/LICENSE
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)     2268 2023-06-17 14:58:07.577257 struid-0.0.3/PKG-INFO
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)     1668 2023-06-17 14:26:52.000000 struid-0.0.3/README.md
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)      659 2023-06-17 14:56:57.000000 struid-0.0.3/pyproject.toml
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)       38 2023-06-17 14:58:07.577257 struid-0.0.3/setup.cfg
+drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:58:07.577257 struid-0.0.3/src/
+drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:58:07.577257 struid-0.0.3/src/struid/
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)       40 2023-06-17 14:30:48.000000 struid-0.0.3/src/struid/__init__.py
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)     5912 2023-06-04 13:45:59.000000 struid-0.0.3/src/struid/struid.py
+drwxrwxr-x   0 antisol   (1000) antisol   (1000)        0 2023-06-17 14:58:07.577257 struid-0.0.3/src/struid.egg-info/
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)     2268 2023-06-17 14:58:07.000000 struid-0.0.3/src/struid.egg-info/PKG-INFO
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)      212 2023-06-17 14:58:07.000000 struid-0.0.3/src/struid.egg-info/SOURCES.txt
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)        1 2023-06-17 14:58:07.000000 struid-0.0.3/src/struid.egg-info/dependency_links.txt
+-rw-rw-r--   0 antisol   (1000) antisol   (1000)        7 2023-06-17 14:58:07.000000 struid-0.0.3/src/struid.egg-info/top_level.txt
```

### Comparing `struid-0.0.2/PKG-INFO` & `struid-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struid
-Version: 0.0.2
+Version: 0.0.3
 Summary: Struid - 'Stringy-UUID', an enhanced UUID package
 Author-email: Dale Magee <struid@antisol.org>
 Project-URL: Homepage, https://gitlab.com/AntiSol/struid
 Project-URL: Bug Tracker, https://gitlab.com/AntiSol/struid/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `struid-0.0.2/README.md` & `struid-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `struid-0.0.2/pyproject.toml` & `struid-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "struid"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Dale Magee", email="struid@antisol.org" },
 ]
 description = "Struid - 'Stringy-UUID', an enhanced UUID package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `struid-0.0.2/src/struid/struid.py` & `struid-0.0.3/src/struid/struid.py`

 * *Files identical despite different names*

### Comparing `struid-0.0.2/src/struid.egg-info/PKG-INFO` & `struid-0.0.3/src/struid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struid
-Version: 0.0.2
+Version: 0.0.3
 Summary: Struid - 'Stringy-UUID', an enhanced UUID package
 Author-email: Dale Magee <struid@antisol.org>
 Project-URL: Homepage, https://gitlab.com/AntiSol/struid
 Project-URL: Bug Tracker, https://gitlab.com/AntiSol/struid/-/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

