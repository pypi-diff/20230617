# Comparing `tmp/thelogger-0.2.8-py3-none-any.whl.zip` & `tmp/thelogger-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 13817 bytes, number of entries: 12
+Zip file size: 13930 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      290 b- defN 23-Apr-27 17:45 thelogger/__init__.py
 -rw-rw-rw-  2.0 fat      214 b- defN 23-Apr-27 17:46 thelogger/_ver.py
--rw-rw-rw-  2.0 fat      521 b- defN 23-Apr-01 19:28 thelogger/dirty_timer.py
+-rw-rw-rw-  2.0 fat     1048 b- defN 23-Jun-17 04:29 thelogger/dirty_timer.py
 -rw-rw-rw-  2.0 fat     4234 b- defN 22-Feb-20 09:05 thelogger/logger.py
 -rw-rw-rw-  2.0 fat      140 b- defN 22-Feb-20 09:05 thelogger/notify/__init__.py
 -rw-rw-rw-  2.0 fat     3611 b- defN 22-Feb-20 09:49 thelogger/notify/decorator.py
 -rw-rw-rw-  2.0 fat     6990 b- defN 23-Feb-28 14:35 thelogger/notify/exec_func.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Apr-27 17:49 thelogger-0.2.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6627 b- defN 23-Apr-27 17:49 thelogger-0.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 17:49 thelogger-0.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-27 17:49 thelogger-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      959 b- defN 23-Apr-27 17:49 thelogger-0.2.8.dist-info/RECORD
-12 files, 35246 bytes uncompressed, 12211 bytes compressed:  65.4%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6627 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      960 b- defN 23-Jun-17 04:33 thelogger-0.2.9.dist-info/RECORD
+12 files, 35774 bytes uncompressed, 12324 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: thelogger/notify/decorator.py
 Comment: 
 
 Filename: thelogger/notify/exec_func.py
 Comment: 
 
-Filename: thelogger-0.2.8.dist-info/LICENSE
+Filename: thelogger-0.2.9.dist-info/LICENSE
 Comment: 
 
-Filename: thelogger-0.2.8.dist-info/METADATA
+Filename: thelogger-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: thelogger-0.2.8.dist-info/WHEEL
+Filename: thelogger-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: thelogger-0.2.8.dist-info/top_level.txt
+Filename: thelogger-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: thelogger-0.2.8.dist-info/RECORD
+Filename: thelogger-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## thelogger/dirty_timer.py

```diff
@@ -1,23 +1,43 @@
-# -*- coding: utf-8 -*-
 """
-Created on Sat Oct 24 05:22:37 2019
-
-@author: tommy
+Quick and dirty utilties for timing code.
 """
 
 import os
 import time
+import contextlib
 from datetime import timedelta
 
 def beg():
     beg_tm = time.perf_counter()
     os.environ['the_logger_time'] =  str(beg_tm)
 
 def end():
     end_tm = time.perf_counter()
     beg_tm = float(os.environ['the_logger_time'])
     sec_delta = end_tm - beg_tm
     sec_delta = round(sec_delta, 3)
     exec_tm = str(timedelta(seconds = sec_delta)).rstrip('0')
     print(f"Elapsed Time: {exec_tm}")
+    
+@contextlib.contextmanager 
+def timer():
+    """
+    Context manager that provides timing of code execution.
+
+    Example
+    -------
+    >>> import thelogger as tl
+    >>> import time 
+    >>> with timer():
+    ...     time.sleep(1)
+    Elapsed Time: 0:00:00.999
+
+    """
+    beg_tm = time.perf_counter()
+    yield 
+    end_tm = time.perf_counter()
+    sec_delta = end_tm - beg_tm
+    sec_delta = round(sec_delta, 3)
+    exec_tm = str(timedelta(seconds = sec_delta)).rstrip('0')
+    print(f"Elapsed Time: {exec_tm}")
```

## Comparing `thelogger-0.2.8.dist-info/LICENSE` & `thelogger-0.2.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `thelogger-0.2.8.dist-info/METADATA` & `thelogger-0.2.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thelogger
-Version: 0.2.8
+Version: 0.2.9
 Summary: Easy logging, timing and email notifications of code execution.
 Home-page: https://github.com/tom1919/TheLogger
 Author: Tom1919
 Author-email: py.notify1@gmail.com
 License: Apache 2.0
 Keywords: log,logging,logger,email,timimg,notification
 Platform: UNKNOWN
```

## Comparing `thelogger-0.2.8.dist-info/RECORD` & `thelogger-0.2.9.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 thelogger/__init__.py,sha256=aXHT7R_c4u3msy_jb7tjmVQwO-u4Wa9pZWd_VW9pXGE,290
 thelogger/_ver.py,sha256=v27jnS60TKa54IbFVzSTknhDiKMS4J3KCuFTOffZqRU,214
-thelogger/dirty_timer.py,sha256=OqPvoJPlyQb8EkLNF-N4rvzaKY84WcT5n6xYunGkcDo,521
+thelogger/dirty_timer.py,sha256=TVEG_MX2gUYmLaldbWvdcQShqJ53bePjeCNQpF-BNsg,1048
 thelogger/logger.py,sha256=JTyQbecMYpi1n7zKoVe9sohS6tTy87Bx2UnCDHb4-N4,4234
 thelogger/notify/__init__.py,sha256=X0cVRenLKIbnOoapwPN9KJvtwXaHycKVb-ZTZ8tmuWQ,140
 thelogger/notify/decorator.py,sha256=kiiVpcCayMsdtGtiOtswHaa_v8OzSQjXnKnoSvrt0Uk,3611
 thelogger/notify/exec_func.py,sha256=uN4mbHtdmG4-djWnEzomVeFfbOJ6jHqlNmydolX5QwU,6990
-thelogger-0.2.8.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-thelogger-0.2.8.dist-info/METADATA,sha256=2G7iZOyytF2QSoe8VdTHalbkIwU--9yFBkbmFMme__g,6627
-thelogger-0.2.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-thelogger-0.2.8.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
-thelogger-0.2.8.dist-info/RECORD,,
+thelogger-0.2.9.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+thelogger-0.2.9.dist-info/METADATA,sha256=xqYm73rf1ldnibNxIEV_X08iwTvHLNZdsEXLJFhsNw8,6627
+thelogger-0.2.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+thelogger-0.2.9.dist-info/top_level.txt,sha256=6qGJ7TaRPKJuypP1ToyTCDT03pcvwWZ-vqDreYaUfjQ,10
+thelogger-0.2.9.dist-info/RECORD,,
```

