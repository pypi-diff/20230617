# Comparing `tmp/bunnyApi-0.1.1.tar.gz` & `tmp/bunnyapi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bunnyApi-0.1.1.tar", max compression
+gzip compressed data, was "bunnyapi-0.1.5.tar", max compression
```

## Comparing `bunnyApi-0.1.1.tar` & `bunnyapi-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       93 2021-03-31 23:40:47.327942 bunnyApi-0.1.1/bunnyapi/__init__.py
--rw-r--r--   0        0        0     3471 2021-04-01 01:01:35.626717 bunnyApi-0.1.1/bunnyapi/collections.py
--rw-r--r--   0        0        0     6827 2021-08-18 17:44:36.659438 bunnyApi-0.1.1/bunnyapi/videos.py
--rw-r--r--   0        0        0      351 2021-08-18 17:45:24.073942 bunnyApi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      618 2021-08-18 17:45:58.099338 bunnyApi-0.1.1/setup.py
--rw-r--r--   0        0        0      415 2021-08-18 17:45:58.100126 bunnyApi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      449 2022-10-22 23:04:46.381264 bunnyapi-0.1.5/bunnyapi/__init__.py
+-rw-r--r--   0        0        0     3471 2021-04-01 01:01:35.626717 bunnyapi-0.1.5/bunnyapi/collections.py
+-rw-r--r--   0        0        0     2057 2022-10-19 22:17:32.519828 bunnyapi-0.1.5/bunnyapi/storage.py
+-rw-r--r--   0        0        0     7207 2023-06-16 00:26:26.819257 bunnyapi-0.1.5/bunnyapi/videos.py
+-rw-r--r--   0        0        0      409 2023-06-15 23:57:30.968040 bunnyapi-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 bunnyapi-0.1.5/PKG-INFO
```

### Comparing `bunnyApi-0.1.1/bunnyapi/collections.py` & `bunnyapi-0.1.5/bunnyapi/collections.py`

 * *Files identical despite different names*

### Comparing `bunnyApi-0.1.1/bunnyapi/videos.py` & `bunnyapi-0.1.5/bunnyapi/videos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import BinaryIO
 import requests
 import json
 
 class VideosApi:
     
     def __init__(self, api_key: str, library_id: str):
         """
@@ -63,30 +64,29 @@
         dict: HTTP status report.
         """
         url = f'{self._base_url}/{self._library_id}/videos/{video_id}'
         r = requests.delete(url, headers=self._headers)
         r.raise_for_status()
         return r.json()
     
-    def upload_video(self, video_id: str, path: str) -> dict:
+    def upload_video(self, video_id: str, file: BinaryIO) -> dict:
         """
         Upload a video file to a video object.
 
         Parameters:
         video_id (str): The id of the video
         path (str): path of the file to upload
         
         Returns:
         dict: HTTP status response
         """
         url = f'{self._base_url}/{self._library_id}/videos/{video_id}'
-        with open(path, 'rb') as f:
-            r = requests.put(url, headers=self._headers, data=f)
-            r.raise_for_status()
-            return r.json()
+        r = requests.put(url, headers=self._headers, data=file)
+        r.raise_for_status()
+        return r.json()
 
     
     def list_videos(self, page='1', items_per_page='100', order_by='date', search=None, collection_id=None):
         """
         Retrieve a list of all videos from a library.
 
         Parameters:
@@ -163,15 +163,17 @@
         Returns:
         dict: HTTP status message
         """
         url = f'{self._base_url}/{self._library_id}/videos/{video_id}/fetch'
         payload = {'url' : video_url}
         if fetch_headers:
             payload.update(fetch_headers)
-        r = requests.post(url, data=json.dumps(payload), headers=self._headers)
+        headers = self._headers
+        headers.update({"accept": "application/json", "content-type": "application/*+json"})
+        r = requests.post(url, data=json.dumps(payload), headers=headers)
         r.raise_for_status()
         return r.json()
     
     # TODO: TEST
     def add_caption(self, video_id: str, srclang: str, label: str, captions_file: str) -> dict:
         """
         Add captions to a video
@@ -208,7 +210,13 @@
         Returns:
         dict: HTTP status message
         """
         url = f'{self._base_url}/{self._library_id}/{video_id}/captions/{srclang}'
         r = requests.delete(url, headers=self._headers)
         r.raise_for_status()
         return r.json()
+
+    def get_video_stats(self, video_id: str, fromDate: str):
+        url = f'{self._base_url}/{self._library_id}/statistics?videoGuid={video_id}&fromDate={fromDate}'
+        r = requests.get(url, headers=self._headers)
+        r.raise_for_status()
+        return r.json()
```

