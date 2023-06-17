# Comparing `tmp/auto-env-config-1.0.8.tar.gz` & `tmp/auto-env-config-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-env-config-1.0.8.tar", last modified: Mon Mar 27 06:39:17 2023, max compression
+gzip compressed data, was "auto-env-config-1.0.9.tar", last modified: Sat Jun 17 02:51:51 2023, max compression
```

## Comparing `auto-env-config-1.0.8.tar` & `auto-env-config-1.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-03-27 06:39:17.111232 auto-env-config-1.0.8/
--rw-r--r--   0 1zql1      (501) staff       (20)     1059 2022-12-25 04:52:48.000000 auto-env-config-1.0.8/LICENSE.txt
--rw-r--r--   0 1zql1      (501) staff       (20)     1197 2023-03-27 06:39:17.111120 auto-env-config-1.0.8/PKG-INFO
--rw-r--r--   0 1zql1      (501) staff       (20)      697 2023-03-27 06:33:39.000000 auto-env-config-1.0.8/README.md
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-03-27 06:39:17.110378 auto-env-config-1.0.8/aec/
--rw-r--r--   0 1zql1      (501) staff       (20)     7010 2023-03-27 06:30:07.000000 auto-env-config-1.0.8/aec/__init__.py
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-03-27 06:39:17.110937 auto-env-config-1.0.8/auto_env_config.egg-info/
--rw-r--r--   0 1zql1      (501) staff       (20)     1197 2023-03-27 06:39:16.000000 auto-env-config-1.0.8/auto_env_config.egg-info/PKG-INFO
--rw-r--r--   0 1zql1      (501) staff       (20)      202 2023-03-27 06:39:17.000000 auto-env-config-1.0.8/auto_env_config.egg-info/SOURCES.txt
--rw-r--r--   0 1zql1      (501) staff       (20)        1 2023-03-27 06:39:16.000000 auto-env-config-1.0.8/auto_env_config.egg-info/dependency_links.txt
--rw-r--r--   0 1zql1      (501) staff       (20)        4 2023-03-27 06:39:17.000000 auto-env-config-1.0.8/auto_env_config.egg-info/top_level.txt
--rw-r--r--   0 1zql1      (501) staff       (20)       38 2023-03-27 06:39:17.111404 auto-env-config-1.0.8/setup.cfg
--rw-r--r--   0 1zql1      (501) staff       (20)     1177 2023-03-27 06:39:14.000000 auto-env-config-1.0.8/setup.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-06-17 02:51:51.210142 auto-env-config-1.0.9/
+-rw-r--r--   0 1zql1      (501) staff       (20)     1059 2022-12-25 04:52:48.000000 auto-env-config-1.0.9/LICENSE.txt
+-rw-r--r--   0 1zql1      (501) staff       (20)      881 2023-06-17 02:51:51.210016 auto-env-config-1.0.9/PKG-INFO
+-rw-r--r--   0 1zql1      (501) staff       (20)      401 2023-06-17 02:49:32.000000 auto-env-config-1.0.9/README.md
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-06-17 02:51:51.209155 auto-env-config-1.0.9/aec/
+-rw-r--r--   0 1zql1      (501) staff       (20)     3148 2023-06-17 02:50:54.000000 auto-env-config-1.0.9/aec/__init__.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-06-17 02:51:51.209818 auto-env-config-1.0.9/auto_env_config.egg-info/
+-rw-r--r--   0 1zql1      (501) staff       (20)      881 2023-06-17 02:51:51.000000 auto-env-config-1.0.9/auto_env_config.egg-info/PKG-INFO
+-rw-r--r--   0 1zql1      (501) staff       (20)      202 2023-06-17 02:51:51.000000 auto-env-config-1.0.9/auto_env_config.egg-info/SOURCES.txt
+-rw-r--r--   0 1zql1      (501) staff       (20)        1 2023-06-17 02:51:51.000000 auto-env-config-1.0.9/auto_env_config.egg-info/dependency_links.txt
+-rw-r--r--   0 1zql1      (501) staff       (20)        4 2023-06-17 02:51:51.000000 auto-env-config-1.0.9/auto_env_config.egg-info/top_level.txt
+-rw-r--r--   0 1zql1      (501) staff       (20)       38 2023-06-17 02:51:51.210194 auto-env-config-1.0.9/setup.cfg
+-rw-r--r--   0 1zql1      (501) staff       (20)     1177 2023-06-17 02:49:32.000000 auto-env-config-1.0.9/setup.py
```

### Comparing `auto-env-config-1.0.8/LICENSE.txt` & `auto-env-config-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `auto-env-config-1.0.8/PKG-INFO` & `auto-env-config-1.0.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: auto-env-config
-Version: 1.0.8
+Version: 1.0.9
 Summary: Configuring your python environment automatically.
 Home-page: 
 Author: 曾钦李
 Author-email: 1838696034@qq.com
 Maintainer: 
 Maintainer-email: 
 License: MIT License
-Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -28,34 +27,17 @@
 ```
 ### Use config
 ```json
 {
   "pip_index": "https://pypi.org/simple",
   "packages": [
     {
-      "name": "numpy",
+      "package_name": "numpy",
       "version": "1.22.0"
     }
-  ],
-  "files": [
-    {
-      "path": "/data",
-      "nt_command": "mkdir -p /data"
-    },
-    {
-      "path": "/data/requirements.txt",
-      "posix_command": "echo numpy==1.22.0 > /data/requirements.txt"
-    }
-  ],
-  "script": [
-    {
-      "command": "python -m pip install -r requirements.txt"
-    }
   ]
 }
 ```
 ```python
 import aec
 aec.install('install.config.json')
 ```
-
-
```

### Comparing `auto-env-config-1.0.8/auto_env_config.egg-info/PKG-INFO` & `auto-env-config-1.0.9/auto_env_config.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: auto-env-config
-Version: 1.0.8
+Version: 1.0.9
 Summary: Configuring your python environment automatically.
 Home-page: 
 Author: 曾钦李
 Author-email: 1838696034@qq.com
 Maintainer: 
 Maintainer-email: 
 License: MIT License
-Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -28,34 +27,17 @@
 ```
 ### Use config
 ```json
 {
   "pip_index": "https://pypi.org/simple",
   "packages": [
     {
-      "name": "numpy",
+      "package_name": "numpy",
       "version": "1.22.0"
     }
-  ],
-  "files": [
-    {
-      "path": "/data",
-      "nt_command": "mkdir -p /data"
-    },
-    {
-      "path": "/data/requirements.txt",
-      "posix_command": "echo numpy==1.22.0 > /data/requirements.txt"
-    }
-  ],
-  "script": [
-    {
-      "command": "python -m pip install -r requirements.txt"
-    }
   ]
 }
 ```
 ```python
 import aec
 aec.install('install.config.json')
 ```
-
-
```

### Comparing `auto-env-config-1.0.8/setup.py` & `auto-env-config-1.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='auto-env-config',  # 包名
-    version='v1.0.8',  # 版本
+    version='v1.0.9',  # 版本
     description="Configuring your python environment automatically.",  # 包简介
     long_description=open('README.md', encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     long_description_content_type='text/markdown',
     include_package_data=True,  # 是否允许上传资源文件
     author='曾钦李',  # 作者
     author_email='1838696034@qq.com',  # 作者邮件
     maintainer='',  # 维护者
```

