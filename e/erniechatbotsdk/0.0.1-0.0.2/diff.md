# Comparing `tmp/erniechatbotsdk-0.0.1.tar.gz` & `tmp/erniechatbotsdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erniechatbotsdk-0.0.1.tar", last modified: Sat Jun 17 12:09:57 2023, max compression
+gzip compressed data, was "erniechatbotsdk-0.0.2.tar", last modified: Sat Jun 17 12:11:45 2023, max compression
```

## Comparing `erniechatbotsdk-0.0.1.tar` & `erniechatbotsdk-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:09:57.516376 erniechatbotsdk-0.0.1/
--rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.1/LICENSE
--rw-r--r--   0 tk         (501) staff       (20)     2400 2023-06-17 12:09:57.515383 erniechatbotsdk-0.0.1/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)     1809 2023-06-17 11:47:23.000000 erniechatbotsdk-0.0.1/README.md
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:09:57.504545 erniechatbotsdk-0.0.1/erniebot/
--rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 10:38:05.000000 erniechatbotsdk-0.0.1/erniebot/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      487 2023-06-17 10:56:36.000000 erniechatbotsdk-0.0.1/erniebot/erniebot.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:09:57.505682 erniechatbotsdk-0.0.1/erniebot/error/
--rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.1/erniebot/error/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.1/erniebot/error/customerror.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:09:57.507660 erniechatbotsdk-0.0.1/erniebot/service/
--rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.1/erniebot/service/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)     2265 2023-06-17 10:49:24.000000 erniechatbotsdk-0.0.1/erniebot/service/explain.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:09:57.509647 erniechatbotsdk-0.0.1/erniebot/util/
--rw-r--r--   0 tk         (501) staff       (20)       61 2023-06-17 05:36:28.000000 erniechatbotsdk-0.0.1/erniebot/util/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)     2570 2023-06-17 11:26:35.000000 erniechatbotsdk-0.0.1/erniebot/util/httputils.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:09:57.514070 erniechatbotsdk-0.0.1/erniechatbotsdk.egg-info/
--rw-r--r--   0 tk         (501) staff       (20)     2400 2023-06-17 12:09:57.000000 erniechatbotsdk-0.0.1/erniechatbotsdk.egg-info/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)      429 2023-06-17 12:09:57.000000 erniechatbotsdk-0.0.1/erniechatbotsdk.egg-info/SOURCES.txt
--rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 12:09:57.000000 erniechatbotsdk-0.0.1/erniechatbotsdk.egg-info/dependency_links.txt
--rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 12:09:57.000000 erniechatbotsdk-0.0.1/erniechatbotsdk.egg-info/requires.txt
--rw-r--r--   0 tk         (501) staff       (20)        9 2023-06-17 12:09:57.000000 erniechatbotsdk-0.0.1/erniechatbotsdk.egg-info/top_level.txt
--rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 12:09:57.516584 erniechatbotsdk-0.0.1/setup.cfg
--rw-r--r--   0 tk         (501) staff       (20)      909 2023-06-17 12:09:43.000000 erniechatbotsdk-0.0.1/setup.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.458472 erniechatbotsdk-0.0.2/
+-rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.2/LICENSE
+-rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 12:11:45.457541 erniechatbotsdk-0.0.2/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)     1812 2023-06-17 12:11:28.000000 erniechatbotsdk-0.0.2/README.md
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.441579 erniechatbotsdk-0.0.2/erniebot/
+-rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 10:38:05.000000 erniechatbotsdk-0.0.2/erniebot/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      487 2023-06-17 10:56:36.000000 erniechatbotsdk-0.0.2/erniebot/erniebot.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.444371 erniechatbotsdk-0.0.2/erniebot/error/
+-rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.2/erniebot/error/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.2/erniebot/error/customerror.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.447664 erniechatbotsdk-0.0.2/erniebot/service/
+-rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.2/erniebot/service/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)     2265 2023-06-17 10:49:24.000000 erniechatbotsdk-0.0.2/erniebot/service/explain.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.450451 erniechatbotsdk-0.0.2/erniebot/util/
+-rw-r--r--   0 tk         (501) staff       (20)       61 2023-06-17 05:36:28.000000 erniechatbotsdk-0.0.2/erniebot/util/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)     2570 2023-06-17 11:26:35.000000 erniechatbotsdk-0.0.2/erniebot/util/httputils.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.456521 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/
+-rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)      429 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/requires.txt
+-rw-r--r--   0 tk         (501) staff       (20)        9 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/top_level.txt
+-rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 12:11:45.458709 erniechatbotsdk-0.0.2/setup.cfg
+-rw-r--r--   0 tk         (501) staff       (20)      909 2023-06-17 12:11:39.000000 erniechatbotsdk-0.0.2/setup.py
```

### Comparing `erniechatbotsdk-0.0.1/LICENSE` & `erniechatbotsdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.1/PKG-INFO` & `erniechatbotsdk-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erniechatbotsdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Baidu Wenxin word api package
 Author: Tk
 Author-email: tkzhu66@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 ErnieBot请求地址：https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/completions
 ErnieBot-turbo请求地址： https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/eb-instant
 的简单封装
 
 # 安装
 使用pip进行安装
 ```
-pip install erniebotchat
+pip install erniechatbotsdk
 ```
 # 使用教程
 ## 首先构建请求参数
 ```
 class RequestBody:
     def __init__(self,messages,temperature=None,top_p=None,penalty_score=None,stream=None,user_id=None):
         self.messages=messages
```

### Comparing `erniechatbotsdk-0.0.1/README.md` & `erniechatbotsdk-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ErnieBot请求地址：https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/completions
 ErnieBot-turbo请求地址： https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/eb-instant
 的简单封装
 
 # 安装
 使用pip进行安装
 ```
-pip install erniebotchat
+pip install erniechatbotsdk
 ```
 # 使用教程
 ## 首先构建请求参数
 ```
 class RequestBody:
     def __init__(self,messages,temperature=None,top_p=None,penalty_score=None,stream=None,user_id=None):
         self.messages=messages
```

### Comparing `erniechatbotsdk-0.0.1/erniebot/service/explain.py` & `erniechatbotsdk-0.0.2/erniebot/service/explain.py`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.1/erniebot/util/httputils.py` & `erniechatbotsdk-0.0.2/erniebot/util/httputils.py`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.1/erniechatbotsdk.egg-info/PKG-INFO` & `erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erniechatbotsdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Baidu Wenxin word api package
 Author: Tk
 Author-email: tkzhu66@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 ErnieBot请求地址：https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/completions
 ErnieBot-turbo请求地址： https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/eb-instant
 的简单封装
 
 # 安装
 使用pip进行安装
 ```
-pip install erniebotchat
+pip install erniechatbotsdk
 ```
 # 使用教程
 ## 首先构建请求参数
 ```
 class RequestBody:
     def __init__(self,messages,temperature=None,top_p=None,penalty_score=None,stream=None,user_id=None):
         self.messages=messages
```

### Comparing `erniechatbotsdk-0.0.1/setup.py` & `erniechatbotsdk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="erniechatbotsdk",
-    version="0.0.1",
+    version="0.0.2",
     description="Baidu Wenxin word api package",
     author="Tk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="tkzhu66@gmail.com",
     packages=find_packages(),
     install_requires=[
```

