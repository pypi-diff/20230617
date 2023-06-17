# Comparing `tmp/simple-interpolator-0.0.9.tar.gz` & `tmp/simple-interpolator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-interpolator-0.0.9.tar", last modified: Fri Jun 16 10:14:06 2023, max compression
+gzip compressed data, was "simple-interpolator-0.1.0.tar", last modified: Sat Jun 17 10:27:22 2023, max compression
```

## Comparing `simple-interpolator-0.0.9.tar` & `simple-interpolator-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 10:14:06.289884 simple-interpolator-0.0.9/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 10:14:06.289884 simple-interpolator-0.0.9/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-16 10:14:06.289884 simple-interpolator-0.0.9/setup.cfg
--rw-r--r--   0 stef      (1000) stef      (1000)      806 2023-06-16 10:13:51.000000 simple-interpolator-0.0.9/setup.py
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 10:14:06.286551 simple-interpolator-0.0.9/simple_interpolator/
--rw-r--r--   0 stef      (1000) stef      (1000)       88 2023-06-16 10:10:20.000000 simple-interpolator-0.0.9/simple_interpolator/__init__.py
--rw-r--r--   0 stef      (1000) stef      (1000)     1692 2023-06-16 10:09:35.000000 simple-interpolator-0.0.9/simple_interpolator/interpolator.py
--rw-r--r--   0 stef      (1000) stef      (1000)      578 2023-06-16 08:48:52.000000 simple-interpolator-0.0.9/simple_interpolator/stylizer.py
-drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-16 10:14:06.289884 simple-interpolator-0.0.9/simple_interpolator.egg-info/
--rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/PKG-INFO
--rw-r--r--   0 stef      (1000) stef      (1000)      322 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/SOURCES.txt
--rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/dependency_links.txt
--rw-r--r--   0 stef      (1000) stef      (1000)       27 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/requires.txt
--rw-r--r--   0 stef      (1000) stef      (1000)       20 2023-06-16 10:14:06.000000 simple-interpolator-0.0.9/simple_interpolator.egg-info/top_level.txt
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:27:22.362262 simple-interpolator-0.1.0/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-17 10:27:22.362262 simple-interpolator-0.1.0/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)     2855 2023-06-17 09:43:55.000000 simple-interpolator-0.1.0/README.md
+-rw-r--r--   0 stef      (1000) stef      (1000)       38 2023-06-17 10:27:22.362262 simple-interpolator-0.1.0/setup.cfg
+-rw-r--r--   0 stef      (1000) stef      (1000)      794 2023-06-17 10:27:06.000000 simple-interpolator-0.1.0/setup.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:27:22.358929 simple-interpolator-0.1.0/simple_interpolator/
+-rw-r--r--   0 stef      (1000) stef      (1000)      310 2023-06-17 09:58:56.000000 simple-interpolator-0.1.0/simple_interpolator/__init__.py
+-rw-r--r--   0 stef      (1000) stef      (1000)     2302 2023-06-17 10:15:06.000000 simple-interpolator-0.1.0/simple_interpolator/interpolator.py
+-rw-r--r--   0 stef      (1000) stef      (1000)      664 2023-06-16 14:59:49.000000 simple-interpolator-0.1.0/simple_interpolator/stylizer.py
+drwxr-xr-x   0 stef      (1000) stef      (1000)        0 2023-06-17 10:27:22.362262 simple-interpolator-0.1.0/simple_interpolator.egg-info/
+-rw-r--r--   0 stef      (1000) stef      (1000)      494 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/PKG-INFO
+-rw-r--r--   0 stef      (1000) stef      (1000)      332 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/SOURCES.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)        1 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/dependency_links.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)       17 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/requires.txt
+-rw-r--r--   0 stef      (1000) stef      (1000)       20 2023-06-17 10:27:22.000000 simple-interpolator-0.1.0/simple_interpolator.egg-info/top_level.txt
```

### Comparing `simple-interpolator-0.0.9/setup.py` & `simple-interpolator-0.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 DESCRIPTION = 'A simple interpolator.'
 
 # Setting up
 setup(
     name="simple-interpolator",
     version=VERSION,
     author="var-pi (Stefan Ehin)",
     author_email="<stefanehin4@gmail.com>",
     description=DESCRIPTION,
     packages=find_packages(),
-    install_requires=['matplotlib','numpy','functools'],
+    install_requires=['matplotlib','numpy'],
     keywords=['python', 'interpolation', 'bilinear', 'math', 'graph', '3D'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `simple-interpolator-0.0.9/simple_interpolator/stylizer.py` & `simple-interpolator-0.1.0/simple_interpolator/stylizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,12 +9,14 @@
         case 1:
             return b
         case other:
             return b+str(p).translate(SUP)
 
 def f_as_text(b,power_touples,accuracy):
     return functools.reduce(
-        lambda acc, i : acc+("·" if i != 0 else "")+
-        str(b[i] if accuracy == -1 else round(b[i],accuracy))+
+        lambda acc, i : acc+
+        ("" if round(b[i],accuracy)==0 else 
+        (("+" if b[i]>=0 else "-") if i != 0 else "")+
+        str(abs(b[i]) if accuracy == -1 else abs(round(b[i],accuracy)))+
         ((stylize_power("x", power_touples[i][0]))+
-         stylize_power("y", power_touples[i][1])), 
+         stylize_power("y", power_touples[i][1]))), 
         range(len(b)), "")
```

