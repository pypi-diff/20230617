# Comparing `tmp/tgsdl-1.0.3.tar.gz` & `tmp/tgsdl-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgsdl-1.0.3.tar", last modified: Thu Jun 15 17:22:35 2023, max compression
+gzip compressed data, was "tgsdl-1.0.4.tar", last modified: Sat Jun 17 09:33:58 2023, max compression
```

## Comparing `tgsdl-1.0.3.tar` & `tgsdl-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:22:35.642053 tgsdl-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-15 17:22:24.000000 tgsdl-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 17:22:24.000000 tgsdl-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-15 17:22:35.642053 tgsdl-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-15 17:22:24.000000 tgsdl-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 17:22:35.642053 tgsdl-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-15 17:22:24.000000 tgsdl-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:22:35.638053 tgsdl-1.0.3/tgsdl/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-15 17:22:24.000000 tgsdl-1.0.3/tgsdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-15 17:22:24.000000 tgsdl-1.0.3/tgsdl/tgsdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:22:35.642053 tgsdl-1.0.3/tgsdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-15 17:22:35.000000 tgsdl-1.0.3/tgsdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-15 17:22:35.000000 tgsdl-1.0.3/tgsdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:22:35.000000 tgsdl-1.0.3/tgsdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-15 17:22:35.000000 tgsdl-1.0.3/tgsdl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-15 17:22:35.000000 tgsdl-1.0.3/tgsdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 17:22:35.000000 tgsdl-1.0.3/tgsdl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:33:58.634646 tgsdl-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-17 09:33:49.000000 tgsdl-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 09:33:49.000000 tgsdl-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-17 09:33:58.634646 tgsdl-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-17 09:33:49.000000 tgsdl-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 09:33:58.634646 tgsdl-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-17 09:33:49.000000 tgsdl-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:33:58.630646 tgsdl-1.0.4/tgsdl/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 09:33:49.000000 tgsdl-1.0.4/tgsdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-17 09:33:49.000000 tgsdl-1.0.4/tgsdl/tgsdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:33:58.634646 tgsdl-1.0.4/tgsdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 09:33:58.000000 tgsdl-1.0.4/tgsdl.egg-info/top_level.txt
```

### Comparing `tgsdl-1.0.3/LICENSE` & `tgsdl-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tgsdl-1.0.3/PKG-INFO` & `tgsdl-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgsdl
-Version: 1.0.3
+Version: 1.0.4
 Summary: Telegram Sticker Pack Downloader Library
 Home-page: https://github.com/lillisfeb/TGSDL/
 Author: Bevlil
 Author-email: voidlillis@gmail.com
 License: MIT
 Keywords: telegram,bot,sticker,download,stickerpack
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tgsdl-1.0.3/README.md` & `tgsdl-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tgsdl-1.0.3/setup.py` & `tgsdl-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
 readme_path = os.path.join(current_dir, 'README.md')
 
 setup(
     name='tgsdl',
-    version='1.0.3',
+    version='1.0.4',
     description='Telegram Sticker Pack Downloader Library',
     author='Bevlil',
     author_email='voidlillis@gmail.com',
     url='https://github.com/lillisfeb/TGSDL/',
     long_description = open(readme_path).read(),
     long_description_content_type='text/markdown',
     keywords=['telegram', 'bot', 'sticker', 'download', 'stickerpack'],
```

### Comparing `tgsdl-1.0.3/tgsdl/tgsdl.py` & `tgsdl-1.0.4/tgsdl/tgsdl.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 
     def api(self, pack_url):
         pack = self.url(pack_url)
         params = {'bev': pack}
         req = requests.get(self.api_url, params=params)
         if req.status_code == 200:
             return req.json()
+        elif req.status_code == 404:
+        	return red("Sticker Pack Not Found")
         else:
             return red("Something went wrong")
 
     def download_file(self, file_data, folder_name):
         try:
 	        name = file_data['name']
 	        download_url = file_data['url']
```

### Comparing `tgsdl-1.0.3/tgsdl.egg-info/PKG-INFO` & `tgsdl-1.0.4/tgsdl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgsdl
-Version: 1.0.3
+Version: 1.0.4
 Summary: Telegram Sticker Pack Downloader Library
 Home-page: https://github.com/lillisfeb/TGSDL/
 Author: Bevlil
 Author-email: voidlillis@gmail.com
 License: MIT
 Keywords: telegram,bot,sticker,download,stickerpack
 Classifier: Programming Language :: Python :: 3
```

