# Comparing `tmp/kaspersmicrobit-0.4.1.tar.gz` & `tmp/kaspersmicrobit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaspersmicrobit-0.4.1.tar", last modified: Tue Jun 13 22:11:42 2023, max compression
+gzip compressed data, was "kaspersmicrobit-0.4.2.tar", last modified: Sat Jun 17 12:56:03 2023, max compression
```

## Comparing `kaspersmicrobit-0.4.1.tar` & `kaspersmicrobit-0.4.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:11:42.554957 kaspersmicrobit-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (122)    15550 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)     7087 2023-06-13 22:11:42.554957 kaspersmicrobit-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6192 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-06-13 22:11:42.554957 kaspersmicrobit-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:11:42.542957 kaspersmicrobit-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:11:42.546957 kaspersmicrobit-0.4.1/src/kaspersmicrobit/
--rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7087 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/bluetoothdevice.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:11:42.550957 kaspersmicrobit-0.4.1/src/kaspersmicrobit/bluetoothprofile/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/bluetoothprofile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15825 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/bluetoothprofile/characteristics.py
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/bluetoothprofile/services.py
--rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/errors.py
--rw-r--r--   0 runner    (1001) docker     (122)     9171 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/kaspersmicrobit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:11:42.554957 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/accelerometer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5895 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/buttons.py
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/device_information.py
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/event.py
--rw-r--r--   0 runner    (1001) docker     (122)     7409 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/generic_access.py
--rw-r--r--   0 runner    (1001) docker     (122)    13348 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/io_pin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/led.py
--rw-r--r--   0 runner    (1001) docker     (122)    13044 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/leddisplay.py
--rw-r--r--   0 runner    (1001) docker     (122)    10383 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/magnetometer.py
--rw-r--r--   0 runner    (1001) docker     (122)     4097 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/temperature.py
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/uart.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/v1_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/v1_legacy_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5682 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/v2_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit/tkinter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:11:42.546957 kaspersmicrobit-0.4.1/src/kaspersmicrobit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7087 2023-06-13 22:11:42.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-13 22:11:42.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 22:11:42.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-13 22:11:42.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-13 22:11:42.000000 kaspersmicrobit-0.4.1/src/kaspersmicrobit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 22:11:42.554957 kaspersmicrobit-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     8843 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/tests/test_bluetoothdevice.py
--rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/tests/test_do_in_tkinter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (122)     4134 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/tests/test_io_pin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-06-13 22:11:32.000000 kaspersmicrobit-0.4.1/tests/test_leddisplay.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 12:56:03.258885 kaspersmicrobit-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    15550 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     7087 2023-06-17 12:56:03.258885 kaspersmicrobit-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6192 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1053 2023-06-17 12:56:03.258885 kaspersmicrobit-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 12:56:03.254885 kaspersmicrobit-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 12:56:03.254885 kaspersmicrobit-0.4.2/src/kaspersmicrobit/
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/bluetoothdevice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 12:56:03.254885 kaspersmicrobit-0.4.2/src/kaspersmicrobit/bluetoothprofile/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/bluetoothprofile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15825 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/bluetoothprofile/characteristics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5165 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/bluetoothprofile/services.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3409 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9171 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/kaspersmicrobit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 12:56:03.258885 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7498 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/accelerometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5895 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/device_information.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7409 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/generic_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13348 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/io_pin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/led.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13044 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/leddisplay.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10383 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/magnetometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4097 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/uart.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/v1_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/v1_legacy_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5682 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/v2_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2408 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit/tkinter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 12:56:03.254885 kaspersmicrobit-0.4.2/src/kaspersmicrobit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7087 2023-06-17 12:56:03.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-17 12:56:03.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-17 12:56:03.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-06-17 12:56:03.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-06-17 12:56:03.000000 kaspersmicrobit-0.4.2/src/kaspersmicrobit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-17 12:56:03.258885 kaspersmicrobit-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    10689 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/tests/test_bluetoothdevice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2401 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/tests/test_do_in_tkinter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4134 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/tests/test_io_pin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2569 2023-06-17 12:55:54.000000 kaspersmicrobit-0.4.2/tests/test_leddisplay.py
```

### Comparing `kaspersmicrobit-0.4.1/LICENSE.md` & `kaspersmicrobit-0.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/PKG-INFO` & `kaspersmicrobit-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaspersmicrobit
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python package to connect to the Bluetooth LE GATT services of BBC micro:bit devices. Use your micro:bit as a wireless game controller!
 Home-page: https://github.com/janickr/kaspersmicrobit
 Author: Janick Reynders
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: Documentation, https://kaspersmicrobit.readthedocs.io/en/stable
 Keywords: microbit,bluetooth,ble,python-for-kids,gatt
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kaspersmicrobit-0.4.1/README.md` & `kaspersmicrobit-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/setup.cfg` & `kaspersmicrobit-0.4.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kaspersmicrobit
-version = 0.4.1
+version = 0.4.2
 author = Janick Reynders
 description = A python package to connect to the Bluetooth LE GATT services of BBC micro:bit devices. Use your micro:bit as a wireless game controller!
 license = Mozilla Public License 2.0 (MPL 2.0)
 license_files = LICENSE.md
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/janickr/kaspersmicrobit
```

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/bluetoothdevice.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/bluetoothdevice.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
 class BluetoothEventLoop(metaclass=ABCMeta):
     @abstractmethod
     def run_async(self, coroutine) -> concurrent.futures.Future:
         pass
 
     @abstractmethod
+    def wrap_future(self, future: concurrent.futures.Future) -> asyncio.Future:
+        pass
+
+    @abstractmethod
     def create_future(self) -> asyncio.Future:
         pass
 
 
 class ThreadEventLoop(BluetoothEventLoop):
     _singleton = None
 
@@ -38,14 +42,17 @@
     @staticmethod
     def _start_background_loop(loop: asyncio.AbstractEventLoop) -> None:
         loop.run_forever()
 
     def run_async(self, coroutine) -> concurrent.futures.Future:
         return asyncio.run_coroutine_threadsafe(coroutine, self.loop)
 
+    def wrap_future(self, future: concurrent.futures.Future) -> asyncio.Future:
+        return asyncio.wrap_future(future, loop=self.loop)
+
     def create_future(self) -> asyncio.Future:
         return self.loop.create_future()
 
     @staticmethod
     def single_thread():
         if not ThreadEventLoop._singleton:
             ThreadEventLoop._singleton = ThreadEventLoop()
@@ -104,16 +111,16 @@
                             This is probably not what you want. If your really want to do this wrap your callback in
                             kaspersmicrobit.tkinter.do_in_tkinter(tk, your_callback)""") from e
                     raise e
 
             return suggest_do_in_tkinter
 
         def do_on_callback_executor(fn: Callable[[BleakGATTCharacteristic, bytearray], None]):
-            def submit_to_executor(sender: BleakGATTCharacteristic, data: bytearray):
-                return asyncio.wrap_future(BluetoothDevice._callback_executor.submit(fn, sender, data))
+            async def submit_to_executor(sender: BleakGATTCharacteristic, data: bytearray):
+                await self._loop.wrap_future(BluetoothDevice._callback_executor.submit(fn, sender, data))
 
             return submit_to_executor
 
         logger.info("(%s) Enable notify %s %s", self._client.address, service, characteristic)
         gatt_characteristic = self._find_gatt_attribute(service, characteristic)
         self._loop.run_async(
             self._client.start_notify(gatt_characteristic, do_on_callback_executor(wrap_try_catch(callback)))
```

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/bluetoothprofile/characteristics.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/bluetoothprofile/characteristics.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/bluetoothprofile/services.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/bluetoothprofile/services.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/errors.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/errors.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/kaspersmicrobit.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/kaspersmicrobit.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/accelerometer.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/accelerometer.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/buttons.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/buttons.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/device_information.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/device_information.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/event.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/event.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/events.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/events.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/generic_access.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/generic_access.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/io_pin.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/io_pin.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/led.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/led.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/leddisplay.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/leddisplay.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/magnetometer.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/magnetometer.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/temperature.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/temperature.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/uart.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/uart.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/v1_events.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/v1_events.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/v1_legacy_events.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/v1_legacy_events.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/services/v2_events.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/services/v2_events.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit/tkinter.py` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit/tkinter.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit.egg-info/PKG-INFO` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaspersmicrobit
-Version: 0.4.1
+Version: 0.4.2
 Summary: A python package to connect to the Bluetooth LE GATT services of BBC micro:bit devices. Use your micro:bit as a wireless game controller!
 Home-page: https://github.com/janickr/kaspersmicrobit
 Author: Janick Reynders
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: Documentation, https://kaspersmicrobit.readthedocs.io/en/stable
 Keywords: microbit,bluetooth,ble,python-for-kids,gatt
 Classifier: Programming Language :: Python :: 3
```

### Comparing `kaspersmicrobit-0.4.1/src/kaspersmicrobit.egg-info/SOURCES.txt` & `kaspersmicrobit-0.4.2/src/kaspersmicrobit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/tests/test_bluetoothdevice.py` & `kaspersmicrobit-0.4.2/tests/test_bluetoothdevice.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #  This Source Code Form is subject to the terms of the Mozilla Public
 #  License, v. 2.0. If a copy of the MPL was not distributed with this
 #  file, You can obtain one at https://mozilla.org/MPL/2.0/.
+import asyncio
+import inspect
 import re
-from typing import List, Union
+from typing import List, Union, Callable, Awaitable
 from unittest.mock import patch
 from uuid import UUID
+from concurrent.futures import TimeoutError
 
 import pytest
 from bleak.backends.descriptor import BleakGATTDescriptor
 from bleak.backends.service import BleakGATTService
 
 from kaspersmicrobit.bluetoothdevice import BluetoothDevice, ThreadEventLoop
 from kaspersmicrobit.errors import BluetoothCharacteristicNotFound, BluetoothServiceNotFound
@@ -125,40 +128,87 @@
     client.start_notify.return_value = None
     callback_data = None
 
     def callback(sender, data):
         nonlocal callback_data
         callback_data = data
 
-    BluetoothDevice(client).notify(Service.TEMPERATURE, Characteristic.TEMPERATURE, callback)
+    device = BluetoothDevice(client)
+    device.notify(Service.TEMPERATURE, Characteristic.TEMPERATURE, callback)
     characteristic, new_callback = client.start_notify.call_args.args
     client.start_notify.assert_awaited()
 
     assert characteristic == gatt_characteristic
 
-    new_callback(sender=-1, data=b'the data')
+    invoke_callback(device, new_callback, sender=characteristic, data=b'the data').result(1)
     assert callback_data == b'the data'
 
 
-@pytest.mark.skip(reason="tested manually, need new approach")
 def test_notify_suggests_do_in_tkinter_on_tk_error(client):
     gatt_characteristic = setup_characteristic(client, Service.TEMPERATURE, Characteristic.TEMPERATURE)
     client.start_notify.return_value = None
 
     def callback(sender, data):
         raise RuntimeError("main thread is not in main loop")
 
-    BluetoothDevice(client).notify(Service.TEMPERATURE, Characteristic.TEMPERATURE, callback)
+    device = BluetoothDevice(client)
+    device.notify(Service.TEMPERATURE, Characteristic.TEMPERATURE, callback)
     characteristic, new_callback = client.start_notify.call_args.args
     client.start_notify.assert_awaited()
 
     assert characteristic == gatt_characteristic
 
     with pytest.raises(RuntimeError, match=r"You tried to call tkinter API.*"):
-        new_callback(sender=-1, data=b'this should fail')
+        invoke_callback(device, new_callback, sender=characteristic, data=b'this should fail').result(1)
+
+
+def test_notify_if_call_on_device_in_callback_it_does_not_block(client):
+    gatt_characteristic = setup_characteristic(client, Service.TEMPERATURE, Characteristic.TEMPERATURE)
+    client.start_notify.return_value = None
+
+    device = BluetoothDevice(client)
+
+    def callback(sender, data):
+        device.read(Service.TEMPERATURE, Characteristic.TEMPERATURE)
+
+    device.notify(Service.TEMPERATURE, Characteristic.TEMPERATURE, callback)
+    characteristic, new_callback = client.start_notify.call_args.args
+    client.start_notify.assert_awaited()
+
+    assert characteristic == gatt_characteristic
+
+    future = invoke_callback(device, new_callback, sender=characteristic, data=b'this should not block')
+
+    async def should_be_invoked():
+        pass
+
+    try:
+        device._loop.run_async(should_be_invoked()).result(3)
+    except TimeoutError:
+        ThreadEventLoop._singleton = None  # throw away the broken eventloop + Thread, so other tests run clean
+        pytest.fail('Eventloop was blocked')
+
+    future.result()
+    client.read_gatt_char.assert_awaited()
+    client.read_gatt_char.assert_called_with(characteristic)
+
+
+def invoke_callback(
+        device: BluetoothDevice,
+        fn: Callable[[BleakGATTCharacteristic, bytearray], Union[None, Awaitable[None]]],
+        sender: BleakGATTCharacteristic, data: bytes):
+
+    async def call_the_callback(fn, sender, data):
+        if inspect.iscoroutinefunction(fn):
+            f = asyncio.ensure_future(fn(sender, data), loop=device._loop.loop)
+            await asyncio.wait_for(f, 3)
+        else:
+            fn(sender, data)
+
+    return device._loop.run_async(call_the_callback(fn, sender, bytearray(data)))
 
 
 def test_wait_for_calls_notify_and_blocks_until_first_notification(client):
     gatt_characteristic = setup_characteristic(client, Service.MAGNETOMETER, Characteristic.MAGNETOMETER_CALIBRATION)
     client.start_notify.return_value = None
     client.stop_notify.return_value = None
     future = BluetoothDevice(client).wait_for(Service.MAGNETOMETER, Characteristic.MAGNETOMETER_CALIBRATION)
```

### Comparing `kaspersmicrobit-0.4.1/tests/test_do_in_tkinter.py` & `kaspersmicrobit-0.4.2/tests/test_do_in_tkinter.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/tests/test_event.py` & `kaspersmicrobit-0.4.2/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/tests/test_io_pin.py` & `kaspersmicrobit-0.4.2/tests/test_io_pin.py`

 * *Files identical despite different names*

### Comparing `kaspersmicrobit-0.4.1/tests/test_leddisplay.py` & `kaspersmicrobit-0.4.2/tests/test_leddisplay.py`

 * *Files identical despite different names*

