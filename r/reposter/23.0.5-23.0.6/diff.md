# Comparing `tmp/reposter-23.0.5.tar.gz` & `tmp/reposter-23.0.6.tar.gz`

## Comparing `reposter-23.0.5.tar` & `reposter-23.0.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 reposter-23.0.5/build.sh
--rwxr-xr-x   0        0        0     5052 2020-02-02 00:00:00.000000 reposter-23.0.5/changelog.md
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 reposter-23.0.5/start.sh
--rw-r--r--   0        0        0   145233 2020-02-02 00:00:00.000000 reposter-23.0.5/img/filled.png
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 reposter-23.0.5/img/filled.svg
--rw-r--r--   0        0        0    56452 2020-02-02 00:00:00.000000 reposter-23.0.5/img/transparent.png
--rwxr-xr-x   0        0        0     5157 2020-02-02 00:00:00.000000 reposter-23.0.5/img/transparent.svg
--rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 reposter-23.0.5/launcher/reposter.bat
--rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 reposter-23.0.5/launcher/reposter.sh
--rwxr-xr-x   0        0        0     2699 2020-02-02 00:00:00.000000 reposter-23.0.5/launcher/reposter_win.py
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/__init__.py
--rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/__main__.py
--rwxr-xr-x   0        0        0    64590 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/main.py
--rwxr-xr-x   0        0        0     4106 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/setup.py
--rwxr-xr-x   0        0        0     8709 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/icons/icon.ico
--rwxr-xr-x   0        0        0     4296 2020-02-02 00:00:00.000000 reposter-23.0.5/reposter/icons/icon.svg
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 reposter-23.0.5/.gitignore
--rwxr-xr-x   0        0        0      794 2020-02-02 00:00:00.000000 reposter-23.0.5/pyproject.toml
--rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 reposter-23.0.5/readme.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 reposter-23.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 reposter-23.0.6/build.sh
+-rwxr-xr-x   0        0        0     5110 2020-02-02 00:00:00.000000 reposter-23.0.6/changelog.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 reposter-23.0.6/setup.sh
+-rwxr-xr-x   0        0        0       49 2020-02-02 00:00:00.000000 reposter-23.0.6/start.sh
+-rw-r--r--   0        0        0   145233 2020-02-02 00:00:00.000000 reposter-23.0.6/img/filled.png
+-rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 reposter-23.0.6/img/filled.svg
+-rw-r--r--   0        0        0    56452 2020-02-02 00:00:00.000000 reposter-23.0.6/img/transparent.png
+-rwxr-xr-x   0        0        0     5157 2020-02-02 00:00:00.000000 reposter-23.0.6/img/transparent.svg
+-rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 reposter-23.0.6/launcher/reposter.bat
+-rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 reposter-23.0.6/launcher/reposter.sh
+-rwxr-xr-x   0        0        0     2699 2020-02-02 00:00:00.000000 reposter-23.0.6/launcher/reposter_win.py
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/__init__.py
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/__main__.py
+-rwxr-xr-x   0        0        0    65237 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/main.py
+-rwxr-xr-x   0        0        0     4106 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/setup.py
+-rwxr-xr-x   0        0        0     8709 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/icons/icon.ico
+-rwxr-xr-x   0        0        0     4296 2020-02-02 00:00:00.000000 reposter-23.0.6/reposter/icons/icon.svg
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 reposter-23.0.6/.gitignore
+-rwxr-xr-x   0        0        0      794 2020-02-02 00:00:00.000000 reposter-23.0.6/pyproject.toml
+-rwxr-xr-x   0        0        0     1153 2020-02-02 00:00:00.000000 reposter-23.0.6/readme.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 reposter-23.0.6/PKG-INFO
```

### Comparing `reposter-23.0.5/changelog.md` & `reposter-23.0.6/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 - the ability to specify which messages will not be reposted using pyrogram filters
 
 ## known bugs
 
 - hyperlinks not supported
 - forwarded messages are reposted without author
 
+## 23.0.6
+
+- fixed photos with captions was not reposted
+
 ## 23.0.5
 
 - fixed dependecies
 
 ## 23.0.4
 
 - improved errors handling
```

### Comparing `reposter-23.0.5/img/filled.png` & `reposter-23.0.6/img/filled.png`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/img/filled.svg` & `reposter-23.0.6/img/filled.svg`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/img/transparent.png` & `reposter-23.0.6/img/transparent.png`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/img/transparent.svg` & `reposter-23.0.6/img/transparent.svg`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/launcher/reposter.bat` & `reposter-23.0.6/launcher/reposter.bat`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/launcher/reposter.sh` & `reposter-23.0.6/launcher/reposter.sh`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/launcher/reposter_win.py` & `reposter-23.0.6/launcher/reposter_win.py`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/reposter/main.py` & `reposter-23.0.6/reposter/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     errors,
 )
 from urllib import request as r
 import gmanka_yml as yml
 import pyrogram as pg
 import humanize
 import platform
+import datetime
 import hashlib
 import rich
 import time
 import json
 import sys
 import os
 
@@ -1370,33 +1371,29 @@
 def resend(
     msg: types.Message,
     target: int,
     log_msg: types.Message,
     reply_to_msg = None,
 ) -> types.Message:
     if msg.caption:
-        if 'файл номер' not in msg.caption:
-            return
         captions = list(
             text_wrap(
                 msg.caption
             )
         )
         first_caption = captions[0]
         other_captions = captions[1:]
     first_caption = None
     other_captions = []
-
     kwargs = {
         'msg': msg,
         'target': target,
         'log_msg': log_msg,
         'caption': first_caption,
     }
-
     if msg.poll:
         try:
             options = []
             for option in msg.poll.options:
                 options.append(
                     option.text
                 )
@@ -1416,14 +1413,15 @@
         )
     elif msg.photo:
         new_msg = resend_file(
             **kwargs,
             file = msg.photo,
             send_method = bot.send_photo,
         )
+        c.log(new_msg)
     elif msg.video:
         new_msg = resend_file(
             **kwargs,
             file = msg.video,
             send_method = bot.send_video,
             width = msg.video.width,
             height = msg.video.height,
@@ -1572,14 +1570,19 @@
             return new_msg
         else:
             new_msg = resend(
                 msg = src_msg,
                 target = target_id,
                 log_msg = log_msg,
             )
+            if not new_msg:
+                bot.send_message(
+                    chat_id = temp_data.logs_chat.id,
+                    text = 'error: no message was reposted'
+                )
             msg_in_history[
                 target_id
             ] = new_msg.id
             history.to_file()
             return new_msg
     except PollException:
         return False
@@ -1634,16 +1637,14 @@
     target_id,
     log_msg,
     msg_in_history,
     is_media_group,
 ) -> types.Message:
     if not src_msg.caption:
         return
-    if 'файл номер' not in src_msg.caption:
-        return
     if is_media_group:
         new_msg: types.Message = forward_media_group(
             msg = src_msg,
             target = target_id,
             log_msg = log_msg,
         )
     else:
@@ -2131,37 +2132,61 @@
         init_recursive_repost(
             _,
             src_msg,
             deleted,
             force,
         )
     except Exception:
-        error_path = f'{proj_path}/error.txt'
-        with open(
-            error_path,
-            'w',
-        ) as file:
-            c_error = rich.console.Console(
-                width = 80,
-                file = file,
-            )
-            c_error.print_exception(
-                show_locals = True
-            )
-        c.print_exception(
-            show_locals = True
-        )
-        c_log.print_exception(
-            show_locals = True
-        )
         bot.send_document(
             chat_id = temp_data.logs_chat.id,
-            document = error_path,
-            reply_to_message_id = log_msg,
+            document = write_error(),
+        )
+
+
+def write_error() -> str:
+    max_errors_in_dir = 30
+    errors_path = modules_path.joinpath('errors')
+    errors_path.mkdir(
+        exist_ok = True,
+        parents = True,
+    )
+    all_errors = list(
+        errors_path.iterdir()
+    )
+    all_errors.sort()
+    while len(
+        all_errors
+    ) >= max_errors_in_dir:
+        all_errors[0].unlink()
+        all_errors.remove(all_errors[0])
+    file_date = datetime.datetime.now().strftime("%Y.%m.%d_%H.%M")
+    test_error_path = errors_path.joinpath(file_date)
+    error_path = Path(
+        f'{test_error_path}.txt'
+    )
+    index = 2
+    while error_path.exists():
+        error_path = Path(
+            f'{test_error_path}_{index}.txt'
+        )
+        index += 1
+    with open(
+        error_path,
+        'w',
+        encoding = "utf-8",
+    ) as file:
+        c_error = rich.console.Console(
+            width = 80,
+            file = file,
+        )
+        c_error.print_exception(
+            show_locals = True
         )
+    c.log(f'error written to {error_path}')
+    return str(error_path)
 
 
 def clean_link(
     link: str,
 ) -> str:
     if not link:
         return
```

### Comparing `reposter-23.0.5/reposter/setup.py` & `reposter-23.0.6/reposter/setup.py`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/reposter/icons/icon.ico` & `reposter-23.0.6/reposter/icons/icon.ico`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/reposter/icons/icon.svg` & `reposter-23.0.6/reposter/icons/icon.svg`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/pyproject.toml` & `reposter-23.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   "gmanka_yml==22.0.1",
   "pyrogram",
   "tgcrypto",
   "humanize",
   "rich",
 ]
 name = "reposter"
-version = "23.0.5"
+version = "23.0.6"
 authors = [
   { name="gmanka", email="gmankab@gmail.com" },
 ]
 description = "python script for reposting messages from telegram channels"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `reposter-23.0.5/readme.md` & `reposter-23.0.6/readme.md`

 * *Files identical despite different names*

### Comparing `reposter-23.0.5/PKG-INFO` & `reposter-23.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reposter
-Version: 23.0.5
+Version: 23.0.6
 Summary: python script for reposting messages from telegram channels
 Project-URL: Homepage, https://github.com/gmankab/reposter
 Project-URL: Documentation, https://github.com/gmankab/reposter
 Project-URL: Bug Tracker, https://github.com/gmankab/reposter/issues
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

