# Comparing `tmp/pyais-2.5.4.tar.gz` & `tmp/pyais-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyais-2.5.4.tar", last modified: Tue May 30 10:03:37 2023, max compression
+gzip compressed data, was "dist/pyais-2.5.5.tar", last modified: Sat Jun 17 13:16:08 2023, max compression
```

## Comparing `pyais-2.5.4.tar` & `pyais-2.5.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:03:37.000000 pyais-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    23826 2023-05-30 10:03:37.000000 pyais-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-05-30 10:03:26.000000 pyais-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:03:37.000000 pyais-2.5.4/pyais/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/ais_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    64765 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-05-30 10:03:26.000000 pyais-2.5.4/pyais/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:03:37.000000 pyais-2.5.4/pyais.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23826 2023-05-30 10:03:37.000000 pyais-2.5.4/pyais.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-30 10:03:37.000000 pyais-2.5.4/pyais.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:03:37.000000 pyais-2.5.4/pyais.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 10:03:37.000000 pyais-2.5.4/pyais.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-30 10:03:37.000000 pyais-2.5.4/pyais.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 10:03:37.000000 pyais-2.5.4/pyais.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:03:37.000000 pyais-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-30 10:03:26.000000 pyais-2.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:03:37.000000 pyais-2.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/mock_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    58995 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_decode_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    32404 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_file_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_generic_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_nmea.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_tag_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_talker_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_tcp_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/test_udp_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:03:37.000000 pyais-2.5.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/utils/generate_msg_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/utils/skip.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-30 10:03:26.000000 pyais-2.5.4/tests/utils/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    23826 2023-06-17 13:16:08.000000 pyais-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19303 2023-06-17 13:15:57.000000 pyais-2.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/ais_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64765 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12681 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16440 2023-06-17 13:15:57.000000 pyais-2.5.5/pyais/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23826 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 13:16:08.000000 pyais-2.5.5/pyais.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:16:08.000000 pyais-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-17 13:15:57.000000 pyais-2.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/mock_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58995 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_decode_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32404 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_file_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_generic_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_nmea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_tag_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_talker_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_tcp_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/test_udp_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:16:08.000000 pyais-2.5.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/utils/generate_msg_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/utils/skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-17 13:15:57.000000 pyais-2.5.5/tests/utils/timeout.py
```

### Comparing `pyais-2.5.4/PKG-INFO` & `pyais-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.5.4
+Version: 2.5.5
 Summary: Ais message decoding
 Home-page: https://github.com/M0r13n/pyais
 Author: Leon Morten Richter
 Author-email: leon.morten@gmail.com
 License: MIT
 Description: # pyais
```

### Comparing `pyais-2.5.4/README.md` & `pyais-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais/__init__.py` & `pyais-2.5.5/pyais/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pyais.messages import NMEAMessage, ANY_MESSAGE, AISSentence
 from pyais.stream import TCPConnection, FileReaderStream, IterMessages
 from pyais.encode import encode_dict, encode_msg, ais_to_nmea_0183
 from pyais.decode import decode
 from pyais.tracker import AISTracker, AISTrack
 
 __license__ = 'MIT'
-__version__ = '2.5.4'
+__version__ = '2.5.5'
 __author__ = 'Leon Morten Richter'
 
 __all__ = (
     'encode_dict',
     'encode_msg',
     'ais_to_nmea_0183',
     'NMEAMessage',
```

### Comparing `pyais-2.5.4/pyais/ais_types.py` & `pyais-2.5.5/pyais/ais_types.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais/constants.py` & `pyais-2.5.5/pyais/constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais/decode.py` & `pyais-2.5.5/pyais/decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais/encode.py` & `pyais-2.5.5/pyais/encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais/exceptions.py` & `pyais-2.5.5/pyais/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais/main.py` & `pyais-2.5.5/pyais/main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais/messages.py` & `pyais-2.5.5/pyais/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1613,18 +1613,18 @@
         addressed = kwargs.get('addressed', False)
         structured = kwargs.get('structured', False)
 
         if addressed:
             if structured:
                 return MessageType26AddressedStructured.create(**kwargs)
             else:
-                return MessageType26BroadcastStructured.create(**kwargs)
+                return MessageType26AddressedUnstructured.create(**kwargs)
         else:
             if structured:
-                return MessageType26AddressedUnstructured.create(**kwargs)
+                return MessageType26AddressedStructured.create(**kwargs)
             else:
                 return MessageType26BroadcastUnstructured.create(**kwargs)
 
     @classmethod
     def from_bitarray(cls, bit_arr: bitarray) -> "ANY_MESSAGE":
         addressed: int = get_int(bit_arr, 38, 39)
         structured: int = get_int(bit_arr, 39, 40)
```

### Comparing `pyais-2.5.4/pyais/stream.py` & `pyais-2.5.5/pyais/stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais/tracker.py` & `pyais-2.5.5/pyais/tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais/util.py` & `pyais-2.5.5/pyais/util.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/pyais.egg-info/PKG-INFO` & `pyais-2.5.5/pyais.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyais
-Version: 2.5.4
+Version: 2.5.5
 Summary: Ais message decoding
 Home-page: https://github.com/M0r13n/pyais
 Author: Leon Morten Richter
 Author-email: leon.morten@gmail.com
 License: MIT
 Description: # pyais
```

### Comparing `pyais-2.5.4/pyais.egg-info/SOURCES.txt` & `pyais-2.5.5/pyais.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/setup.py` & `pyais-2.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/mock_sender.py` & `pyais-2.5.5/tests/mock_sender.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/mock_server.py` & `pyais-2.5.5/tests/mock_server.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_constants.py` & `pyais-2.5.5/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_decode.py` & `pyais-2.5.5/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_decode_raw.py` & `pyais-2.5.5/tests/test_decode_raw.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_encode.py` & `pyais-2.5.5/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_examples.py` & `pyais-2.5.5/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_file_stream.py` & `pyais-2.5.5/tests/test_file_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_generic_stream.py` & `pyais-2.5.5/tests/test_generic_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_main.py` & `pyais-2.5.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_nmea.py` & `pyais-2.5.5/tests/test_nmea.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_socket.py` & `pyais-2.5.5/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_tag_block.py` & `pyais-2.5.5/tests/test_tag_block.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_talker_ids.py` & `pyais-2.5.5/tests/test_talker_ids.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_tcp_stream.py` & `pyais-2.5.5/tests/test_tcp_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_tracker.py` & `pyais-2.5.5/tests/test_tracker.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/test_udp_stream.py` & `pyais-2.5.5/tests/test_udp_stream.py`

 * *Files identical despite different names*

### Comparing `pyais-2.5.4/tests/utils/generate_msg_interface.py` & `pyais-2.5.5/tests/utils/generate_msg_interface.py`

 * *Files identical despite different names*

