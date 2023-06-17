# Comparing `tmp/watch-diff-1.1.2.tar.gz` & `tmp/watch-diff-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watch-diff-1.1.2.tar", last modified: Sat Jun 17 15:17:58 2023, max compression
+gzip compressed data, was "watch-diff-1.1.3.tar", last modified: Sat Jun 17 15:20:04 2023, max compression
```

## Comparing `watch-diff-1.1.2.tar` & `watch-diff-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:17:58.312111 watch-diff-1.1.2/
--rw-r--r--   0 berfr     (1000) berfr     (1000)     1086 2023-03-05 14:46:00.000000 watch-diff-1.1.2/LICENSE
--rw-r--r--   0 berfr     (1000) berfr     (1000)     2003 2023-06-17 15:17:58.312111 watch-diff-1.1.2/PKG-INFO
--rw-r--r--   0 berfr     (1000) berfr     (1000)     1653 2023-06-17 15:13:15.000000 watch-diff-1.1.2/README.md
--rw-r--r--   0 berfr     (1000) berfr     (1000)       38 2023-06-17 15:17:58.312111 watch-diff-1.1.2/setup.cfg
--rw-r--r--   0 berfr     (1000) berfr     (1000)      990 2023-03-05 14:46:00.000000 watch-diff-1.1.2/setup.py
-drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:17:58.309111 watch-diff-1.1.2/tests/
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     1272 2021-06-12 21:44:03.000000 watch-diff-1.1.2/tests/test_watch_diff.py
-drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:17:58.310111 watch-diff-1.1.2/watch_diff/
--rw-r--r--   0 berfr     (1000) berfr     (1000)      198 2023-06-17 15:14:10.000000 watch-diff-1.1.2/watch_diff/__init__.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     3112 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/__main__.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     1051 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/command.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     1477 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/diff.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     2759 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/email.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     1353 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/format.py
-drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:17:58.312111 watch-diff-1.1.2/watch_diff.egg-info/
--rw-r--r--   0 berfr     (1000) berfr     (1000)     2003 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/PKG-INFO
--rw-r--r--   0 berfr     (1000) berfr     (1000)      385 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/SOURCES.txt
--rw-r--r--   0 berfr     (1000) berfr     (1000)        1 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/dependency_links.txt
--rw-r--r--   0 berfr     (1000) berfr     (1000)       56 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/entry_points.txt
--rw-r--r--   0 berfr     (1000) berfr     (1000)       78 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/requires.txt
--rw-r--r--   0 berfr     (1000) berfr     (1000)       11 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/top_level.txt
+drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:20:04.936572 watch-diff-1.1.3/
+-rw-r--r--   0 berfr     (1000) berfr     (1000)     1086 2023-03-05 14:46:00.000000 watch-diff-1.1.3/LICENSE
+-rw-r--r--   0 berfr     (1000) berfr     (1000)     2001 2023-06-17 15:20:04.936572 watch-diff-1.1.3/PKG-INFO
+-rw-r--r--   0 berfr     (1000) berfr     (1000)     1653 2023-06-17 15:13:15.000000 watch-diff-1.1.3/README.md
+-rw-r--r--   0 berfr     (1000) berfr     (1000)       38 2023-06-17 15:20:04.936572 watch-diff-1.1.3/setup.cfg
+-rw-r--r--   0 berfr     (1000) berfr     (1000)      988 2023-06-17 15:18:48.000000 watch-diff-1.1.3/setup.py
+drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:20:04.933572 watch-diff-1.1.3/tests/
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     1272 2021-06-12 21:44:03.000000 watch-diff-1.1.3/tests/test_watch_diff.py
+drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:20:04.934572 watch-diff-1.1.3/watch_diff/
+-rw-r--r--   0 berfr     (1000) berfr     (1000)      198 2023-06-17 15:19:54.000000 watch-diff-1.1.3/watch_diff/__init__.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     3112 2021-06-12 21:44:05.000000 watch-diff-1.1.3/watch_diff/__main__.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     1051 2021-06-12 21:44:05.000000 watch-diff-1.1.3/watch_diff/command.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     1477 2021-06-12 21:44:05.000000 watch-diff-1.1.3/watch_diff/diff.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     2759 2021-06-12 21:44:05.000000 watch-diff-1.1.3/watch_diff/email.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     1353 2021-06-12 21:44:05.000000 watch-diff-1.1.3/watch_diff/format.py
+drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:20:04.936572 watch-diff-1.1.3/watch_diff.egg-info/
+-rw-r--r--   0 berfr     (1000) berfr     (1000)     2001 2023-06-17 15:20:04.000000 watch-diff-1.1.3/watch_diff.egg-info/PKG-INFO
+-rw-r--r--   0 berfr     (1000) berfr     (1000)      385 2023-06-17 15:20:04.000000 watch-diff-1.1.3/watch_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 berfr     (1000) berfr     (1000)        1 2023-06-17 15:20:04.000000 watch-diff-1.1.3/watch_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 berfr     (1000) berfr     (1000)       56 2023-06-17 15:20:04.000000 watch-diff-1.1.3/watch_diff.egg-info/entry_points.txt
+-rw-r--r--   0 berfr     (1000) berfr     (1000)       78 2023-06-17 15:20:04.000000 watch-diff-1.1.3/watch_diff.egg-info/requires.txt
+-rw-r--r--   0 berfr     (1000) berfr     (1000)       11 2023-06-17 15:20:04.000000 watch-diff-1.1.3/watch_diff.egg-info/top_level.txt
```

### Comparing `watch-diff-1.1.2/LICENSE` & `watch-diff-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.2/PKG-INFO` & `watch-diff-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: watch-diff
-Version: 1.1.2
+Version: 1.1.3
 Summary: Watch command output and get notified on changes
 Home-page: https://github.com/francisbergin/watch-diff
 Author: francisbergin
-Author-email: francisbergin.dev@gmail.com
+Author-email: francisbergin@hotmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # watch-diff
```

### Comparing `watch-diff-1.1.2/README.md` & `watch-diff-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.2/setup.py` & `watch-diff-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 setup(
     name="watch-diff",
     version=version,
     description="Watch command output and get notified on changes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="francisbergin",
-    author_email="francisbergin.dev@gmail.com",
+    author_email="francisbergin@hotmail.com",
     python_requires=">=3.7",
     url="https://github.com/francisbergin/watch-diff",
     packages=["watch_diff"],
     extras_require={
         "dev": [
             "black==23.1.0",
             "setuptools==67.4.0",
```

### Comparing `watch-diff-1.1.2/tests/test_watch_diff.py` & `watch-diff-1.1.3/tests/test_watch_diff.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.2/watch_diff/__main__.py` & `watch-diff-1.1.3/watch_diff/__main__.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.2/watch_diff/command.py` & `watch-diff-1.1.3/watch_diff/command.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.2/watch_diff/diff.py` & `watch-diff-1.1.3/watch_diff/diff.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.2/watch_diff/email.py` & `watch-diff-1.1.3/watch_diff/email.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.2/watch_diff/format.py` & `watch-diff-1.1.3/watch_diff/format.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.2/watch_diff.egg-info/PKG-INFO` & `watch-diff-1.1.3/watch_diff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: watch-diff
-Version: 1.1.2
+Version: 1.1.3
 Summary: Watch command output and get notified on changes
 Home-page: https://github.com/francisbergin/watch-diff
 Author: francisbergin
-Author-email: francisbergin.dev@gmail.com
+Author-email: francisbergin@hotmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # watch-diff
```

