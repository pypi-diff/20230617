# Comparing `tmp/macrometa-target-collection-0.0.78.tar.gz` & `tmp/macrometa-target-collection-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.78.tar", last modified: Sat Jun 17 09:04:23 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.79.tar", last modified: Sat Jun 17 09:14:04 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.78.tar` & `macrometa-target-collection-0.0.79.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17589 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 09:04:23.000000 macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-17 09:04:04.000000 macrometa-target-collection-0.0.78/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 09:04:23.893329 macrometa-target-collection-0.0.78/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:14:04.381694 macrometa-target-collection-0.0.79/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-06-17 09:13:38.000000 macrometa-target-collection-0.0.79/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 09:14:04.381694 macrometa-target-collection-0.0.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 09:13:38.000000 macrometa-target-collection-0.0.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:14:04.381694 macrometa-target-collection-0.0.79/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-17 09:13:38.000000 macrometa-target-collection-0.0.79/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17631 2023-06-17 09:13:38.000000 macrometa-target-collection-0.0.79/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:14:04.381694 macrometa-target-collection-0.0.79/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-17 09:14:04.000000 macrometa-target-collection-0.0.79/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-17 09:14:04.000000 macrometa-target-collection-0.0.79/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:14:04.000000 macrometa-target-collection-0.0.79/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 09:14:04.000000 macrometa-target-collection-0.0.79/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-17 09:14:04.000000 macrometa-target-collection-0.0.79/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 09:14:04.000000 macrometa-target-collection-0.0.79/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-17 09:13:39.000000 macrometa-target-collection-0.0.79/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 09:14:04.385694 macrometa-target-collection-0.0.79/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.78/LICENSE` & `macrometa-target-collection-0.0.79/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.78/PKG-INFO` & `macrometa-target-collection-0.0.79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.78
+Version: 0.0.79
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.78/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.79/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.78/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.79/macrometa_target_collection/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         """Acquire the lock and update last executed time."""
         with self._lock:
             self.last_executed_time = value
 
     def set_is_completed(self, value) -> None:
         """Acquire the lock and set is completed flag."""
         with self._lock:
-            self._is_completed = value
+            self.is_completed = value
 
 
 def emit_state(state):
     if state is not None:
         line = json.dumps(state)
         logger.debug('Emitting state {}'.format(line))
         sys.stdout.write("{}\n".format(line))
@@ -338,15 +338,15 @@
 
 
 async def process_batch(collection: StandardCollection, record_batch: RecordBatch) -> None:
     count = 0
     # As soon as persist_messages is completed process_batch should also exit
     while not record_batch.is_completed:
         count += 1
-        logger.info("***** Entered process batch.....")
+        logger.info(f"***** Entered process batch..... is_completed: {record_batch.is_completed}")
         await asyncio.sleep(record_batch.interval)
         timedelta = datetime.now(timezone.utc) - ensure_datetime(record_batch.last_executed_time)
         if timedelta.total_seconds() >= record_batch.min_time_gap:
             # if batch has records that need to be processed but haven't reached batch size then process them.
             try_upsert(collection, record_batch, force=True)
         if count > 20:
             logger.warn("process batch exception raised..")
```

### Comparing `macrometa-target-collection-0.0.78/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.79/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.78
+Version: 0.0.79
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.78/pyproject.toml` & `macrometa-target-collection-0.0.79/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.78"
+version = "0.0.79"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

