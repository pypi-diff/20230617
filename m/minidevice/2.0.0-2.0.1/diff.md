# Comparing `tmp/minidevice-2.0.0.tar.gz` & `tmp/minidevice-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-2.0.0.tar", last modified: Sat Jun 17 06:56:59 2023, max compression
+gzip compressed data, was "minidevice-2.0.1.tar", last modified: Sat Jun 17 11:56:11 2023, max compression
```

## Comparing `minidevice-2.0.0.tar` & `minidevice-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 06:56:59.764848 minidevice-2.0.0/
--rw-rw-rw-   0        0        0     1967 2023-06-17 06:56:59.763848 minidevice-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1673 2023-06-17 06:56:51.000000 minidevice-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 06:56:59.749830 minidevice-2.0.0/minidevice/
--rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.0/minidevice/QueueUtils.py
--rw-rw-rw-   0        0        0      184 2023-06-17 06:51:06.000000 minidevice-2.0.0/minidevice/__init__.py
--rw-rw-rw-   0        0        0    20912 2023-06-17 06:49:35.000000 minidevice-2.0.0/minidevice/adb.py
--rw-rw-rw-   0        0        0    20595 2023-06-17 06:00:01.000000 minidevice-2.0.0/minidevice/images.py
--rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.0/minidevice/logger.py
--rw-rw-rw-   0        0        0    12786 2023-06-17 06:49:51.000000 minidevice-2.0.0/minidevice/minicap.py
--rw-rw-rw-   0        0        0     1678 2023-06-17 06:50:00.000000 minidevice-2.0.0/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      658 2023-06-17 06:08:54.000000 minidevice-2.0.0/minidevice/screencap.py
--rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.0/minidevice/touch.py
-drwxrwxrwx   0        0        0        0 2023-06-17 06:56:59.762831 minidevice-2.0.0/minidevice.egg-info/
--rw-rw-rw-   0        0        0     1967 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-17 06:56:59.000000 minidevice-2.0.0/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 06:56:59.764848 minidevice-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-06-17 06:47:30.000000 minidevice-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:56:11.391829 minidevice-2.0.1/
+-rw-rw-rw-   0        0        0     1967 2023-06-17 11:56:11.391829 minidevice-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1673 2023-06-17 06:56:51.000000 minidevice-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 11:56:11.375022 minidevice-2.0.1/minidevice/
+-rw-rw-rw-   0        0        0     2745 2023-06-17 11:43:36.000000 minidevice-2.0.1/minidevice/DriodCast.py
+-rw-rw-rw-   0        0        0     2178 2023-06-17 02:36:57.000000 minidevice-2.0.1/minidevice/QueueUtils.py
+-rw-rw-rw-   0        0        0      226 2023-06-17 09:14:51.000000 minidevice-2.0.1/minidevice/__init__.py
+-rw-rw-rw-   0        0        0    20907 2023-06-17 11:44:42.000000 minidevice-2.0.1/minidevice/adb.py
+-rw-rw-rw-   0        0        0    20595 2023-06-17 06:00:01.000000 minidevice-2.0.1/minidevice/images.py
+-rw-rw-rw-   0        0        0       27 2023-06-17 05:48:23.000000 minidevice-2.0.1/minidevice/logger.py
+-rw-rw-rw-   0        0        0    12786 2023-06-17 06:49:51.000000 minidevice-2.0.1/minidevice/minicap.py
+-rw-rw-rw-   0        0        0     1678 2023-06-17 06:50:00.000000 minidevice-2.0.1/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      658 2023-06-17 06:08:54.000000 minidevice-2.0.1/minidevice/screencap.py
+-rw-rw-rw-   0        0        0      267 2023-06-17 05:58:10.000000 minidevice-2.0.1/minidevice/touch.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:56:11.389820 minidevice-2.0.1/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     1967 2023-06-17 11:56:11.000000 minidevice-2.0.1/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-06-17 11:56:11.000000 minidevice-2.0.1/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 11:56:11.000000 minidevice-2.0.1/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-17 11:56:11.000000 minidevice-2.0.1/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-17 11:56:11.000000 minidevice-2.0.1/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 11:56:11.392808 minidevice-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      754 2023-06-17 11:56:06.000000 minidevice-2.0.1/setup.py
```

### Comparing `minidevice-2.0.0/PKG-INFO` & `minidevice-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.0
+Version: 2.0.1
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.0/README.md` & `minidevice-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.0/minidevice/QueueUtils.py` & `minidevice-2.0.1/minidevice/QueueUtils.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.0/minidevice/adb.py` & `minidevice-2.0.1/minidevice/adb.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,21 +23,21 @@
         """执行shell脚本语句,获取返回的源数据"""
         adb_command = [ADB_PATH]
         if self.device:
             adb_command.extend(["-s", self.device])
         adb_command.extend(command)
         try:
             process = subprocess.Popen(
-                adb_command, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL
+                adb_command, stdout=subprocess.PIPE, stderr=subprocess.PIPE
             )
             data, err = process.communicate(timeout=10)
             if process.returncode == 0:
                 return data
             else:
-                logger.error("\nADB命令执行失败\n报错信息:{}".format(err))
+                logger.error("ADB命令执行失败\n报错信息:{}".format(err))
         except FileNotFoundError:
             logger.error("ADB不存在或无法执行")
         except subprocess.TimeoutExpired:
             logger.error("ADB命令执行超时")
 
     def _run_adb_command(self, command: list):
         adb_command = [ADB_PATH]
```

### Comparing `minidevice-2.0.0/minidevice/images.py` & `minidevice-2.0.1/minidevice/images.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.0/minidevice/minicap.py` & `minidevice-2.0.1/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.0/minidevice/minitouch.py` & `minidevice-2.0.1/minidevice/minitouch.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.0/minidevice/screencap.py` & `minidevice-2.0.1/minidevice/screencap.py`

 * *Files identical despite different names*

### Comparing `minidevice-2.0.0/minidevice.egg-info/PKG-INFO` & `minidevice-2.0.1/minidevice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 2.0.0
+Version: 2.0.1
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku/minidevice
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Requires-Python: >=3
```

### Comparing `minidevice-2.0.0/setup.py` & `minidevice-2.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='2.0.0',
+      version='2.0.1',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku/minidevice',
       license='MIT',
       keywords='game',
       project_urls={},
       packages=find_packages(),
       include_package_data=True,
       install_requires=['opencv-python>=4.7.0.72',
-                        'pyminitouch>=0.3.3',],
+                        'pyminitouch>=0.3.3'
+                        ],
       python_requires='>=3'
       )
```

