# Comparing `tmp/pydatawork-0.0.5.tar.gz` & `tmp/pydatawork-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.0.5.tar", last modified: Sat Jun 17 10:14:10 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.0.6.tar", last modified: Sat Jun 17 10:27:33 2023, max compression
```

## Comparing `pydatawork-0.0.5.tar` & `pydatawork-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 10:14:10.000000 pydatawork-0.0.5/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      744 2023-06-17 10:14:10.000000 pydatawork-0.0.5/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      196 2023-06-17 09:33:33.000000 pydatawork-0.0.5/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      744 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1056 2023-06-17 10:13:17.000000 pydatawork-0.0.5/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-17 10:14:10.000000 pydatawork-0.0.5/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-17 10:13:32.000000 pydatawork-0.0.5/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 10:27:33.000000 pydatawork-0.0.6/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1168 2023-06-17 10:27:33.000000 pydatawork-0.0.6/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      484 2023-06-17 10:26:09.000000 pydatawork-0.0.6/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1168 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-17 10:27:33.000000 pydatawork-0.0.6/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1056 2023-06-17 10:13:17.000000 pydatawork-0.0.6/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-17 10:27:33.000000 pydatawork-0.0.6/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-17 10:27:03.000000 pydatawork-0.0.6/setup.py
```

### Comparing `pydatawork-0.0.5/pydatawork.py` & `pydatawork-0.0.6/pydatawork.py`

 * *Files identical despite different names*

### Comparing `pydatawork-0.0.5/setup.py` & `pydatawork-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.0.5',
+    version='0.0.6',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

