# Comparing `tmp/dpy-toolbox-0.0.1b8.tar.gz` & `tmp/dpy-toolbox-0.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpy-toolbox-0.0.1b8.tar", last modified: Wed Oct 26 21:54:03 2022, max compression
+gzip compressed data, was "dpy-toolbox-0.0.1b9.tar", last modified: Thu Oct 27 00:45:38 2022, max compression
```

## Comparing `dpy-toolbox-0.0.1b8.tar` & `dpy-toolbox-0.0.1b9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-26 21:54:03.675699 dpy-toolbox-0.0.1b8/
--rw-r--r--   0 julius     (503) staff       (20)     1155 2022-10-26 21:54:03.675326 dpy-toolbox-0.0.1b8/PKG-INFO
--rw-rw-r--   0 julius     (503) staff       (20)      463 2022-05-11 15:46:32.000000 dpy-toolbox-0.0.1b8/README.md
-drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-26 21:54:03.664564 dpy-toolbox-0.0.1b8/dpy_toolbox/
--rw-r--r--   0 julius     (503) staff       (20)     2521 2022-10-26 20:54:31.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/CustomContext.py
--rw-r--r--   0 julius     (503) staff       (20)     4487 2022-10-23 11:42:31.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/EmojiReact.py
--rw-r--r--   0 julius     (503) staff       (20)      838 2022-05-10 23:27:18.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/NewHelpClasses.py
--rw-r--r--   0 julius     (503) staff       (20)      664 2022-10-26 17:37:27.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/__init__.py
--rw-r--r--   0 julius     (503) staff       (20)      181 2022-05-09 11:41:47.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/__main__.py
--rw-r--r--   0 julius     (503) staff       (20)     3970 2022-10-26 21:28:03.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/bot.py
-drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-26 21:54:03.668591 dpy-toolbox-0.0.1b8/dpy_toolbox/core/
--rw-r--r--   0 julius     (503) staff       (20)      277 2022-10-26 20:54:31.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/core/__init__.py
--rw-r--r--   0 julius     (503) staff       (20)      850 2022-10-26 20:57:54.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/core/default.py
--rw-r--r--   0 julius     (503) staff       (20)      798 2022-06-25 19:24:47.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/core/errors.py
--rw-r--r--   0 julius     (503) staff       (20)     1549 2022-10-25 19:38:10.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/core/events.py
--rw-r--r--   0 julius     (503) staff       (20)      762 2022-10-23 11:44:07.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/permissions.py
-drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-26 21:54:03.672467 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/
--rw-r--r--   0 julius     (503) staff       (20)     3456 2022-06-25 08:10:25.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/__init__.py
--rw-r--r--   0 julius     (503) staff       (20)     5924 2022-06-25 06:52:43.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/base.py
--rw-r--r--   0 julius     (503) staff       (20)     2059 2022-06-23 23:30:19.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/encodings.py
--rw-r--r--   0 julius     (503) staff       (20)     9417 2022-06-25 08:16:49.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/gateway.py
--rw-r--r--   0 julius     (503) staff       (20)      350 2022-06-23 13:14:53.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/injecter.py
--rw-r--r--   0 julius     (503) staff       (20)     6846 2022-06-24 15:17:07.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/old_gateway.py
--rw-r--r--   0 julius     (503) staff       (20)    16946 2022-06-25 08:16:49.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/opus.py
--rw-r--r--   0 julius     (503) staff       (20)    11390 2022-06-25 19:47:22.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/sink.py
--rw-r--r--   0 julius     (503) staff       (20)    30017 2022-06-25 19:28:42.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/sink/voice_client.py
-drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-26 21:54:03.674651 dpy-toolbox-0.0.1b8/dpy_toolbox/ui/
--rw-r--r--   0 julius     (503) staff       (20)     2188 2022-06-21 02:17:31.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/ui/ButtonReact.py
--rw-r--r--   0 julius     (503) staff       (20)     4868 2022-10-26 21:50:14.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/ui/Modal.py
--rw-r--r--   0 julius     (503) staff       (20)     9857 2022-06-05 00:27:38.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/ui/Paginator.py
--rw-r--r--   0 julius     (503) staff       (20)      251 2022-10-26 21:28:03.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/ui/__init__.py
--rw-r--r--   0 julius     (503) staff       (20)     2206 2022-05-18 22:21:47.000000 dpy-toolbox-0.0.1b8/dpy_toolbox/ui/core.py
-drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-26 21:54:03.666834 dpy-toolbox-0.0.1b8/dpy_toolbox.egg-info/
--rw-r--r--   0 julius     (503) staff       (20)     1155 2022-10-26 21:54:03.000000 dpy-toolbox-0.0.1b8/dpy_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 julius     (503) staff       (20)      870 2022-10-26 21:54:03.000000 dpy-toolbox-0.0.1b8/dpy_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 julius     (503) staff       (20)        1 2022-10-26 21:54:03.000000 dpy-toolbox-0.0.1b8/dpy_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 julius     (503) staff       (20)       11 2022-10-26 21:54:03.000000 dpy-toolbox-0.0.1b8/dpy_toolbox.egg-info/requires.txt
--rw-r--r--   0 julius     (503) staff       (20)       12 2022-10-26 21:54:03.000000 dpy-toolbox-0.0.1b8/dpy_toolbox.egg-info/top_level.txt
--rw-r--r--   0 julius     (503) staff       (20)       38 2022-10-26 21:54:03.675813 dpy-toolbox-0.0.1b8/setup.cfg
--rw-r--r--   0 julius     (503) staff       (20)     1585 2022-10-26 21:53:56.000000 dpy-toolbox-0.0.1b8/setup.py
+drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-27 00:45:38.979832 dpy-toolbox-0.0.1b9/
+-rw-r--r--   0 julius     (503) staff       (20)     1155 2022-10-27 00:45:38.979516 dpy-toolbox-0.0.1b9/PKG-INFO
+-rw-rw-r--   0 julius     (503) staff       (20)      463 2022-05-11 15:46:32.000000 dpy-toolbox-0.0.1b9/README.md
+drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-27 00:45:38.964777 dpy-toolbox-0.0.1b9/dpy_toolbox/
+-rw-r--r--   0 julius     (503) staff       (20)     2521 2022-10-26 20:54:31.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/CustomContext.py
+-rw-r--r--   0 julius     (503) staff       (20)     4487 2022-10-23 11:42:31.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/EmojiReact.py
+-rw-r--r--   0 julius     (503) staff       (20)      838 2022-05-10 23:27:18.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/NewHelpClasses.py
+-rw-r--r--   0 julius     (503) staff       (20)      664 2022-10-26 17:37:27.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/__init__.py
+-rw-r--r--   0 julius     (503) staff       (20)      181 2022-05-09 11:41:47.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/__main__.py
+-rw-r--r--   0 julius     (503) staff       (20)     4002 2022-10-27 00:19:06.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/bot.py
+drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-27 00:45:38.970088 dpy-toolbox-0.0.1b9/dpy_toolbox/core/
+-rw-r--r--   0 julius     (503) staff       (20)      277 2022-10-26 20:54:31.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/core/__init__.py
+-rw-r--r--   0 julius     (503) staff       (20)      850 2022-10-26 20:57:54.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/core/default.py
+-rw-r--r--   0 julius     (503) staff       (20)      798 2022-06-25 19:24:47.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/core/errors.py
+-rw-r--r--   0 julius     (503) staff       (20)     1549 2022-10-25 19:38:10.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/core/events.py
+-rw-r--r--   0 julius     (503) staff       (20)      762 2022-10-23 11:44:07.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/permissions.py
+drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-27 00:45:38.975494 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/
+-rw-r--r--   0 julius     (503) staff       (20)     3471 2022-10-27 00:19:06.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/__init__.py
+-rw-r--r--   0 julius     (503) staff       (20)     5924 2022-06-25 06:52:43.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/base.py
+-rw-r--r--   0 julius     (503) staff       (20)     2059 2022-06-23 23:30:19.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/encodings.py
+-rw-r--r--   0 julius     (503) staff       (20)     9417 2022-06-25 08:16:49.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/gateway.py
+-rw-r--r--   0 julius     (503) staff       (20)      350 2022-06-23 13:14:53.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/injecter.py
+-rw-r--r--   0 julius     (503) staff       (20)     6846 2022-06-24 15:17:07.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/old_gateway.py
+-rw-r--r--   0 julius     (503) staff       (20)    16946 2022-06-25 08:16:49.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/opus.py
+-rw-r--r--   0 julius     (503) staff       (20)    12989 2022-10-27 00:44:39.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/sink.py
+-rw-r--r--   0 julius     (503) staff       (20)    30017 2022-06-25 19:28:42.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/sink/voice_client.py
+drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-27 00:45:38.978779 dpy-toolbox-0.0.1b9/dpy_toolbox/ui/
+-rw-r--r--   0 julius     (503) staff       (20)     2188 2022-06-21 02:17:31.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/ui/ButtonReact.py
+-rw-r--r--   0 julius     (503) staff       (20)     4868 2022-10-26 21:50:14.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/ui/Modal.py
+-rw-r--r--   0 julius     (503) staff       (20)     9857 2022-06-05 00:27:38.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/ui/Paginator.py
+-rw-r--r--   0 julius     (503) staff       (20)      251 2022-10-26 21:28:03.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/ui/__init__.py
+-rw-r--r--   0 julius     (503) staff       (20)     2206 2022-05-18 22:21:47.000000 dpy-toolbox-0.0.1b9/dpy_toolbox/ui/core.py
+drwxr-xr-x   0 julius     (503) staff       (20)        0 2022-10-27 00:45:38.966941 dpy-toolbox-0.0.1b9/dpy_toolbox.egg-info/
+-rw-r--r--   0 julius     (503) staff       (20)     1155 2022-10-27 00:45:38.000000 dpy-toolbox-0.0.1b9/dpy_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 julius     (503) staff       (20)      870 2022-10-27 00:45:38.000000 dpy-toolbox-0.0.1b9/dpy_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 julius     (503) staff       (20)        1 2022-10-27 00:45:38.000000 dpy-toolbox-0.0.1b9/dpy_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 julius     (503) staff       (20)       24 2022-10-27 00:45:38.000000 dpy-toolbox-0.0.1b9/dpy_toolbox.egg-info/requires.txt
+-rw-r--r--   0 julius     (503) staff       (20)       12 2022-10-27 00:45:38.000000 dpy-toolbox-0.0.1b9/dpy_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 julius     (503) staff       (20)       38 2022-10-27 00:45:38.979934 dpy-toolbox-0.0.1b9/setup.cfg
+-rw-r--r--   0 julius     (503) staff       (20)     1604 2022-10-27 00:44:49.000000 dpy-toolbox-0.0.1b9/setup.py
```

### Comparing `dpy-toolbox-0.0.1b8/PKG-INFO` & `dpy-toolbox-0.0.1b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpy-toolbox
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Discord.py simplifier
 Author: TheWever (Wever#3255)
 Author-email: <nonarrator@gmail.com>
 Project-URL: Github, https://github.com/TheWever/dpy-toolbox
 Project-URL: Documentation, https://dpy-toolbox.rtfd.io/
 Project-URL: Discord, https://discord.gg/rnEwUJ7Fhc
 Keywords: discord.py,discord,utils,tools,toolbox
```

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/CustomContext.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/CustomContext.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/EmojiReact.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/EmojiReact.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/NewHelpClasses.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/NewHelpClasses.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/__init__.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/bot.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union, Callable, Optional
 from discord.ext import commands
 from discord.types.snowflake import Snowflake
 import discord
-from .sink import to_SinkVoiceClient, MP3Sink, SinkVoiceClient, SinkVoiceChannel, to_SinkVoiceChannel
+from .sink import to_SinkVoiceClient, MP3Sink, SinkVoiceClient, SinkVoiceChannel, to_SinkVoiceChannel, VirtualSink
 
 from .core import (
     EventFunctionWrapper
 )
 
 from .ui import *
 from .CustomContext import CustomContext
@@ -21,15 +21,16 @@
     "ButtonDisplay",
     "to_SinkVoiceClient",
     "SinkVoiceClient",
     "MP3Sink",
     "SinkVoiceChannel",
     "to_SinkVoiceChannel",
     "QuestioningModal",
-    "SingleQuestion"
+    "SingleQuestion",
+    "VirtualSink"
 )
 
 
 class toolbox:
     DEFAULT_EVENTS = (
         "on_message",
         "on_raw_reaction_add",
```

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/core/default.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/core/default.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/core/errors.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/core/errors.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/core/events.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/core/events.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/permissions.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/permissions.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/sink/__init__.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/sink/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .voice_client import SinkVoiceClient
 from .gateway import DiscordSinkWebSocket
 from . import opus
 from discord import VoiceClient
-from .sink import Sink, VirtualSink
+from .sink import Sink, VirtualSink, UnvirtualSink
 from .encodings import MP3Sink
 from .base import SinkVoiceChannel
 import discord
 import traceback
 import asyncio
 import types
```

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/sink/base.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/sink/base.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/sink/encodings.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/sink/encodings.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/sink/gateway.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/sink/gateway.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/sink/old_gateway.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/sink/old_gateway.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/sink/opus.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/sink/opus.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/sink/sink.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/sink/sink.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from discord import DiscordException
-import wave
 import logging
 import os
 import threading
 import time
 import subprocess
 import sys
 import struct
 import io
-from pydub import AudioSegment
 import wave
+from pydub import AudioSegment
 from ..core import try_exc
 _log = logging.getLogger(__name__)
 
 __all__ = (
     "Filters",
     "Sink",
     "AudioData",
     "RawData",
+    "UnvirtualSink",
+    "VirtualSink"
 )
 
 class SinkException(DiscordException):
     pass
 
 if sys.platform != "win32":
     CREATE_NO_WINDOW = 0
@@ -69,16 +70,14 @@
         if self.finished:
             return
         self.vc.stop_listening()
 
 
 class RawData:
     """Handles raw data from Discord so that it can be decrypted and decoded to be used.
-
-    .. versionadded:: 2.0
     """
 
     def __init__(self, data, client):
         self.data = bytearray(data)
         self.client = client
 
         self.header = data[:12]
@@ -93,15 +92,14 @@
 
         self.user_id = None
 
 
 class AudioData:
     """Handles data that's been completely decrypted and decoded and is ready to be saved to file.
 
-    .. versionadded:: 2.0
     Raises
     ------
     ClientException
         The AudioData is already finished writing,
         The AudioData is still writing
     """
 
@@ -141,15 +139,15 @@
         # name = os.path.split(self.file)[1]
         # name = name.split(".")[0] + f".{encoding}"
         self.file_name = f'{self.file_name[:self.file_name.rfind(".")]}.{encoding}'
 
 
 class Sink(Filters):
     """A Sink "stores" all the audio data.
-    .. versionadded:: 2.0
+    .. versionadded:: 0.0.1b6
     Parameters
     ----------
     encoding: :class:`string`
         The encoding to use. Valid types include wav, mp3, and pcm (even though it's not an actual encoding).
     output_path: :class:`string`
         A path to where the audio files should be output.
 
@@ -258,17 +256,17 @@
 
         if self.hide_output:
             try_exc(os.remove, out_path)
         if self.hide_input:
             try_exc(os.remove, audio.file_name)
         audio.on_format(self.encoding)
 
-class VirtualSink(Filters):
+class UnvirtualSink(Filters):
     """A Sink "stores" all the audio data.
-    .. versionadded:: 2.0
+    .. versionadded:: 0.0.1b6
     Parameters
     ----------
     encoding: :class:`string`
         The encoding to use. Valid types include wav, mp3, and pcm (even though it's not an actual encoding).
     output_path: :class:`string`
         A path to where the audio files should be output.
 
@@ -372,8 +370,65 @@
                 f.setframerate(self.vc.decoder.SAMPLING_RATE)
                 f.writeframes(data)
 
         os.remove(in_path)
         r = open(out_path, 'rb').read()
         if self.hide_output:
             os.remove(out_path)
-        return r
+        return r
+
+
+class VirtualSink(Filters):
+    """A Sink "stores" all the audio data.
+    .. versionadded:: 0.0.1b9
+    Parameters
+    ----------
+    encoding: :class:`string`
+        The encoding to use. Valid types include wav, mp3, and pcm (even though it's not an actual encoding).
+    output_path: :class:`string`
+        A path to where the audio files should be output.
+
+    Raises
+    ------
+    ClientException
+        An invalid encoding type was specified.
+        Audio may only be formatted after recording is finished.
+    """
+
+    def __init__(self, *,  filters=None):
+        if filters is None:
+            filters = default_filters
+        self.filters = filters
+        Filters.__init__(self, **self.filters)
+
+        self.encoding = "mp3"
+        self.vc = None
+        self.audio_data = {}
+
+    def init(self, vc):  # called under listen
+        self.vc = vc
+        super().init()
+
+    @Filters.interface
+    def write(self, data, user):
+        if user not in self.audio_data:
+            file = io.BytesIO()
+            self.audio_data.update({user: file})
+
+        self.audio_data[user].write(data)
+
+    def cleanup(self):
+        self.finished = True
+        for x in self.audio_data.values():
+            x.seek(0)
+
+    def format_audio(self):
+        if self.vc.recording:
+            raise SinkException(
+                "Audio may only be formatted after recording is finished."
+            )
+
+    @property
+    def result(self):
+        self.cleanup()
+        return {k: AudioSegment.from_file(v, format="pcm", sample_width=96000, frame_rate=30, channels=2) for k, v in self.audio_data.items()}
+
```

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/sink/voice_client.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/sink/voice_client.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/ui/ButtonReact.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/ui/ButtonReact.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/ui/Modal.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/ui/Modal.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/ui/Paginator.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/ui/Paginator.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox/ui/core.py` & `dpy-toolbox-0.0.1b9/dpy_toolbox/ui/core.py`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox.egg-info/PKG-INFO` & `dpy-toolbox-0.0.1b9/dpy_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpy-toolbox
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Discord.py simplifier
 Author: TheWever (Wever#3255)
 Author-email: <nonarrator@gmail.com>
 Project-URL: Github, https://github.com/TheWever/dpy-toolbox
 Project-URL: Documentation, https://dpy-toolbox.rtfd.io/
 Project-URL: Discord, https://discord.gg/rnEwUJ7Fhc
 Keywords: discord.py,discord,utils,tools,toolbox
```

### Comparing `dpy-toolbox-0.0.1b8/dpy_toolbox.egg-info/SOURCES.txt` & `dpy-toolbox-0.0.1b9/dpy_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dpy-toolbox-0.0.1b8/setup.py` & `dpy-toolbox-0.0.1b9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1b8'
+VERSION = '0.0.1b9'
 DESCRIPTION = "Discord.py simplifier"
 LONG_DESCRIPTION = 'This package extends the discord.py library by making complex commands  and functions easier to use. This library will most certainly work with any other library based on d.py like Pycord. I am still working on this lib and looking forward to adding new features [5/7/2022]. This is an early alpha and might be buggy. If you want to report a bug or suggest a feature add me on discord: Wever#3255.'
 
 # Setting up
 setup(
     name="dpy-toolbox",
     version=VERSION,
     author="TheWever (Wever#3255)",
     author_email="<nonarrator@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['discord.py'],
+    install_requires=['discord.py', 'PyNaCl', 'pydub'],
     keywords=['discord.py', 'discord', 'utils', 'tools', 'toolbox'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

