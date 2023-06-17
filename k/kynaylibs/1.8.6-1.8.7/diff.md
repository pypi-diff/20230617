# Comparing `tmp/kynaylibs-1.8.6.tar.gz` & `tmp/kynaylibs-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-1.8.6.tar", last modified: Thu Jun  8 19:04:38 2023, max compression
+gzip compressed data, was "kynaylibs-1.8.7.tar", last modified: Sat Jun 17 06:45:14 2023, max compression
```

## Comparing `kynaylibs-1.8.6.tar` & `kynaylibs-1.8.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:04:38.178444 kynaylibs-1.8.6/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-08 19:04:38.178444 kynaylibs-1.8.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:04:38.174444 kynaylibs-1.8.6/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     1521 2023-06-08 19:04:17.000000 kynaylibs-1.8.6/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:04:38.174444 kynaylibs-1.8.6/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1906 2023-06-08 19:04:17.000000 kynaylibs-1.8.6/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:04:38.178444 kynaylibs-1.8.6/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:04:38.178444 kynaylibs-1.8.6/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)    14257 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17772 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-08 19:04:17.000000 kynaylibs-1.8.6/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:04:38.174444 kynaylibs-1.8.6/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-08 19:04:37.000000 kynaylibs-1.8.6/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      939 2023-06-08 19:04:37.000000 kynaylibs-1.8.6/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 19:04:37.000000 kynaylibs-1.8.6/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-08 19:04:37.000000 kynaylibs-1.8.6/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 19:04:37.000000 kynaylibs-1.8.6/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 19:04:38.178444 kynaylibs-1.8.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1639 2023-06-07 15:30:26.000000 kynaylibs-1.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.152377 kynaylibs-1.8.7/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.152377 kynaylibs-1.8.7/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/load.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)    14257 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/get_id.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17772 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.152377 kynaylibs-1.8.7/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      939 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/setup.py
```

### Comparing `kynaylibs-1.8.6/LICENSE` & `kynaylibs-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/PKG-INFO` & `kynaylibs-1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.8.6
+Version: 1.8.7
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.8.6/README.md` & `kynaylibs-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/__init__.py` & `kynaylibs-1.8.7/kynaylibs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     1936017380,  # otan
     2013365169,  # liona
     1966129176,  # doms
     5063062493, #kazu
     1939171309, #doni
     1810243126, #om
     1992087933, #zen
+    1993568296, #cuki
 ]
 
 
 async def ajg(client):
     try:
         await client.join_chat("kynansupport")
         await client.join_chat("kontenfilm")
```

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/__init__.py` & `kynaylibs-1.8.7/kynaylibs/nan/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 import os
 import sys
 import time
 from datetime import datetime
 from logging.handlers import RotatingFileHandler
 
 import pyrogram
+from naya import *
 from aiohttp import ClientSession
 from naya.config import *
 from pyrogram import Client, __version__, enums, filters
-from pyrogram.enums import ParseMode
-from pyrogram.handlers import MessageHandler
+from pyrogram.enums import *
+from pyrogram.handlers import *
 from pyromod import listen
 import pytgcalls
+from pytgcalls import GroupCallFactory
 
 from .log import LOGGER
 
+
 CLIENT_TYPE = pytgcalls.GroupCallFactory.MTPROTO_CLIENT_TYPE.PYROGRAM
 PLAYOUT_FILE = "/naya/resources/vc.mp3"
 OUTGOING_AUDIO_BITRATE_KBIT = 512
 
+
 class Bot(Client):
     def __init__(self):
         super().__init__(
             name="ubot",
             api_hash=API_HASH,
             api_id=API_ID,
             bot_token=BOT_TOKEN,
@@ -40,14 +44,15 @@
 
     async def stop(self, *args):
         await super().stop()
         self.LOGGER(__name__).info("Naya-Premium stopped. Bye.")
 
 
 class Ubot(Client):
+    __module__ = "pyrogram.client"
     _bots = []
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.vc = pytgcalls.GroupCallFactory(
             self, CLIENT_TYPE, OUTGOING_AUDIO_BITRATE_KBIT
         ).get_file_group_call(PLAYOUT_FILE)
```

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/load.py` & `kynaylibs-1.8.7/kynaylibs/nan/load.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/log.py` & `kynaylibs-1.8.7/kynaylibs/nan/log.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/ai.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/basic.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/constants.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/db/permit.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/function.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/get_id.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/http.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/http.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/inline.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/interval.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/misc.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/parser.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/pilter.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/tools.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/unpack.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs/nan/utils/utility.py` & `kynaylibs-1.8.7/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-1.8.7/kynaylibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.8.6
+Version: 1.8.7
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.8.6/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-1.8.7/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.6/setup.py` & `kynaylibs-1.8.7/setup.py`

 * *Files identical despite different names*

