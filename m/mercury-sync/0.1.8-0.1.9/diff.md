# Comparing `tmp/mercury-sync-0.1.8.tar.gz` & `tmp/mercury-sync-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercury-sync-0.1.8.tar", last modified: Sat Jun 17 15:35:11 2023, max compression
+gzip compressed data, was "mercury-sync-0.1.9.tar", last modified: Sat Jun 17 17:40:03 2023, max compression
```

## Comparing `mercury-sync-0.1.8.tar` & `mercury-sync-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/tcp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/udp/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/udp/mercury_sync_udp_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/connection/udp/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/udp/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/encryption/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/encryption/aes_gcm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/env/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/env/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/env/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/env/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/env/time_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/hooks/client_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/hooks/server_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/hooks/stream_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/models/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/models/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/service/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/snowflake/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/snowflake/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/mercury_sync/snowflake/snowflake_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/mercury_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 15:35:11.000000 mercury-sync-0.1.8/mercury_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:35:11.684693 mercury-sync-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 15:35:08.000000 mercury-sync-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.105645 mercury-sync-0.1.9/mercury_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16728 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/udp/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/udp/mercury_sync_udp_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/connection/udp/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/udp/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync/encryption/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/encryption/aes_gcm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/env/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/env/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/env/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/env/time_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/hooks/client_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/hooks/server_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/hooks/stream_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/models/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/mercury_sync/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/snowflake/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/snowflake/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/mercury_sync/snowflake/snowflake_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:40:03.109645 mercury-sync-0.1.9/mercury_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 17:40:03.000000 mercury-sync-0.1.9/mercury_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 17:40:03.113645 mercury-sync-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-17 17:40:00.000000 mercury-sync-0.1.9/setup.py
```

### Comparing `mercury-sync-0.1.8/LICENSE` & `mercury-sync-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/PKG-INFO` & `mercury-sync-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.8/README.md` & `mercury-sync-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py` & `mercury-sync-0.1.9/mercury_sync/connection/tcp/mercury_sync_tcp_connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         return ssl_ctx
 
     async def connect_client(
         self,
         address: Tuple[str, int],
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
-    ):
+    ) -> Coroutine[Any, Any, asyncio.Transport]:
         
         if cert_path and key_path:
             self._client_ssl_context = self._create_client_ssl_context(
                 cert_path=cert_path,
                 key_path=key_path
             ) 
 
@@ -189,29 +189,32 @@
         return ssl_ctx
 
     async def send(
         self, 
         event_name: bytes,
         data: bytes, 
         address: Tuple[str, int]
-    ) -> str:
+    ) -> Tuple[int, Dict[str, Any]]:
         
         async with self._semaphore:
             self._last_call.append(event_name)
 
             client_transport = self._client_transports.get(address)
 
-            item = pickle.dumps((
-                'request',
-                next(self.id_generator),
-                event_name,
-                data,
-                self.host,
-                self.port
-            ))
+            item = pickle.dumps(
+                (
+                    'request',
+                    next(self.id_generator),
+                    event_name,
+                    data,
+                    self.host,
+                    self.port
+                ),
+                protocol=pickle.HIGHEST_PROTOCOL
+            )
 
             encrypted_message = self._encryptor.encrypt(item)
             compressed = self._compressor.compress(encrypted_message)
 
             client_transport.write(compressed)
 
             waiter = self._loop.create_future()
@@ -234,42 +237,48 @@
             )
     
     async def stream(
         self, 
         event_name: str,
         data: Any, 
         address: Tuple[str, int]
-    ): 
+    ) -> AsyncIterable[Tuple[int, Dict[str, Any]]]: 
         
         async with self._semaphore:
             self._last_call.append(event_name)
 
             client_transport = self._client_transports.get(address)
 
 
             if self._stream is False:
-                item = pickle.dumps((
-                    'stream_connect',
-                    next(self.id_generator),
-                    event_name,
-                    data,
-                    self.host,
-                    self.port
-                ))
+                item = pickle.dumps(
+                    (
+                        'stream_connect',
+                        next(self.id_generator),
+                        event_name,
+                        data,
+                        self.host,
+                        self.port
+                    ),
+                    protocol=pickle.HIGHEST_PROTOCOL
+                )
 
 
             else:
-                item = pickle.dumps((
-                    'stream',
-                    next(self.id_generator),
-                    event_name,
-                    data,
-                    self.host,
-                    self.port
-                ))
+                item = pickle.dumps(
+                    (
+                        'stream',
+                        next(self.id_generator),
+                        event_name,
+                        data,
+                        self.host,
+                        self.port
+                    ),
+                    protocol=pickle.HIGHEST_PROTOCOL
+                )
 
             encrypted_message = self._encryptor.encrypt(item)
             compressed = self._compressor.compress(encrypted_message)
 
             client_transport.write(compressed)
 
             waiter = self._loop.create_future()
@@ -279,22 +288,25 @@
 
             if self._stream is False:
 
                 self.queue[event_name].pop()
 
                 self._stream = True
 
-                item = pickle.dumps((
-                    'stream',
-                    next(self.id_generator),
-                    event_name,
-                    data,
-                    self.host,
-                    self.port
-                ))
+                item = pickle.dumps(
+                    (
+                        'stream',
+                        next(self.id_generator),
+                        event_name,
+                        data,
+                        self.host,
+                        self.port
+                    ),
+                    pickle.HIGHEST_PROTOCOL
+                )
 
                 encrypted_message = self._encryptor.encrypt(item)
                 compressed = self._compressor.compress(encrypted_message)
 
                 client_transport.write(compressed)
 
                 waiter = self._loop.create_future()
@@ -322,15 +334,15 @@
 
         self.queue.clear()
 
     def read(
         self,
         data: bytes,
         transport: asyncio.Transport
-    ):
+    ) -> None:
         decompressed = b''
 
         try:
             decompressed = self._decompressor.decompress(data)
 
         except Exception as decompression_error:
             self._pending_exceptions.append(
@@ -465,103 +477,106 @@
                 waiter.set_result(None)
 
     async def _read(
         self,
         event_name: str,
         coroutine: Coroutine,
         transport: asyncio.Transport
-    ):
+    ) -> Coroutine[Any, Any, None]:
         response: Message = await coroutine
 
         item = pickle.dumps(
             (
                 'response', 
                 next(self.id_generator),
                 event_name,
                 response.to_data(), 
                 self.host,
                 self.port
-            )
+            ),
+            protocol=pickle.HIGHEST_PROTOCOL
         )
 
         encrypted_message = self._encryptor.encrypt(item)
         compressed = self._compressor.compress(encrypted_message)
 
         transport.write(compressed)
 
     async def _read_iterator(
         self,
         event_name: str,
         coroutine: AsyncIterable[Message],
         transport: asyncio.Transport       
-    ):
+    ) -> Coroutine[Any, Any, None]:
   
         async for response in coroutine:
             item = pickle.dumps(
                 (
                     'response', 
                     next(self.id_generator),
                     event_name,
                     response.to_data(), 
                     self.host,
                     self.port
-                )
+                ),
+                protocol=pickle.HIGHEST_PROTOCOL
             )
 
             encrypted_message = self._encryptor.encrypt(item)
             compressed = self._compressor.compress(encrypted_message)
 
             transport.write(compressed)
 
     async def _initialize_stream(
         self,
         event_name: str,
         transport: asyncio.Transport            
-    ):
+    ) -> Coroutine[Any, Any, None]:
         message = Message()
         item = pickle.dumps(
             (
                 'response', 
                 next(self.id_generator),
                 event_name,
                 message.to_data(), 
                 self.host,
                 self.port
-            )
+            ),
+            protocol=pickle.HIGHEST_PROTOCOL
         )
 
         encrypted_message = self._encryptor.encrypt(item)
         compressed = self._compressor.compress(encrypted_message)
 
         transport.write(compressed)
 
     async def _send_error(
         self,
         error_message: str,
         transport: asyncio.Transport
-    ):
+    ) -> Coroutine[Any, Any, None]:
+        
         error = Message(
-            host=self.host,
-            port=self.port,
             error=error_message
         )
 
         item = pickle.dumps(
             (
                 'response', 
                 next(self.id_generator),
                 None,
                 error.to_data(), 
                 self.host,
                 self.port
-            )
+            ),
+            protocol=pickle.HIGHEST_PROTOCOL
         )
 
         encrypted_message = self._encryptor.encrypt(item)
         compressed = self._compressor.compress(encrypted_message)
 
         transport.write(compressed)
         
-    def close(self):
+    def close(self) -> None:
         self._stream = False
```

### Comparing `mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py` & `mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_client_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py` & `mercury-sync-0.1.9/mercury_sync/connection/tcp/protocols/mercury_sync_tcp_server_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync/connection/udp/mercury_sync_udp_connection.py` & `mercury-sync-0.1.9/mercury_sync/connection/udp/mercury_sync_udp_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self._compressor = zstandard.ZstdCompressor()
         self._decompressor = zstandard.ZstdDecompressor()
 
     def connect(
         self, 
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
-    ):
+    ) -> None:
 
         udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
         udp_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
         if cert_path and key_path:
             self._udp_ssl_context = self._create_udp_ssl_context(
                 cert_path=cert_path,
@@ -123,22 +123,22 @@
         return ssl_ctx
     
     async def send(
         self, 
         event_name: str,
         data: Any, 
         addr: Tuple[str, int]
-    ) -> Tuple[int, Any]:
+    ) -> Tuple[int, Dict[str, Any]]:
 
         item = pickle.dumps((
             'request',
             next(self.id_generator),
             event_name,
             data
-        ))
+        ), protocol=pickle.HIGHEST_PROTOCOL)
 
         encrypted_message = self._encryptor.encrypt(item)
         compressed = self._compressor.compress(encrypted_message)
         
         self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
@@ -161,22 +161,22 @@
         )
 
     async def stream(
         self, 
         event_name: str,
         data: Any, 
         addr: Tuple[str, int]
-    ): 
+    ) -> AsyncIterable[Tuple[int, Dict[str, Any]]]: 
 
         item = pickle.dumps((
             'stream',
             next(self.id_generator),
             event_name,
             data
-        ))
+        ), protocol=pickle.HIGHEST_PROTOCOL)
 
         encrypted_message = self._encryptor.encrypt(item)
         compressed = self._compressor.compress(encrypted_message)
         
         self._transport.sendto(compressed, addr)
 
         waiter = self._loop.create_future()
@@ -201,15 +201,15 @@
 
         self.queue.clear()
 
     def read(
         self,
         data: bytes, 
         addr: Tuple[str, int]
-    ):
+    ) -> None:
         
         decrypted = self._encryptor.decrypt(
             self._decompressor.decompress(data)
         )
 
         result: Tuple[
             str, 
@@ -278,48 +278,50 @@
 
 
     async def _read(
         self,
         event_name: str,
         coroutine: Coroutine,
         addr: Tuple[str, int]
-    ):
+    ) -> Coroutine[Any, Any, None]:
         response: Message = await coroutine
 
         item = pickle.dumps(
             (
                 'response', 
                 next(self.id_generator),
                 event_name,
                 response.to_data()
-            )
+            ),
+            protocol=pickle.HIGHEST_PROTOCOL
         )
 
         encrypted_message = self._encryptor.encrypt(item)
         compressed = self._compressor.compress(encrypted_message)
 
         self._transport.sendto(compressed, addr)
 
     async def _read_iterator(
         self,
         event_name: str,
         coroutine: AsyncIterable[Message],
         addr: Tuple[str, int]    
-    ):
+    ) -> Coroutine[Any, Any, None]:
         async for response in coroutine:
 
             item = pickle.dumps(
                 (
                     'response', 
                     next(self.id_generator),
                     event_name,
                     response.to_data()
-                )
+                ),
+                protocol=pickle.HIGHEST_PROTOCOL
             )
 
             encrypted_message = self._encryptor.encrypt(item)
             compressed = self._compressor.compress(encrypted_message)
 
             self._transport.sendto(compressed, addr)
 
-    def close(self):
+    def close(self) -> None:
         pass
```

### Comparing `mercury-sync-0.1.8/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py` & `mercury-sync-0.1.9/mercury_sync/connection/udp/protocols/mercury_sync_udp_protocol.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync/encryption/aes_gcm.py` & `mercury-sync-0.1.9/mercury_sync/encryption/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync/env/env.py` & `mercury-sync-0.1.9/mercury_sync/env/env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync/env/load_env.py` & `mercury-sync-0.1.9/mercury_sync/env/load_env.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync/env/time_parser.py` & `mercury-sync-0.1.9/mercury_sync/env/time_parser.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync/hooks/client_hook.py` & `mercury-sync-0.1.9/mercury_sync/hooks/client_hook.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 from mercury_sync.service import Service
+from typing import Dict, Tuple, Any, Coroutine
 
 
 def client(
     call_name: str, 
     as_tcp: bool=False
 ):
```

### Comparing `mercury-sync-0.1.8/mercury_sync/hooks/stream_hook.py` & `mercury-sync-0.1.9/mercury_sync/hooks/stream_hook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
             
 
 import functools
 from mercury_sync.service import Service
-from mercury_sync.models.message import Message
+from typing import Dict, Any, AsyncIterable, Tuple, Coroutine
 
 
 def stream(
     call_name: str, 
     as_tcp: bool=False
 ):
```

### Comparing `mercury-sync-0.1.8/mercury_sync/service/service.py` & `mercury-sync-0.1.9/mercury_sync/service/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 from mercury_sync.env import load_env, Env
 from mercury_sync.models.error import Error
 from mercury_sync.models.message import Message
 from typing import (
     Tuple, 
     Dict, 
     Optional,
-    get_args
+    get_args,
+    Union,
+    AsyncIterable
 )
 
 
 def handle_loop_stop(signame, tcp_connection: MercurySyncTCPConnection):
         try:
             tcp_connection.close()
 
@@ -95,15 +97,15 @@
 
                 is_stream = inspect.isasyncgenfunction(method)
 
                 if is_stream:
 
                     response_type = rpc_signature.return_annotation
                     args = get_args(response_type)
-                    response_model = args[0]
+                    response_model: Message = args[0]
 
                     self._response_parsers[method.target] = response_model
 
                 else:
 
                     response_model = rpc_signature.return_annotation
                     self._response_parsers[method.target] = response_model
@@ -121,41 +123,41 @@
                 )
             )
 
     def start(
         self,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
-    ):
+    ) -> None:
         self._tcp_connection.connect(
             cert_path=cert_path,
             key_path=key_path
         )
         self._udp_connection.connect(cert_path=cert_path)
 
     async def connect(
         self,
         remote: Message,
         cert_path: Optional[str]=None,
         key_path: Optional[str]=None
-    ):
+    ) -> None:
         address = (remote.host, remote.port)
         self._host_map[remote.__class__.__name__] = address
 
         await self._tcp_connection.connect_client(
             (remote.host, remote.port + 1),
             cert_path=cert_path,
             key_path=key_path
         )
 
     async def send(
         self, 
         event_name: str,
         message: Message
-    ):
+    ) -> Tuple[int, Union[Message, Error]]:
         (host, port)  = self._host_map.get(message.__class__.__name__)
         address = (
             host,
             port
         )
 
         shard_id, data = await self._udp_connection.send(
@@ -169,15 +171,15 @@
         )
         return shard_id, response_data
     
     async def send_tcp(
         self,
         event_name: str,
         message: Message
-    ):
+    ) -> Tuple[int, Union[Message, Error]]:
         (host, port)  = self._host_map.get(message.__class__.__name__)
         address = (
             host,
             port + 1
         )
 
         shard_id, data = await self._tcp_connection.send(
@@ -195,15 +197,15 @@
         )
         return shard_id, response_data
     
     async def stream(
         self,
         event_name: str,
         message: Message
-    ):
+    ) -> AsyncIterable[Tuple[int, Union[Message, Error]]]:
         (host, port)  = self._host_map.get(message.__class__.__name__)
         address = (
             host,
             port
         )
 
         async for response in self._udp_connection.stream(
@@ -218,15 +220,15 @@
 
             yield shard_id, response_data
 
     async def stream_tcp(
         self,
         event_name: str,
         message: Message
-    ):
+    ) -> AsyncIterable[Tuple[int, Union[Message, Error]]]:
         (host, port)  = self._host_map.get(message.__class__.__name__)
         address = (
             host,
             port + 1
         )
 
         async for response in self._tcp_connection.stream(
@@ -241,10 +243,10 @@
 
             response_data = self._response_parsers.get(event_name)(
                 **data
             )
 
             yield shard_id, response_data
     
-    async def close(self):
+    async def close(self) -> None:
         self._tcp_connection.close()
         self._udp_connection.close()
```

### Comparing `mercury-sync-0.1.8/mercury_sync/snowflake/snowflake.py` & `mercury-sync-0.1.9/mercury_sync/snowflake/snowflake.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync/snowflake/snowflake_generator.py` & `mercury-sync-0.1.9/mercury_sync/snowflake/snowflake_generator.py`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/mercury_sync.egg-info/PKG-INFO` & `mercury-sync-0.1.9/mercury_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercury-sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: A pure-Python, asyncio based library for authoring distributed systems
 Home-page: https://github.com/scorbettUM/mercury-sync
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,python,distributed systems,swim,serf,distributed
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mercury-sync-0.1.8/mercury_sync.egg-info/SOURCES.txt` & `mercury-sync-0.1.9/mercury_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mercury-sync-0.1.8/setup.py` & `mercury-sync-0.1.9/setup.py`

 * *Files identical despite different names*

