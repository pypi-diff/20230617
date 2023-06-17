# Comparing `tmp/pydatawork-0.0.3.tar.gz` & `tmp/pydatawork-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.0.3.tar", last modified: Thu Jun 15 10:40:13 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.0.4.tar", last modified: Sat Jun 17 09:33:41 2023, max compression
```

## Comparing `pydatawork-0.0.3.tar` & `pydatawork-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 10:40:13.000000 pydatawork-0.0.3/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      582 2023-06-15 10:40:13.000000 pydatawork-0.0.3/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       74 2023-06-15 10:00:20.000000 pydatawork-0.0.3/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      582 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-15 10:40:13.000000 pydatawork-0.0.3/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1052 2023-06-15 10:29:59.000000 pydatawork-0.0.3/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-15 10:40:13.000000 pydatawork-0.0.3/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-15 10:39:40.000000 pydatawork-0.0.3/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 09:33:41.000000 pydatawork-0.0.4/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      744 2023-06-17 09:33:41.000000 pydatawork-0.0.4/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      196 2023-06-17 09:33:33.000000 pydatawork-0.0.4/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      744 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1052 2023-06-15 10:29:59.000000 pydatawork-0.0.4/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-17 09:33:41.000000 pydatawork-0.0.4/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-17 09:32:30.000000 pydatawork-0.0.4/setup.py
```

### Comparing `pydatawork-0.0.3/PKG-INFO` & `pydatawork-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.3
+Version: 0.0.4
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
+        ###### Sat Jun 17 17:32:47 CST 2023
+        修改了导入方式，使用下面的导入方式：
+        ```shell
+        import pydatawork
+        ```
         
         ###### Thu Jun 15 13:23:43 CST 2023
         数据工作相关的分享。
```

### Comparing `pydatawork-0.0.3/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.0.4/pydatawork.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.3
+Version: 0.0.4
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description: 
         
+        ###### Sat Jun 17 17:32:47 CST 2023
+        修改了导入方式，使用下面的导入方式：
+        ```shell
+        import pydatawork
+        ```
         
         ###### Thu Jun 15 13:23:43 CST 2023
         数据工作相关的分享。
```

### Comparing `pydatawork-0.0.3/pydatawork.py` & `pydatawork-0.0.4/pydatawork.py`

 * *Files identical despite different names*

### Comparing `pydatawork-0.0.3/setup.py` & `pydatawork-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.0.3',
+    version='0.0.4',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

