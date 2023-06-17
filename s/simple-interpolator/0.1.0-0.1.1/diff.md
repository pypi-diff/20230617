# Comparing `tmp/simple-interpolator-0.1.0.tar.gz` & `tmp/simple-interpolator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-interpolator-0.1.0.tar", last modified: Sat Jun 17 10:27:22 2023, max compression
+gzip compressed data, was "simple-interpolator-0.1.1.tar", last modified: Sat Jun 17 10:31:38 2023, max compression
```

## Comparing `simple-interpolator-0.1.0.tar` & `simple-interpolator-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:27:22.362262 simple-interpolator-0.1.0/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-17 10:27:22.362262 simple-interpolator-0.1.0/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)     2855 2023-06-17 09:43:55.000000 simple-interpolator-0.1.0/README.md
--rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-17 10:27:22.362262 simple-interpolator-0.1.0/setup.cfg
--rw-r--r--   0 stef      (1000) stef      (1000)      794 2023-06-17 10:27:06.000000 simple-interpolator-0.1.0/setup.py
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:27:22.358929 simple-interpolator-0.1.0/simple_interpolator/
--rw-r--r--   0 stef      (1000) stef      (1000)      310 2023-06-17 09:58:56.000000 simple-interpolator-0.1.0/simple_interpolator/__init__.py
--rw-r--r--   0 stef      (1000) stef      (1000)     2302 2023-06-17 10:15:06.000000 simple-interpolator-0.1.0/simple_interpolator/interpolator.py
--rw-r--r--   0 stef      (1000) stef      (1000)      664 2023-06-16 14:59:49.000000 simple-interpolator-0.1.0/simple_interpolator/stylizer.py
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:27:22.362262 simple-interpolator-0.1.0/simple_interpolator.egg-info/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)      332 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/SOURCES.txt
--rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/dependency_links.txt
--rw-r--r--   0 stef      (1000) stef      (1000)       17 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/requires.txt
--rw-r--r--   0 stef      (1000) stef      (1000)       20 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/top_level.txt
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:31:38.031640 simple-interpolator-0.1.1/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-17 10:31:38.028307 simple-interpolator-0.1.1/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)     2855 2023-06-17 09:43:55.000000 simple-interpolator-0.1.1/README.md
+-rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-17 10:31:38.031640 simple-interpolator-0.1.1/setup.cfg
+-rw-r--r--   0 stef      (1000) stef      (1000)      794 2023-06-17 10:31:36.000000 simple-interpolator-0.1.1/setup.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:31:38.028307 simple-interpolator-0.1.1/simple_interpolator/
+-rw-r--r--   0 stef      (1000) stef      (1000)       57 2023-06-17 10:31:04.000000 simple-interpolator-0.1.1/simple_interpolator/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2269 2023-06-17 10:30:44.000000 simple-interpolator-0.1.1/simple_interpolator/interpolator.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      664 2023-06-16 14:59:49.000000 simple-interpolator-0.1.1/simple_interpolator/stylizer.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:31:38.028307 simple-interpolator-0.1.1/simple_interpolator.egg-info/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)      332 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/SOURCES.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/dependency_links.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)       17 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/requires.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)       20 2023-06-17 10:31:37.000000 simple-interpolator-0.1.1/simple_interpolator.egg-info/top_level.txt
```

### Comparing `simple-interpolator-0.1.0/README.md` & `simple-interpolator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `simple-interpolator-0.1.0/setup.py` & `simple-interpolator-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'A simple interpolator.'
 
 # Setting up
 setup(
     name="simple-interpolator",
     version=VERSION,
     author="var-pi (Stefan Ehin)",
```

### Comparing `simple-interpolator-0.1.0/simple_interpolator/interpolator.py` & `simple-interpolator-0.1.1/simple_interpolator/interpolator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import functools
 import math
-# from simple_interpolator.stylizer import f_as_text
-from stylizer import f_as_text
+from simple_interpolator.stylizer import f_as_text
 
 class Interpolator:
     def __init__(self, data):
         self.data = data
         self.__power_touples = self.__generate_power_touples()
         self.__b = self.__generate_b()
         self.f = self.__generate_f()
```

### Comparing `simple-interpolator-0.1.0/simple_interpolator/stylizer.py` & `simple-interpolator-0.1.1/simple_interpolator/stylizer.py`

 * *Files identical despite different names*

