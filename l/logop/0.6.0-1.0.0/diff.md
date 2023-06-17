# Comparing `tmp/logop-0.6.0.tar.gz` & `tmp/logop-1.0.0.tar.gz`

## Comparing `logop-0.6.0.tar` & `logop-1.0.0.tar`

### file list

```diff
@@ -1,5 +1,17 @@
--rw-r--r--   0        0        0    15295 2020-02-02 00:00:00.000000 logop-0.6.0/src/logop/__init__.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 logop-0.6.0/LICENSE
--rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 logop-0.6.0/README.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 logop-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 logop-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 logop-1.0.0/README_old.md
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 logop-1.0.0/docs/format.md
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 logop-1.0.0/docs/level.md
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 logop-1.0.0/docs/logging.md
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 logop-1.0.0/docs/logoutput.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 logop-1.0.0/src/logop/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 logop-1.0.0/src/logop/exceptions.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 logop-1.0.0/src/logop/format.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 logop-1.0.0/src/logop/level.py
+-rw-r--r--   0        0        0    12657 2020-02-02 00:00:00.000000 logop-1.0.0/src/logop/logging.py
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 logop-1.0.0/src/logop/logoutput.py
+-rw-r--r--   0        0        0    15312 2020-02-02 00:00:00.000000 logop-1.0.0/src/logop/old.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 logop-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 logop-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 logop-1.0.0/README.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 logop-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 logop-1.0.0/PKG-INFO
```

### Comparing `logop-0.6.0/src/logop/__init__.py` & `logop-1.0.0/src/logop/old.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- codeing:utf-8 -*-
+# -*- coding:utf-8 -*-
 
 # *project:     pylogop
 # *Author:      numLinka
 
 
 import os
 import sys
@@ -10,20 +10,20 @@
 import datetime
 import threading
 import multiprocessing
 
 from typing import Union
 
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 
-ALL      = - 0x80
-TRACE    = - 0x40
-DEBUG    = - 0x20
+ALL      = ~ 0x7F
+TRACE    = ~ 0x40
+DEBUG    = ~ 0x20
 INFO     =   0x00
 WARN     =   0x20
 WARNING  =   0x20
 SEVERE   =   0x30
 ERROR    =   0x40
 FATAL    =   0x60
 CRITICAL =   0x60
@@ -120,15 +120,15 @@
         if '$(.message)' not in op_format:
             raise ValueError('$(.message) must be included in format.')
 
         op = op_character_variable(op_format, content)
         ops = f'{op}\n'
         level = content.get('level', 0)
 
-        if level < 0x10:
+        if level < ERROR:
             sys.stdout.write(ops)
             sys.stdout.flush()
 
         else:
             sys.stderr.write(ops)
             sys.stderr.flush()
 
@@ -146,24 +146,24 @@
             raise ValueError('$(.message) must be included in format.')
 
         op = op_character_variable(op_format, content)
         level = content.get('level', 0)
         if level < 0x10:
             ops = f'{op}\n'
 
-        elif 0x10 <= level < 0x40:
+        elif WARN <= level < ERROR:
             ops = f'\033[1;33m{op}\033[0m\n'
 
-        elif 0x40 <= level < 0x80:
+        elif ERROR <= level <= OFF:
             ops = f'\033[1;31m{op}\033[0m\n'
 
         else:
-            ops = f'{op}\n'
+            ops = f'\033[0m{op}\033[0m\n'
 
-        if level < 0x10:
+        if level < ERROR:
             sys.stdout.write(ops)
             sys.stdout.flush()
 
         else:
             sys.stderr.write(ops)
             sys.stderr.flush()
```

### Comparing `logop-0.6.0/README.md` & `logop-1.0.0/README_old.md`

 * *Files identical despite different names*

### Comparing `logop-0.6.0/pyproject.toml` & `logop-1.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logop"
-version = "0.6.0"
+version = "1.0.0"
 authors = [
-  { name="numLinka", email="numlinka@163.com" },
+  { name="numLinka", email="" },
 ]
 description = "A simple log module"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

