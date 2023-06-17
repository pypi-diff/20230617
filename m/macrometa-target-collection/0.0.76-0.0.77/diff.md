# Comparing `tmp/macrometa-target-collection-0.0.76.tar.gz` & `tmp/macrometa-target-collection-0.0.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.76.tar", last modified: Sat Jun 17 07:27:48 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.77.tar", last modified: Sat Jun 17 08:19:50 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.76.tar` & `macrometa-target-collection-0.0.77.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-17 07:27:26.000000 macrometa-target-collection-0.0.76/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 07:27:26.000000 macrometa-target-collection-0.0.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-17 07:27:26.000000 macrometa-target-collection-0.0.76/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17287 2023-06-17 07:27:26.000000 macrometa-target-collection-0.0.76/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-17 07:27:27.000000 macrometa-target-collection-0.0.76/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:19:50.832147 macrometa-target-collection-0.0.77/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 08:19:50.832147 macrometa-target-collection-0.0.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:19:50.828147 macrometa-target-collection-0.0.77/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17329 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:19:50.832147 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 08:19:50.832147 macrometa-target-collection-0.0.77/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.76/LICENSE` & `macrometa-target-collection-0.0.77/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.76/PKG-INFO` & `macrometa-target-collection-0.0.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.76
+Version: 0.0.77
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.76/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.77/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.76/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.77/macrometa_target_collection/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,14 +195,16 @@
     schemas = {}
     key_properties = {}
     validators = {}
     count = 0
 
     messages = read_stdin()
     async for message in messages:
+        if not message:
+            break
         try:
             o = json.loads(message)
         except json.decoder.JSONDecodeError as e:
             # Increment ingest_errors metric
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.error(f"Unable to parse:\n{message}")
             raise e
```

### Comparing `macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.76
+Version: 0.0.77
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.76/pyproject.toml` & `macrometa-target-collection-0.0.77/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.76"
+version = "0.0.77"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

