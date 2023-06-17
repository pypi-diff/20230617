# Comparing `tmp/webhooklib-0.3.1.tar.gz` & `tmp/webhooklib-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.3.1.tar", last modified: Sat Jun 17 14:22:08 2023, max compression
+gzip compressed data, was "webhooklib-0.3.2.tar", last modified: Sat Jun 17 14:25:08 2023, max compression
```

## Comparing `webhooklib-0.3.1.tar` & `webhooklib-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:08.331491 webhooklib-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 14:22:08.331491 webhooklib-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 14:21:53.000000 webhooklib-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 14:21:53.000000 webhooklib-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:22:08.331491 webhooklib-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:08.327491 webhooklib-0.3.1/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 14:21:53.000000 webhooklib-0.3.1/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-17 14:21:53.000000 webhooklib-0.3.1/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 14:21:53.000000 webhooklib-0.3.1/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 14:21:53.000000 webhooklib-0.3.1/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 14:21:53.000000 webhooklib-0.3.1/webhooklib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-17 14:21:53.000000 webhooklib-0.3.1/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-17 14:21:53.000000 webhooklib-0.3.1/webhooklib/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 14:21:53.000000 webhooklib-0.3.1/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 14:21:53.000000 webhooklib-0.3.1/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:22:08.327491 webhooklib-0.3.1/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 14:22:08.000000 webhooklib-0.3.1/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 14:22:08.000000 webhooklib-0.3.1/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:22:08.000000 webhooklib-0.3.1/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 14:22:08.000000 webhooklib-0.3.1/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 14:22:08.000000 webhooklib-0.3.1/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:25:08.688144 webhooklib-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 14:25:08.688144 webhooklib-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 14:24:53.000000 webhooklib-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 14:24:53.000000 webhooklib-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:25:08.688144 webhooklib-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:25:08.688144 webhooklib-0.3.2/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 14:24:53.000000 webhooklib-0.3.2/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-17 14:24:53.000000 webhooklib-0.3.2/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 14:24:53.000000 webhooklib-0.3.2/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 14:24:53.000000 webhooklib-0.3.2/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 14:24:53.000000 webhooklib-0.3.2/webhooklib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-17 14:24:53.000000 webhooklib-0.3.2/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-17 14:24:53.000000 webhooklib-0.3.2/webhooklib/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 14:24:53.000000 webhooklib-0.3.2/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 14:24:53.000000 webhooklib-0.3.2/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:25:08.688144 webhooklib-0.3.2/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 14:25:08.000000 webhooklib-0.3.2/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 14:25:08.000000 webhooklib-0.3.2/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:25:08.000000 webhooklib-0.3.2/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 14:25:08.000000 webhooklib-0.3.2/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 14:25:08.000000 webhooklib-0.3.2/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.3.1/pyproject.toml` & `webhooklib-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webhooklib"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = " tool for remote process call"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
@@ -32,15 +32,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [tool.bumpver]
-current_version = "v0.3.1"
+current_version = "v0.3.2"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `webhooklib-0.3.1/webhooklib/client.py` & `webhooklib-0.3.2/webhooklib/client.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.3.1/webhooklib/models.py` & `webhooklib-0.3.2/webhooklib/models.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.3.1/webhooklib/pipeline.py` & `webhooklib-0.3.2/webhooklib/pipeline.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.3.1/webhooklib/process_wrapper.py` & `webhooklib-0.3.2/webhooklib/process_wrapper.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.3.1/webhooklib/server.py` & `webhooklib-0.3.2/webhooklib/server.py`

 * *Files identical despite different names*

