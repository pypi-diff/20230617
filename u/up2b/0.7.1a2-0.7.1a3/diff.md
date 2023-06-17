# Comparing `tmp/up2b-0.7.1a2.tar.gz` & `tmp/up2b-0.7.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up2b-0.7.1a2.tar", last modified: Fri Apr 28 12:05:25 2023, max compression
+gzip compressed data, was "up2b-0.7.1a3.tar", last modified: Sat Jun 17 03:07:32 2023, max compression
```

## Comparing `up2b-0.7.1a2.tar` & `up2b-0.7.1a3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.184493 up2b-0.7.1a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.168493 up2b-0.7.1a2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.172493 up2b-0.7.1a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-28 12:05:13.000000 up2b-0.7.1a2/.github/workflows/check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-28 12:05:13.000000 up2b-0.7.1a2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-28 12:05:13.000000 up2b-0.7.1a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-28 12:05:13.000000 up2b-0.7.1a2/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-28 12:05:13.000000 up2b-0.7.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-28 12:05:25.184493 up2b-0.7.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-04-28 12:05:13.000000 up2b-0.7.1a2/README.en_US.md
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-28 12:05:13.000000 up2b-0.7.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-28 12:05:13.000000 up2b-0.7.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 12:05:13.000000 up2b-0.7.1a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 12:05:25.184493 up2b-0.7.1a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.172493 up2b-0.7.1a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.176493 up2b-0.7.1a2/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28768 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/images/1.png
--rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/images/2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/images/3.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 12:05:13.000000 up2b-0.7.1a2/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.176493 up2b-0.7.1a2/up2b/
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.180493 up2b-0.7.1a2/up2b/up2b_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.184493 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/imgtg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/imgtu.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/up2b_api/sm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-28 12:05:13.000000 up2b-0.7.1a2/up2b/up2b_lib/watermark.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 12:05:25.176493 up2b-0.7.1a2/up2b.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 12:05:25.000000 up2b-0.7.1a2/up2b.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.003206 up2b-0.7.1a3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.003206 up2b-0.7.1a3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-17 03:07:21.000000 up2b-0.7.1a3/.github/workflows/check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 03:07:21.000000 up2b-0.7.1a3/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-17 03:07:21.000000 up2b-0.7.1a3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-17 03:07:21.000000 up2b-0.7.1a3/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-17 03:07:21.000000 up2b-0.7.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-17 03:07:32.007206 up2b-0.7.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-17 03:07:21.000000 up2b-0.7.1a3/README.en_US.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-17 03:07:21.000000 up2b-0.7.1a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-17 03:07:21.000000 up2b-0.7.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 03:07:21.000000 up2b-0.7.1a3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 03:07:32.007206 up2b-0.7.1a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.003206 up2b-0.7.1a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28768 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/images/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/images/2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/images/3.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/up2b/
+-rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/up2b/up2b_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/imgtg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/imgtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/sm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/watermark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/up2b.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/top_level.txt
```

### Comparing `up2b-0.7.1a2/.github/workflows/check.yaml` & `up2b-0.7.1a3/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/.github/workflows/publish.yaml` & `up2b-0.7.1a3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/LICENSE` & `up2b-0.7.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/PKG-INFO` & `up2b-0.7.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up2b
-Version: 0.7.1a2
+Version: 0.7.1a3
 Summary: 上传图片到图床
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: up2b Version: 0.7.1a2 Summary:
+Metadata-Version: 2.1 Name: up2b Version: 0.7.1a3 Summary:
 ä¸ä¼ å¾çå°å¾åº Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2021 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `up2b-0.7.1a2/README.en_US.md` & `up2b-0.7.1a3/README.en_US.md`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/README.md` & `up2b-0.7.1a3/README.md`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/pyproject.toml` & `up2b-0.7.1a3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "up2b"
-authors = [
-    {name = "thep0y", email = "thepoy@163.com"},
-]
+authors = [{ name = "thep0y", email = "thepoy@163.com" }]
 description = "上传图片到图床"
 readme = "README.md"
 requires-python = ">=3"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 classifiers = ["Programming Language :: Python :: 3"]
 keywords = ["typora", "image bed", "upload"]
 dependencies = [
     "requests",
     "click",
-    "colorful-logger>=0.2.0a4",
-    "typing_extensions; python_version<'3.8'"
+    "colorful-logger>=0.2.0b1",
+    "typing_extensions; python_version<'3.8'",
 ]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/thep0y/up2b"
 repository = "https://github.com/thep0y/up2b"
 
@@ -46,8 +44,8 @@
 [tool.black]
 line-length = 88
 target-version = ['py36', 'py37', 'py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pyright]
 pythonVersion = '3.11'
-venv = 'dev'
+venv = 'dev'
```

### Comparing `up2b-0.7.1a2/tests/images/1.png` & `up2b-0.7.1a3/tests/images/1.png`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/tests/images/2.jpeg` & `up2b-0.7.1a3/tests/images/2.jpeg`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/tests/images/3.jpeg` & `up2b-0.7.1a3/tests/images/3.jpeg`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/tests/server.py` & `up2b-0.7.1a3/tests/server.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/tests/test_upload.py` & `up2b-0.7.1a3/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/tests/test_utils.py` & `up2b-0.7.1a3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/__init__.py` & `up2b-0.7.1a3/up2b/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,15 +256,18 @@
 def _read_image_bed(
     auto_compress: bool = False,
     add_watermark: bool = False,
     ignore_cache: bool = False,
 ) -> Union[SM, Imgtu, Imgtg, Github]:
     conf = read_conf()
 
-    selected_code = conf["image_bed"]
+    selected_code = conf.get("image_bed")
+    if not selected_code:
+        logger.fatal("当前图床为空，请先选择要使用的图床")
+
     assert isinstance(selected_code, int)
 
     try:
         code = ImageBedCode(selected_code)
 
         return IMAGE_BEDS[code](
             auto_compress=auto_compress,
@@ -313,38 +316,36 @@
                     }
                 )
             )
 
 
 def print_list() -> int:
     conf = read_conf()
-    auth_data: Optional[AuthData] = conf.get("auth_data")  # type: ignore
+    auth_data: AuthData = conf.get("auth_data", {})  # type: ignore
 
     if not auth_data:
         selected_code = conf.get("image_bed")
         if selected_code is None:
-            logger.fatal(
+            logger.warning(
                 "no image bed selected, "
                 + "you need to use `--choose-site` or `-c` to select the image bed first."
             )
 
-        assert isinstance(selected_code, int)
-
-        code = ImageBedCode(selected_code)
+        if selected_code:
+            code = ImageBedCode(selected_code)
 
-        logger.warning(
-            "no authentication information has been configured",
-            image_bed=ds.format_with_multiple_styles(
-                IMAGE_BEDS[code]().__str__(),
-                ds.backgorud_color.dark_gray,
-                ds.foreground_color.white,
-            ),
-            code=selected_code,
-        )
-        return 0
+            logger.warning(
+                "no authentication information has been configured",
+                image_bed=ds.format_with_multiple_styles(
+                    IMAGE_BEDS[code]().__str__(),
+                    ds.backgorud_color.dark_gray,
+                    ds.foreground_color.white,
+                ),
+                code=selected_code,
+            )
 
     def print_item(symbol, color, idx):
         ib = IMAGE_BEDS[ImageBedCode(idx)]()
         click.echo(
             f"""{ds.format_with_one_style(" " + symbol, color)} {idx} {ib}: {ib.description}"""
         )
```

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/cache.py` & `up2b-0.7.1a3/up2b/up2b_lib/cache.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/constants.py` & `up2b-0.7.1a3/up2b/up2b_lib/constants.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/custom_types.py` & `up2b-0.7.1a3/up2b/up2b_lib/custom_types.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/i18n.py` & `up2b-0.7.1a3/up2b/up2b_lib/i18n.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/log.py` & `up2b-0.7.1a3/up2b/up2b_lib/log.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/__init__.py` & `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/__init__.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/__init__.pyi` & `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/__init__.pyi`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/github.py` & `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/github.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/imgtg.py` & `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/imgtg.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/imgtu.py` & `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/imgtu.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/up2b_api/sm.py` & `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/sm.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/utils.py` & `up2b-0.7.1a3/up2b/up2b_lib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,19 +53,21 @@
 
 
 def read_conf() -> ConfigFile:  # type: ignore
     if os.getenv("UP2B_TEST"):
         return {}
 
     if not CONF_FILE.exists():
-        logger.fatal(
+        logger.warning(
             "the configuration file is not found, "
             + "you need to use `--choose-site` or `-c` to select the image bed first."
         )
 
+        return {}
+
     try:
         with CONF_FILE.open(encoding="utf-8") as f:
             conf: ConfigFile = json.loads(f.read())
     except Exception as e:
         logger.fatal("unkown error", err=e)
     else:
         return conf
```

### Comparing `up2b-0.7.1a2/up2b/up2b_lib/watermark.py` & `up2b-0.7.1a3/up2b/up2b_lib/watermark.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a2/up2b.egg-info/PKG-INFO` & `up2b-0.7.1a3/up2b.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up2b
-Version: 0.7.1a2
+Version: 0.7.1a3
 Summary: 上传图片到图床
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: up2b Version: 0.7.1a2 Summary:
+Metadata-Version: 2.1 Name: up2b Version: 0.7.1a3 Summary:
 ä¸ä¼ å¾çå°å¾åº Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2021 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `up2b-0.7.1a2/up2b.egg-info/SOURCES.txt` & `up2b-0.7.1a3/up2b.egg-info/SOURCES.txt`

 * *Files identical despite different names*

