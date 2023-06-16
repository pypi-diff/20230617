# Comparing `tmp/protoletariat-3.2.8.tar.gz` & `tmp/protoletariat-3.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protoletariat-3.2.8.tar", max compression
+gzip compressed data, was "protoletariat-3.2.9.tar", max compression
```

## Comparing `protoletariat-3.2.8.tar` & `protoletariat-3.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-23 03:43:28.809007 protoletariat-3.2.8/LICENSE
--rw-r--r--   0        0        0     5066 2023-05-23 03:43:28.809007 protoletariat-3.2.8/README.md
--rw-r--r--   0        0        0       66 2023-05-23 03:44:46.997105 protoletariat-3.2.8/protoletariat/__init__.py
--rw-r--r--   0        0        0     4333 2023-05-23 03:43:28.813007 protoletariat-3.2.8/protoletariat/__main__.py
--rw-r--r--   0        0        0     6661 2023-05-23 03:43:28.813007 protoletariat-3.2.8/protoletariat/fdsetgen.py
--rw-r--r--   0        0        0     7641 2023-05-23 03:43:28.813007 protoletariat-3.2.8/protoletariat/rewrite.py
--rw-r--r--   0        0        0        0 2023-05-23 03:43:28.813007 protoletariat-3.2.8/protoletariat/tests/__init__.py
--rw-r--r--   0        0        0    24371 2023-05-23 03:43:28.813007 protoletariat-3.2.8/protoletariat/tests/conftest.py
--rw-r--r--   0        0        0     7772 2023-05-23 03:43:28.813007 protoletariat-3.2.8/protoletariat/tests/test_fix_imports.py
--rw-r--r--   0        0        0     3004 2023-05-23 03:43:28.813007 protoletariat-3.2.8/protoletariat/tests/test_rewrite.py
--rw-r--r--   0        0        0     3849 2023-05-23 03:44:51.441112 protoletariat-3.2.8/pyproject.toml
--rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 protoletariat-3.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-27 01:03:23.510212 protoletariat-3.2.9/LICENSE
+-rw-r--r--   0        0        0     5066 2023-05-27 01:03:23.510212 protoletariat-3.2.9/README.md
+-rw-r--r--   0        0        0       66 2023-05-27 01:04:27.750120 protoletariat-3.2.9/protoletariat/__init__.py
+-rw-r--r--   0        0        0     4333 2023-05-27 01:03:23.514212 protoletariat-3.2.9/protoletariat/__main__.py
+-rw-r--r--   0        0        0     6661 2023-05-27 01:03:23.514212 protoletariat-3.2.9/protoletariat/fdsetgen.py
+-rw-r--r--   0        0        0     7641 2023-05-27 01:03:23.514212 protoletariat-3.2.9/protoletariat/rewrite.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:03:23.514212 protoletariat-3.2.9/protoletariat/tests/__init__.py
+-rw-r--r--   0        0        0    24371 2023-05-27 01:03:23.514212 protoletariat-3.2.9/protoletariat/tests/conftest.py
+-rw-r--r--   0        0        0     7772 2023-05-27 01:03:23.514212 protoletariat-3.2.9/protoletariat/tests/test_fix_imports.py
+-rw-r--r--   0        0        0     3004 2023-05-27 01:03:23.514212 protoletariat-3.2.9/protoletariat/tests/test_rewrite.py
+-rw-r--r--   0        0        0     3849 2023-05-27 01:04:30.746120 protoletariat-3.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6425 1970-01-01 00:00:00.000000 protoletariat-3.2.9/PKG-INFO
```

### Comparing `protoletariat-3.2.8/LICENSE` & `protoletariat-3.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.8/README.md` & `protoletariat-3.2.9/README.md`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.8/protoletariat/__main__.py` & `protoletariat-3.2.9/protoletariat/__main__.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.8/protoletariat/fdsetgen.py` & `protoletariat-3.2.9/protoletariat/fdsetgen.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.8/protoletariat/rewrite.py` & `protoletariat-3.2.9/protoletariat/rewrite.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.8/protoletariat/tests/conftest.py` & `protoletariat-3.2.9/protoletariat/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.8/protoletariat/tests/test_fix_imports.py` & `protoletariat-3.2.9/protoletariat/tests/test_fix_imports.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.8/protoletariat/tests/test_rewrite.py` & `protoletariat-3.2.9/protoletariat/tests/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `protoletariat-3.2.8/pyproject.toml` & `protoletariat-3.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "protoletariat"
-version = "3.2.8"
+version = "3.2.9"
 packages = [{ include = "protoletariat" }]
 homepage = "https://github.com/cpcloud/protoletariat"
 repository = "https://github.com/cpcloud/protoletariat"
 description = "Python protocol buffers for the rest of us"
 authors = ["Phillip Cloud <417981+cpcloud@users.noreply.github.com>"]
 maintainers = ["Phillip Cloud <417981+cpcloud@users.noreply.github.com>"]
 license = "Apache-2.0"
```

### Comparing `protoletariat-3.2.8/PKG-INFO` & `protoletariat-3.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protoletariat
-Version: 3.2.8
+Version: 3.2.9
 Summary: Python protocol buffers for the rest of us
 Home-page: https://github.com/cpcloud/protoletariat
 License: Apache-2.0
 Author: Phillip Cloud
 Author-email: 417981+cpcloud@users.noreply.github.com
 Maintainer: Phillip Cloud
 Maintainer-email: 417981+cpcloud@users.noreply.github.com
```

