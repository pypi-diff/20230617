# Comparing `tmp/webhooklib-0.2.0.tar.gz` & `tmp/webhooklib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.2.0.tar", last modified: Sat Jun 17 06:20:33 2023, max compression
+gzip compressed data, was "webhooklib-0.2.1.tar", last modified: Sat Jun 17 11:25:47 2023, max compression
```

## Comparing `webhooklib-0.2.0.tar` & `webhooklib-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:20:33.017095 webhooklib-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 06:20:33.017095 webhooklib-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 06:20:15.000000 webhooklib-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-17 06:20:15.000000 webhooklib-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 06:20:33.017095 webhooklib-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:20:33.013095 webhooklib-0.2.0/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 06:20:15.000000 webhooklib-0.2.0/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-17 06:20:15.000000 webhooklib-0.2.0/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 06:20:15.000000 webhooklib-0.2.0/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 06:20:15.000000 webhooklib-0.2.0/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-17 06:20:15.000000 webhooklib-0.2.0/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-17 06:20:15.000000 webhooklib-0.2.0/webhooklib/process_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 06:20:15.000000 webhooklib-0.2.0/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-17 06:20:15.000000 webhooklib-0.2.0/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:20:33.013095 webhooklib-0.2.0/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 06:20:33.000000 webhooklib-0.2.0/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-17 06:20:33.000000 webhooklib-0.2.0/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:20:33.000000 webhooklib-0.2.0/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 06:20:33.000000 webhooklib-0.2.0/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 06:20:33.000000 webhooklib-0.2.0/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:25:47.148180 webhooklib-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 11:25:47.148180 webhooklib-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 11:25:32.000000 webhooklib-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 11:25:32.000000 webhooklib-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 11:25:47.148180 webhooklib-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:25:47.148180 webhooklib-0.2.1/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 11:25:32.000000 webhooklib-0.2.1/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-17 11:25:32.000000 webhooklib-0.2.1/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 11:25:32.000000 webhooklib-0.2.1/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 11:25:32.000000 webhooklib-0.2.1/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 11:25:32.000000 webhooklib-0.2.1/webhooklib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-17 11:25:32.000000 webhooklib-0.2.1/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-17 11:25:32.000000 webhooklib-0.2.1/webhooklib/process_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 11:25:32.000000 webhooklib-0.2.1/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 11:25:32.000000 webhooklib-0.2.1/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:25:47.148180 webhooklib-0.2.1/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 11:25:47.000000 webhooklib-0.2.1/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-17 11:25:47.000000 webhooklib-0.2.1/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:25:47.000000 webhooklib-0.2.1/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 11:25:47.000000 webhooklib-0.2.1/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 11:25:47.000000 webhooklib-0.2.1/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.2.0/pyproject.toml` & `webhooklib-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webhooklib"
-version = "0.2.0"
+version = "0.2.1"
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
-current_version = "v0.2.0"
+current_version = "v0.2.1"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
@@ -69,14 +69,16 @@
     "D", #docstrings
     "Q", # quotes
     "ARG005", # Unused lambda argument
     "PTH123", # `open()` should be replaced by `Path.open()`
     "N812", # lowercase imported as non lowercase
     "T201",
     "S113",
+    "A003",
+    "G004",
 ]
 
 [tool.ruff.per-file-ignores]
 "examples/*" = ["INP001"]
 "tests/*" = ["S101", "PLR2004"]
 
 [tool.ruff.isort]
@@ -101,14 +103,15 @@
     "unspecified-encoding",
     "wildcard-import",
     "unused-wildcard-import",
     "keyword-arg-before-vararg",
     "too-few-public-methods",
     "consider-using-with",
     "import-error",
+    "logging-fstring-interpolation",
 ]
 
 [tool.pylint-per-file-ignores]
 "server.py" = "import-error"
 
 # ==============================================================================
```

### Comparing `webhooklib-0.2.0/webhooklib/client.py` & `webhooklib-0.2.1/webhooklib/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 
 import requests
 from redis import Redis
 
 from webhooklib import config
+from webhooklib import exceptions
 from webhooklib.models import ShellCommand
 from webhooklib.models import ShellResult
 
 ENV_PREFIX = 'WEBHOOK_ENV_'
 
 
 def main():
@@ -35,20 +36,23 @@
     response = requests.post(url, headers=headers, json=command.dict())
 
     if not response.ok:
         print(response.status_code)
         print(response.text)
         raise SystemExit(1)
 
-    assert response.json() == {'process-created': 'ok'}
+    if response.json() != {'process-created': 'ok'}:
+        raise exceptions.ProcessCreateError(response.text)
+
     print(response.json())
     key = f'{config.PROCESS_DONE}:{command.id}'
     print(key)
     _, message = redis.brpop(key)
     result = ShellResult.parse_raw(message)
-    print(result)
-    assert result.returncode == 0
+    result.pprint()
+    if result.returncode != 0:
+        raise exceptions.ProcessResultError
     redis.delete(key)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `webhooklib-0.2.0/webhooklib/process_wrapper.py` & `webhooklib-0.2.1/webhooklib/process_wrapper.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.2.0/webhooklib/server.py` & `webhooklib-0.2.1/webhooklib/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import logging
 import os
 import secrets
 import shutil
 from pathlib import Path
 from threading import Thread
```

