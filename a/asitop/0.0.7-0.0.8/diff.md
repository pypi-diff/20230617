# Comparing `tmp/asitop-0.0.7.tar.gz` & `tmp/asitop-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asitop-0.0.7.tar", last modified: Wed Nov  3 09:39:28 2021, max compression
+gzip compressed data, was "asitop-0.0.8.tar", last modified: Wed Nov  3 09:45:24 2021, max compression
```

## Comparing `asitop-0.0.7.tar` & `asitop-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tlkh       (501) staff       (20)        0 2021-11-03 09:39:28.281465 asitop-0.0.7/
--rw-r--r--   0 tlkh       (501) staff       (20)     1068 2021-10-27 15:50:42.000000 asitop-0.0.7/LICENSE
--rw-r--r--   0 tlkh       (501) staff       (20)      503 2021-11-03 09:39:28.281360 asitop-0.0.7/PKG-INFO
--rw-r--r--   0 tlkh       (501) staff       (20)      965 2021-10-28 15:11:16.000000 asitop-0.0.7/README.md
-drwxr-xr-x   0 tlkh       (501) staff       (20)        0 2021-11-03 09:39:28.280384 asitop-0.0.7/asitop/
--rw-r--r--   0 tlkh       (501) staff       (20)        0 2021-10-27 15:38:17.000000 asitop-0.0.7/asitop/__init__.py
--rw-r--r--   0 tlkh       (501) staff       (20)    11500 2021-11-03 09:38:33.000000 asitop-0.0.7/asitop/asitop.py
--rw-r--r--   0 tlkh       (501) staff       (20)     2455 2021-11-03 05:51:20.000000 asitop-0.0.7/asitop/parsers.py
--rw-r--r--   0 tlkh       (501) staff       (20)     3300 2021-11-03 08:29:30.000000 asitop-0.0.7/asitop/utils.py
-drwxr-xr-x   0 tlkh       (501) staff       (20)        0 2021-11-03 09:39:28.281223 asitop-0.0.7/asitop.egg-info/
--rw-r--r--   0 tlkh       (501) staff       (20)      503 2021-11-03 09:39:28.000000 asitop-0.0.7/asitop.egg-info/PKG-INFO
--rw-r--r--   0 tlkh       (501) staff       (20)      307 2021-11-03 09:39:28.000000 asitop-0.0.7/asitop.egg-info/SOURCES.txt
--rw-r--r--   0 tlkh       (501) staff       (20)        1 2021-11-03 09:39:28.000000 asitop-0.0.7/asitop.egg-info/dependency_links.txt
--rw-r--r--   0 tlkh       (501) staff       (20)       47 2021-11-03 09:39:28.000000 asitop-0.0.7/asitop.egg-info/entry_points.txt
--rw-r--r--   0 tlkh       (501) staff       (20)        1 2021-10-28 13:47:34.000000 asitop-0.0.7/asitop.egg-info/not-zip-safe
--rw-r--r--   0 tlkh       (501) staff       (20)       15 2021-11-03 09:39:28.000000 asitop-0.0.7/asitop.egg-info/requires.txt
--rw-r--r--   0 tlkh       (501) staff       (20)        7 2021-11-03 09:39:28.000000 asitop-0.0.7/asitop.egg-info/top_level.txt
--rw-r--r--   0 tlkh       (501) staff       (20)       38 2021-11-03 09:39:28.281500 asitop-0.0.7/setup.cfg
--rw-r--r--   0 tlkh       (501) staff       (20)      868 2021-11-03 09:39:08.000000 asitop-0.0.7/setup.py
+drwxr-xr-x   0 tlkh       (501) staff       (20)        0 2021-11-03 09:45:24.489544 asitop-0.0.8/
+-rw-r--r--   0 tlkh       (501) staff       (20)     1068 2021-10-27 15:50:42.000000 asitop-0.0.8/LICENSE
+-rw-r--r--   0 tlkh       (501) staff       (20)      503 2021-11-03 09:45:24.489439 asitop-0.0.8/PKG-INFO
+-rw-r--r--   0 tlkh       (501) staff       (20)      965 2021-10-28 15:11:16.000000 asitop-0.0.8/README.md
+drwxr-xr-x   0 tlkh       (501) staff       (20)        0 2021-11-03 09:45:24.488673 asitop-0.0.8/asitop/
+-rw-r--r--   0 tlkh       (501) staff       (20)        0 2021-10-27 15:38:17.000000 asitop-0.0.8/asitop/__init__.py
+-rw-r--r--   0 tlkh       (501) staff       (20)    11519 2021-11-03 09:44:59.000000 asitop-0.0.8/asitop/asitop.py
+-rw-r--r--   0 tlkh       (501) staff       (20)     2455 2021-11-03 05:51:20.000000 asitop-0.0.8/asitop/parsers.py
+-rw-r--r--   0 tlkh       (501) staff       (20)     3300 2021-11-03 08:29:30.000000 asitop-0.0.8/asitop/utils.py
+drwxr-xr-x   0 tlkh       (501) staff       (20)        0 2021-11-03 09:45:24.489312 asitop-0.0.8/asitop.egg-info/
+-rw-r--r--   0 tlkh       (501) staff       (20)      503 2021-11-03 09:45:24.000000 asitop-0.0.8/asitop.egg-info/PKG-INFO
+-rw-r--r--   0 tlkh       (501) staff       (20)      307 2021-11-03 09:45:24.000000 asitop-0.0.8/asitop.egg-info/SOURCES.txt
+-rw-r--r--   0 tlkh       (501) staff       (20)        1 2021-11-03 09:45:24.000000 asitop-0.0.8/asitop.egg-info/dependency_links.txt
+-rw-r--r--   0 tlkh       (501) staff       (20)       47 2021-11-03 09:45:24.000000 asitop-0.0.8/asitop.egg-info/entry_points.txt
+-rw-r--r--   0 tlkh       (501) staff       (20)        1 2021-10-28 13:47:34.000000 asitop-0.0.8/asitop.egg-info/not-zip-safe
+-rw-r--r--   0 tlkh       (501) staff       (20)       15 2021-11-03 09:45:24.000000 asitop-0.0.8/asitop.egg-info/requires.txt
+-rw-r--r--   0 tlkh       (501) staff       (20)        7 2021-11-03 09:45:24.000000 asitop-0.0.8/asitop.egg-info/top_level.txt
+-rw-r--r--   0 tlkh       (501) staff       (20)       38 2021-11-03 09:45:24.489580 asitop-0.0.8/setup.cfg
+-rw-r--r--   0 tlkh       (501) staff       (20)      868 2021-11-03 09:45:04.000000 asitop-0.0.8/setup.py
```

### Comparing `asitop-0.0.7/LICENSE` & `asitop-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `asitop-0.0.7/README.md` & `asitop-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `asitop-0.0.7/asitop/asitop.py` & `asitop-0.0.8/asitop/asitop.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from collections import deque
 from dashing import VSplit, HSplit, HGauge, HChart
 from .utils import *
 
 
 parser = argparse.ArgumentParser(description='asitop: Performance monitoring CLI tool for Apple Silicon')
 parser.add_argument('--interval', type=int, default=1,
-                    help='Display interval, and sampling interval for powermetrics')
+                    help='Display interval and sampling interval for powermetrics (seconds)')
 parser.add_argument('--color', type=int, default=2,
                     help='Choose display color (0~8)')
 parser.add_argument('--avg', type=int, default=30,
-                    help='Interval for averaged values')
+                    help='Interval for averaged values (seconds)')
 args = parser.parse_args()
 
 
 def main():
     print("\n[1/3] Loading ASITOP\n")
 
     ui = VSplit(
```

### Comparing `asitop-0.0.7/asitop/parsers.py` & `asitop-0.0.8/asitop/parsers.py`

 * *Files identical despite different names*

### Comparing `asitop-0.0.7/asitop/utils.py` & `asitop-0.0.8/asitop/utils.py`

 * *Files identical despite different names*

### Comparing `asitop-0.0.7/setup.py` & `asitop-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 long_description = 'Performance monitoring CLI tool for Apple Silicon'
 
 setup(
     name='asitop',
-    version='0.0.7',
+    version='0.0.8',
     author='Timothy Liu',
     author_email='tlkh.xms@gmail.com',
     url='https://github.com/tlkh/asitop',
     description='Performance monitoring CLI tool for Apple Silicon',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

