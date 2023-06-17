# Comparing `tmp/yaman-0.1.0.tar.gz` & `tmp/yaman-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaman-0.1.0.tar", max compression
+gzip compressed data, was "yaman-0.1.1.tar", max compression
```

## Comparing `yaman-0.1.0.tar` & `yaman-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0    35149 2021-07-10 11:17:31.194770 yaman-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     2636 2023-06-17 15:20:42.172670 yaman-0.1.0/README.md
--rw-r--r--   0        0        0      673 2023-06-17 15:28:42.328071 yaman-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0     4047 2023-06-17 15:21:26.726509 yaman-0.1.0/yaman.py
--rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 yaman-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-07-10 11:17:31.194770 yaman-0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     2636 2023-06-17 15:20:42.172670 yaman-0.1.1/README.md
+-rw-r--r--   0        0        0      724 2023-06-17 16:25:10.636680 yaman-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2021-07-10 11:17:31.194770 yaman-0.1.1/src/__init__.py
+-rwxr-xr-x   0        0        0        0 2021-07-10 11:17:31.194770 yaman-0.1.1/src/interface/__init__.py
+-rwxr-xr-x   0        0        0       93 2021-07-10 11:17:31.194770 yaman-0.1.1/src/interface/guake.py
+-rwxr-xr-x   0        0        0     3369 2021-07-10 11:17:31.194770 yaman-0.1.1/src/interface/yakuake.py
+-rwxr-xr-x   0        0        0     2607 2023-06-17 16:15:53.713605 yaman-0.1.1/src/sessionBuilder.py
+-rwxr-xr-x   0        0        0     1520 2021-07-10 11:17:31.194770 yaman-0.1.1/src/sessionManager.py
+-rw-r--r--   0        0        0     3429 1970-01-01 00:00:00.000000 yaman-0.1.1/PKG-INFO
```

### Comparing `yaman-0.1.0/LICENSE` & `yaman-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yaman-0.1.0/README.md` & `yaman-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `yaman-0.1.0/pyproject.toml` & `yaman-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [tool.poetry]
 name = "yaman"
-version = "0.1.0"
+version = "0.1.1"
 description = "Yakuake terminal manager"
 authors = ["Rok Andrée <rok@andree.si>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["terminal", "yakuake"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: POSIX :: Linux",
     "Topic :: Utilities"
 ]
+packages = [
+    { include = "src", from = "." }
+]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 PyYAML = "^6.0"
 click = "^8.1.3"
 
 [build-system]
```

### Comparing `yaman-0.1.0/PKG-INFO` & `yaman-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaman
-Version: 0.1.0
+Version: 0.1.1
 Summary: Yakuake terminal manager
 License: GPLv3
 Keywords: terminal,yakuake
 Author: Rok Andrée
 Author-email: rok@andree.si
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

