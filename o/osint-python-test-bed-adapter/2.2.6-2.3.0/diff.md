# Comparing `tmp/osint-python-test-bed-adapter-2.2.6.tar.gz` & `tmp/osint-python-test-bed-adapter-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint-python-test-bed-adapter-2.2.6.tar", last modified: Wed Jun 14 11:05:03 2023, max compression
+gzip compressed data, was "osint-python-test-bed-adapter-2.3.0.tar", last modified: Sat Jun 17 00:33:05 2023, max compression
```

## Comparing `osint-python-test-bed-adapter-2.2.6.tar` & `osint-python-test-bed-adapter-2.3.0.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.6/LICENSE
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3165 2023-06-13 08:56:50.000000 osint-python-test-bed-adapter-2.2.6/README.md
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.208029 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/PKG-INFO
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      782 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/requires.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-14 11:05:03.000000 osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/top_level.txt
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/setup.cfg
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-14 10:59:52.000000 osint-python-test-bed-adapter-2.2.6/setup.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.208029 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1361 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/__init__.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2481 2023-06-14 11:02:28.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/consumer_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1660 2023-03-16 17:49:08.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/heartbeat_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2999 2023-06-07 19:48:38.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/log_manager.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2122 2023-04-06 23:32:08.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/producer_manager.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/options/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/options/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/options/test_bed_options.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/services/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        0 2023-03-14 11:55:32.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/services/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2065 2023-03-14 12:17:24.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/services/http_server.py
-drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-14 11:05:03.211362 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/__init__.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/helpers.py
--rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/key.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1064 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.0/LICENSE
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3165 2023-06-13 08:56:50.000000 osint-python-test-bed-adapter-2.3.0/README.md
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3592 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      703 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)        1 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       39 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/requires.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       17 2023-06-17 00:33:05.000000 osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/top_level.txt
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       38 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/setup.cfg
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      758 2023-06-16 22:11:18.000000 osint-python-test-bed-adapter-2.3.0/setup.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1389 2023-06-17 00:32:44.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/__init__.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       68 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3796 2023-06-17 00:23:16.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/consumer_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1699 2023-06-16 22:08:43.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/heartbeat_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2883 2023-06-16 22:08:43.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/log_manager.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     2102 2023-06-17 00:23:16.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/producer_manager.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/options/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       31 2022-04-23 22:07:41.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/options/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     3486 2023-06-01 22:28:40.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/options/test_bed_options.py
+drwxr-xr-x   0 mindpetk  (1000) mindpetk  (1000)        0 2023-06-17 00:33:05.450774 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)       22 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/__init__.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)      598 2022-09-07 21:58:21.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/helpers.py
+-rw-r--r--   0 mindpetk  (1000) mindpetk  (1000)     1005 2023-03-16 17:51:41.000000 osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/key.py
```

### Comparing `osint-python-test-bed-adapter-2.2.6/LICENSE` & `osint-python-test-bed-adapter-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.6/PKG-INFO` & `osint-python-test-bed-adapter-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.2.6
+Version: 2.3.0
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.2.6/README.md` & `osint-python-test-bed-adapter-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/PKG-INFO` & `osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osint-python-test-bed-adapter
-Version: 2.2.6
+Version: 2.3.0
 Summary: Python adapter for Kafka
 Home-page: https://github.com/OSINT-VDU-TNO/python-adapter
 Author: TimovdK
 Author-email: timo_kuil@hotmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `osint-python-test-bed-adapter-2.2.6/osint_python_test_bed_adapter.egg-info/SOURCES.txt` & `osint-python-test-bed-adapter-2.3.0/osint_python_test_bed_adapter.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,12 +10,10 @@
 test_bed_adapter/kafka/__init__.py
 test_bed_adapter/kafka/consumer_manager.py
 test_bed_adapter/kafka/heartbeat_manager.py
 test_bed_adapter/kafka/log_manager.py
 test_bed_adapter/kafka/producer_manager.py
 test_bed_adapter/options/__init__.py
 test_bed_adapter/options/test_bed_options.py
-test_bed_adapter/services/__init__.py
-test_bed_adapter/services/http_server.py
 test_bed_adapter/utils/__init__.py
 test_bed_adapter/utils/helpers.py
 test_bed_adapter/utils/key.py
```

### Comparing `osint-python-test-bed-adapter-2.2.6/setup.py` & `osint-python-test-bed-adapter-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="osint-python-test-bed-adapter",
-    version="2.2.6",
+    version="2.3.0",
     author="TimovdK",
     author_email="timo_kuil@hotmail.com",
     description="Python adapter for Kafka",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OSINT-VDU-TNO/python-adapter",
     include_package_data=True,
```

### Comparing `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/__init__.py` & `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from .options.test_bed_options import TestBedOptions
+import logging
+from typing import Optional
+
 from confluent_kafka.schema_registry import SchemaRegistryClient
+
 from .kafka.heartbeat_manager import HeartbeatManager
-import logging
+from .options.test_bed_options import TestBedOptions
 
 
 class TestBedAdapter:
     def __init__(self, test_bed_options: TestBedOptions):
-
+        self.logger = logging.getLogger(__name__)
         self.test_bed_options = test_bed_options
         self.default_producer_topics = ["system_heartbeat"]
-        self.heartbeat_manager: HeartbeatManager = None
+        self.heartbeat_manager: HeartbeatManager = Optional[HeartbeatManager]
 
     def initialize(self):
-        logging.info("Initializing test bed")
+        self.logger.info("Initializing test bed")
         self.init_and_start_heartbeat()
-        self.connected = True
 
     def init_and_start_heartbeat(self):
         schema_registry_conf = {'url': self.test_bed_options.schema_registry}
         schema_registry_client = SchemaRegistryClient(schema_registry_conf)
 
         if "system_heartbeat-value" in schema_registry_client.get_subjects():
             self.heartbeat_manager = HeartbeatManager(
                 options=self.test_bed_options, kafka_topic='system_heartbeat')
-            self.heartbeat_manager.start_heartbeat_async()
+            self.heartbeat_manager.start()
         else:
             logging.error(
                 "Heartbeat could not be initialized, No schema found for topic system_heartbeat")
 
     def stop(self):
         # Stop the heartbeat thread
         if self.heartbeat_manager is not None:
             self.heartbeat_manager.stop()
-        self.connected = False
```

### Comparing `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/consumer_manager.py` & `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/consumer_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,103 @@
-import time
+import logging
+from threading import Thread
+from time import time, sleep
 
 from confluent_kafka import DeserializingConsumer
 from confluent_kafka.schema_registry import SchemaRegistryClient
 from confluent_kafka.schema_registry.avro import AvroDeserializer
 
 from ..options.test_bed_options import TestBedOptions
 
 
-class ConsumerManager:
-    def __init__(self, options: TestBedOptions, kafka_topic, handle_message, run):
+class ConsumerManager(Thread):
+    def __init__(self, options: TestBedOptions, kafka_topic, handle_message):
+        super().__init__()
+        self.logger = logging.getLogger(__name__)
+        self.daemon = True
         self.options = options
         self.handle_message = handle_message
-        self.run = run
+        self.running = True
+
+        self.latest_message = None
 
         sr_conf = {'url': self.options.schema_registry}
         schema_registry_client = SchemaRegistryClient(sr_conf)
+
         self.avro_deserializer = AvroDeserializer(schema_registry_client)
         self.schema = schema_registry_client.get_latest_version(kafka_topic + "-value")
         self.schema_str = self.schema.schema.schema_str
         self.kafka_topic = kafka_topic
 
-        consumer_conf = {'bootstrap.servers': self.options.kafka_host,
-                         'key.deserializer': self.avro_deserializer,
-                         'value.deserializer': self.avro_deserializer,
-                         'group.id': self.options.consumer_group,
-                         'message.max.bytes': self.options.message_max_bytes,
-                         'auto.offset.reset': self.options.offset_type}
+        consumer_conf = {
+            'bootstrap.servers': self.options.kafka_host,
+            'key.deserializer': self.avro_deserializer,
+            'value.deserializer': self.avro_deserializer,
+            'group.id': self.options.consumer_group,
+            'message.max.bytes': self.options.message_max_bytes,
+            'auto.offset.reset': self.options.offset_type
+        }
+
         self.consumer = DeserializingConsumer(consumer_conf)
+        self.consumer.subscribe([kafka_topic])
 
-        def on_assign(c, ps):
-            for p in ps:
-                p.offset = 0
-            c.assign(ps)
-
-        if self.options.offset_type == 'earliest':
-            self.consumer.subscribe([kafka_topic], on_assign=on_assign)
-        else:
-            self.consumer.subscribe([kafka_topic])
+    def run(self):
+        self.reset_partition_offsets()
+        self.ingore_messages()
+        self.use_latest_message()
+        self.listen()
 
-    def listen(self):
-        _start_time = time.time()
-        _latest_message = None
+    def stop(self):
+        self.running = False
 
+    def reset_partition_offsets(self):
+        """Reset partition offsets to beginning"""
+        if self.options.offset_type != 'earliest':
+            return
+        try:
+            # Need to poll to get assigned partitions
+            self.latest_message = self.consumer.poll(1)
+            # Wait for partitions to be assigned
+            partitions = []
+            while not partitions and self.latest_message is None:
+                sleep(1)
+                self.latest_message = self.consumer.poll(10)
+                partitions = self.consumer.assignment()
+            #  Reset partitions to beginning
+            for partition in partitions:
+                partition.offset = 0
+                # Seek to beginning
+                self.consumer.seek(partition)
+                self.consumer.commit()
+        except Exception as e:
+            self.logger.error(f"Error resetting partition offsets: {e}")
+            return
+
+    def ingore_messages(self):
+        """Ignore messages for a period of time"""
+        _start_time = time()
         # Ignore messages for a period of time
-        while True and self.options.ignore_timeout:
+        if not self.options.ignore_timeout:
+            return
+        while True:
             msg = self.consumer.poll(1)
             if msg:
-                _latest_message = msg
-            elapsed_time = time.time() - _start_time
+                self.latest_message = msg
+            elapsed_time = time() - _start_time
             if elapsed_time > self.options.ignore_timeout:
                 break
-        if _latest_message and self.options.use_latest:
-            self.handle_message(_latest_message.value(), _latest_message.topic())
 
+    def use_latest_message(self):
+        """Use the latest message on the topic"""
+        if self.latest_message and self.options.use_latest:
+            self.handle_message(self.latest_message.value(), self.latest_message.topic())
+
+    def listen(self):
+        """Listen for messages on the topic and handle them with the provided callback"""
         # Continue to listen for messages
-        while self.run():
+        while self.running:
             msg = self.consumer.poll(1)
             if msg is None:
                 continue
             self.handle_message(msg.value(), msg.topic())
-
-        self.consumer.close()
-
-    def stop(self):
+        # Close down consumer to commit final offsets.
         self.consumer.close()
```

### Comparing `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/heartbeat_manager.py` & `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/heartbeat_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,53 @@
-from ..options.test_bed_options import TestBedOptions
-from .producer_manager import ProducerManager
-from ..utils.helpers import Helpers
-
 import copy
 import datetime
-import urllib.request
+import logging
 import socket
 import time
+import urllib.request
+from threading import Thread
+
+from .producer_manager import ProducerManager
+from ..options.test_bed_options import TestBedOptions
 
 
-class HeartbeatManager:
+class HeartbeatManager(Thread):
+
     def __init__(self, options: TestBedOptions, kafka_topic):
+        super().__init__()
+        self.daemon = True
+        self.logger = logging.getLogger(__name__)
+
         self.options = copy.deepcopy(options)
         self.options.string_key_type = 'group_id'
+        self.running = True
 
-        self.helper = Helpers()
-        self.interval_thread = {}
-
-        self.kafka_heartbeat_producer = ProducerManager(
-            options=self.options, kafka_topic=kafka_topic)
-
-    def start_heartbeat_async(self):
-        print('Heartbeat Started')
-        self.interval_thread = self.helper.set_interval(
-            self.send_heartbeat_message, self.options.heartbeat_interval)
+        # Message parameters
+        try:
+            self.external_IP = str(urllib.request.urlopen("https://api.ipify.org").read().decode("utf-8"))
+        except:
+            self.external_IP = "unknown"
+        self.host_name = str(socket.gethostname())
+        self.host_IP = str(socket.gethostbyname(self.host_name))
+
+        self.kafka_heartbeat_producer = ProducerManager(options=self.options, kafka_topic=kafka_topic)
+
+    def run(self):
+        self.logger.info("Heartbeat Started")
+        while self.running:
+            self.send_heartbeat_message()
+            time.sleep(self.options.heartbeat_interval)
 
     def send_heartbeat_message(self):
         date = datetime.datetime.utcnow()
         date_ms = int(time.mktime(date.timetuple())) * 1000
 
-        # Get data for origin stringified json
-        hostName = str(socket.gethostname())
-        hostIP = str(socket.gethostbyname(hostName))
-        try:
-            externalIP = str(urllib.request.urlopen(
-                "http://ipv4bot.whatismyipaddress.com").read().decode("utf-8"))
-        except urllib.error.URLError as e:
-            externalIP = "unknown"
-
-        message_json = {"id": self.options.consumer_group, "alive": date_ms,
-                        "origin": "{hostname: %s, localIP: %s, externalIP: %s}" % (hostName, hostIP, externalIP)}
-
-        messages = [message_json]
-        self.kafka_heartbeat_producer.send_messages(messages=messages)
+        message_json = {
+            "id": self.options.consumer_group,
+            "alive": date_ms,
+            "origin": "{hostname: %s, localIP: %s, externalIP: %s}" % (
+                self.host_name, self.host_IP, self.external_IP)
+        }
+        self.kafka_heartbeat_producer.send_messages(messages=[message_json])
 
     def stop(self):
         self.kafka_heartbeat_producer.stop()
```

### Comparing `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/log_manager.py` & `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/log_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import json
 import time
 from datetime import datetime
 from enum import Enum
 
 from .producer_manager import ProducerManager
 from ..options.test_bed_options import TestBedOptions
-from ..utils.helpers import Helpers
 
 
 class BColors:
     OKBLUE = '\033[94m'
     WARNING = '\033[93m'
     FAIL = '\033[91m'
     ENDC = '\033[0m'
@@ -49,19 +48,15 @@
 
 
 class LogManager:
     def __init__(self, options: TestBedOptions, kafka_topic='system_logging'):
         self.options = copy.deepcopy(options)
         self.options.string_key_type = 'group_id'
 
-        self.helper = Helpers()
-        self.interval_thread = {}
-
-        self.kafka_log_producer = ProducerManager(
-            options=self.options, kafka_topic=kafka_topic)
+        self.kafka_log_producer = ProducerManager(options=self.options, kafka_topic=kafka_topic)
 
     def sill(self, msg):
         self.log(LogLevel.Sill, msg)
 
     def debug(self, msg):
         self.log(LogLevel.Debug, msg)
```

### Comparing `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/kafka/producer_manager.py` & `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/kafka/producer_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import time
+from datetime import datetime
+
 from confluent_kafka import SerializingProducer
 from confluent_kafka.schema_registry import SchemaRegistryClient
 from confluent_kafka.schema_registry.avro import AvroSerializer
-from datetime import datetime
-import time
 
-from ..utils.key import generate_key
 from ..options.test_bed_options import TestBedOptions
+from ..utils.key import generate_key
 
 
 class ProducerManager:
     def __init__(self, options: TestBedOptions, kafka_topic):
         self.options = options
         self.kafka_topic = kafka_topic
 
@@ -34,16 +35,15 @@
     def send_messages(self, messages: list):
         for m in messages:
             date = datetime.utcnow()
             date_ms = int(time.mktime(date.timetuple())) * 1000
             k = generate_key(m, self.options)
             self.producer.poll(0.0)
             try:
-                self.producer.produce(
-                    topic=self.kafka_topic, key=k, value=m, timestamp=date_ms)
+                self.producer.produce(topic=self.kafka_topic, key=k, value=m, timestamp=date_ms)
             except ValueError:
                 print("Invalid input, discarding record...")
                 continue
 
             self.producer.flush()
 
     def stop(self):
```

### Comparing `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/options/test_bed_options.py` & `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/options/test_bed_options.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/helpers.py` & `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `osint-python-test-bed-adapter-2.2.6/test_bed_adapter/utils/key.py` & `osint-python-test-bed-adapter-2.3.0/test_bed_adapter/utils/key.py`

 * *Files identical despite different names*

