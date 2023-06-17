# Comparing `tmp/dfipy-1.0.0.tar.gz` & `tmp/dfipy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfipy-1.0.0.tar", max compression
+gzip compressed data, was "dfipy-1.0.1.tar", max compression
```

## Comparing `dfipy-1.0.0.tar` & `dfipy-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      568 2023-06-16 14:58:35.487264 dfipy-1.0.0/LICENCE
--rw-r--r--   0        0        0     1713 2023-06-16 14:58:35.487264 dfipy-1.0.0/README.md
--rw-r--r--   0        0        0       27 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/__init__.py
--rw-r--r--   0        0        0    11774 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/analyse.py
--rw-r--r--   0        0        0     1537 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/client.py
--rw-r--r--   0        0        0     3648 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/connect.py
--rw-r--r--   0        0        0    20524 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/get.py
--rw-r--r--   0        0        0      351 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/models.py
--rw-r--r--   0        0        0     3064 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/polygons.py
--rw-r--r--   0        0        0     5325 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/show.py
--rw-r--r--   0        0        0     8731 2023-06-16 14:58:35.487264 dfipy-1.0.0/dfi/validate.py
--rw-r--r--   0        0        0     1985 2023-06-16 14:58:42.711287 dfipy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 dfipy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      568 2023-06-17 20:34:31.360243 dfipy-1.0.1/LICENCE
+-rw-r--r--   0        0        0     1713 2023-06-17 20:34:31.360243 dfipy-1.0.1/README.md
+-rw-r--r--   0        0        0       27 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/__init__.py
+-rw-r--r--   0        0        0    11774 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/analyse.py
+-rw-r--r--   0        0        0     1537 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/client.py
+-rw-r--r--   0        0        0     3648 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/connect.py
+-rw-r--r--   0        0        0    20533 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/get.py
+-rw-r--r--   0        0        0      351 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/models.py
+-rw-r--r--   0        0        0     3064 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/polygons.py
+-rw-r--r--   0        0        0     5325 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/show.py
+-rw-r--r--   0        0        0     8731 2023-06-17 20:34:31.360243 dfipy-1.0.1/dfi/validate.py
+-rw-r--r--   0        0        0     1985 2023-06-17 20:34:40.048340 dfipy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 dfipy-1.0.1/PKG-INFO
```

### Comparing `dfipy-1.0.0/LICENCE` & `dfipy-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.0/README.md` & `dfipy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.0/dfi/analyse.py` & `dfipy-1.0.1/dfi/analyse.py`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.0/dfi/client.py` & `dfipy-1.0.1/dfi/client.py`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.0/dfi/connect.py` & `dfipy-1.0.1/dfi/connect.py`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.0/dfi/get.py` & `dfipy-1.0.1/dfi/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Composition of the class Connection.
 """
 import json
 import logging
 import warnings
 from datetime import datetime
 from time import sleep
-from typing import List, Optional, Tuple, Union
+from typing import Any, List, Optional, Tuple, Union
 
 import pandas as pd
 import requests
 import sseclient
 from tqdm import tqdm
 
 from dfi import models, validate
@@ -363,15 +363,15 @@
                 params["startTime"], params["endTime"] = unpack_and_convert_time_interval(time_interval)
             min_lng, min_lat, max_lng, max_lat = polygon
             with self.conn.api_get(
                 f"bounding-box/{min_lng}/{min_lat}/{max_lng}/{max_lat}/entities", params=params, stream=True
             ) as response:
                 self._receive_entities(response)
 
-    def _receive_entities(self, response: requests.models.Response) -> List[any]:
+    def _receive_entities(self, response: requests.models.Response) -> List[Any]:
         """
         Helper function to parse clients events as entities and optionally show the progress bar.
         """
         client = sseclient.SSEClient(response)
         results = []
         results_found = False
         previous = 0
@@ -397,24 +397,24 @@
             else:
                 _raise_unexpected_event_found(event)
 
         if not results_found:
             _raise_message_event_not_reached()
         return results
 
-    def _receive_history(self, response: requests.models.Response) -> List[any]:
+    def _receive_history(self, response: requests.models.Response) -> List[Any]:
         """
         Helper function to parse clients events as history and optionally show the progress bar.
         """
         client = sseclient.SSEClient(response)
 
         results = []
         results_found = False
         previous = 0
-        for event in (pbar := tqdm(client.events(), disable=self.conn.progress_bar)):
+        for event in (pbar := tqdm(client.events(), disable=not self.conn.progress_bar)):
             if event.event == "keepAlive":
                 continue
             elif event.event == "finish":
                 break
             elif event.event == "message":
                 results_found = True
                 results += json.loads(event.data)
```

### Comparing `dfipy-1.0.0/dfi/polygons.py` & `dfipy-1.0.1/dfi/polygons.py`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.0/dfi/show.py` & `dfipy-1.0.1/dfi/show.py`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.0/dfi/validate.py` & `dfipy-1.0.1/dfi/validate.py`

 * *Files identical despite different names*

### Comparing `dfipy-1.0.0/pyproject.toml` & `dfipy-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ] # List of note tags to take in consideration, separated by a comma.
 
 [tool.poetry]
 name = "dfipy"
 # Package versions are derived from Git tags in CI and overridden during
 # building/publishing. See build/publish jobs in .gitlab-ci.yml.
 # Keep the following version at 0.0.0 as it is not used anyway.
-version = "1.0.0"
+version = "1.0.1"
 description = "DFI api python wrapper"
 authors = [
   "Maurizio Morriello <maurizio.morriello@generalsystem.com>",
   "Sebastiano Ferraris <sebastiano.ferraris@generalsystem.com>",
 ]
 readme = "README.md"
 include = ["LICENCE"]
```

### Comparing `dfipy-1.0.0/PKG-INFO` & `dfipy-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dfipy
-Version: 1.0.0
+Version: 1.0.1
 Summary: DFI api python wrapper
 Author: Maurizio Morriello
 Author-email: maurizio.morriello@generalsystem.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

