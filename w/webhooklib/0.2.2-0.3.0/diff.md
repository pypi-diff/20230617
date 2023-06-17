# Comparing `tmp/webhooklib-0.2.2.tar.gz` & `tmp/webhooklib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webhooklib-0.2.2.tar", last modified: Sat Jun 17 12:54:35 2023, max compression
+gzip compressed data, was "webhooklib-0.3.0.tar", last modified: Sat Jun 17 13:53:07 2023, max compression
```

## Comparing `webhooklib-0.2.2.tar` & `webhooklib-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:54:35.388586 webhooklib-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 12:54:35.384585 webhooklib-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 12:54:17.000000 webhooklib-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 12:54:17.000000 webhooklib-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 12:54:35.388586 webhooklib-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:54:35.384585 webhooklib-0.2.2/webhooklib/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 12:54:17.000000 webhooklib-0.2.2/webhooklib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-17 12:54:17.000000 webhooklib-0.2.2/webhooklib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 12:54:17.000000 webhooklib-0.2.2/webhooklib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 12:54:17.000000 webhooklib-0.2.2/webhooklib/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 12:54:17.000000 webhooklib-0.2.2/webhooklib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-17 12:54:17.000000 webhooklib-0.2.2/webhooklib/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 12:54:17.000000 webhooklib-0.2.2/webhooklib/process_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 12:54:17.000000 webhooklib-0.2.2/webhooklib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:54:35.384585 webhooklib-0.2.2/webhooklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 12:54:35.000000 webhooklib-0.2.2/webhooklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-17 12:54:35.000000 webhooklib-0.2.2/webhooklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 12:54:35.000000 webhooklib-0.2.2/webhooklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 12:54:35.000000 webhooklib-0.2.2/webhooklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 12:54:35.000000 webhooklib-0.2.2/webhooklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:53:07.349344 webhooklib-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 13:53:07.349344 webhooklib-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 13:52:52.000000 webhooklib-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 13:52:52.000000 webhooklib-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:53:07.349344 webhooklib-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:53:07.349344 webhooklib-0.3.0/webhooklib/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 13:52:52.000000 webhooklib-0.3.0/webhooklib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-17 13:52:52.000000 webhooklib-0.3.0/webhooklib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 13:52:52.000000 webhooklib-0.3.0/webhooklib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-17 13:52:52.000000 webhooklib-0.3.0/webhooklib/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 13:52:52.000000 webhooklib-0.3.0/webhooklib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-17 13:52:52.000000 webhooklib-0.3.0/webhooklib/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-17 13:52:52.000000 webhooklib-0.3.0/webhooklib/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 13:52:52.000000 webhooklib-0.3.0/webhooklib/process_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-17 13:52:52.000000 webhooklib-0.3.0/webhooklib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:53:07.349344 webhooklib-0.3.0/webhooklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-17 13:53:07.000000 webhooklib-0.3.0/webhooklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 13:53:07.000000 webhooklib-0.3.0/webhooklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:53:07.000000 webhooklib-0.3.0/webhooklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-17 13:53:07.000000 webhooklib-0.3.0/webhooklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 13:53:07.000000 webhooklib-0.3.0/webhooklib.egg-info/top_level.txt
```

### Comparing `webhooklib-0.2.2/pyproject.toml` & `webhooklib-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webhooklib"
-version = "0.2.2"
+version = "0.3.0"
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
-current_version = "v0.2.2"
+current_version = "v0.3.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
```

### Comparing `webhooklib-0.2.2/webhooklib/client.py` & `webhooklib-0.3.0/webhooklib/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 from webhooklib import exceptions
 from webhooklib.models import ShellCommand
 from webhooklib.models import ShellResult
 
 ENV_PREFIX = 'WEBHOOK_ENV_'
 
 
+# def wait_n_jobs_quota(redis: Redis, n: int) -> None:
+#     pass
+
+
 def main():
     redis = Redis.from_url(os.environ['REDIS_URL'], decode_responses=True)
 
     url = os.environ['WEBHOOK_URL']
     payload = {
         'cmd': sys.argv[1:],
     }
```

### Comparing `webhooklib-0.2.2/webhooklib/models.py` & `webhooklib-0.3.0/webhooklib/models.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.2.2/webhooklib/process_wrapper.py` & `webhooklib-0.3.0/webhooklib/process_wrapper.py`

 * *Files identical despite different names*

### Comparing `webhooklib-0.2.2/webhooklib/server.py` & `webhooklib-0.3.0/webhooklib/server.py`

 * *Files identical despite different names*

