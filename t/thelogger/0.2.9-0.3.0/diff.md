# Comparing `tmp/thelogger-0.2.9-py3-none-any.whl.zip` & `tmp/thelogger-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13930 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      290 b- defN 23-Apr-27 17:45 thelogger/__init__.py
+Zip file size: 13928 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      297 b- defN 23-Jun-17 04:40 thelogger/__init__.py
 -rw-rw-rw-  2.0 fat      214 b- defN 23-Apr-27 17:46 thelogger/_ver.py
--rw-rw-rw-  2.0 fat     1048 b- defN 23-Jun-17 04:29 thelogger/dirty_timer.py
+-rw-rw-rw-  2.0 fat     1046 b- defN 23-Jun-17 04:34 thelogger/dirty_timer.py
 -rw-rw-rw-  2.0 fat     4234 b- defN 22-Feb-20 09:05 thelogger/logger.py
 -rw-rw-rw-  2.0 fat      140 b- defN 22-Feb-20 09:05 thelogger/notify/__init__.py
 -rw-rw-rw-  2.0 fat     3611 b- defN 22-Feb-20 09:49 thelogger/notify/decorator.py
 -rw-rw-rw-  2.0 fat     6990 b- defN 23-Feb-28 14:35 thelogger/notify/exec_func.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6627 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      960 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/RECORD
-12 files, 35774 bytes uncompressed, 12324 bytes compressed:  65.6%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-17 04:41 thelogger-0.3.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6627 b- defN 23-Jun-17 04:41 thelogger-0.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-17 04:41 thelogger-0.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-17 04:41 thelogger-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      960 b- defN 23-Jun-17 04:41 thelogger-0.3.0.dist-info/RECORD
+12 files, 35779 bytes uncompressed, 12322 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: thelogger/notify/decorator.py
 Comment: 
 
 Filename: thelogger/notify/exec_func.py
 Comment: 
 
-Filename: thelogger-0.2.9.dist-info/LICENSE
+Filename: thelogger-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: thelogger-0.2.9.dist-info/METADATA
+Filename: thelogger-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: thelogger-0.2.9.dist-info/WHEEL
+Filename: thelogger-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: thelogger-0.2.9.dist-info/top_level.txt
+Filename: thelogger-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: thelogger-0.2.9.dist-info/RECORD
+Filename: thelogger-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## thelogger/__init__.py

```diff
@@ -5,10 +5,10 @@
 Easy logging, timing and email notifications of code execution.
 
 @author: tommy
 """
 
 from .logger import logger, log, lg
 from .notify import notify
-from .dirty_timer import beg, end
+from .dirty_timer import beg, end, timer
 
 from ._ver import __version__
```

## thelogger/dirty_timer.py

```diff
@@ -27,15 +27,14 @@
     Example
     -------
     >>> import thelogger as tl
     >>> import time 
     >>> with timer():
     ...     time.sleep(1)
     Elapsed Time: 0:00:00.999
-
     """
     beg_tm = time.perf_counter()
     yield 
     end_tm = time.perf_counter()
     sec_delta = end_tm - beg_tm
     sec_delta = round(sec_delta, 3)
     exec_tm = str(timedelta(seconds = sec_delta)).rstrip('0')
```

## Comparing `thelogger-0.2.9.dist-info/LICENSE` & `thelogger-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `thelogger-0.2.9.dist-info/METADATA` & `thelogger-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thelogger
-Version: 0.2.9
+Version: 0.3.0
 Summary: Easy logging, timing and email notifications of code execution.
 Home-page: https://github.com/tom1919/TheLogger
 Author: Tom1919
 Author-email: py.notify1@gmail.com
 License: Apache 2.0
 Keywords: log,logging,logger,email,timimg,notification
 Platform: UNKNOWN
```

