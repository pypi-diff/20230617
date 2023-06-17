# Comparing `tmp/ayt-api-0.1.1.tar.gz` & `tmp/ayt-api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayt-api-0.1.1.tar", last modified: Fri Oct 28 08:50:34 2022, max compression
+gzip compressed data, was "ayt-api-0.1.2.tar", last modified: Sat Jun 17 11:22:07 2023, max compression
```

## Comparing `ayt-api-0.1.1.tar` & `ayt-api-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 bsauter   (1000) bsauter   (1000)        0 2022-10-28 08:50:34.503325 ayt-api-0.1.1/
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)     1068 2022-10-28 07:45:36.000000 ayt-api-0.1.1/LICENSE.md
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)     3413 2022-10-28 08:50:34.506659 ayt-api-0.1.1/PKG-INFO
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)     3067 2022-10-28 07:45:36.000000 ayt-api-0.1.1/README.md
-drwxr-xr-x   0 bsauter   (1000) bsauter   (1000)        0 2022-10-28 08:50:34.503325 ayt-api-0.1.1/ayt_api/
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)      484 2022-10-28 07:45:36.000000 ayt-api-0.1.1/ayt_api/__init__.py
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)    10581 2022-10-28 07:45:36.000000 ayt-api-0.1.1/ayt_api/api.py
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)     5356 2022-10-28 08:01:59.000000 ayt-api-0.1.1/ayt_api/exceptions.py
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)    48326 2022-10-28 07:45:36.000000 ayt-api-0.1.1/ayt_api/types.py
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)      595 2022-10-28 07:45:36.000000 ayt-api-0.1.1/ayt_api/utils.py
-drwxr-xr-x   0 bsauter   (1000) bsauter   (1000)        0 2022-10-28 08:50:34.503325 ayt-api-0.1.1/ayt_api.egg-info/
--rwxr-xr-x   0 bsauter   (1000) bsauter   (1000)     3413 2022-10-28 08:50:33.000000 ayt-api-0.1.1/ayt_api.egg-info/PKG-INFO
--rwxr-xr-x   0 bsauter   (1000) bsauter   (1000)      284 2022-10-28 08:50:34.000000 ayt-api-0.1.1/ayt_api.egg-info/SOURCES.txt
--rwxr-xr-x   0 bsauter   (1000) bsauter   (1000)        1 2022-10-28 08:50:34.000000 ayt-api-0.1.1/ayt_api.egg-info/dependency_links.txt
--rwxr-xr-x   0 bsauter   (1000) bsauter   (1000)       63 2022-10-28 08:50:34.000000 ayt-api-0.1.1/ayt_api.egg-info/requires.txt
--rwxr-xr-x   0 bsauter   (1000) bsauter   (1000)        8 2022-10-28 08:50:34.000000 ayt-api-0.1.1/ayt_api.egg-info/top_level.txt
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)       79 2022-10-28 08:50:34.506659 ayt-api-0.1.1/setup.cfg
--rw-r--r--   0 bsauter   (1000) bsauter   (1000)      849 2022-10-28 08:44:18.000000 ayt-api-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:22:07.010930 ayt-api-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-17 11:21:56.000000 ayt-api-0.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-17 11:22:07.010930 ayt-api-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-17 11:21:56.000000 ayt-api-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:22:07.010930 ayt-api-0.1.2/ayt_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51228 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-17 11:21:56.000000 ayt-api-0.1.2/ayt_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:22:07.010930 ayt-api-0.1.2/ayt_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 11:22:07.000000 ayt-api-0.1.2/ayt_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-17 11:21:56.000000 ayt-api-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 11:21:56.000000 ayt-api-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-17 11:22:07.010930 ayt-api-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-17 11:21:56.000000 ayt-api-0.1.2/setup.py
```

### Comparing `ayt-api-0.1.1/LICENSE.md` & `ayt-api-0.1.2/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 
-Copyright (c) 2022 Revnoplex
+Copyright (c) 2022-2023 Revnoplex
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ayt-api-0.1.1/PKG-INFO` & `ayt-api-0.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-Metadata-Version: 2.1
-Name: ayt-api
-Version: 0.1.1
-Summary: An Asynchronous, Object oriented python library for the YouTube api
-Home-page: https://github.com/Revnoplex/ayt-api
-Author: Revnoplex
-Author-email: revnoplex.business@protonmail.com
-License: MIT
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
+![PyPI](https://img.shields.io/pypi/v/ayt-api?style=for-the-badge&logo=pypi)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ayt-api?style=for-the-badge&logo=python)
+![GitHub release (latest by date)](https://img.shields.io/github/v/release/Revnoplex/ayt-api?style=for-the-badge&logo=github)
 # ayt-api
-An Asynchronous, Object oriented python library for the YouTube api
+A Basic Asynchronous, Object oriented python library for the YouTube api
 
 ## What makes ayt-api different?
-The diffrence with this library and other libraries is that it uses 
-asynchronous api calls and responces are formatted as object oriented data. 
+The difference with this library and other libraries is that it uses 
+asynchronous api calls and responses are formatted as object-oriented data. 
 
-The library is also designed towards being used in discord bots, particularly ones using the discord.py library and forks of it
+The library is also designed towards being used in python based discord bots that use an asynchronous discord api wrapper
 
 ## Installation
 
 ### Stable Release:
-The most recent stable release on pypi
+The latest stable version is available on pypi
 #### Windows:
 ```powershell
 python -m pip install -U ayt-api
 ```
 
-#### Linux and Mac os:
-```bash
+#### Unix based OSes (Linux, Mac OS, etc.):
+The pip command can vary between diffrent unix based OSes but should be simular to these:
+```sh
+python3 -m pip install -U ayt-api
+
+# or
+
 pip3 install -U ayt-api
-````
+```
 
 ### Latest Commit:
-Installing the latest commit from here
+Installing the latest commit from here. You will need git or something simular installed to download the library
 #### Windows:
 ```powershell
 python -m pip install -U "git+https://github.com/Revnoplex/ayt-api.git"
 ```
 
-#### Linux and Mac os:
-```bash
+#### Unix based OSes (Linux, Mac OS, etc.):
+The pip command can vary between diffrent unix based OSes but should be simular to these:
+```sh
+python3 -m pip install -U git+https://github.com/Revnoplex/ayt-api.git
+
+# or
+
 pip3 install -U git+https://github.com/Revnoplex/ayt-api.git
-````
+```
 
 ## Usage
 First of all to use this library, you will need an API key. To get one, [see here for instructions](https://developers.google.com/youtube/v3/getting-started)
 
 ### Basic video data fetching:
 ```python
 import asyncio
```

### Comparing `ayt-api-0.1.1/ayt_api/api.py` & `ayt-api-0.1.2/ayt_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class AsyncYoutubeAPI:
     """Represents the main class for running all the tools
     Attributes:
         key (str): The API key used to access the YouTube API. To get an API key,
             see instructions here: https://developers.google.com/youtube/v3/getting-started
         api_version (str):
             The API version to use. defaults to 3
-        call_url_prefix (str): The start of the youtube API call url to use
+        call_url_prefix (str): The start of the YouTube API call url to use
         timeout (ClientTimeout): The timeout if the api does not respond
         ignore_ssl (bool): whether to ignore any verification errors with the ssl certificate.
                 This is useful for using the api on a restricted network.
     """
     def __init__(self, yt_api_key: str, api_version: str = '3', timeout: int = 5, ignore_ssl: bool = False):
         """
         Args:
@@ -61,15 +61,15 @@
                         if "error" in res_data:
                             raise HTTPException(playlist_metadata_response, f'{res_data["error"].get("code")}:'
                                                                             f'{res_data["error"].get("message")}')
                         if res_data["pageInfo"].get("totalResults") < 1:
                             raise PlaylistNotFound(playlist_id)
                         else:
                             res_json = res_data.get("items")[0]
-                            return YoutubePlaylistMetadata(res_json, call_url)
+                            return YoutubePlaylistMetadata(res_json, call_url, self)
                     else:
                         message = f'The youtube API returned the following error code: ' \
                                   f'{playlist_metadata_response.status}'
                         if playlist_metadata_response.content_type == "application/json":
                             res_data = await playlist_metadata_response.json()
                             if "error" in res_data:
                                 error_data = res_data["error"]
@@ -113,15 +113,15 @@
                             raise PlaylistNotFound(playlist_id)
                         else:
                             res_json = res_data.get("items")
                             videos_next_page = []
                             if res_data.get("nextPageToken") is not None:
                                 videos_next_page = await self.get_videos_from_playlist(
                                     playlist_id, next_page=res_data["nextPageToken"])
-                            videos = [PlaylistVideoMetadata(vid_item, call_url) for vid_item in res_json]
+                            videos = [PlaylistVideoMetadata(vid_item, call_url, self) for vid_item in res_json]
                             return videos + videos_next_page
                     elif playlist_videos_response.status == 404:
                         raise PlaylistNotFound(playlist_id)
                     else:
                         message = f'The youtube API returned the following error code: ' \
                                   f'{playlist_videos_response.status}'
                         if playlist_videos_response.content_type == "application/json":
```

### Comparing `ayt-api-0.1.1/ayt_api/exceptions.py` & `ayt-api-0.1.2/ayt_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayt-api-0.1.1/ayt_api/types.py` & `ayt-api-0.1.2/ayt_api/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime
-import sys
 from typing import Union, Optional
 import isodate
 from .exceptions import MissingDataFromMetadata
 
 
 class YoutubeThumbnail:
     """Data for an individual YouTube thumbnail.
@@ -22,24 +21,37 @@
         """
         self.data = data
         self.url: Optional[str] = data.get("url")
         self.width: Optional[int] = data.get("width")
         self.height: Optional[int] = data.get("height")
         self.resolution = "{}x{}".format(self.width, self.height)
 
+    def __str__(self):
+        return self.url
+
+    def __repr__(self):
+        return f"YoutubeThumbnail({self.url}, {self.width},{self.height})"
+
 
 class YoutubeThumbnailMetadata:
     """Data for the available thumbnails of a video"""
     def __init__(self, thumbnail_metadata: dict):
         """
         Args:
             thumbnail_metadata (dict): the raw thumbnail metadata to provide
         """
         self.metadata = thumbnail_metadata
 
+    def __str__(self):
+        return f"Available Resolutions: {', '.join(self.metadata.keys())}"
+
+    def __repr__(self):
+        return f"YoutubeThumbnailMetadata(default={repr(self.default)},medium={repr(self.medium)}," \
+               f"high={repr(self.high)},standard={repr(self.standard)},maxres={repr(self.maxres)})"
+
     @property
     def default(self) -> Optional[YoutubeThumbnail]:
         """The default video thumbnail. Could be None.
         Returns:
             Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be None"""
         if self.metadata.get("default") is not None:
             return YoutubeThumbnail(self.metadata["default"])
@@ -73,14 +85,15 @@
         """The maximum resolution video thumbnail. Could be None
         Returns:
             Optional[YoutubeThumbnail]: A YouTube thumbnail object. Could be None"""
         if self.metadata.get("maxres") is not None:
             return YoutubeThumbnail(self.metadata["maxres"])
 
 
+
 class LocalName:
     """Represents the video title and description in a local language if available
     Attributes:
         data (dict): The raw data associated with the local text
         language (Optional[str]): The language code
         title (str): The title in a local language
         description (str): The description in a local language
@@ -126,16 +139,16 @@
     Attributes:
         acb (Optional[str]): The video's Australian Classification Board (ACB) or Australian Communications and Media
             Authority (ACMA) rating. ACMA ratings are used to classify children's television programming.
         youtube (Optional[str]): A rating that YouTube uses to identify age-restricted content.
     """
     def __init__(self, data: dict):
         """
-
-        :param data:
+        Args:
+            data(dict): The raw content rating data
         """
         self.acb: Optional[str] = data.get("acbRating")
         self.agcom: Optional[str] = data.get("agcomRating")
         self.anatel: Optional[str] = data.get("anatelRating")
         self.bbfc: Optional[str] = data.get("bbfcRatingRating")
         self.bfvc: Optional[str] = data.get("bfvcRatingRating")
         self.bmukk: Optional[str] = data.get("bmukkRatingRating")
@@ -245,15 +258,15 @@
         if data.get("recordingDate") is None:
             self.date: Optional[datetime.datetime] = None
         else:
             self.date: Optional[datetime.datetime] = isodate.parse_datetime(data["recordingDate"])
 
 
 class VideoStream:
-    """Metadata about a video stream for a youtube video
+    """Metadata about a video stream for a YouTube video
     Attributes:
         data (dict): The raw video stream data used to construct this class
         width (int): The encoded video content's width in pixels.
         height (int): The encoded video content's height in pixels.
         resolution (str): width x height
         frame_rate (float): The video stream's frame rate, in frames per second.
         aspect_ratio (float): The video content's display aspect ratio
@@ -281,15 +294,15 @@
             self.rotation: str = data["rotation"]
             self.vendor: str = data["vendor"]
         except KeyError as missing_snippet_data:
             raise MissingDataFromMetadata(str(missing_snippet_data), data, missing_snippet_data)
 
 
 class AudioStream:
-    """Metadata about an audio stream for a youtube video
+    """Metadata about an audio stream for a YouTube video
     Attributes:
         data (dict): The raw audio stream data used to construct this class
         channel_count (int): The number of audio channels that the stream contains.
         codec (string): The audio codec that the stream uses.
         bitrate (int): The audio stream's bitrate, in bits per second.
         vendor (string):
             A value that uniquely identifies a video vendor. Typically, the value is a four-letter vendor code.
@@ -314,31 +327,41 @@
     """Contains information about the progress YouTube has made in processing the video.
     Attributes:
         data (dict): The raw processing progress data used to construct this class
         parts_total (int): An estimate of the total number of parts that need to be processed for the video.
         parts_processed (int): The number of parts of the video that YouTube has already processed.
         time_left (Optional[datetime.timedelta]):
             An estimate of the amount of time, in milliseconds, that YouTube needs to finish processing the video.
+        percentage (int): The percentage of the video that has been processed
     """
     def __init__(self, data: dict):
         """
         Args:
             data (dict): Raw processing progress
         """
         self.data = data
         try:
             self.parts_total: int = data["partsTotal"]
             self.parts_processed: int = data["partsProcessed"]
             if data.get('timeLeftMs') is None:
                 self.time_left: Optional[datetime.timedelta] = None
             else:
                 self.time_left: Optional[datetime.timedelta] = datetime.timedelta(milliseconds=data["timeLeftMs"])
+            self.percentage: int = round(self.parts_processed/self.parts_total*100)
         except KeyError as missing_snippet_data:
             raise MissingDataFromMetadata(str(missing_snippet_data), data, missing_snippet_data)
 
+    def __str__(self):
+        if self.time_left:
+            return f"Processing {self.parts_processed}/{self.parts_total} " \
+                   f"({round(self.parts_processed/self.parts_total*100)}%) ETA: {self.time_left}"
+        else:
+            return f"Processing {self.parts_processed}/{self.parts_total} " \
+                   f"({round(self.parts_processed / self.parts_total * 100)}%)"
+
 
 class TagSuggestion:
     """
     A list of keyword tags that could be added to the video's metadata to increase the likelihood that users will
         locate your video when searching or browsing on YouTube.
     Attributes:
         data (dict): The raw tag suggestions data used to construct this class
@@ -350,158 +373,25 @@
         Args:
             data (dict): The raw tag suggestions data
         """
         self.data = data
         self.tag: str = data["tag"]
         self.category_restricts: Optional[list[str]] = data.get("categoryRestricts")
 
-
-class YoutubePlaylistMetadata:
-    """Data class for YouTube playlists
-    Attributes:
-        metadata (dict): The raw API response used to construct this class
-        call_url (str): The url used to call the API. Intended use is for debugging purposes
-        id (str): The ID of the playlist. Example: "PLwZcI0zn-Jhemx2m_gpYqQfnc3l4xA4fp" from the url:
-            "https://www.youtube.com/playlist?list=PLwZcI0zn-Jhemx2m_gpYqQfnc3l4xA4fp"
-        url (str): The URL of the playlist
-        snippet (dict): The raw snippet data used to construct this class
-        status (dict): The raw status data used to construct part of this class
-        content_details (dict): The raw content details data used to construct part of this class
-        player (dict): The raw player data used to construct part of this class
-        raw_localisations (Optional[dict]): The raw localisation data used to construct part of this class
-        published_at (datetime.datetime): The date and time the playlist was published
-        channel_id (Optional[str]): The id of the channel that created the playlist
-        channel_url (Optional[str]): The url of the channel that created the playlist
-        title (str): The title of the playlist
-        description (str): The description of the playlist
-        thumbnails (YoutubeThumbnailMetadata): The available thumbnails the playlist has
-        channel_title: (Optional[str]) The name of the channel that created the playlist
-        default_language (Optional[str]): The default language the video is set in. Can be None
-        localised (Optional[LocalName]): The localised language of the title and description of the video
-        localized (Optional[LocalName]): an alias of localised
-        visibility (Optional[str]): The video's privacy status. Can be private, public or unlisted
-        item_count (Optional[int]): The number of items in the playlist
-        embed_html (Optional[str]): An <iframe> tag that embeds a player that plays the video.
-        localisations (Optional[list[LocalName]]): contains translations of the video's metadata.
-        localizations (Optional[list[LocalName]]): an alias of localisations
-    """
-    def __init__(self, metadata: dict, call_url: str):
-        """
-        Args:
-            metadata (dict): The raw API response to provide
-            call_url (str): The url used to call the API. Intended use is for debugging purposes
-        Raises:
-            MissingDataFromMetaData: There is malformed data in the metadata provided
-        """
-        try:
-            self.metadata = metadata
-            self.call_url = call_url
-            self.id: str = metadata["id"]
-            self.url: str = f'https://www.youtube.com/playlist?list={self.id}'
-            self.snippet: dict = metadata["snippet"]
-            self.status: dict = metadata["status"]
-            self.content_details: dict = metadata["contentDetails"]
-            self.player: dict = metadata["player"]
-            self.raw_localisations: Optional[dict] = metadata.get("localizations")
-            self.published_at = isodate.parse_datetime(self.snippet["publishedAt"])
-            self.channel_id: Optional[str] = self.snippet.get("channelId")
-            if self.channel_id is None:
-                self.channel_url: Optional[str] = None
-            else:
-                self.channel_url: Optional[str] = f'https://www.youtube.com/channel/{self.channel_id}'
-            self.title: str = self.snippet["title"]
-            self.description: str = self.snippet["description"]
-            self.thumbnails = YoutubeThumbnailMetadata(self.snippet["thumbnails"])
-            self.channel_title: Optional[str] = self.snippet.get("channelTitle")
-            self.default_language: Optional[str] = self.snippet.get("defaultLanguage")
-            if self.snippet.get("localized") is None:
-                self.localised: Optional[LocalName] = None
-            else:
-                self.localised: Optional[LocalName] = LocalName(self.snippet["localized"])
-                self.localized = self.localised
-            self.visibility: Optional[str] = self.status.get("privacyStatus")
-            self.item_count: Optional[int] = self.content_details.get("itemCount")
-            self.embed_html: Optional[str] = self.player.get("embedHtml")
-            if self.raw_localisations is None:
-                self.localisations: Optional[list[LocalName]] = None
-            else:
-                self.localisations: Optional[list[LocalName]] = []
-                for localisation_name, localisation_value in self.raw_localisations.items():
-                    self.localisations.append(LocalName(localisation_value, localisation_name))
-            self.localizations = self.localisations
-        except KeyError as missing_snippet_data:
-            raise MissingDataFromMetadata(str(missing_snippet_data), metadata, missing_snippet_data)
+    def __str__(self):
+        if self.category_restricts:
+            return f'Tag Suggestion: "{self.tag}" with restrictions: {",".join(self.category_restricts)}'
+        else:
+            return f'Tag Suggestion: "{self.tag}"'
 
 
 class ABCVideoMetadata:
     pass
 
 
-class PlaylistVideoMetadata(ABCVideoMetadata):
-    """A data class for videos in a playlist
-    Attributes:
-        metadata (dict): The raw metadata from the API call used to construct this class
-        call_url (str): The url used to call the API. Intended use is for debugging purposes
-        id (str): The ID of the video in the playlist. Example: "dQw4w9WgXcQ" from the url:
-            "https://www.youtube.com/watch?v=dQw4w9WgXcQ". Look familiar?
-        position (int): The position in the playlist the video is in
-        url (str): The URL of the video
-        title (str): The title of the video
-        description (str): The description of the video
-        added_at (datetime.datetime): The date and time the video was added to the playlist
-        thumbnails (YoutubeThumbnailMetadata): The available thumbnails the video has
-        channel_title: (Optional[str]) The name of the channel that the video belongs to
-        channel_id (Optional[str]): The id of the channel that the video belongs to
-        channel_url (Optional[str]): The url of the channel that the video belongs to
-        playlist_id (str): The ID of the playlist the video is in
-        playlist_url (str): The URL of the playlist the video is in
-        published_at (datetime.datetime): The date and time the video was published
-        available (bool): whether the video in the playlist is playable hasn't been deleted or made private.
-            This is determined by checking if the video has an upload date.
-        note (Optional[str]): A user-generated note for this item.
-        visibility (str): The playlist item's privacy status. Can be public, private or unlisted
-    """
-    def __init__(self, metadata: dict, call_url: str):
-        """
-        Args:
-            metadata: The snippet metadata of the video in the playlist
-            call_url (str): The url used to call the API. Intended use is for debugging purposes
-        Raises:
-            MissingDataFromMetaData: There is malformed data in the metadata provided
-        """
-        try:
-            self.metadata = metadata
-            self.call_url = call_url
-            self.snippet: dict = metadata["snippet"]
-            self.content_details: dict = metadata["contentDetails"]
-            self.status: dict = metadata["status"]
-            self.added_at = isodate.parse_datetime(self.snippet["publishedAt"])
-            self.position: int = self.snippet["position"]
-            self.id: str = self.content_details["videoId"]
-            self.url: str = f'https://www.youtube.com/watch?v={self.id}'
-            self.title: str = self.snippet.get("title")
-            self.description: str = self.snippet.get('description')
-            self.thumbnails = YoutubeThumbnailMetadata(self.snippet["thumbnails"])
-            self.channel_id: Optional[str] = self.snippet.get("videoOwnerChannelId")
-            if self.channel_id is None:
-                self.channel_url: Optional[str] = None
-            else:
-                self.channel_url: Optional[str] = f'https://www.youtube.com/channel/{self.channel_id}'
-            self.channel_title: Optional[str] = self.snippet.get("videoOwnerChannelTitle")
-            self.playlist_id: str = self.snippet["playlistId"]
-            self.playlist_url = f'https://www.youtube.com/playlist?list={self.playlist_id}'
-            self.note: Optional[str] = self.content_details.get("note")
-            self.published_at = None if self.content_details.get("videoPublishedAt") is None else \
-                isodate.parse_datetime(self.content_details["videoPublishedAt"])
-            self.available = bool(self.published_at)
-            self.visibility: str = self.status.get("privacyStatus")
-        except KeyError as missing_snippet_data:
-            raise MissingDataFromMetadata(str(missing_snippet_data), metadata, missing_snippet_data)
-
-
 class YoutubeVideoMetadata(ABCVideoMetadata):
     """A data class containing video data such as the title, id, description, channel, etc.
         Attributes:
             metadata (dict): The raw API response used to construct this class
             call_url (str): The url used to call the API. Intended use is for debugging purposes
             id (str): The ID of the video. Example: "dQw4w9WgXcQ" from the url:
                 "https://www.youtube.com/watch?v=dQw4w9WgXcQ". Look familiar?
@@ -517,16 +407,16 @@
             title (str): The title of the video
             description (str): The description of the video
             published_at (datetime.datetime): The date and time the video was published
             thumbnails (YoutubeThumbnailMetadata): The available thumbnails the video has
             channel_title: (Optional[str]) The name of the channel that the video belongs to
             channel_id (Optional[str]): The id of the channel that the video belongs to
             channel_url (Optional[str]): The url of the channel that the video belongs to.
-            tags (Optional[list[str]]): The tags the uploaded has provided to make the video appear in search results relating
-                to it
+            tags (Optional[list[str]]): The tags the uploaded has provided to make the video appear in search results
+                relating to it
             category_id (int): The id of the category that was set for the video
             live_broadcast_content: (str): Indicates if the video is a livestream and if it is live
             default_language (Optional[str]): The default language the video is set in
             localised (Optional[LocalName]): The localised language of the title and description of the video
             localized (Optional[LocalName]): an alias of localised
             default_audio_language (Optional[str]): The default audio language the video is set in
             duration (Union[isodate.Duration, datetime.timedelta, _NotImplementedType]): The length of the video
@@ -703,14 +593,191 @@
                     self.localisations.append(LocalName(localisation[1], localisation[0]))
             self.localizations = self.localisations
 
         except KeyError as missing_snippet_data:
             raise MissingDataFromMetadata(str(missing_snippet_data), metadata, missing_snippet_data)
 
 
+class PlaylistVideoMetadata(ABCVideoMetadata):
+    """A data class for videos in a playlist
+    Attributes:
+        metadata (dict): The raw metadata from the API call used to construct this class
+        call_url (str): The url used to call the API. Intended use is for debugging purposes
+        id (str): The ID of the video in the playlist. Example: "dQw4w9WgXcQ" from the url:
+            "https://www.youtube.com/watch?v=dQw4w9WgXcQ". Look familiar?
+        position (int): The position in the playlist the video is in
+        url (str): The URL of the video
+        title (str): The title of the video
+        description (str): The description of the video
+        added_at (datetime.datetime): The date and time the video was added to the playlist
+        thumbnails (YoutubeThumbnailMetadata): The available thumbnails the video has
+        channel_title: (Optional[str]) The name of the channel that the video belongs to
+        channel_id (Optional[str]): The id of the channel that the video belongs to
+        channel_url (Optional[str]): The url of the channel that the video belongs to
+        playlist_id (str): The ID of the playlist the video is in
+        playlist_url (str): The URL of the playlist the video is in
+        published_at (datetime.datetime): The date and time the video was published
+        available (bool): whether the video in the playlist is playable hasn't been deleted or made private.
+            This is determined by checking if the video has an upload date.
+        note (Optional[str]): A user-generated note for this item.
+        visibility (str): The playlist item's privacy status. Can be public, private or unlisted
+    """
+    def __init__(self, metadata: dict, call_url: str, call_data):
+        """
+        Args:
+            metadata: The snippet metadata of the video in the playlist
+            call_url (str): The url used to call the API. Intended use is for debugging purposes
+        Raises:
+            MissingDataFromMetaData: There is malformed data in the metadata provided
+        """
+        try:
+            self.metadata = metadata
+            self.call_url = call_url
+            self._call_data = call_data
+            self.snippet: dict = metadata["snippet"]
+            self.content_details: dict = metadata["contentDetails"]
+            self.status: dict = metadata["status"]
+            self.added_at = isodate.parse_datetime(self.snippet["publishedAt"])
+            self.position: int = self.snippet["position"]
+            self.id: str = self.content_details["videoId"]
+            self.url: str = f'https://www.youtube.com/watch?v={self.id}'
+            self.title: str = self.snippet.get("title")
+            self.description: str = self.snippet.get('description')
+            self.thumbnails = YoutubeThumbnailMetadata(self.snippet["thumbnails"])
+            self.channel_id: Optional[str] = self.snippet.get("videoOwnerChannelId")
+            if self.channel_id is None:
+                self.channel_url: Optional[str] = None
+            else:
+                self.channel_url: Optional[str] = f'https://www.youtube.com/channel/{self.channel_id}'
+            self.channel_title: Optional[str] = self.snippet.get("videoOwnerChannelTitle")
+            self.playlist_id: str = self.snippet["playlistId"]
+            self.playlist_url = f'https://www.youtube.com/playlist?list={self.playlist_id}'
+            self.note: Optional[str] = self.content_details.get("note")
+            self.published_at = None if self.content_details.get("videoPublishedAt") is None else \
+                isodate.parse_datetime(self.content_details["videoPublishedAt"])
+            self.available = bool(self.published_at)
+            self.visibility: str = self.status.get("privacyStatus")
+        except KeyError as missing_snippet_data:
+            raise MissingDataFromMetadata(str(missing_snippet_data), metadata, missing_snippet_data)
+
+    async def extended_data(self) -> YoutubeVideoMetadata:
+        """Fetches extended information on the video in the playlist
+
+        This ia an api call which then returns a
+        :class:`YoutubeVideoMetadata` object
+
+        Returns:
+            YoutubeVideoMetadata: The video object containing data of the video
+        Raises:
+            HTTPException: Fetching the metadata failed
+            VideoNotFound: The video does not exist
+            aiohttp.ClientError: There was a problem sending the request to the api
+            InvalidInput: The input is not a playlist id
+        """
+        from .api import AsyncYoutubeAPI
+        api: AsyncYoutubeAPI = self._call_data
+        return await api.get_video_metadata(self.id)
+
+
+class YoutubePlaylistMetadata:
+    """Data class for YouTube playlists
+    Attributes:
+        metadata (dict): The raw API response used to construct this class
+        call_url (str): The url used to call the API. Intended use is for debugging purposes
+        id (str): The ID of the playlist. Example: "PLwZcI0zn-Jhemx2m_gpYqQfnc3l4xA4fp" from the url:
+            "https://www.youtube.com/playlist?list=PLwZcI0zn-Jhemx2m_gpYqQfnc3l4xA4fp"
+        url (str): The URL of the playlist
+        snippet (dict): The raw snippet data used to construct this class
+        status (dict): The raw status data used to construct part of this class
+        content_details (dict): The raw content details data used to construct part of this class
+        player (dict): The raw player data used to construct part of this class
+        raw_localisations (Optional[dict]): The raw localisation data used to construct part of this class
+        published_at (datetime.datetime): The date and time the playlist was published
+        channel_id (Optional[str]): The id of the channel that created the playlist
+        channel_url (Optional[str]): The url of the channel that created the playlist
+        title (str): The title of the playlist
+        description (str): The description of the playlist
+        thumbnails (YoutubeThumbnailMetadata): The available thumbnails the playlist has
+        channel_title: (Optional[str]) The name of the channel that created the playlist
+        default_language (Optional[str]): The default language the video is set in. Can be None
+        localised (Optional[LocalName]): The localised language of the title and description of the video
+        localized (Optional[LocalName]): an alias of localised
+        visibility (Optional[str]): The video's privacy status. Can be private, public or unlisted
+        item_count (Optional[int]): The number of items in the playlist
+        embed_html (Optional[str]): An <iframe> tag that embeds a player that plays the video.
+        localisations (Optional[list[LocalName]]): contains translations of the video's metadata.
+        localizations (Optional[list[LocalName]]): an alias of localisations
+    """
+    def __init__(self, metadata: dict, call_url: str, call_data):
+        """
+        Args:
+            metadata (dict): The raw API response to provide
+            call_url (str): The url used to call the API. Intended use is for debugging purposes
+        Raises:
+            MissingDataFromMetaData: There is malformed data in the metadata provided
+        """
+        try:
+            self.metadata = metadata
+            self.call_url = call_url
+            self._call_data = call_data
+            self.id: str = metadata["id"]
+            self.url: str = f'https://www.youtube.com/playlist?list={self.id}'
+            self.snippet: dict = metadata["snippet"]
+            self.status: dict = metadata["status"]
+            self.content_details: dict = metadata["contentDetails"]
+            self.player: dict = metadata["player"]
+            self.raw_localisations: Optional[dict] = metadata.get("localizations")
+            self.published_at = isodate.parse_datetime(self.snippet["publishedAt"])
+            self.channel_id: Optional[str] = self.snippet.get("channelId")
+            if self.channel_id is None:
+                self.channel_url: Optional[str] = None
+            else:
+                self.channel_url: Optional[str] = f'https://www.youtube.com/channel/{self.channel_id}'
+            self.title: str = self.snippet["title"]
+            self.description: str = self.snippet["description"]
+            self.thumbnails = YoutubeThumbnailMetadata(self.snippet["thumbnails"])
+            self.channel_title: Optional[str] = self.snippet.get("channelTitle")
+            self.default_language: Optional[str] = self.snippet.get("defaultLanguage")
+            if self.snippet.get("localized") is None:
+                self.localised: Optional[LocalName] = None
+            else:
+                self.localised: Optional[LocalName] = LocalName(self.snippet["localized"])
+                self.localized = self.localised
+            self.visibility: Optional[str] = self.status.get("privacyStatus")
+            self.item_count: Optional[int] = self.content_details.get("itemCount")
+            self.embed_html: Optional[str] = self.player.get("embedHtml")
+            if self.raw_localisations is None:
+                self.localisations: Optional[list[LocalName]] = None
+            else:
+                self.localisations: Optional[list[LocalName]] = []
+                for localisation_name, localisation_value in self.raw_localisations.items():
+                    self.localisations.append(LocalName(localisation_value, localisation_name))
+            self.localizations = self.localisations
+        except KeyError as missing_snippet_data:
+            raise MissingDataFromMetadata(str(missing_snippet_data), metadata, missing_snippet_data)
+
+    async def fetch_videos(self) -> list[PlaylistVideoMetadata]:
+        """
+        Fetches a list of the videos in the playlist
+
+        This is an api call which returns a list of
+        :class:`PlaylistVideoMetadata` objects
+        Returns:
+            list[PlaylistVideoMetadata]: A list containing playlist video objects
+        Raises:
+            HTTPException: Fetching the metadata failed
+            PlaylistNotFound: The playlist does not exist
+            aiohttp.ClientError: There was a problem sending the request to the api
+            InvalidInput: The input is not a playlist id
+        """
+        from .api import AsyncYoutubeAPI
+        api: AsyncYoutubeAPI = self._call_data
+        return await api.get_videos_from_playlist(self.id)
+
+
 class AuthorisedYoutubeVideoMetadata(YoutubeVideoMetadata):
     """
     A data class containing owner only information video data such as the file and processing information.
 
         THis class is used if authorisation is provided that you are the owner of the video. It contains
         attributes only accessible by the video owner as well as attributes inherited
         from :class:`YoutubeVideoMetadata`
```

### Comparing `ayt-api-0.1.1/ayt_api/utils.py` & `ayt-api-0.1.2/ayt_api/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 def strip_video_id(url: str) -> str:
     """supported urls:
     https://www.youtube.com/watch?v=ID
 
     https://www.youtube.com/v/ID
 
     https://youtu.be/ID"
```

