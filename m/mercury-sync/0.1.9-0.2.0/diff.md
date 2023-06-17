# Comparing `tmp/mercury-sync-0.1.9.tar.gz` & `tmp/mercury-sync-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.1.9.tar", last modified: Sat Jun 17 17:40:03 2023, max compression
+gzip compressed data, was "mercury-sync-0.2.0.tar", last modified: Sat Jun 17 18:19:04 2023, max compression
```

## Comparing `mercury-sync-0.1.9.tar` & `mercury-sync-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.105645 mercury-sync-0.1.9/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.264842 mercury-sync-0.2.0/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:19:04.260842 mercury-sync-0.2.0/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 18:19:04.000000 mercury-sync-0.2.0/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 18:19:04.268842 mercury-sync-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 18:18:58.000000 mercury-sync-0.2.0/setup.py
```

### Comparing `mercury-sync-0.1.9/LICENSE` & `mercury-sync-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/PKG-INFO` & `mercury-sync-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.9
+Version: 0.2.0
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.9/README.md` & `mercury-sync-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.2.0/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pickle
 import socket
 import ssl
 import zstandard
 from collections import deque, defaultdict
 from mercury_sync.encryption import AESGCMFernet
 from mercury_sync.env import Env
+from mercury_sync.env.time_parser import TimeParser
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import (
     Tuple, 
     Deque, 
     Any, 
     Dict, 
@@ -48,16 +49,15 @@
 
         self._client_transports: Dict[str, asyncio.Transport] = {}
         self._server: asyncio.Server = None
         self._loop = asyncio.get_event_loop()
         self.queue: Dict[str, Deque[Tuple[str, int, float, Any]] ] = defaultdict(deque)
         self.parsers: Dict[str, Message] = {}
         self._waiters: Dict[str, Deque[asyncio.Future]] = defaultdict(deque)
-        self._pending_responses: Dict[str, Deque[asyncio.Task]] = defaultdict(deque)
-        self._pending_exceptions: Deque[asyncio.Task] = deque()
+        self._pending_responses: Deque[asyncio.Task]= deque()
         self._last_call: Deque[str] = deque()
 
         self._sent_values = deque()
         self.connected = False
         self._server_socket = None
         self._stream = False
         
@@ -69,22 +69,28 @@
         
         self._client_ssl_context: Union[ssl.SSLContext, None] = None
         self._server_ssl_context: Union[ssl.SSLContext, None] = None
         
         self._encryptor = AESGCMFernet(env)
         self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
         self._compressor = zstandard.ZstdCompressor()
+
         self._decompressor = zstandard.ZstdDecompressor()
+        self._running = False
+        self._cleanup_task: Union[asyncio.Task, None] = None
+        self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
 
     def connect(
         self,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ):
 
+        self._running = True
+
         if cert_path and key_path:
             self._server_ssl_context = self._create_server_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path
             ) 
 
         if self.connected is False:
@@ -103,14 +109,16 @@
                 ssl=self._server_ssl_context
             )
 
             self._server = self._loop.run_until_complete(server)
 
             self.connected = True
 
+            self._cleanup_task = self._loop.create_task(self._cleanup())
+
     def _create_server_ssl_context(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ) -> ssl.SSLContext:
         
         if self._server_cert_path is None:
@@ -183,14 +191,22 @@
         ssl_ctx.load_cert_chain(cert_path, keyfile=key_path)
         ssl_ctx.load_verify_locations(cafile=cert_path)
         ssl_ctx.check_hostname = False
         ssl_ctx.verify_mode = ssl.VerifyMode.CERT_REQUIRED
         ssl_ctx.set_ciphers('ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384')
 
         return ssl_ctx
+    
+    async def _cleanup(self):
+        while self._running:
+            await asyncio.sleep(self._cleanup_interval)
+
+            for pending in list(self._pending_responses):
+                if pending.done() or pending.cancelled():
+                    self._pending_responses.pop()
 
     async def send(
         self, 
         event_name: bytes,
         data: bytes, 
         address: Tuple[str, int]
     ) -> Tuple[int, Dict[str, Any]]:
@@ -341,15 +357,15 @@
     ) -> None:
         decompressed = b''
 
         try:
             decompressed = self._decompressor.decompress(data)
 
         except Exception as decompression_error:
-            self._pending_exceptions.append(
+            self._pending_responses.append(
                 asyncio.create_task(
                     self._send_error(
                         error_message=str(decompression_error),
                         transport=transport
                     )
                 )
             )
@@ -381,15 +397,15 @@
             event_name,
             payload, 
             incoming_host, 
             incoming_port
         ) = result
 
         if message_type == 'request':
-            self._pending_responses[event_name].append(
+            self._pending_responses.append(
                 asyncio.create_task(
                     self._read(
                         event_name,
                         self.events.get(event_name)(
                             shard_id,
                             self.parsers[event_name](**payload)
                         ),
@@ -405,15 +421,15 @@
                 shard_id,
                 event_name,
                 payload, 
                 incoming_host,
                 incoming_port
             ))
 
-            self._pending_responses[event_name].append(
+            self._pending_responses.append(
                 asyncio.create_task(
                     self._initialize_stream(
                         event_name,
                         transport
                     )
                 )
             )
@@ -431,15 +447,15 @@
                 shard_id,
                 event_name,
                 payload, 
                 incoming_host,
                 incoming_port
             ))
 
-            self._pending_responses[event_name].append(
+            self._pending_responses.append(
                 asyncio.create_task(
                     self._read_iterator(
                         event_name,
                         self.events.get(event_name)(
                             shard_id,
                             self.parsers[event_name](**payload)
                         ),
@@ -572,11 +588,13 @@
         )
 
         encrypted_message = self._encryptor.encrypt(item)
         compressed = self._compressor.compress(encrypted_message)
 
         transport.write(compressed)
         
-    def close(self) -> None:
+    async def close(self) -> None:
         self._stream = False
+        self._running = False
+        await self._cleanup_task
```

### Comparing `mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.2.0/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.2.0/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import ssl
 import zstandard
 from collections import deque, defaultdict
 from dtls import do_patch
 from mercury_sync.connection.udp.protocols import MercurySyncUDPProtocol
 from mercury_sync.encryption import AESGCMFernet
 from mercury_sync.env import Env
+from mercury_sync.env.time_parser import TimeParser
 from mercury_sync.models.message import Message
 from mercury_sync.snowflake.snowflake_generator import SnowflakeGenerator
 from typing import (
     Tuple, 
     Deque, 
     Any, 
     Dict, 
@@ -47,31 +48,37 @@
         ] = {}
 
         self._transport: asyncio.DatagramTransport = None
         self._loop = asyncio.get_event_loop()
         self.queue: Dict[str, Deque[Tuple[str, int, float, Any]] ] = defaultdict(deque)
         self.parsers: Dict[str, Message] = {}
         self._waiters: Dict[str, Deque[asyncio.Future]] = defaultdict(deque)
-        self._pending_requests = deque()
-        self._pending_responses = deque()
+        self._pending_responses: Deque[asyncio.Task] = deque()
 
         self._udp_cert_path: Union[str, None] = None
         self._udp_key_path: Union[str, None] = None
         self._udp_ssl_context: Union[ssl.SSLContext, None] = None
 
         self._encryptor = AESGCMFernet(env)
         self._semaphore = asyncio.Semaphore(env.MERCURY_SYNC_MAX_CONCURRENCY)
         self._compressor = zstandard.ZstdCompressor()
         self._decompressor = zstandard.ZstdDecompressor()
+        
+        self._running = False
+        self._cleanup_task: Union[asyncio.Task, None] = None
+        self._cleanup_interval = TimeParser(env.MERCURY_SYNC_CLEANUP_INTERVAL).time
+
 
     def connect(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ) -> None:
+        
+        self._running = True
 
         udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
         udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
         if cert_path and key_path:
             self._udp_ssl_context = self._create_udp_ssl_context(
                 cert_path=cert_path,
@@ -93,14 +100,16 @@
             ),
             sock=udp_socket
         )
 
         transport, _ = self._loop.run_until_complete(server)
         self._transport = transport
 
+        self._cleanup_task = self._loop.create_task(self._cleanup())
+
     def _create_udp_ssl_context(
         self,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
     ) -> ssl.SSLContext: 
         
         if self._udp_cert_path is None:
@@ -118,14 +127,22 @@
         ssl_ctx.load_verify_locations(cafile=cert_path)
         ssl_ctx.check_hostname = False
         ssl_ctx.verify_mode = ssl.VerifyMode.CERT_REQUIRED
         ssl_ctx.set_ciphers('ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384')
         
         return ssl_ctx
     
+    async def _cleanup(self):
+        while self._running:
+            await asyncio.sleep(self._cleanup_interval)
+
+            for pending in list(self._pending_responses):
+                if pending.done() or pending.cancelled():
+                    self._pending_responses.pop()
+    
     async def send(
         self, 
         event_name: str,
         data: Any, 
         addr: Tuple[str, int]
     ) -> Tuple[int, Dict[str, Any]]:
 
@@ -319,9 +336,10 @@
             )
 
             encrypted_message = self._encryptor.encrypt(item)
             compressed = self._compressor.compress(encrypted_message)
 
             self._transport.sendto(compressed, addr)
 
-    def close(self) -> None:
-        pass
+    async def close(self) -> None:
+        self._running = False
+        await self._cleanup_task
```

### Comparing `mercury-sync-0.1.9/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.2.0/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.2.0/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/env/env.py` & `mercury-sync-0.2.0/mercury_sync/env/env.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 )
 
 
 PrimaryType = Union[str, int, float, bytes, bool]
 
 
 class Env(BaseModel):
+    MERCURY_SYNC_CLEANUP_INTERVAL: StrictStr='10s'
     MERCURY_SYNC_MAX_CONCURRENCY: StrictInt=2048
     MERCURY_SYNC_AUTH_SECRET: StrictStr
 
     @classmethod
     def types_map(self) -> Dict[str, Callable[[str], PrimaryType]]:
         return {
+            'MERCURY_SYNC_CLEANUP_INTERVAL': str,
             'MERCURY_SYNC_MAX_CONCURRENCY': int,
             'MERCURY_SYNC_AUTH_SECRET': str
         }
```

### Comparing `mercury-sync-0.1.9/mercury_sync/env/load_env.py` & `mercury-sync-0.2.0/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/env/time_parser.py` & `mercury-sync-0.2.0/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.2.0/mercury_sync/hooks/client_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.2.0/mercury_sync/hooks/stream_hook.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/service/service.py` & `mercury-sync-0.2.0/mercury_sync/service/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,9 +244,9 @@
             response_data = self._response_parsers.get(event_name)(
                 **data
             )
 
             yield shard_id, response_data
     
     async def close(self) -> None:
-        self._tcp_connection.close()
-        self._udp_connection.close()
+        await self._tcp_connection.close()
+        await self._udp_connection.close()
```

### Comparing `mercury-sync-0.1.9/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.2.0/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.2.0/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.2.0/mercury_sync.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.9
+Version: 0.2.0
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.9/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.2.0/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.9/setup.py` & `mercury-sync-0.2.0/setup.py`

 * *Files identical despite different names*

