# Comparing `tmp/webhooklib-0.1.7.tar.gz` & `tmp/webhooklib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.1.7.tar", last modified: Thu Jun 15 14:31:03 2023, max compression
+gzip compressed data, was "webhooklib-0.1.9.tar", last modified: Sat Jun 17 04:35:41 2023, max compression
```

## Comparing `webhooklib-0.1.7.tar` & `webhooklib-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:31:03.961381 webhooklib-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 14:31:03.961381 webhooklib-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-15 14:30:45.000000 webhooklib-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-15 14:30:45.000000 webhooklib-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:31:03.961381 webhooklib-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:31:03.961381 webhooklib-0.1.7/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/process_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-15 14:30:45.000000 webhooklib-0.1.7/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:31:03.961381 webhooklib-0.1.7/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-15 14:31:03.000000 webhooklib-0.1.7/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:35:41.771869 webhooklib-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 04:35:41.771869 webhooklib-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 04:35:26.000000 webhooklib-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-17 04:35:26.000000 webhooklib-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 04:35:41.771869 webhooklib-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:35:41.771869 webhooklib-0.1.9/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 04:35:26.000000 webhooklib-0.1.9/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-17 04:35:26.000000 webhooklib-0.1.9/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 04:35:26.000000 webhooklib-0.1.9/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 04:35:26.000000 webhooklib-0.1.9/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-17 04:35:26.000000 webhooklib-0.1.9/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-17 04:35:26.000000 webhooklib-0.1.9/webhooklib/process_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 04:35:26.000000 webhooklib-0.1.9/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-17 04:35:26.000000 webhooklib-0.1.9/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:35:41.771869 webhooklib-0.1.9/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 04:35:41.000000 webhooklib-0.1.9/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-17 04:35:41.000000 webhooklib-0.1.9/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 04:35:41.000000 webhooklib-0.1.9/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 04:35:41.000000 webhooklib-0.1.9/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 04:35:41.000000 webhooklib-0.1.9/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.1.7/pyproject.toml` & `webhooklib-0.1.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webhooklib"
-version = "0.1.7"
+version = "0.1.9"
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
-current_version = "v0.1.7"
+current_version = "v0.1.9"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `webhooklib-0.1.7/webhooklib/client.py` & `webhooklib-0.1.9/webhooklib/client.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.1.7/webhooklib/process_wrapper.py` & `webhooklib-0.1.9/webhooklib/process_wrapper.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.1.7/webhooklib/server.py` & `webhooklib-0.1.9/webhooklib/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,17 +39,18 @@
             detail='access denied: invalid token',
         )
     if shutil.which(command.cmd[0]) is None:
         raise HTTPException(
             status.HTTP_400_BAD_REQUEST,
             detail=f'command {command.cmd[0]} not found',
         )
-    cwd = Path(command.cwd)
-    if not (cwd.is_dir() and cwd.exists()):
-        raise HTTPException(
-            status.HTTP_400_BAD_REQUEST,
-            detail=f'directory {command.cwd} not found',
-        )
+    if command.cwd is not None:
+        cwd = Path(command.cwd)
+        if not (cwd.is_dir() and cwd.exists()):
+            raise HTTPException(
+                status.HTTP_400_BAD_REQUEST,
+                detail=f'directory {command.cwd} not found',
+            )
 
     t = Thread(target=run_subprocess, args=(command, redis))
     t.start()
     return {'process-created': 'ok'}
```

