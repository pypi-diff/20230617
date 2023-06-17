# Comparing `tmp/yunpancli-0.0.8.tar.gz` & `tmp/yunpancli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunpancli-0.0.8.tar", last modified: Fri Jun 16 09:28:31 2023, max compression
+gzip compressed data, was "yunpancli-0.0.9.tar", last modified: Fri Jun 16 09:43:22 2023, max compression
```

## Comparing `yunpancli-0.0.8.tar` & `yunpancli-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:28:31.505240 yunpancli-0.0.8/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.8/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:28:31.505324 yunpancli-0.0.8/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.8/README.md
--rw-r--r--   0 mac        (501) staff       (20)      138 2023-06-16 09:28:31.505654 yunpancli-0.0.8/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      689 2023-06-16 09:27:59.000000 yunpancli-0.0.8/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:28:31.504050 yunpancli-0.0.8/yunpancli/
--rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.8/yunpancli/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     9933 2023-06-16 09:27:37.000000 yunpancli-0.0.8/yunpancli/baidu_pan_sdk.py
--rw-r--r--   0 mac        (501) staff       (20)     7241 2023-05-26 02:59:50.000000 yunpancli-0.0.8/yunpancli/base.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:28:31.505116 yunpancli-0.0.8/yunpancli.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)       26 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-06-16 09:28:31.000000 yunpancli-0.0.8/yunpancli.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:43:22.575371 yunpancli-0.0.9/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.9/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:43:22.575470 yunpancli-0.0.9/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.9/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      138 2023-06-16 09:43:22.575819 yunpancli-0.0.9/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      689 2023-06-16 09:43:12.000000 yunpancli-0.0.9/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:43:22.573960 yunpancli-0.0.9/yunpancli/
+-rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.9/yunpancli/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     9932 2023-06-16 09:42:27.000000 yunpancli-0.0.9/yunpancli/baidu_pan_sdk.py
+-rw-r--r--   0 mac        (501) staff       (20)     7241 2023-05-26 02:59:50.000000 yunpancli-0.0.9/yunpancli/base.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:43:22.574998 yunpancli-0.0.9/yunpancli.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:43:22.000000 yunpancli-0.0.9/yunpancli.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-06-16 09:43:22.000000 yunpancli-0.0.9/yunpancli.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-16 09:43:22.000000 yunpancli-0.0.9/yunpancli.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-06-16 09:43:22.000000 yunpancli-0.0.9/yunpancli.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (501) staff       (20)       26 2023-06-16 09:43:22.000000 yunpancli-0.0.9/yunpancli.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2023-06-16 09:43:22.000000 yunpancli-0.0.9/yunpancli.egg-info/top_level.txt
```

### Comparing `yunpancli-0.0.8/LICENSE` & `yunpancli-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.8/setup.py` & `yunpancli-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yunpancli",
     entry_points={"console_scripts": ["pancli=yunpancli:main"]},
-    version="0.0.8",
+    version="0.0.9",
     author="Tang Yubin",
     author_email="tang-yu-bin@qq.com",
     description="cloud storage CLI (Command Line Interface)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/aierwiki/yunpancli",
     packages=setuptools.find_packages(),
```

### Comparing `yunpancli-0.0.8/yunpancli/baidu_pan_sdk.py` & `yunpancli-0.0.9/yunpancli/baidu_pan_sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,24 +80,24 @@
                     'access_token': access_token,
                     'path': remote_path,
                     'type': 'tmpfile',
                     'uploadid': uploadid,
                     'partseq': seq
                 }
                 api = BaiduPanSDK.UPLOAD_API + urlencode(params)
-                res = requests.post(api, files=files).json()
+                res = requests.post(api, files=files)
                 # 如果失败了则重试10次
-                if res['errno'] != 0:
+                if res.status_code != 200:
                     for _ in range(10):
                         sleep(2)
-                        res = requests.post(api, files=files).json()
-                        if res['errno'] == 0:
+                        res = requests.post(api, files=files)
+                        if res.status_code != 200:
                             break
-                if res['errno'] != 0:      
-                    print(BaiduPanSDK.ERROR_INFO.get(res['errno'], '未知错误'))
+                if res.status_code != 200:      
+                    print(BaiduPanSDK.ERROR_INFO.get(res.status_code, '未知错误'))
                     return False
         
         return True
         
     def precreate(self, local_file_path, remote_file_path, access_token):  
         block_list = []
         with open(local_file_path, 'rb') as f:
@@ -119,20 +119,20 @@
             'path': remote_file_path,
             'size': size,
             'isdir': 0,
             'autoinit': 1,
             'block_list': block_list
         }
         api = BaiduPanSDK.PRECREATE_API + urlencode(params)
-        res = requests.post(api, data=data).json()
-        if res['errno'] != 0:
-            print(BaiduPanSDK.ERROR_INFO.get(res['errno'], '未知错误'))
+        res = requests.post(api, data=data)
+        if res.status_code != 200:
+            print(BaiduPanSDK.ERROR_INFO.get(res.status_code, '未知错误'))
             return None, None, None
-        json_resp = json.loads(res.content)
-        return json_resp['uploadid'], size, block_list
+        result = json.loads(res.content)
+        return result['uploadid'], size, block_list
         
     def upload_file(self, local_file_path, remote_file_path, access_token):
         logger.debug(f"upload {local_file_path} to {remote_file_path}")
         # 1. 预上传
         uploadid, size, block_list = self.precreate(local_file_path, remote_file_path, access_token)
         if uploadid is None:
             return False
```

### Comparing `yunpancli-0.0.8/yunpancli/base.py` & `yunpancli-0.0.9/yunpancli/base.py`

 * *Files identical despite different names*

