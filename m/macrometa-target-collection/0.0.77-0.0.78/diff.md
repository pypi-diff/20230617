# Comparing `tmp/macrometa-target-collection-0.0.77.tar.gz` & `tmp/macrometa-target-collection-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.77.tar", last modified: Sat Jun 17 08:19:50 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.78.tar", last modified: Sat Jun 17 09:04:23 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.77.tar` & `macrometa-target-collection-0.0.78.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:19:50.832147 macrometa-target-collection-0.0.77/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 08:19:50.832147 macrometa-target-collection-0.0.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:19:50.828147 macrometa-target-collection-0.0.77/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17329 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:19:50.832147 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 08:19:50.000000 macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-17 08:19:21.000000 macrometa-target-collection-0.0.77/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 08:19:50.832147 macrometa-target-collection-0.0.77/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17589 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.77/LICENSE` & `macrometa-target-collection-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.77/PKG-INFO` & `macrometa-target-collection-0.0.78/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.77
+Version: 0.0.78
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.77/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.78/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.77/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.78/macrometa_target_collection/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -178,33 +178,37 @@
 
 
 async def read_stdin() -> AsyncIterable[str]:
     loop = asyncio.get_event_loop()
     reader = asyncio.StreamReader()
     reader_protocol = asyncio.StreamReaderProtocol(reader)
     await loop.connect_read_pipe(lambda: reader_protocol, sys.stdin)
-    while True:
+    while not reader.at_eof():
         line = await reader.readline()
         if not line:
             break
+        if line == b'' and reader.at_eof():
+            logger.info("reached here 2...")
+            break
         yield line.decode('utf-8').rstrip('\r\n')
+    logger.info("reached here 3...")
 
 
 async def persist_messages(collection: StandardCollection,
                            record_batch: RecordBatch, state):
 
     schemas = {}
     key_properties = {}
     validators = {}
     count = 0
 
     messages = read_stdin()
     async for message in messages:
         if not message:
-            break
+            logger.info("reached here 1...")
         try:
             o = json.loads(message)
         except json.decoder.JSONDecodeError as e:
             # Increment ingest_errors metric
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.error(f"Unable to parse:\n{message}")
             raise e
@@ -297,16 +301,18 @@
             validators[stream] = Draft4Validator((o['schema']))
             key_properties[stream] = o['key_properties']
         else:
             # Increment ingest_errors metric
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.warning("Unknown message type {} in message {}".format(o['type'], o))
 
+    logger.info("reached here 4...")
     scrape_complete_flag.labels(workflow_label).inc()
     record_batch.set_is_completed(True)
+    logger.info("reached here 5...")
 
 
 def ensure_datetime(time_extracted):
     if isinstance(time_extracted, str):
         time_extracted = datetime.strptime(time_extracted, "%Y-%m-%dT%H:%M:%S.%fZ")
         # Make the datetime object timezone-aware by setting it to UTC timezone
         time_extracted = time_extracted.replace(tzinfo=timezone.utc)
```

### Comparing `macrometa-target-collection-0.0.77/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.77
+Version: 0.0.78
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.77/pyproject.toml` & `macrometa-target-collection-0.0.78/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.77"
+version = "0.0.78"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

