# Comparing `tmp/minidevice-2.0.2.tar.gz` & `tmp/minidevice-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.0.2.tar", last modified: Sat Jun 17 14:26:44 2023, max compression
+gzip compressed data, was "minidevice-2.0.3.tar", last modified: Sat Jun 17 14:49:00 2023, max compression
```

## Comparing `minidevice-2.0.2.tar` & `minidevice-2.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 14:26:44.343754 minidevice-2.0.2/
--rw-rw-rw-   0        0        0     2263 2023-06-17 14:26:44.343754 minidevice-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1969 2023-06-17 14:07:39.000000 minidevice-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 14:26:44.313953 minidevice-2.0.2/minidevice/
--rw-rw-rw-   0        0        0     2745 2023-06-17 13:52:23.000000 minidevice-2.0.2/minidevice/DroidCast.py
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.2/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      226 2023-06-17 13:50:45.000000 minidevice-2.0.2/minidevice/__init__.py
--rw-rw-rw-   0        0        0    20907 2023-06-17 11:44:42.000000 minidevice-2.0.2/minidevice/adb.py
--rw-rw-rw-   0        0        0    20709 2023-06-17 14:09:56.000000 minidevice-2.0.2/minidevice/images.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.2/minidevice/logger.py
--rw-rw-rw-   0        0        0    12786 2023-06-17 06:49:51.000000 minidevice-2.0.2/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1678 2023-06-17 06:50:00.000000 minidevice-2.0.2/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      658 2023-06-17 06:08:54.000000 minidevice-2.0.2/minidevice/screencap.py
--rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.2/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-06-17 14:26:44.341830 minidevice-2.0.2/minidevice.egg-info/
--rw-rw-rw-   0        0        0     2263 2023-06-17 14:26:44.000000 minidevice-2.0.2/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-06-17 14:26:44.000000 minidevice-2.0.2/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 14:26:44.000000 minidevice-2.0.2/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-17 14:26:44.000000 minidevice-2.0.2/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-17 14:26:44.000000 minidevice-2.0.2/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 14:26:44.343754 minidevice-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      754 2023-06-17 14:16:07.000000 minidevice-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 14:49:00.051511 minidevice-2.0.3/
+-rw-rw-rw-   0        0        0     2263 2023-06-17 14:49:00.051511 minidevice-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1969 2023-06-17 14:48:33.000000 minidevice-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 14:49:00.036788 minidevice-2.0.3/minidevice/
+-rw-rw-rw-   0        0        0     2745 2023-06-17 13:52:23.000000 minidevice-2.0.3/minidevice/DroidCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.3/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      226 2023-06-17 14:47:51.000000 minidevice-2.0.3/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    20907 2023-06-17 11:44:42.000000 minidevice-2.0.3/minidevice/adb.py
+-rw-rw-rw-   0        0        0    20709 2023-06-17 14:09:56.000000 minidevice-2.0.3/minidevice/images.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.3/minidevice/logger.py
+-rw-rw-rw-   0        0        0    12786 2023-06-17 06:49:51.000000 minidevice-2.0.3/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1678 2023-06-17 06:50:00.000000 minidevice-2.0.3/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      658 2023-06-17 06:08:54.000000 minidevice-2.0.3/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.3/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-06-17 14:49:00.049560 minidevice-2.0.3/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     2263 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-17 14:48:59.000000 minidevice-2.0.3/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 14:49:00.052487 minidevice-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-17 14:47:58.000000 minidevice-2.0.3/setup.py
```

### Comparing `minidevice-2.0.2/PKG-INFO` & `minidevice-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.2
+Version: 2.0.3
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.2/README.md` & `minidevice-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.2/minidevice/DroidCast.py` & `minidevice-2.0.3/minidevice/DroidCast.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.2/minidevice/QueueUtils.py` & `minidevice-2.0.3/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.2/minidevice/adb.py` & `minidevice-2.0.3/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.2/minidevice/images.py` & `minidevice-2.0.3/minidevice/images.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.2/minidevice/minicap.py` & `minidevice-2.0.3/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.2/minidevice/minitouch.py` & `minidevice-2.0.3/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.2/minidevice/screencap.py` & `minidevice-2.0.3/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.2/minidevice.egg-info/PKG-INFO` & `minidevice-2.0.3/minidevice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.2
+Version: 2.0.3
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.2/setup.py` & `minidevice-2.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.0.2',
+      version='2.0.3',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
```

