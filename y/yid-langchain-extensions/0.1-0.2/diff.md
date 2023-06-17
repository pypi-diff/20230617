# Comparing `tmp/yid_langchain_extensions-0.1.tar.gz` & `tmp/yid_langchain_extensions-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yid_langchain_extensions-0.1.tar", last modified: Sat Jun 17 10:32:49 2023, max compression
+gzip compressed data, was "yid_langchain_extensions-0.2.tar", last modified: Sat Jun 17 11:02:14 2023, max compression
```

## Comparing `yid_langchain_extensions-0.1.tar` & `yid_langchain_extensions-0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 yid        (501) staff       (20)        0 2023-06-17 10:32:49.201798 yid_langchain_extensions-0.1/
--rw-r--r--   0 yid        (501) staff       (20)     1075 2023-06-13 19:23:50.000000 yid_langchain_extensions-0.1/LICENSE
--rw-r--r--   0 yid        (501) staff       (20)      561 2023-06-17 10:32:49.201665 yid_langchain_extensions-0.1/PKG-INFO
--rw-r--r--   0 yid        (501) staff       (20)      105 2023-06-17 10:19:40.000000 yid_langchain_extensions-0.1/README.md
--rw-r--r--   0 yid        (501) staff       (20)       38 2023-06-17 10:32:49.201843 yid_langchain_extensions-0.1/setup.cfg
--rw-r--r--   0 yid        (501) staff       (20)      712 2023-06-17 10:30:53.000000 yid_langchain_extensions-0.1/setup.py
-drwxr-xr-x   0 yid        (501) staff       (20)        0 2023-06-17 10:32:49.199512 yid_langchain_extensions-0.1/tests/
--rw-r--r--   0 yid        (501) staff       (20)        0 2023-06-17 10:16:28.000000 yid_langchain_extensions-0.1/tests/__init__.py
-drwxr-xr-x   0 yid        (501) staff       (20)        0 2023-06-17 10:32:49.199638 yid_langchain_extensions-0.1/yid_langchain_extensions/
--rw-r--r--   0 yid        (501) staff       (20)        0 2023-06-17 10:15:01.000000 yid_langchain_extensions-0.1/yid_langchain_extensions/__init__.py
-drwxr-xr-x   0 yid        (501) staff       (20)        0 2023-06-17 10:32:49.200759 yid_langchain_extensions-0.1/yid_langchain_extensions/output_parser/
--rw-r--r--   0 yid        (501) staff       (20)        0 2023-06-09 18:39:56.000000 yid_langchain_extensions-0.1/yid_langchain_extensions/output_parser/__init__.py
--rw-r--r--   0 yid        (501) staff       (20)      214 2023-06-17 09:48:05.000000 yid_langchain_extensions-0.1/yid_langchain_extensions/output_parser/direct_parser.py
--rw-r--r--   0 yid        (501) staff       (20)     2286 2023-06-17 10:05:17.000000 yid_langchain_extensions-0.1/yid_langchain_extensions/output_parser/thoughts_and_tools_parser.py
-drwxr-xr-x   0 yid        (501) staff       (20)        0 2023-06-17 10:32:49.201344 yid_langchain_extensions-0.1/yid_langchain_extensions/tools/
--rw-r--r--   0 yid        (501) staff       (20)        0 2023-06-09 18:40:10.000000 yid_langchain_extensions-0.1/yid_langchain_extensions/tools/__init__.py
--rw-r--r--   0 yid        (501) staff       (20)      567 2023-06-09 18:08:13.000000 yid_langchain_extensions-0.1/yid_langchain_extensions/tools/agent_as_tool.py
--rw-r--r--   0 yid        (501) staff       (20)      489 2023-06-09 18:46:10.000000 yid_langchain_extensions-0.1/yid_langchain_extensions/tools/utils.py
-drwxr-xr-x   0 yid        (501) staff       (20)        0 2023-06-17 10:32:49.200292 yid_langchain_extensions-0.1/yid_langchain_extensions.egg-info/
--rw-r--r--   0 yid        (501) staff       (20)      561 2023-06-17 10:32:49.000000 yid_langchain_extensions-0.1/yid_langchain_extensions.egg-info/PKG-INFO
--rw-r--r--   0 yid        (501) staff       (20)      626 2023-06-17 10:32:49.000000 yid_langchain_extensions-0.1/yid_langchain_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 yid        (501) staff       (20)        1 2023-06-17 10:32:49.000000 yid_langchain_extensions-0.1/yid_langchain_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 yid        (501) staff       (20)       19 2023-06-17 10:32:49.000000 yid_langchain_extensions-0.1/yid_langchain_extensions.egg-info/requires.txt
--rw-r--r--   0 yid        (501) staff       (20)       31 2023-06-17 10:32:49.000000 yid_langchain_extensions-0.1/yid_langchain_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:14.977657 yid_langchain_extensions-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-17 11:02:14.977657 yid_langchain_extensions-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 11:02:14.977657 yid_langchain_extensions-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:14.973657 yid_langchain_extensions-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:14.973657 yid_langchain_extensions-0.2/yid_langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/yid_langchain_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:14.977657 yid_langchain_extensions-0.2/yid_langchain_extensions/output_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/yid_langchain_extensions/output_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/yid_langchain_extensions/output_parser/direct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/yid_langchain_extensions/output_parser/thoughts_and_tools_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:14.977657 yid_langchain_extensions-0.2/yid_langchain_extensions/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/yid_langchain_extensions/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/yid_langchain_extensions/tools/agent_as_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 11:02:02.000000 yid_langchain_extensions-0.2/yid_langchain_extensions/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:02:14.977657 yid_langchain_extensions-0.2/yid_langchain_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-17 11:02:14.000000 yid_langchain_extensions-0.2/yid_langchain_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-17 11:02:14.000000 yid_langchain_extensions-0.2/yid_langchain_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:02:14.000000 yid_langchain_extensions-0.2/yid_langchain_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 11:02:14.000000 yid_langchain_extensions-0.2/yid_langchain_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-17 11:02:14.000000 yid_langchain_extensions-0.2/yid_langchain_extensions.egg-info/top_level.txt
```

### Comparing `yid_langchain_extensions-0.1/LICENSE` & `yid_langchain_extensions-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.1/PKG-INFO` & `yid_langchain_extensions-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid_langchain_extensions
-Version: 0.1
+Version: 0.2
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.1/setup.py` & `yid_langchain_extensions-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='yid_langchain_extensions',
-    version='0.1',
+    version='0.2',
     author='Dmitrii Rashchenko',
     author_email='dimitree54@gmail.com',
     packages=find_packages(),
     description='Useful classes extending langchain library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dimitree54/yid_langchain_extensions',
```

### Comparing `yid_langchain_extensions-0.1/yid_langchain_extensions/output_parser/thoughts_and_tools_parser.py` & `yid_langchain_extensions-0.2/yid_langchain_extensions/output_parser/thoughts_and_tools_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.1/yid_langchain_extensions/tools/agent_as_tool.py` & `yid_langchain_extensions-0.2/yid_langchain_extensions/tools/agent_as_tool.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.1/yid_langchain_extensions.egg-info/PKG-INFO` & `yid_langchain_extensions-0.2/yid_langchain_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid-langchain-extensions
-Version: 0.1
+Version: 0.2
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.1/yid_langchain_extensions.egg-info/SOURCES.txt` & `yid_langchain_extensions-0.2/yid_langchain_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

