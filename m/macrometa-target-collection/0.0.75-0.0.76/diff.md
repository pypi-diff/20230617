# Comparing `tmp/macrometa-target-collection-0.0.75.tar.gz` & `tmp/macrometa-target-collection-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.75.tar", last modified: Fri Jun 16 21:41:38 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.76.tar", last modified: Sat Jun 17 07:27:48 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.75.tar` & `macrometa-target-collection-0.0.76.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:41:38.161006 macrometa-target-collection-0.0.75/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-16 21:41:18.000000 macrometa-target-collection-0.0.75/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 21:41:38.161006 macrometa-target-collection-0.0.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 21:41:18.000000 macrometa-target-collection-0.0.75/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:41:38.161006 macrometa-target-collection-0.0.75/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-16 21:41:18.000000 macrometa-target-collection-0.0.75/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17067 2023-06-16 21:41:18.000000 macrometa-target-collection-0.0.75/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 21:41:38.161006 macrometa-target-collection-0.0.75/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-16 21:41:38.000000 macrometa-target-collection-0.0.75/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-16 21:41:38.000000 macrometa-target-collection-0.0.75/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 21:41:38.000000 macrometa-target-collection-0.0.75/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-16 21:41:38.000000 macrometa-target-collection-0.0.75/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 21:41:38.000000 macrometa-target-collection-0.0.75/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 21:41:38.000000 macrometa-target-collection-0.0.75/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-16 21:41:18.000000 macrometa-target-collection-0.0.75/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 21:41:38.161006 macrometa-target-collection-0.0.75/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-17 07:27:26.000000 macrometa-target-collection-0.0.76/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 07:27:26.000000 macrometa-target-collection-0.0.76/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-17 07:27:26.000000 macrometa-target-collection-0.0.76/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17287 2023-06-17 07:27:26.000000 macrometa-target-collection-0.0.76/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 07:27:48.000000 macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-17 07:27:27.000000 macrometa-target-collection-0.0.76/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 07:27:48.324909 macrometa-target-collection-0.0.76/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.75/LICENSE` & `macrometa-target-collection-0.0.76/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.75/PKG-INFO` & `macrometa-target-collection-0.0.76/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.75
+Version: 0.0.76
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.75/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.76/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.75/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.76/macrometa_target_collection/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
 import hashlib
-import io
 import json
 import os
 import re
 import sys
 import time
 from datetime import datetime, timezone
 from threading import Lock
@@ -16,14 +15,15 @@
 import requests
 from adjust_precision_for_schema import adjust_decimal_precision_for_schema
 from c8 import C8Client, DocumentInsertError
 from c8.collection import StandardCollection
 from jsonschema import Draft4Validator
 from prometheus_client import Counter, Gauge, start_http_server
 from singer import get_logger
+from typing import AsyncIterable
 
 from macrometa_target_collection import extract_gdn_host
 
 logger = get_logger('macrometa_target_collection')
 
 DEFAULT_BATCH_SIZE_ROWS = 500
 DEFAULT_BATCH_FLUSH_INTERVAL = 10
@@ -116,15 +116,14 @@
 
 def try_upsert(collection: StandardCollection, record_batch: RecordBatch, force=False):
     if record_batch.length() > 0 and (record_batch.length() >= record_batch.max_batch_size or force):
         logger.info(f"*** Inside try_upsert if condition. ***")
         start_time = time.time()
         insert_end_time = None
         to_insert, to_delete = record_batch.flush()
-        all_records = to_insert
         to_update = []
 
         if len(to_insert) > 0:
             records_array = remove_time_extracted(to_insert)
             for i, r in enumerate(collection.insert_many(records_array)):
                 if type(r) is DocumentInsertError:
                     to_update.append(to_insert[i])
@@ -154,18 +153,18 @@
             start_delete = time.time()
             try_delete(collection, to_delete)
             end_delete = time.time()
             if end_delete - start_delete > 10:
                 logger.info(
                     f"*** Delete Took {end_delete - start_delete}seconds")
         end_time = time.time()
-        if end_time - start_time > 10:
+        if end_time - start_time > 1:
             logger.warn(
                 f"Insert took {insert_end_time - start_time} *** "
-                f"*** Batch Process Took {end_time - start_time}seconds to process:{all_records} ***")
+                f"*** Batch Process Took {end_time - start_time}seconds to process: ***")
     record_batch.update_last_executed_time(datetime.now(timezone.utc))
 
 
 def remove_time_extracted(records):
     return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
 
 
@@ -174,23 +173,36 @@
         collection.delete_many(delete_list)
     except Exception as e:
         # Increment ingest_errors metric
         ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
         logger.warn(f'Failed to delete records with keys: {delete_list}. {e}')
 
 
+async def read_stdin() -> AsyncIterable[str]:
+    loop = asyncio.get_event_loop()
+    reader = asyncio.StreamReader()
+    reader_protocol = asyncio.StreamReaderProtocol(reader)
+    await loop.connect_read_pipe(lambda: reader_protocol, sys.stdin)
+    while True:
+        line = await reader.readline()
+        if not line:
+            break
+        yield line.decode('utf-8').rstrip('\r\n')
+
+
 async def persist_messages(collection: StandardCollection,
-                           messages: io.TextIOWrapper, record_batch: RecordBatch, state):
-    await asyncio.sleep(0)
+                           record_batch: RecordBatch, state):
+
     schemas = {}
     key_properties = {}
     validators = {}
     count = 0
 
-    for message in messages:
+    messages = read_stdin()
+    async for message in messages:
         try:
             o = json.loads(message)
         except json.decoder.JSONDecodeError as e:
             # Increment ingest_errors metric
             ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
             logger.error(f"Unable to parse:\n{message}")
             raise e
@@ -298,18 +310,18 @@
         time_extracted = time_extracted.replace(tzinfo=timezone.utc)
     elif time_extracted.tzinfo is None:
         # If the datetime object is timezone-naive, set it to UTC timezone
         time_extracted = time_extracted.replace(tzinfo=timezone.utc)
     return time_extracted
 
 
-async def setup_batch_task(collection: StandardCollection,  messages: io.TextIOWrapper,
+async def setup_batch_task(collection: StandardCollection,
                            record_batch: RecordBatch, state) -> None:
     event_loop = asyncio.get_event_loop()
-    persist_messages_coro = persist_messages(collection, messages, record_batch, state)
+    persist_messages_coro = persist_messages(collection, record_batch, state)
     asyncio.run_coroutine_threadsafe(persist_messages_coro, event_loop)
     process_batch_coro = process_batch(collection, record_batch)
     asyncio.run_coroutine_threadsafe(process_batch_coro, event_loop)
 
     # Wait for all Futures to complete and propagate any exceptions raised
     await asyncio.gather(
         persist_messages_coro,
@@ -356,16 +368,15 @@
 
     if not client.has_collection(target_collection):
         client.create_collection(name=target_collection)
 
     state = None
     collection = client.get_collection(target_collection)
     record_batch = RecordBatch(config)
-    input_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
-    await setup_batch_task(collection, input_messages, record_batch, state)
+    await setup_batch_task(collection, record_batch, state)
 
     # There can still be records in the `record_batch` which is not processed,
     # So, we have to force process it one last time before the workflow terminates.
     try_upsert(collection, record_batch, force=True)
 
     if is_metrics_enabled.lower() == 'true':
         # Wait for Prometheus to scrape the metrics
```

### Comparing `macrometa-target-collection-0.0.75/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.76/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.75
+Version: 0.0.76
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.75/pyproject.toml` & `macrometa-target-collection-0.0.76/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.75"
+version = "0.0.76"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

