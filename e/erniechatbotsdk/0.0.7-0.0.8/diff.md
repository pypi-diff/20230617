# Comparing `tmp/erniechatbotsdk-0.0.7.tar.gz` & `tmp/erniechatbotsdk-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erniechatbotsdk-0.0.7.tar", last modified: Sat Jun 17 15:49:55 2023, max compression
+gzip compressed data, was "erniechatbotsdk-0.0.8.tar", last modified: Sat Jun 17 16:24:01 2023, max compression
```

## Comparing `erniechatbotsdk-0.0.7.tar` & `erniechatbotsdk-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:49:55.671080 erniechatbotsdk-0.0.7/
--rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.7/LICENSE
--rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 15:49:55.670309 erniechatbotsdk-0.0.7/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)     1812 2023-06-17 12:11:28.000000 erniechatbotsdk-0.0.7/README.md
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:49:55.658822 erniechatbotsdk-0.0.7/erniebotchat/
--rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 14:58:33.000000 erniechatbotsdk-0.0.7/erniebotchat/__init__.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:49:55.660936 erniechatbotsdk-0.0.7/erniebotchat/baiduinfo/
--rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 15:38:30.000000 erniechatbotsdk-0.0.7/erniebotchat/baiduinfo/Baidu.py
--rw-r--r--   0 tk         (501) staff       (20)       24 2023-06-17 15:39:28.000000 erniechatbotsdk-0.0.7/erniebotchat/baiduinfo/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      487 2023-06-17 14:24:33.000000 erniechatbotsdk-0.0.7/erniebotchat/erniebot.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:49:55.662640 erniechatbotsdk-0.0.7/erniebotchat/error/
--rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.7/erniebotchat/error/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.7/erniebotchat/error/customerror.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:49:55.664319 erniechatbotsdk-0.0.7/erniebotchat/service/
--rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.7/erniebotchat/service/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)     2301 2023-06-17 15:42:26.000000 erniechatbotsdk-0.0.7/erniebotchat/service/explain.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 15:49:55.669193 erniechatbotsdk-0.0.7/erniechatbotsdk.egg-info/
--rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 15:49:55.000000 erniechatbotsdk-0.0.7/erniechatbotsdk.egg-info/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)      467 2023-06-17 15:49:55.000000 erniechatbotsdk-0.0.7/erniechatbotsdk.egg-info/SOURCES.txt
--rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 15:49:55.000000 erniechatbotsdk-0.0.7/erniechatbotsdk.egg-info/dependency_links.txt
--rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 15:49:55.000000 erniechatbotsdk-0.0.7/erniechatbotsdk.egg-info/requires.txt
--rw-r--r--   0 tk         (501) staff       (20)       13 2023-06-17 15:49:55.000000 erniechatbotsdk-0.0.7/erniechatbotsdk.egg-info/top_level.txt
--rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 15:49:55.671290 erniechatbotsdk-0.0.7/setup.cfg
--rw-r--r--   0 tk         (501) staff       (20)      909 2023-06-17 15:49:24.000000 erniechatbotsdk-0.0.7/setup.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.677259 erniechatbotsdk-0.0.8/
+-rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.8/LICENSE
+-rw-r--r--   0 tk         (501) staff       (20)     2167 2023-06-17 16:24:01.676398 erniechatbotsdk-0.0.8/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)     1576 2023-06-17 16:08:12.000000 erniechatbotsdk-0.0.8/README.md
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.666574 erniechatbotsdk-0.0.8/erniebotchat/
+-rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 14:58:33.000000 erniechatbotsdk-0.0.8/erniebotchat/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      488 2023-06-17 16:20:59.000000 erniechatbotsdk-0.0.8/erniebotchat/erniebot.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.668544 erniechatbotsdk-0.0.8/erniebotchat/error/
+-rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.8/erniebotchat/error/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.8/erniebotchat/error/customerror.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.670342 erniechatbotsdk-0.0.8/erniebotchat/service/
+-rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.8/erniebotchat/service/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)     2710 2023-06-17 16:21:57.000000 erniechatbotsdk-0.0.8/erniebotchat/service/explain.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 16:24:01.675268 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/
+-rw-r--r--   0 tk         (501) staff       (20)     2167 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)      400 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/requires.txt
+-rw-r--r--   0 tk         (501) staff       (20)       13 2023-06-17 16:24:01.000000 erniechatbotsdk-0.0.8/erniechatbotsdk.egg-info/top_level.txt
+-rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 16:24:01.677501 erniechatbotsdk-0.0.8/setup.cfg
+-rw-r--r--   0 tk         (501) staff       (20)      979 2023-06-17 16:13:36.000000 erniechatbotsdk-0.0.8/setup.py
```

### Comparing `erniechatbotsdk-0.0.7/LICENSE` & `erniechatbotsdk-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.7/erniebotchat/service/explain.py` & `erniechatbotsdk-0.0.8/erniebotchat/service/explain.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-from ..baiduinfo.Baidu import BaseConfig
 from ..error.customerror import CustomError
 import aiohttp
 import json
+class Baidu:
+    TOKEN="https://aip.baidubce.com/oauth/2.0/token?grant_type=client_credentials&client_id={apikey}&client_secret={secretkey}"
+    ERNIEBOT="https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/completions?access_token={access_token}"
+    ERNIEBOTTURBO="https://aip.baidubce.com/rpc/2.0/ai_custom/v1/wenxinworkshop/chat/eb-instant?access_token={access_token}"
+    ERNIEBOT_NAME="erniebot"
+    ERNIEBOTTURBO_NAME="erniebotturbo"
 TOKEN = None
 Templat='{"messages": [{"role": "user", "content": "message"}], "temperature": null, "top_p": null, "penalty_score": null, "stream": null, "user_id": null}'
-class Explain(BaseConfig):
+class Explain(Baidu):
     
     def __init__(self,apikey,secretkey):
         self.apikey=apikey
         self.secretkey=secretkey
 
     async def getToken(self):
         global TOKEN
```

### Comparing `erniechatbotsdk-0.0.7/setup.py` & `erniechatbotsdk-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="erniechatbotsdk",
-    version="0.0.7",
+    version="0.0.8",
     description="Baidu Wenxin word api package",
     author="Tk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="tkzhu66@gmail.com",
-    packages=find_packages(),
+    #packages=find_packages(),
+    package_data={
+        'erniebotchat':['erniebotchat/*'],
+    },
     install_requires=[
         "wcwidth"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

