# Comparing `tmp/pyrademacher-0.9.8.tar.gz` & `tmp/pyrademacher-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrademacher-0.9.8.tar", last modified: Thu Jun  8 10:13:55 2023, max compression
+gzip compressed data, was "pyrademacher-0.9.9.tar", last modified: Thu Jun  8 10:41:35 2023, max compression
```

## Comparing `pyrademacher-0.9.8.tar` & `pyrademacher-0.9.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:13:55.279914 pyrademacher-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-08 10:13:55.279914 pyrademacher-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:13:55.279914 pyrademacher-0.9.8/homepilot/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/actuator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15020 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/homepilot/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:13:55.279914 pyrademacher-0.9.8/pyrademacher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-08 10:13:55.000000 pyrademacher-0.9.8/pyrademacher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-08 10:13:55.000000 pyrademacher-0.9.8/pyrademacher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:13:55.000000 pyrademacher-0.9.8/pyrademacher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 10:13:55.000000 pyrademacher-0.9.8/pyrademacher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 10:13:55.000000 pyrademacher-0.9.8/pyrademacher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:13:55.279914 pyrademacher-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:13:55.279914 pyrademacher-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/tests/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-08 10:13:43.000000 pyrademacher-0.9.8/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:41:35.683511 pyrademacher-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-08 10:41:35.683511 pyrademacher-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:41:35.679511 pyrademacher-0.9.9/homepilot/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15020 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/homepilot/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:41:35.683511 pyrademacher-0.9.9/pyrademacher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-08 10:41:35.000000 pyrademacher-0.9.9/pyrademacher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-08 10:41:35.000000 pyrademacher-0.9.9/pyrademacher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:41:35.000000 pyrademacher-0.9.9/pyrademacher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 10:41:35.000000 pyrademacher-0.9.9/pyrademacher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 10:41:35.000000 pyrademacher-0.9.9/pyrademacher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:41:35.683511 pyrademacher-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:41:35.679511 pyrademacher-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/tests/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-08 10:41:25.000000 pyrademacher-0.9.9/tests/test_thermostat.py
```

### Comparing `pyrademacher-0.9.8/LICENSE` & `pyrademacher-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/PKG-INFO` & `pyrademacher-0.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrademacher
-Version: 0.9.8
+Version: 0.9.9
 Summary: Control devices connected to your Rademacher Homepilot (or Start2Smart) hub
 Home-page: https://github.com/peribeir/pyrademacher
 Author: Pedro Ribeiro
 Author-email: pedroeusebio@gmail.com
 Project-URL: Bug Tracker, https://github.com/peribeir/pyrademacher/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrademacher-0.9.8/README.md` & `pyrademacher-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/homepilot/actuator.py` & `pyrademacher-0.9.9/homepilot/actuator.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/homepilot/api.py` & `pyrademacher-0.9.9/homepilot/api.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/homepilot/const.py` & `pyrademacher-0.9.9/homepilot/const.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/homepilot/cover.py` & `pyrademacher-0.9.9/homepilot/cover.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/homepilot/device.py` & `pyrademacher-0.9.9/homepilot/device.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/homepilot/hub.py` & `pyrademacher-0.9.9/homepilot/hub.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     _hub_type: str
     _hw_platform: str
     _sw_platform: str
     _fw_version: str
     _duofern_stick_version: str
     _fw_update_available: bool
     _fw_update_version: str
+    _download_progress: int | bool
+    _auto_update: bool
     _release_notes: str
     _led_status: bool
 
     def __init__(
         self,
         api,
         did,
@@ -101,17 +103,27 @@
         self.fw_update_version = (
             state["status"]["new_version"]
             if "new_version" in state["status"] and self.fw_update_available
             else state["status"]["version"]
         )
         self.release_notes = (
             state["status"]["release_notes"]
-            if "new_version" in state["status"] and self.fw_update_available
+            if "release_notes" in state["status"] and self.fw_update_available
             else ""
         )
+        self.download_progress = (
+            state["status"]["download_progress"]
+            if "download_progress" in state["status"]
+            else False
+        )
+        self.auto_update = (
+            state["status"]["auto_update"]
+            if "auto_update" in state["status"]
+            else False
+        )
         self.led_status = state["led"]["status"] == "enabled"
 
     async def async_ping(self):
         pass
 
     async def async_turn_led_on(self) -> None:
         await self.api.async_turn_led_on()
@@ -159,14 +171,30 @@
         return self._release_notes
 
     @release_notes.setter
     def release_notes(self, release_notes):
         self._release_notes = release_notes
 
     @property
+    def download_progress(self):
+        return self._download_progress
+
+    @download_progress.setter
+    def download_progress(self, download_progress):
+        self._download_progress = download_progress
+
+    @property
+    def auto_update(self):
+        return self._auto_update
+
+    @auto_update.setter
+    def auto_update(self, auto_update):
+        self._auto_update = auto_update
+
+    @property
     def fw_update_version(self):
         return self._fw_update_version
 
     @fw_update_version.setter
     def fw_update_version(self, fw_update_version):
         self._fw_update_version = fw_update_version
```

### Comparing `pyrademacher-0.9.8/homepilot/manager.py` & `pyrademacher-0.9.9/homepilot/manager.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/homepilot/sensor.py` & `pyrademacher-0.9.9/homepilot/sensor.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/homepilot/switch.py` & `pyrademacher-0.9.9/homepilot/switch.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/homepilot/thermostat.py` & `pyrademacher-0.9.9/homepilot/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/pyrademacher.egg-info/PKG-INFO` & `pyrademacher-0.9.9/pyrademacher.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrademacher
-Version: 0.9.8
+Version: 0.9.9
 Summary: Control devices connected to your Rademacher Homepilot (or Start2Smart) hub
 Home-page: https://github.com/peribeir/pyrademacher
 Author: Pedro Ribeiro
 Author-email: pedroeusebio@gmail.com
 Project-URL: Bug Tracker, https://github.com/peribeir/pyrademacher/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrademacher-0.9.8/pyrademacher.egg-info/SOURCES.txt` & `pyrademacher-0.9.9/pyrademacher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/setup.py` & `pyrademacher-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyrademacher",
-    version="0.9.8",
+    version="0.9.9",
     author="Pedro Ribeiro",
     author_email="pedroeusebio@gmail.com",
     description="Control devices connected to your Rademacher Homepilot "
     "(or Start2Smart) hub",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peribeir/pyrademacher",
```

### Comparing `pyrademacher-0.9.8/tests/test_api.py` & `pyrademacher-0.9.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/tests/test_cover.py` & `pyrademacher-0.9.9/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/tests/test_hub.py` & `pyrademacher-0.9.9/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/tests/test_manager.py` & `pyrademacher-0.9.9/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/tests/test_sensor.py` & `pyrademacher-0.9.9/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/tests/test_switch.py` & `pyrademacher-0.9.9/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.8/tests/test_thermostat.py` & `pyrademacher-0.9.9/tests/test_thermostat.py`

 * *Files identical despite different names*

