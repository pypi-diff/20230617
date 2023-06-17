# Comparing `tmp/erniechatbotsdk-0.0.4.tar.gz` & `tmp/erniechatbotsdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erniechatbotsdk-0.0.4.tar", last modified: Sat Jun 17 15:25:46 2023, max compression
+gzip compressed data, was "erniechatbotsdk-0.0.5.tar", last modified: Sat Jun 17 15:29:48 2023, max compression
```

## Comparing `erniechatbotsdk-0.0.4.tar` & `erniechatbotsdk-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:25:46.260049 erniechatbotsdk-0.0.4/
--rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.4/LICENSE
--rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 15:25:46.258885 erniechatbotsdk-0.0.4/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)     1812 2023-06-17 12:11:28.000000 erniechatbotsdk-0.0.4/README.md
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:25:46.246323 erniechatbotsdk-0.0.4/erniebot/
--rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 14:58:33.000000 erniechatbotsdk-0.0.4/erniebot/__init__.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:25:46.248627 erniechatbotsdk-0.0.4/erniebot/baiduinfo/
--rw-r--r--   0 tk         (501) staff       (20)       24 2023-06-17 15:23:17.000000 erniechatbotsdk-0.0.4/erniebot/baiduinfo/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      454 2023-06-17 15:22:46.000000 erniechatbotsdk-0.0.4/erniebot/baiduinfo/baidu.py
--rw-r--r--   0 tk         (501) staff       (20)      487 2023-06-17 14:24:33.000000 erniechatbotsdk-0.0.4/erniebot/erniebot.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:25:46.251323 erniechatbotsdk-0.0.4/erniebot/error/
--rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.4/erniebot/error/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.4/erniebot/error/customerror.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:25:46.253169 erniechatbotsdk-0.0.4/erniebot/service/
--rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.4/erniebot/service/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)     2301 2023-06-17 15:23:47.000000 erniechatbotsdk-0.0.4/erniebot/service/explain.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:25:46.257899 erniechatbotsdk-0.0.4/erniechatbotsdk.egg-info/
--rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 15:25:46.000000 erniechatbotsdk-0.0.4/erniechatbotsdk.egg-info/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)      435 2023-06-17 15:25:46.000000 erniechatbotsdk-0.0.4/erniechatbotsdk.egg-info/SOURCES.txt
--rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 15:25:46.000000 erniechatbotsdk-0.0.4/erniechatbotsdk.egg-info/dependency_links.txt
--rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 15:25:46.000000 erniechatbotsdk-0.0.4/erniechatbotsdk.egg-info/requires.txt
--rw-r--r--   0 tk         (501) staff       (20)        9 2023-06-17 15:25:46.000000 erniechatbotsdk-0.0.4/erniechatbotsdk.egg-info/top_level.txt
--rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 15:25:46.260227 erniechatbotsdk-0.0.4/setup.cfg
--rw-r--r--   0 tk         (501) staff       (20)      978 2023-06-17 15:17:09.000000 erniechatbotsdk-0.0.4/setup.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:29:48.397015 erniechatbotsdk-0.0.5/
+-rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.5/LICENSE
+-rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 15:29:48.396115 erniechatbotsdk-0.0.5/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)     1812 2023-06-17 12:11:28.000000 erniechatbotsdk-0.0.5/README.md
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:29:48.384167 erniechatbotsdk-0.0.5/erniebotchat/
+-rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 14:58:33.000000 erniechatbotsdk-0.0.5/erniebotchat/__init__.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:29:48.385790 erniechatbotsdk-0.0.5/erniebotchat/baiduinfo/
+-rw-r--r--   0 tk         (501) staff       (20)       24 2023-06-17 15:23:17.000000 erniechatbotsdk-0.0.5/erniebotchat/baiduinfo/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      454 2023-06-17 15:22:46.000000 erniechatbotsdk-0.0.5/erniebotchat/baiduinfo/baidu.py
+-rw-r--r--   0 tk         (501) staff       (20)      487 2023-06-17 14:24:33.000000 erniechatbotsdk-0.0.5/erniebotchat/erniebot.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:29:48.388882 erniechatbotsdk-0.0.5/erniebotchat/error/
+-rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.5/erniebotchat/error/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.5/erniebotchat/error/customerror.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:29:48.390646 erniechatbotsdk-0.0.5/erniebotchat/service/
+-rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.5/erniebotchat/service/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)     2301 2023-06-17 15:23:47.000000 erniechatbotsdk-0.0.5/erniebotchat/service/explain.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:29:48.395055 erniechatbotsdk-0.0.5/erniechatbotsdk.egg-info/
+-rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 15:29:48.000000 erniechatbotsdk-0.0.5/erniechatbotsdk.egg-info/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)      467 2023-06-17 15:29:48.000000 erniechatbotsdk-0.0.5/erniechatbotsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 15:29:48.000000 erniechatbotsdk-0.0.5/erniechatbotsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 15:29:48.000000 erniechatbotsdk-0.0.5/erniechatbotsdk.egg-info/requires.txt
+-rw-r--r--   0 tk         (501) staff       (20)       13 2023-06-17 15:29:48.000000 erniechatbotsdk-0.0.5/erniechatbotsdk.egg-info/top_level.txt
+-rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 15:29:48.397247 erniechatbotsdk-0.0.5/setup.cfg
+-rw-r--r--   0 tk         (501) staff       (20)      909 2023-06-17 15:29:43.000000 erniechatbotsdk-0.0.5/setup.py
```

### Comparing `erniechatbotsdk-0.0.4/LICENSE` & `erniechatbotsdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.4/PKG-INFO` & `erniechatbotsdk-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erniechatbotsdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Baidu Wenxin word api package
 Author: Tk
 Author-email: tkzhu66@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erniechatbotsdk-0.0.4/README.md` & `erniechatbotsdk-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.4/erniebot/service/explain.py` & `erniechatbotsdk-0.0.5/erniebotchat/service/explain.py`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.4/erniechatbotsdk.egg-info/PKG-INFO` & `erniechatbotsdk-0.0.5/erniechatbotsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erniechatbotsdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Baidu Wenxin word api package
 Author: Tk
 Author-email: tkzhu66@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erniechatbotsdk-0.0.4/setup.py` & `erniechatbotsdk-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="erniechatbotsdk",
-    version="0.0.4",
+    version="0.0.5",
     description="Baidu Wenxin word api package",
     author="Tk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="tkzhu66@gmail.com",
     packages=find_packages(),
-    package_data={
-        "my_package": ["erniebot/base/*"],
-    },
     install_requires=[
         "wcwidth"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

