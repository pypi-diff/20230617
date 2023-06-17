# Comparing `tmp/erniechatbotsdk-0.0.2.tar.gz` & `tmp/erniechatbotsdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erniechatbotsdk-0.0.2.tar", last modified: Sat Jun 17 12:11:45 2023, max compression
+gzip compressed data, was "erniechatbotsdk-0.0.3.tar", last modified: Sat Jun 17 14:45:58 2023, max compression
```

## Comparing `erniechatbotsdk-0.0.2.tar` & `erniechatbotsdk-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.458472 erniechatbotsdk-0.0.2/
--rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.2/LICENSE
--rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 12:11:45.457541 erniechatbotsdk-0.0.2/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)     1812 2023-06-17 12:11:28.000000 erniechatbotsdk-0.0.2/README.md
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.441579 erniechatbotsdk-0.0.2/erniebot/
--rw-r--r--   0 tk         (501) staff       (20)        0 2023-06-17 10:38:05.000000 erniechatbotsdk-0.0.2/erniebot/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      487 2023-06-17 10:56:36.000000 erniechatbotsdk-0.0.2/erniebot/erniebot.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.444371 erniechatbotsdk-0.0.2/erniebot/error/
--rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.2/erniebot/error/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.2/erniebot/error/customerror.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.447664 erniechatbotsdk-0.0.2/erniebot/service/
--rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.2/erniebot/service/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)     2265 2023-06-17 10:49:24.000000 erniechatbotsdk-0.0.2/erniebot/service/explain.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.450451 erniechatbotsdk-0.0.2/erniebot/util/
--rw-r--r--   0 tk         (501) staff       (20)       61 2023-06-17 05:36:28.000000 erniechatbotsdk-0.0.2/erniebot/util/__init__.py
--rw-r--r--   0 tk         (501) staff       (20)     2570 2023-06-17 11:26:35.000000 erniechatbotsdk-0.0.2/erniebot/util/httputils.py
-drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 12:11:45.456521 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/
--rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/PKG-INFO
--rw-r--r--   0 tk         (501) staff       (20)      429 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/SOURCES.txt
--rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/dependency_links.txt
--rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/requires.txt
--rw-r--r--   0 tk         (501) staff       (20)        9 2023-06-17 12:11:45.000000 erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/top_level.txt
--rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 12:11:45.458709 erniechatbotsdk-0.0.2/setup.cfg
--rw-r--r--   0 tk         (501) staff       (20)      909 2023-06-17 12:11:39.000000 erniechatbotsdk-0.0.2/setup.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 14:45:58.323693 erniechatbotsdk-0.0.3/
+-rw-r--r--   0 tk         (501) staff       (20)     1058 2023-06-17 11:06:14.000000 erniechatbotsdk-0.0.3/LICENSE
+-rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 14:45:58.322777 erniechatbotsdk-0.0.3/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)     1812 2023-06-17 12:11:28.000000 erniechatbotsdk-0.0.3/README.md
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 14:45:58.311969 erniechatbotsdk-0.0.3/erniebot/
+-rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 13:52:01.000000 erniechatbotsdk-0.0.3/erniebot/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      487 2023-06-17 14:24:33.000000 erniechatbotsdk-0.0.3/erniebot/erniebot.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 14:45:58.313823 erniechatbotsdk-0.0.3/erniebot/error/
+-rw-r--r--   0 tk         (501) staff       (20)       36 2023-06-17 10:09:15.000000 erniechatbotsdk-0.0.3/erniebot/error/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)      148 2023-06-17 10:04:03.000000 erniechatbotsdk-0.0.3/erniebot/error/customerror.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 14:45:58.315973 erniechatbotsdk-0.0.3/erniebot/service/
+-rw-r--r--   0 tk         (501) staff       (20)       28 2023-06-17 04:04:37.000000 erniechatbotsdk-0.0.3/erniebot/service/__init__.py
+-rw-r--r--   0 tk         (501) staff       (20)     2301 2023-06-17 14:41:24.000000 erniechatbotsdk-0.0.3/erniebot/service/explain.py
+drwxr-xr-x   0 tk         (501) staff       (20)        0 2023-06-17 14:45:58.321647 erniechatbotsdk-0.0.3/erniechatbotsdk.egg-info/
+-rw-r--r--   0 tk         (501) staff       (20)     2403 2023-06-17 14:45:58.000000 erniechatbotsdk-0.0.3/erniechatbotsdk.egg-info/PKG-INFO
+-rw-r--r--   0 tk         (501) staff       (20)      376 2023-06-17 14:45:58.000000 erniechatbotsdk-0.0.3/erniechatbotsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 tk         (501) staff       (20)        1 2023-06-17 14:45:58.000000 erniechatbotsdk-0.0.3/erniechatbotsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 tk         (501) staff       (20)        8 2023-06-17 14:45:58.000000 erniechatbotsdk-0.0.3/erniechatbotsdk.egg-info/requires.txt
+-rw-r--r--   0 tk         (501) staff       (20)        9 2023-06-17 14:45:58.000000 erniechatbotsdk-0.0.3/erniechatbotsdk.egg-info/top_level.txt
+-rw-r--r--   0 tk         (501) staff       (20)       38 2023-06-17 14:45:58.323917 erniechatbotsdk-0.0.3/setup.cfg
+-rw-r--r--   0 tk         (501) staff       (20)      909 2023-06-17 14:45:50.000000 erniechatbotsdk-0.0.3/setup.py
```

### Comparing `erniechatbotsdk-0.0.2/LICENSE` & `erniechatbotsdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.2/PKG-INFO` & `erniechatbotsdk-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erniechatbotsdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Baidu Wenxin word api package
 Author: Tk
 Author-email: tkzhu66@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erniechatbotsdk-0.0.2/README.md` & `erniechatbotsdk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `erniechatbotsdk-0.0.2/erniebot/service/explain.py` & `erniechatbotsdk-0.0.3/erniebot/service/explain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from erniebot.config.baseconfig import BaseConfig
-from erniebot.error.customerror import CustomError
-from erniebot.util.httputils import RequestBody
+from ..base.baseconfig import BaseConfig
+from ..error.customerror import CustomError
 import aiohttp
 import json
 TOKEN = None
 Templat='{"messages": [{"role": "user", "content": "message"}], "temperature": null, "top_p": null, "penalty_score": null, "stream": null, "user_id": null}'
 class Explain(BaseConfig):
     
     def __init__(self,apikey,secretkey):
@@ -32,25 +31,28 @@
         token = await self.getToken()
         if bot == self.ERNIEBOT_NAME:
             ernieurl=self.ERNIEBOT.format(access_token=token)
         elif bot == self.ERNIEBOTTURBO_NAME:
             ernieurl=self.ERNIEBOTTURBO.format(access_token=token)
         else:
             raise CustomError(9627,"No model you accessed, please check the model name you passed in, currently only erniebot and erniebotturbo are supported")
-
-        if not isinstance(data,RequestBody):
+        try:
+            json_data=json.loads(data)
+        except json.JSONDecodeError as e:
+            raise CustomError(9528,"The passed parameter is incorrect,example:{}".format(Templat))
+        
+        if(len(json_data["messages"]) % 2 == 0):
             raise CustomError(9528,"The passed parameter is incorrect,example:{}".format(Templat))
-        json_data=json.dumps(data.to_dict(),ensure_ascii=False)
-        print("json_data",json_data)
+
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
         async with aiohttp.ClientSession() as session:
-            async with session.post(ernieurl,data=json_data,headers=headers) as response:
+            async with session.post(ernieurl,data=data,headers=headers) as response:
                 response_data =await response.json()
                 return response_data
```

### Comparing `erniechatbotsdk-0.0.2/erniechatbotsdk.egg-info/PKG-INFO` & `erniechatbotsdk-0.0.3/erniechatbotsdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erniechatbotsdk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Baidu Wenxin word api package
 Author: Tk
 Author-email: tkzhu66@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `erniechatbotsdk-0.0.2/setup.py` & `erniechatbotsdk-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="erniechatbotsdk",
-    version="0.0.2",
+    version="0.0.3",
     description="Baidu Wenxin word api package",
     author="Tk",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email="tkzhu66@gmail.com",
     packages=find_packages(),
     install_requires=[
```

