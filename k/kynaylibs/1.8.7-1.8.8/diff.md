# Comparing `tmp/kynaylibs-1.8.7.tar.gz` & `tmp/kynaylibs-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kynaylibs-1.8.7.tar", last modified: Sat Jun 17 06:45:14 2023, max compression
+gzip compressed data, was "kynaylibs-1.8.8.tar", last modified: Sat Jun 17 06:51:38 2023, max compression
```

## Comparing `kynaylibs-1.8.7.tar` & `kynaylibs-1.8.8.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/
--rw-r--r--   0 root         (0) root         (0)    35182 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.152377 kynaylibs-1.8.7/kynaylibs/
--rw-r--r--   0 root         (0) root         (0)     1543 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.152377 kynaylibs-1.8.7/kynaylibs/nan/
--rw-r--r--   0 root         (0) root         (0)     1980 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/load.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/kynaylibs/nan/utils/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/PyroHelpers.py
--rw-r--r--   0 root         (0) root         (0)      371 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/adminHelpers.py
--rw-r--r--   0 root         (0) root         (0)      651 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/ai.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/aiohttp_helper.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/basic.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/kynaylibs/nan/utils/db/
--rw-r--r--   0 root         (0) root         (0)    14257 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/db/permit.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/function.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/get_id.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/http.py
--rw-r--r--   0 root         (0) root         (0)     2055 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/inline.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/interval.py
--rw-r--r--   0 root         (0) root         (0)     3620 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/misc.py
--rw-r--r--   0 root         (0) root         (0)      555 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/parser.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/pilter.py
--rw-r--r--   0 root         (0) root         (0)    17772 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/tools.py
--rw-r--r--   0 root         (0) root         (0)      567 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2027 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/nan/utils/utility.py
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/kynaylibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:45:14.152377 kynaylibs-1.8.7/kynaylibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2566 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      939 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-17 06:45:13.000000 kynaylibs-1.8.7/kynaylibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 06:45:14.156377 kynaylibs-1.8.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1639 2023-06-17 06:44:57.000000 kynaylibs-1.8.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:51:38.394397 kynaylibs-1.8.8/
+-rw-r--r--   0 root         (0) root         (0)    35182 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-17 06:51:38.394397 kynaylibs-1.8.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:51:38.386397 kynaylibs-1.8.8/kynaylibs/
+-rw-r--r--   0 root         (0) root         (0)     1543 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:51:38.386397 kynaylibs-1.8.8/kynaylibs/nan/
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-17 06:50:30.000000 kynaylibs-1.8.8/kynaylibs/nan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/load.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:51:38.394397 kynaylibs-1.8.8/kynaylibs/nan/utils/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/PyroHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      371 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/adminHelpers.py
+-rw-r--r--   0 root         (0) root         (0)      651 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/ai.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/aiohttp_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/basic.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:51:38.394397 kynaylibs-1.8.8/kynaylibs/nan/utils/db/
+-rw-r--r--   0 root         (0) root         (0)    14257 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/db/permit.py
+-rw-r--r--   0 root         (0) root         (0)     4007 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/function.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/get_id.py
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/http.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/interval.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/misc.py
+-rw-r--r--   0 root         (0) root         (0)      555 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/pilter.py
+-rw-r--r--   0 root         (0) root         (0)    17772 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/tools.py
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/kynaylibs/nan/utils/utility.py
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-17 06:50:30.000000 kynaylibs-1.8.8/kynaylibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 06:51:38.386397 kynaylibs-1.8.8/kynaylibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-06-17 06:51:38.000000 kynaylibs-1.8.8/kynaylibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      939 2023-06-17 06:51:38.000000 kynaylibs-1.8.8/kynaylibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 06:51:38.000000 kynaylibs-1.8.8/kynaylibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-17 06:51:38.000000 kynaylibs-1.8.8/kynaylibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-17 06:51:38.000000 kynaylibs-1.8.8/kynaylibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 06:51:38.398397 kynaylibs-1.8.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-06-17 06:44:57.000000 kynaylibs-1.8.8/setup.py
```

### Comparing `kynaylibs-1.8.7/LICENSE` & `kynaylibs-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/PKG-INFO` & `kynaylibs-1.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.8.7
+Version: 1.8.8
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.8.7/README.md` & `kynaylibs-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/__init__.py` & `kynaylibs-1.8.8/kynaylibs/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/__init__.py` & `kynaylibs-1.8.8/kynaylibs/nan/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,32 +2,25 @@
 import os
 import sys
 import time
 from datetime import datetime
 from logging.handlers import RotatingFileHandler
 
 import pyrogram
-from naya import *
 from aiohttp import ClientSession
 from naya.config import *
 from pyrogram import Client, __version__, enums, filters
-from pyrogram.enums import *
-from pyrogram.handlers import *
+from pyrogram.enums import ParseMode
+from pyrogram.handlers import MessageHandler
 from pyromod import listen
-import pytgcalls
 from pytgcalls import GroupCallFactory
 
 from .log import LOGGER
 
 
-CLIENT_TYPE = pytgcalls.GroupCallFactory.MTPROTO_CLIENT_TYPE.PYROGRAM
-PLAYOUT_FILE = "/naya/resources/vc.mp3"
-OUTGOING_AUDIO_BITRATE_KBIT = 512
-
-
 class Bot(Client):
     def __init__(self):
         super().__init__(
             name="ubot",
             api_hash=API_HASH,
             api_id=API_ID,
             bot_token=BOT_TOKEN,
@@ -49,19 +42,17 @@
 
 class Ubot(Client):
     __module__ = "pyrogram.client"
     _bots = []
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.vc = pytgcalls.GroupCallFactory(
-            self, CLIENT_TYPE, OUTGOING_AUDIO_BITRATE_KBIT
-        ).get_file_group_call(PLAYOUT_FILE)
+        self.group_call = GroupCallFactory(self).get_group_call()
 
-    def on_message(self, filters=filters.Filter, group=1):
+    def on_message(self, filters=filters.Filter, group=-1):
         def decorator(func):
             for bot in self._bots:
                 bot.add_handler(MessageHandler(func, filters), group)
             return func
 
         return decorator
 
@@ -69,8 +60,8 @@
         await super().start()
         if self not in self._bots:
             self._bots.append(self)
 
     async def stop(self, *args):
         await super().stop()
         if self not in self._bots:
-            self._bots.append(self)
+            self._bots.append(self)
```

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/load.py` & `kynaylibs-1.8.8/kynaylibs/nan/load.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/log.py` & `kynaylibs-1.8.8/kynaylibs/nan/log.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/PyroHelpers.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/PyroHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/adminHelpers.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/adminHelpers.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/ai.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/ai.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/aiohttp_helper.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/aiohttp_helper.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/basic.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/basic.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/constants.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/constants.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/db/__init__.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/db/permit.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/db/permit.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/function.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/function.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/get_id.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/get_id.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/http.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/http.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/inline.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/inline.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/interval.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/interval.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/misc.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/parser.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/parser.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/pilter.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/pilter.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/tools.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/tools.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/unpack.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/unpack.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs/nan/utils/utility.py` & `kynaylibs-1.8.8/kynaylibs/nan/utils/utility.py`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/kynaylibs.egg-info/PKG-INFO` & `kynaylibs-1.8.8/kynaylibs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kynaylibs
-Version: 1.8.7
+Version: 1.8.8
 Summary: A Secure and Powerful Python-Pyrogram Based Library For Naya-Pyro.
 Home-page: https://github.com/naya1503/kynaylibs
 Author: naya1503
 Author-email: cosmospanas70@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE (v3)
 Project-URL: Bug Tracker, https://github.com/naya1503/kynaylibs/issues
 Project-URL: Documentation, https://t.me/kynansupport
```

### Comparing `kynaylibs-1.8.7/kynaylibs.egg-info/SOURCES.txt` & `kynaylibs-1.8.8/kynaylibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kynaylibs-1.8.7/setup.py` & `kynaylibs-1.8.8/setup.py`

 * *Files identical despite different names*

