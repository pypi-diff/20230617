# Comparing `tmp/amniotic-0.5.6.tar.gz` & `tmp/amniotic-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amniotic-0.5.6.tar", last modified: Thu Jun 15 14:34:41 2023, max compression
+gzip compressed data, was "amniotic-0.5.7.tar", last modified: Sat Jun 17 17:43:03 2023, max compression
```

## Comparing `amniotic-0.5.6.tar` & `amniotic-0.5.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:41.897549 amniotic-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-15 14:34:41.897549 amniotic-0.5.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:41.893549 amniotic-0.5.6/amniotic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:41.897549 amniotic-0.5.6/amniotic/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/mqtt/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 14:34:38.000000 amniotic-0.5.6/amniotic/version
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-15 14:34:32.000000 amniotic-0.5.6/amniotic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:34:41.893549 amniotic-0.5.6/amniotic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 14:34:41.000000 amniotic-0.5.6/amniotic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:34:41.897549 amniotic-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-15 14:34:32.000000 amniotic-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:43:03.873954 amniotic-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-17 17:43:03.873954 amniotic-0.5.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:43:03.869954 amniotic-0.5.7/amniotic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:43:03.873954 amniotic-0.5.7/amniotic/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20347 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/mqtt/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-17 17:43:00.000000 amniotic-0.5.7/amniotic/version
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-17 17:42:54.000000 amniotic-0.5.7/amniotic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:43:03.869954 amniotic-0.5.7/amniotic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 17:43:03.000000 amniotic-0.5.7/amniotic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 17:43:03.873954 amniotic-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-17 17:42:54.000000 amniotic-0.5.7/setup.py
```

### Comparing `amniotic-0.5.6/PKG-INFO` & `amniotic-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amniotic
-Version: 0.5.6
+Version: 0.5.7
 Summary: A multi-output ambient sound mixer for Home Assistant
 Home-page: https://link.frontmatter.ai/amniotic
 Author: Frontmatter
 License: Copyright © 2022 Frontmatter. All rights reserved.
 Keywords: ambient sound audio white noise masking sleep
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `amniotic-0.5.6/amniotic/audio.py` & `amniotic-0.5.7/amniotic/audio.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.6/amniotic/config.py` & `amniotic-0.5.7/amniotic/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from _socket import gethostname
 from os import getenv
 
 import logging
 import yaml
-from _socket import gethostname
 from appdirs import AppDirs
 from copy import deepcopy
 from dataclasses import dataclass, fields, field
 from distutils.util import strtobool
 from functools import lru_cache
 from getmac import getmac
 from pathlib import Path
@@ -29,14 +29,15 @@
     mqtt_port: int = 1883
     mqtt_username: str = None
     mqtt_password: str = None
     location: str = None
     path_audio: str = APP_DIRS.user_data_dir
     device_names: dict = None
     logging: str = None
+    debug: bool = False
     tele_period: int = 300
     presets: dict = field(default_factory=dict)
     config_raw: dict = field(default_factory=dict)
 
 
     def __post_init__(self):
         path_audio = Path(self.path_audio).absolute()
```

### Comparing `amniotic-0.5.6/amniotic/mqtt/control.py` & `amniotic-0.5.7/amniotic/mqtt/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from time import sleep
+
 import json
 import logging
 import pip
 import threading
 from functools import cached_property
 from johnnydep import JohnnyDist as Package
 from paho.mqtt import client as mqtt
 from pytube import YouTube, Stream
-from time import sleep
 from typing import Optional, Any
 
 from amniotic.audio import Amniotic
 from amniotic.config import NAME
 from amniotic.mqtt.device import Device
 from amniotic.mqtt.loop import Loop
 from amniotic.mqtt.tools import Message, sanitize
@@ -22,14 +23,15 @@
 
     Base representation of an entity for Home Assistant.
 
     """
     PAYLOAD_ONLINE = "Online"
     PAYLOAD_OFFLINE = "Offline"
     HA_PLATFORM = None
+    IS_TELE = False
     NAME = None
     ICON_SUFFIX = None
     VALUE_MAP_ON_OFF = [(OFF := 'OFF'), (ON := 'ON')]
     NA_VALUE = '-'
     value = None
 
     TEST_ALWAYS_UPDATE = False
@@ -172,15 +174,19 @@
         Handle outgoing messages, adding announce, subscriptions to the queue.
 
         """
         if force_announce:
             self.handle_announce()
 
         value = self.get_value()
-        if value != self.value or force_announce:
+
+        is_tele = (not self.IS_TELE) or self.loop.is_telem_loop
+        has_value_changed = value != self.value and is_tele
+
+        if has_value_changed or force_announce:
             self.value = value
             message = Message(self.client.publish, self.topic_state, self.value)
             self.queue.append(message)
 
 
 class Select(Entity):
     """
```

### Comparing `amniotic-0.5.6/amniotic/mqtt/device.py` & `amniotic-0.5.7/amniotic/mqtt/device.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.6/amniotic/mqtt/loop.py` & `amniotic-0.5.7/amniotic/mqtt/loop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from json import JSONDecodeError
+from time import sleep
 
 import json
 import logging
 from copy import deepcopy
 from functools import cached_property
 from paho.mqtt import client as mqtt
-from time import sleep
 from typing import Type
 
 from amniotic.audio import Amniotic
 from amniotic.config import Config, IS_ADDON, PRESET_LAST_KEY
 from amniotic.mqtt.device import Device
 from amniotic.mqtt.tools import Message
 from amniotic.version import __version__
@@ -54,14 +54,15 @@
             entity.topic_command: entity.handle_incoming
             for entity in self.entities.values()
         }
 
         self.queue = []
         self.force_announce_period = self.config.tele_period * 10
         self.has_reconnected = True
+        self.is_telem_loop = False
         self.topic_lwt = self.device.topic_lwt
 
         self.amniotic = amniotic
         self.client = mqtt.Client()
 
         self.client.on_connect = self.on_connect
         self.client.on_message = self.on_message
@@ -171,14 +172,20 @@
 
         if not IS_ADDON:
             sensors += [
                 sensor.UpdateStatus,
                 sensor.Version
             ]
 
+        if self.config.debug:
+            sensors += [
+                sensor.CPU,
+                sensor.Memory,
+            ]
+
         return controls + sensors
 
     def handle_outgoing(self, force_announce=False):
         """
 
         Call entity outgoing methods to add to message queue.
 
@@ -220,24 +227,24 @@
             else:
                 delay = self.DELAY
 
             if not self.client.is_connected():
                 sleep(self.LOOP_PERIOD)
                 continue
 
-            is_telem_loop = loop_count % self.config.tele_period == 0
+            self.is_telem_loop = loop_count % self.config.tele_period == 0
             is_force_announce_loop = loop_count % self.force_announce_period == 0
 
             self.handle_outgoing(force_announce=self.has_reconnected or is_force_announce_loop)
             self.has_reconnected = False
 
             Message.send_many(self.queue, delay=delay)
             self.queue.clear()
 
-            if is_telem_loop:
+            if self.is_telem_loop:
                 self.do_telemetry()
 
             sleep(self.LOOP_PERIOD)
             loop_count += 1
 
         self.close()
```

### Comparing `amniotic-0.5.6/amniotic/mqtt/sensor.py` & `amniotic-0.5.7/amniotic/mqtt/sensor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import psutil as psutil
 from datetime import timedelta
 from typing import Optional, Union, Any
 
 from amniotic.mqtt import control
 from amniotic.version import __version__
 
 
@@ -219,7 +220,53 @@
     Home Assistant version number sensor
 
     """
 
     NAME = 'Current Version'
     ICON_SUFFIX = 'counter'
     message = __version__
+
+
+class CPU(Sensor):
+    """
+
+    Home Assistant sensor showing overview of which Themes are enabled, etc.
+
+    """
+    META_KEY = None
+    NAME = 'CPU Usage'
+    IS_SOURCE_META = False
+    ICON_SUFFIX = 'cpu-64-bit'
+    UOM = '%'
+
+    IS_TELE = True
+
+    def get_value(self, key: Optional[str] = None):
+        """
+
+        Get CPU usage.
+
+        """
+        return psutil.cpu_percent(interval=1)
+
+
+class Memory(Sensor):
+    """
+
+    Home Assistant sensor showing overview of which Themes are enabled, etc.
+
+    """
+    META_KEY = None
+    NAME = 'Memory Usage'
+    IS_SOURCE_META = False
+    ICON_SUFFIX = 'memory'
+    UOM = '%'
+
+    IS_TELE = True
+
+    def get_value(self, key: Optional[str] = None):
+        """
+
+        Get memory usage.
+
+        """
+        return psutil.virtual_memory().percent
```

### Comparing `amniotic-0.5.6/amniotic/mqtt/tools.py` & `amniotic-0.5.7/amniotic/mqtt/tools.py`

 * *Files identical despite different names*

### Comparing `amniotic-0.5.6/amniotic.egg-info/PKG-INFO` & `amniotic-0.5.7/amniotic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amniotic
-Version: 0.5.6
+Version: 0.5.7
 Summary: A multi-output ambient sound mixer for Home Assistant
 Home-page: https://link.frontmatter.ai/amniotic
 Author: Frontmatter
 License: Copyright © 2022 Frontmatter. All rights reserved.
 Keywords: ambient sound audio white noise masking sleep
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `amniotic-0.5.6/setup.py` & `amniotic-0.5.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,15 +26,16 @@
         'paho-mqtt',
         'python-vlc',
         'getmac',
         'pyyaml',
         'appdirs',
         'johnnydep',
         'pytube',
-        'cachetools'
+        'cachetools',
+        'psutil'
     ],
     extras_require={},
     entry_points={
         'console_scripts': [
             'amniotic = amniotic.mqtt.loop:start',
         ],
     }
```

