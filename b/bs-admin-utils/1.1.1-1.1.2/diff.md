# Comparing `tmp/bs_admin_utils-1.1.1.tar.gz` & `tmp/bs_admin_utils-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_admin_utils-1.1.1.tar", last modified: Thu Jun 15 04:03:56 2023, max compression
+gzip compressed data, was "bs_admin_utils-1.1.2.tar", last modified: Sat Jun 17 08:36:32 2023, max compression
```

## Comparing `bs_admin_utils-1.1.1.tar` & `bs_admin_utils-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1067 2023-04-07 03:25:03.000000 bs_admin_utils-1.1.1/LICENSE
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       35 2023-04-07 04:04:08.000000 bs_admin_utils-1.1.1/MANIFEST.in
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      206 2023-04-07 03:35:29.000000 bs_admin_utils-1.1.1/README.md
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-15 04:03:56.371122 bs_admin_utils-1.1.1/bs_admin_utils/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2023-04-07 03:39:05.000000 bs_admin_utils-1.1.1/bs_admin_utils/__init__.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     4220 2023-06-15 04:01:20.000000 bs_admin_utils-1.1.1/bs_admin_utils/api.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      490 2023-04-07 04:11:32.000000 bs_admin_utils-1.1.1/bs_admin_utils/decorators.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1034 2023-04-07 03:48:50.000000 bs_admin_utils-1.1.1/bs_admin_utils/model.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/bs_admin_utils/static/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)   367112 2023-04-07 03:52:07.000000 bs_admin_utils-1.1.1/bs_admin_utils/static/arial.ttf
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     6248 2023-06-14 10:45:34.000000 bs_admin_utils-1.1.1/bs_admin_utils/static/nstc.ttf
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2439 2023-06-14 10:58:06.000000 bs_admin_utils-1.1.1/bs_admin_utils/vercode.py
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2868 2023-04-07 04:10:45.000000 bs_admin_utils-1.1.1/bs_admin_utils/websocket.py
-drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/PKG-INFO
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      479 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       44 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/requires.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       15 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/top_level.txt
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-15 04:03:56.000000 bs_admin_utils-1.1.1/bs_admin_utils.egg-info/zip-safe
--rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-06-15 04:03:56.375122 bs_admin_utils-1.1.1/setup.cfg
--rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      620 2023-06-15 04:01:44.000000 bs_admin_utils-1.1.1/setup.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-17 08:36:32.632758 bs_admin_utils-1.1.2/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1067 2023-04-07 03:25:03.000000 bs_admin_utils-1.1.2/LICENSE
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       35 2023-04-07 04:04:08.000000 bs_admin_utils-1.1.2/MANIFEST.in
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-17 08:36:32.632758 bs_admin_utils-1.1.2/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      206 2023-04-07 03:35:29.000000 bs_admin_utils-1.1.2/README.md
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-17 08:36:32.632758 bs_admin_utils-1.1.2/bs_admin_utils/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       13 2023-04-07 03:39:05.000000 bs_admin_utils-1.1.2/bs_admin_utils/__init__.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     4220 2023-06-15 04:01:20.000000 bs_admin_utils-1.1.2/bs_admin_utils/api.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      490 2023-04-07 04:11:32.000000 bs_admin_utils-1.1.2/bs_admin_utils/decorators.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     1098 2023-06-17 08:33:58.000000 bs_admin_utils-1.1.2/bs_admin_utils/model.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-17 08:36:32.632758 bs_admin_utils-1.1.2/bs_admin_utils/static/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)   367112 2023-04-07 03:52:07.000000 bs_admin_utils-1.1.2/bs_admin_utils/static/arial.ttf
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     6248 2023-06-14 10:45:34.000000 bs_admin_utils-1.1.2/bs_admin_utils/static/nstc.ttf
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2439 2023-06-14 10:58:06.000000 bs_admin_utils-1.1.2/bs_admin_utils/vercode.py
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)     2868 2023-04-07 04:10:45.000000 bs_admin_utils-1.1.2/bs_admin_utils/websocket.py
+drwxrwxr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)        0 2023-06-17 08:36:32.632758 bs_admin_utils-1.1.2/bs_admin_utils.egg-info/
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      260 2023-06-17 08:36:32.000000 bs_admin_utils-1.1.2/bs_admin_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)      479 2023-06-17 08:36:32.000000 bs_admin_utils-1.1.2/bs_admin_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-17 08:36:32.000000 bs_admin_utils-1.1.2/bs_admin_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       44 2023-06-17 08:36:32.000000 bs_admin_utils-1.1.2/bs_admin_utils.egg-info/requires.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       15 2023-06-17 08:36:32.000000 bs_admin_utils-1.1.2/bs_admin_utils.egg-info/top_level.txt
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)        1 2023-06-17 08:36:32.000000 bs_admin_utils-1.1.2/bs_admin_utils.egg-info/zip-safe
+-rw-rw-r--   0 kiki-kanri  (1000) kiki-kanri  (1000)       38 2023-06-17 08:36:32.632758 bs_admin_utils-1.1.2/setup.cfg
+-rwxr-xr-x   0 kiki-kanri  (1000) kiki-kanri  (1000)      620 2023-06-17 08:36:12.000000 bs_admin_utils-1.1.2/setup.py
```

### Comparing `bs_admin_utils-1.1.1/LICENSE` & `bs_admin_utils-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.1/bs_admin_utils/api.py` & `bs_admin_utils-1.1.2/bs_admin_utils/api.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.1/bs_admin_utils/model.py` & `bs_admin_utils-1.1.2/bs_admin_utils/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
     @classmethod
     async def get_or_create(cls, **kwargs):
         if model := await cls.find_one(kwargs):
             return model, False
         return await cls.create(**kwargs), True
 
+    @property
+    def strid(self):
+        return str(self.id)
+
     async def update_doc(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
         return await self.save()
 
     @classmethod
     async def update_or_create(cls, id: str, **kwargs):
```

### Comparing `bs_admin_utils-1.1.1/bs_admin_utils/static/arial.ttf` & `bs_admin_utils-1.1.2/bs_admin_utils/static/arial.ttf`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.1/bs_admin_utils/static/nstc.ttf` & `bs_admin_utils-1.1.2/bs_admin_utils/static/nstc.ttf`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.1/bs_admin_utils/vercode.py` & `bs_admin_utils-1.1.2/bs_admin_utils/vercode.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.1/bs_admin_utils/websocket.py` & `bs_admin_utils-1.1.2/bs_admin_utils/websocket.py`

 * *Files identical despite different names*

### Comparing `bs_admin_utils-1.1.1/setup.py` & `bs_admin_utils-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ],
     packages=find_packages(),
     package_data={
         'bs_admin_utils': ['*.ttf']
     },
     include_package_data=True,
     zip_safe=True,
-    version='1.1.1',
+    version='1.1.2',
     description='Blacksheep admin backend utils classes and function.',
     author='kiki-kanri',
     author_email='a470666@gmail.com',
     keywords=[],
     install_requires=[
         'beanie',
         'blacksheep',
```

