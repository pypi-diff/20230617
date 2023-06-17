# Comparing `tmp/mercury-sync-0.2.0.tar.gz` & `tmp/mercury-sync-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.2.0.tar", last modified: Sat Jun 17 18:19:04 2023, max compression
+gzip compressed data, was "mercury-sync-0.2.1.tar", last modified: Sat Jun 17 18:44:34 2023, max compression
```

## Comparing `mercury-sync-0.2.0.tar` & `mercury-sync-0.2.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17860 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 18:44:34.000000 mercury-sync-0.2.1/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-17 18:44:34.000000 mercury-sync-0.2.1/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:44:34.000000 mercury-sync-0.2.1/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 18:44:34.000000 mercury-sync-0.2.1/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 18:44:34.000000 mercury-sync-0.2.1/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 18:44:34.221310 mercury-sync-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 18:44:31.000000 mercury-sync-0.2.1/setup.py
```

### Comparing `mercury-sync-0.2.0/LICENSE` & `mercury-sync-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/PKG-INFO` & `mercury-sync-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.2.0
+Version: 0.2.1
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.2.0/README.md` & `mercury-sync-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.2.1/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         self._encryptor = AESGCMFernet(env)
         self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
         self._compressor = zstandard.ZstdCompressor()
 
         self._decompressor = zstandard.ZstdDecompressor()
         self._running = False
         self._cleanup_task: Union[asyncio.Task, None] = None
+        self._sleep_task: Union[asyncio.Task, None] = None
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
 
     def connect(
         self,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ):
@@ -194,15 +195,19 @@
         ssl_ctx.verify_mode = ssl.VerifyMode.CERT_REQUIRED
         ssl_ctx.set_ciphers('ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384')
 
         return ssl_ctx
     
     async def _cleanup(self):
         while self._running:
-            await asyncio.sleep(self._cleanup_interval)
+            self._sleep_task = asyncio.create_task(
+                asyncio.sleep(self._cleanup_interval)
+            )
+
+            await self._sleep_task
 
             for pending in list(self._pending_responses):
                 if pending.done() or pending.cancelled():
                     self._pending_responses.pop()
 
     async def send(
         self, 
@@ -591,10 +596,26 @@
         compressed = self._compressor.compress(encrypted_message)
 
         transport.write(compressed)
         
     async def close(self) -> None:
         self._stream = False
         self._running = False
-        await self._cleanup_task
+        
+        self._cleanup_task.cancel()
+        if self._cleanup_task.cancelled() is False:
+            try:
+                self._sleep_task.cancel()
+                if not self._sleep_task.cancelled():
+                    await self._sleep_task
+
+            except asyncio.CancelledError:
+                pass
+
+            try:
+
+                await self._cleanup_task
+
+            except asyncio.CancelledError:
+                pass
```

### Comparing `mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.2.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.2.1/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.2.1/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
         self._encryptor = AESGCMFernet(env)
         self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
         self._compressor = zstandard.ZstdCompressor()
         self._decompressor = zstandard.ZstdDecompressor()
         
         self._running = False
         self._cleanup_task: Union[asyncio.Task, None] = None
+        self._sleep_task: Union[asyncio.Task, None] = None
         self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
 
 
     def connect(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
@@ -129,15 +130,19 @@
         ssl_ctx.verify_mode = ssl.VerifyMode.CERT_REQUIRED
         ssl_ctx.set_ciphers('ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384')
         
         return ssl_ctx
     
     async def _cleanup(self):
         while self._running:
-            await asyncio.sleep(self._cleanup_interval)
+            self._sleep_task = asyncio.create_task(
+                asyncio.sleep(self._cleanup_interval)
+            )
+
+            await self._sleep_task
 
             for pending in list(self._pending_responses):
                 if pending.done() or pending.cancelled():
                     self._pending_responses.pop()
     
     async def send(
         self, 
@@ -338,8 +343,24 @@
             encrypted_message = self._encryptor.encrypt(item)
             compressed = self._compressor.compress(encrypted_message)
 
             self._transport.sendto(compressed, addr)
 
     async def close(self) -> None:
         self._running = False
-        await self._cleanup_task
+        
+        self._cleanup_task.cancel()
+        if self._cleanup_task.cancelled() is False:
+            try:
+                self._sleep_task.cancel()
+                if not self._sleep_task.cancelled():
+                    await self._sleep_task
+
+            except asyncio.CancelledError:
+                pass
+
+            try:
+
+                await self._cleanup_task
+
+            except asyncio.CancelledError:
+                pass
```

### Comparing `mercury-sync-0.2.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.2.1/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.2.1/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/env/env.py` & `mercury-sync-0.2.1/mercury_sync/env/env.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-import psutil
 from pydantic import (
     BaseModel,
     StrictStr,
     StrictInt
 )
 from typing import (
-    Optional, 
     Dict, 
     Union,
     Callable
 )
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
```

### Comparing `mercury-sync-0.2.0/mercury_sync/env/load_env.py` & `mercury-sync-0.2.1/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/env/time_parser.py` & `mercury-sync-0.2.1/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.2.1/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.2.1/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/service/service.py` & `mercury-sync-0.2.1/mercury_sync/service/service.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.2.1/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.2.1/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.2.1/mercury_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.2.0
+Version: 0.2.1
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.2.0/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.2.1/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.2.0/setup.py` & `mercury-sync-0.2.1/setup.py`

 * *Files identical despite different names*

