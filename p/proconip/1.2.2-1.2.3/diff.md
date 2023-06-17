# Comparing `tmp/proconip-1.2.2.tar.gz` & `tmp/proconip-1.2.3.tar.gz`

## Comparing `proconip-1.2.2.tar` & `proconip-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.2/SECURITY.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.2/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.2/.github/workflows/unittest.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.2/src/requirements.txt
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.2/src/setup.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.2/src/proconip/__init__.py
--rw-r--r--   0        0        0     8189 2020-02-02 00:00:00.000000 proconip-1.2.2/src/proconip/api.py
--rw-r--r--   0        0        0    23557 2020-02-02 00:00:00.000000 proconip-1.2.2/src/proconip/definitions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.2/tests/helper.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.2/tests/requirements.txt
--rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.2/tests/test_definitions.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.2/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.2/LICENSE
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.2/README.md
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 proconip-1.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 proconip-1.2.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 proconip-1.2.3/SECURITY.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 proconip-1.2.3/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 proconip-1.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 proconip-1.2.3/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 proconip-1.2.3/src/requirements.txt
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 proconip-1.2.3/src/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.3/src/proconip/__init__.py
+-rw-r--r--   0        0        0     8268 2020-02-02 00:00:00.000000 proconip-1.2.3/src/proconip/api.py
+-rw-r--r--   0        0        0    23557 2020-02-02 00:00:00.000000 proconip-1.2.3/src/proconip/definitions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 proconip-1.2.3/tests/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 proconip-1.2.3/tests/helper.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 proconip-1.2.3/tests/requirements.txt
+-rw-r--r--   0        0        0    12006 2020-02-02 00:00:00.000000 proconip-1.2.3/tests/test_definitions.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 proconip-1.2.3/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 proconip-1.2.3/LICENSE
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 proconip-1.2.3/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 proconip-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 proconip-1.2.3/PKG-INFO
```

### Comparing `proconip-1.2.2/CODE_OF_CONDUCT.md` & `proconip-1.2.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/CONTRIBUTING.md` & `proconip-1.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/.github/workflows/pylint.yml` & `proconip-1.2.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/.github/workflows/python-publish.yml` & `proconip-1.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/.github/workflows/unittest.yml` & `proconip-1.2.3/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/src/proconip/api.py` & `proconip-1.2.3/src/proconip/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 from aiohttp import BasicAuth, ClientSession
 from yarl import URL
 
 from .definitions import (
     API_PATH_GET_STATE,
     API_PATH_USRCFG,
     API_PATH_COMMAND,
+    BadRelayException,
     ConfigObject,
     DosageTarget,
     GetStateData,
     Relay,
-    BadRelayException
 )
 
 
 async def async_get_raw_state(client_session: ClientSession, config: ConfigObject) -> str:
     """Get raw data (csv string) from the GetState.csv interface."""
     url = URL(config.base_url).with_path(API_PATH_GET_STATE)
     result = await client_session.get(url,
                                       auth=BasicAuth(config.username,
                                                      password=config.password))
-    if result.status == 200:
-        return await result.text()
     if result.status in [401, 403]:
         raise BadCredentialsException
+    if result.status != 200:
+        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
+    return await result.text()
 
 
 async def async_get_state(client_session: ClientSession, config: ConfigObject) -> GetStateData:
     """Get structured data from the GetState.csv interface."""
     raw_data = await async_get_raw_state(client_session, config)
     structured_data = GetStateData(raw_data)
     return structured_data
@@ -62,18 +63,18 @@
     bit_state[0] |= relay_bit_mask
     bit_state[1] |= relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
                                        data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
                                        auth=BasicAuth(config.username,
                                                       password=config.password))
-    if result.status != 200:
-        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
+    if result.status != 200:
+        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
 
 
 async def async_switch_off(
         client_session: ClientSession,
         config: ConfigObject,
         current_state: GetStateData,
         relay: Relay) -> None:
@@ -83,18 +84,18 @@
     bit_state[0] |= relay_bit_mask
     bit_state[1] &= ~relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
                                        data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
                                        auth=BasicAuth(config.username,
                                                       password=config.password))
-    if result.status != 200:
-        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
+    if result.status != 200:
+        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
 
 
 async def async_set_auto_mode(
         client_session: ClientSession,
         config: ConfigObject,
         current_state: GetStateData,
         relay: Relay) -> None:
@@ -104,18 +105,18 @@
     bit_state[0] &= ~relay_bit_mask
     bit_state[1] &= ~relay_bit_mask
     url = URL(config.base_url).with_path(API_PATH_USRCFG)
     result = await client_session.post(url,
                                        data=f"ENA={bit_state[0]},{bit_state[1]}&MANUAL=1",
                                        auth=BasicAuth(config.username,
                                                       password=config.password))
-    if result.status != 200:
-        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
+    if result.status != 200:
+        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
 
 
 class RelaySwitch:
     """RelaySwitch class to set relay states via usrcfg.cgi interface."""
     def __init__(self, client_session: ClientSession, config: ConfigObject):
         self.client_session = client_session
         self.config = config
@@ -143,24 +144,24 @@
 
 
 async def async_start_dosage(
         client_session: ClientSession,
         config: ConfigObject,
         dosage_target: DosageTarget,
         dosage_duration: int) -> None:
-    """Start manual dosge for given target and duration."""
+    """Start manual dosage for given target and duration."""
     url = URL(config.base_url)\
         .with_path(API_PATH_COMMAND)\
         .with_query(f"MAN_DOSAGE={dosage_target},{dosage_duration}")
     result = await client_session.get(url, auth=BasicAuth(config.username,
                                                           password=config.password))
-    if result.status != 200:
-        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
     if result.status in [401, 403]:
         raise BadCredentialsException
+    if result.status != 200:
+        raise BadStatusCodeException(f"Unexpected status code: {result.status}")
 
 
 class DosageControl:
     """DosageControl class to start manual dosage via Command.htm endpoint."""
     def __init__(self, client_session: ClientSession, config: ConfigObject):
         self.client_session = client_session
         self.config = config
```

### Comparing `proconip-1.2.2/src/proconip/definitions.py` & `proconip-1.2.3/src/proconip/definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/tests/helper.py` & `proconip-1.2.3/tests/helper.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/tests/test_definitions.py` & `proconip-1.2.3/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/.gitignore` & `proconip-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/LICENSE` & `proconip-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/README.md` & `proconip-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `proconip-1.2.2/pyproject.toml` & `proconip-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "proconip"
-version = "1.2.2"
+version = "1.2.3"
 authors = [
   { name="Yannic Labonte", email="yannic.labonte@gmail.com" },
 ]
 description = "Library for basic interaction with the Procon.IP pool controller unit."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `proconip-1.2.2/PKG-INFO` & `proconip-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proconip
-Version: 1.2.2
+Version: 1.2.3
 Summary: Library for basic interaction with the Procon.IP pool controller unit.
 Project-URL: Homepage, https://github.com/ylabonte/proconip-pypi
 Project-URL: Bug Tracker, https://github.com/ylabonte/proconip-pypi/issues
 Author-email: Yannic Labonte <yannic.labonte@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

