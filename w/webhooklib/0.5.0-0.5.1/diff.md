# Comparing `tmp/webhooklib-0.5.0.tar.gz` & `tmp/webhooklib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.5.0.tar", last modified: Sat Jun 17 18:51:50 2023, max compression
+gzip compressed data, was "webhooklib-0.5.1.tar", last modified: Sat Jun 17 18:54:48 2023, max compression
```

## Comparing `webhooklib-0.5.0.tar` & `webhooklib-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:51:50.104177 webhooklib-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 18:51:50.104177 webhooklib-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 18:51:29.000000 webhooklib-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 18:51:29.000000 webhooklib-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 18:51:50.104177 webhooklib-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:51:50.100176 webhooklib-0.5.0/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 18:51:29.000000 webhooklib-0.5.0/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-17 18:51:29.000000 webhooklib-0.5.0/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-17 18:51:29.000000 webhooklib-0.5.0/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 18:51:29.000000 webhooklib-0.5.0/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 18:51:29.000000 webhooklib-0.5.0/webhooklib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-17 18:51:29.000000 webhooklib-0.5.0/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-17 18:51:29.000000 webhooklib-0.5.0/webhooklib/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-17 18:51:29.000000 webhooklib-0.5.0/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 18:51:29.000000 webhooklib-0.5.0/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:51:50.104177 webhooklib-0.5.0/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 18:51:50.000000 webhooklib-0.5.0/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 18:51:50.000000 webhooklib-0.5.0/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:51:50.000000 webhooklib-0.5.0/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 18:51:50.000000 webhooklib-0.5.0/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 18:51:50.000000 webhooklib-0.5.0/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:54:48.049708 webhooklib-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 18:54:48.049708 webhooklib-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 18:54:33.000000 webhooklib-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 18:54:33.000000 webhooklib-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 18:54:48.049708 webhooklib-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:54:48.049708 webhooklib-0.5.1/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 18:54:33.000000 webhooklib-0.5.1/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-17 18:54:33.000000 webhooklib-0.5.1/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-17 18:54:33.000000 webhooklib-0.5.1/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 18:54:33.000000 webhooklib-0.5.1/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 18:54:33.000000 webhooklib-0.5.1/webhooklib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-17 18:54:33.000000 webhooklib-0.5.1/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-17 18:54:33.000000 webhooklib-0.5.1/webhooklib/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-17 18:54:33.000000 webhooklib-0.5.1/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 18:54:33.000000 webhooklib-0.5.1/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:54:48.049708 webhooklib-0.5.1/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 18:54:48.000000 webhooklib-0.5.1/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 18:54:48.000000 webhooklib-0.5.1/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:54:48.000000 webhooklib-0.5.1/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 18:54:48.000000 webhooklib-0.5.1/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 18:54:48.000000 webhooklib-0.5.1/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.5.0/pyproject.toml` & `webhooklib-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webhooklib"
-version = "0.5.0"
+version = "0.5.1"
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
-current_version = "v0.5.0"
+current_version = "v0.5.1"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `webhooklib-0.5.0/webhooklib/client.py` & `webhooklib-0.5.1/webhooklib/client.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.5.0/webhooklib/models.py` & `webhooklib-0.5.1/webhooklib/models.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.5.0/webhooklib/pipeline.py` & `webhooklib-0.5.1/webhooklib/pipeline.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.5.0/webhooklib/process_wrapper.py` & `webhooklib-0.5.1/webhooklib/process_wrapper.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.5.0/webhooklib/server.py` & `webhooklib-0.5.1/webhooklib/server.py`

 * *Files identical despite different names*

