# Comparing `tmp/mercury-sync-0.1.7.tar.gz` & `tmp/mercury-sync-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.1.7.tar", last modified: Fri Jun 16 05:35:29 2023, max compression
+gzip compressed data, was "mercury-sync-0.1.8.tar", last modified: Sat Jun 17 15:35:11 2023, max compression
```

## Comparing `mercury-sync-0.1.7.tar` & `mercury-sync-0.1.8.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:35:29.259392 mercury-sync-0.1.7/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 05:35:29.000000 mercury-sync-0.1.7/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 05:35:29.263392 mercury-sync-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-16 05:35:24.000000 mercury-sync-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/setup.py
```

### Comparing `mercury-sync-0.1.7/LICENSE` & `mercury-sync-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/PKG-INFO` & `mercury-sync-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.7
+Version: 0.1.8
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.7/README.md` & `mercury-sync-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.1.8/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 import asyncio
-import base64
 import pickle
 import socket
 import ssl
-import zlib
+import zstandard
 from collections import deque, defaultdict
 from mercury_sync.encryption import AESGCMFernet
 from mercury_sync.env import Env
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import (
     Tuple, 
@@ -50,14 +49,16 @@
         self._client_transports: Dict[str, asyncio.Transport] = {}
         self._server: asyncio.Server = None
         self._loop = asyncio.get_event_loop()
         self.queue: Dict[str, Deque[Tuple[str, int, float, Any]] ] = defaultdict(deque)
         self.parsers: Dict[str, Message] = {}
         self._waiters: Dict[str, Deque[asyncio.Future]] = defaultdict(deque)
         self._pending_responses: Dict[str, Deque[asyncio.Task]] = defaultdict(deque)
+        self._pending_exceptions: Deque[asyncio.Task] = deque()
+        self._last_call: Deque[str] = deque()
 
         self._sent_values = deque()
         self.connected = False
         self._server_socket = None
         self._stream = False
         
         self._client_key_path: Union[str, None] = None
@@ -67,14 +68,16 @@
         self._server_cert_path: Union[str, None] = None 
         
         self._client_ssl_context: Union[ssl.SSLContext, None] = None
         self._server_ssl_context: Union[ssl.SSLContext, None] = None
         
         self._encryptor = AESGCMFernet(env)
         self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
+        self._compressor = zstandard.ZstdCompressor()
+        self._decompressor = zstandard.ZstdDecompressor()
 
     def connect(
         self,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ):
 
@@ -189,27 +192,29 @@
         self, 
         event_name: bytes,
         data: bytes, 
         address: Tuple[str, int]
     ) -> str:
         
         async with self._semaphore:
+            self._last_call.append(event_name)
+
             client_transport = self._client_transports.get(address)
 
             item = pickle.dumps((
                 'request',
                 next(self.id_generator),
                 event_name,
                 data,
                 self.host,
                 self.port
             ))
 
             encrypted_message = self._encryptor.encrypt(item)
-            compressed = zlib.compress(encrypted_message)
+            compressed = self._compressor.compress(encrypted_message)
 
             client_transport.write(compressed)
 
             waiter = self._loop.create_future()
             self._waiters[event_name].append(waiter)
 
             await waiter
@@ -232,14 +237,16 @@
         self, 
         event_name: str,
         data: Any, 
         address: Tuple[str, int]
     ): 
         
         async with self._semaphore:
+            self._last_call.append(event_name)
+
             client_transport = self._client_transports.get(address)
 
 
             if self._stream is False:
                 item = pickle.dumps((
                     'stream_connect',
                     next(self.id_generator),
@@ -257,15 +264,15 @@
                     event_name,
                     data,
                     self.host,
                     self.port
                 ))
 
             encrypted_message = self._encryptor.encrypt(item)
-            compressed = zlib.compress(encrypted_message)
+            compressed = self._compressor.compress(encrypted_message)
 
             client_transport.write(compressed)
 
             waiter = self._loop.create_future()
             self._waiters[event_name].append(waiter)
 
             await waiter
@@ -282,15 +289,15 @@
                     event_name,
                     data,
                     self.host,
                     self.port
                 ))
 
                 encrypted_message = self._encryptor.encrypt(item)
-                compressed = zlib.compress(encrypted_message)
+                compressed = self._compressor.compress(encrypted_message)
 
                 client_transport.write(compressed)
 
                 waiter = self._loop.create_future()
                 self._waiters[event_name].append(waiter)
 
                 await waiter
@@ -316,17 +323,40 @@
         self.queue.clear()
 
     def read(
         self,
         data: bytes,
         transport: asyncio.Transport
     ):
-        decrypted = self._encryptor.decrypt(
-            zlib.decompress(data)
-        )
+        decompressed = b''
+
+        try:
+            decompressed = self._decompressor.decompress(data)
+
+        except Exception as decompression_error:
+            self._pending_exceptions.append(
+                asyncio.create_task(
+                    self._send_error(
+                        error_message=str(decompression_error),
+                        transport=transport
+                    )
+                )
+            )
+
+            if len(self._last_call) > 0:
+                event_name = self._last_call.pop()
+                event_waiter = self._waiters[event_name]
+
+                if len(event_waiter) > 0:
+                    waiter = event_waiter.pop()
+                    waiter.set_result(None)
+
+            return
+
+        decrypted = self._encryptor.decrypt(decompressed)
 
         result: Tuple[
             str, 
             int, 
             float, 
             Any, 
             str, 
@@ -410,14 +440,18 @@
 
             if len(event_waiter) > 0:
                 waiter = event_waiter.pop()
                 waiter.set_result(None)
 
 
         else:
+
+            if event_name is None and len(self._last_call) > 0:
+                event_name = self._last_call.pop()
+
             self.queue[event_name].append((
                 message_type, 
                 shard_id,
                 event_name,
                 payload, 
                 incoming_host,
                 incoming_port
@@ -446,15 +480,15 @@
                 response.to_data(), 
                 self.host,
                 self.port
             )
         )
 
         encrypted_message = self._encryptor.encrypt(item)
-        compressed = zlib.compress(encrypted_message)
+        compressed = self._compressor.compress(encrypted_message)
 
         transport.write(compressed)
 
     async def _read_iterator(
         self,
         event_name: str,
         coroutine: AsyncIterable[Message],
@@ -470,15 +504,15 @@
                     response.to_data(), 
                     self.host,
                     self.port
                 )
             )
 
             encrypted_message = self._encryptor.encrypt(item)
-            compressed = zlib.compress(encrypted_message)
+            compressed = self._compressor.compress(encrypted_message)
 
             transport.write(compressed)
 
     async def _initialize_stream(
         self,
         event_name: str,
         transport: asyncio.Transport            
@@ -492,15 +526,42 @@
                 message.to_data(), 
                 self.host,
                 self.port
             )
         )
 
         encrypted_message = self._encryptor.encrypt(item)
-        compressed = zlib.compress(encrypted_message)
+        compressed = self._compressor.compress(encrypted_message)
+
+        transport.write(compressed)
+
+    async def _send_error(
+        self,
+        error_message: str,
+        transport: asyncio.Transport
+    ):
+        error = Message(
+            host=self.host,
+            port=self.port,
+            error=error_message
+        )
+
+        item = pickle.dumps(
+            (
+                'response', 
+                next(self.id_generator),
+                None,
+                error.to_data(), 
+                self.host,
+                self.port
+            )
+        )
+
+        encrypted_message = self._encryptor.encrypt(item)
+        compressed = self._compressor.compress(encrypted_message)
 
         transport.write(compressed)
         
     def close(self):
         self._stream = False
```

### Comparing `mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.1.8/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import asyncio
 import pickle
 import socket
 import ssl
-import zlib
+import zstandard
 from collections import deque, defaultdict
 from dtls import do_patch
 from mercury_sync.connection.udp.protocols import MercurySyncUDPProtocol
 from mercury_sync.encryption import AESGCMFernet
 from mercury_sync.env import Env
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
@@ -56,14 +56,16 @@
 
         self._udp_cert_path: Union[str, None] = None
         self._udp_key_path: Union[str, None] = None
         self._udp_ssl_context: Union[ssl.SSLContext, None] = None
 
         self._encryptor = AESGCMFernet(env)
         self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
+        self._compressor = zstandard.ZstdCompressor()
+        self._decompressor = zstandard.ZstdDecompressor()
 
     def connect(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ):
 
@@ -131,15 +133,15 @@
             'request',
             next(self.id_generator),
             event_name,
             data
         ))
 
         encrypted_message = self._encryptor.encrypt(item)
-        compressed = zlib.compress(encrypted_message)
+        compressed = self._compressor.compress(encrypted_message)
         
         self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
         await waiter
@@ -169,15 +171,15 @@
             'stream',
             next(self.id_generator),
             event_name,
             data
         ))
 
         encrypted_message = self._encryptor.encrypt(item)
-        compressed = zlib.compress(encrypted_message)
+        compressed = self._compressor.compress(encrypted_message)
         
         self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
         self._waiters[event_name].append(waiter)
 
         await waiter
@@ -202,15 +204,15 @@
     def read(
         self,
         data: bytes, 
         addr: Tuple[str, int]
     ):
         
         decrypted = self._encryptor.decrypt(
-            zlib.decompress(data)
+            self._decompressor.decompress(data)
         )
 
         result: Tuple[
             str, 
             int, 
             float, 
             Any, 
@@ -289,15 +291,15 @@
                 next(self.id_generator),
                 event_name,
                 response.to_data()
             )
         )
 
         encrypted_message = self._encryptor.encrypt(item)
-        compressed = zlib.compress(encrypted_message)
+        compressed = self._compressor.compress(encrypted_message)
 
         self._transport.sendto(compressed, addr)
 
     async def _read_iterator(
         self,
         event_name: str,
         coroutine: AsyncIterable[Message],
@@ -311,13 +313,13 @@
                     next(self.id_generator),
                     event_name,
                     response.to_data()
                 )
             )
 
             encrypted_message = self._encryptor.encrypt(item)
-            compressed = zlib.compress(encrypted_message)
+            compressed = self._compressor.compress(encrypted_message)
 
             self._transport.sendto(compressed, addr)
 
     def close(self):
         pass
```

### Comparing `mercury-sync-0.1.7/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.1.8/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.1.8/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/env/env.py` & `mercury-sync-0.1.8/mercury_sync/env/env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/env/load_env.py` & `mercury-sync-0.1.8/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/env/time_parser.py` & `mercury-sync-0.1.8/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.1.8/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.1.8/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/service/service.py` & `mercury-sync-0.1.8/mercury_sync/service/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import random
 import inspect
 import signal
 from inspect import signature
 from mercury_sync.connection.tcp.mercury_sync_tcp_connection import MercurySyncTCPConnection
 from mercury_sync.connection.udp.mercury_sync_udp_connection import MercurySyncUDPConnection
 from mercury_sync.env import load_env, Env
+from mercury_sync.models.error import Error
 from mercury_sync.models.message import Message
 from typing import (
     Tuple, 
     Dict, 
     Optional,
     get_args
 )
@@ -181,14 +182,18 @@
 
         shard_id, data = await self._tcp_connection.send(
             event_name,
             message.to_data(),
             address
         )
 
+
+        if data.get('error'):
+            return shard_id,  Error(**data)
+
         response_data = self._response_parsers.get(event_name)(
             **data
         )
         return shard_id, response_data
     
     async def stream(
         self,
@@ -226,14 +231,18 @@
 
         async for response in self._tcp_connection.stream(
             event_name,
             message.to_data(),
             address
         ):
             shard_id, data = response
+
+            if data.get('error'):
+                yield shard_id, Error(**data)
+
             response_data = self._response_parsers.get(event_name)(
                 **data
             )
 
             yield shard_id, response_data
     
     async def close(self):
```

### Comparing `mercury-sync-0.1.7/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.1.8/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.1.8/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.7/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.1.8/mercury_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.7
+Version: 0.1.8
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.7/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.1.8/mercury_sync.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 mercury_sync/env/load_env.py
 mercury_sync/env/time_parser.py
 mercury_sync/hooks/__init__.py
 mercury_sync/hooks/client_hook.py
 mercury_sync/hooks/server_hook.py
 mercury_sync/hooks/stream_hook.py
 mercury_sync/models/__init__.py
+mercury_sync/models/error.py
 mercury_sync/models/message.py
 mercury_sync/service/__init__.py
 mercury_sync/service/service.py
 mercury_sync/snowflake/__init__.py
 mercury_sync/snowflake/constants.py
 mercury_sync/snowflake/snowflake.py
 mercury_sync/snowflake/snowflake_generator.py
```

### Comparing `mercury-sync-0.1.7/setup.py` & `mercury-sync-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,11 +37,12 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
     install_requires=[
         'pydantic',
-        'python3-dtls'
+        'python3-dtls',
+        'zstandard'
     ],
     python_requires='>=3.10'
 )
```

