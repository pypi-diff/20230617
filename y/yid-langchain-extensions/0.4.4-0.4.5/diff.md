# Comparing `tmp/yid_langchain_extensions-0.4.4.tar.gz` & `tmp/yid_langchain_extensions-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yid_langchain_extensions-0.4.4.tar", last modified: Sat Jun 17 17:54:37 2023, max compression
+gzip compressed data, was "yid_langchain_extensions-0.4.5.tar", last modified: Sat Jun 17 18:00:05 2023, max compression
```

## Comparing `yid_langchain_extensions-0.4.4.tar` & `yid_langchain_extensions-0.4.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:37.634940 yid_langchain_extensions-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 17:54:37.634940 yid_langchain_extensions-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 17:54:37.634940 yid_langchain_extensions-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:37.634940 yid_langchain_extensions-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/tests/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:37.634940 yid_langchain_extensions-0.4.4/yid_langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:37.634940 yid_langchain_extensions-0.4.4/yid_langchain_extensions/output_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions/output_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions/output_parser/action_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions/output_parser/class_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions/output_parser/direct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions/output_parser/thoughts_json_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:37.634940 yid_langchain_extensions-0.4.4/yid_langchain_extensions/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions/tools/agent_as_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 17:54:17.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:54:37.634940 yid_langchain_extensions-0.4.4/yid_langchain_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 17:54:37.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-17 17:54:37.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:54:37.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-17 17:54:37.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-17 17:54:37.000000 yid_langchain_extensions-0.4.4/yid_langchain_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:00:05.497006 yid_langchain_extensions-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 18:00:05.497006 yid_langchain_extensions-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 18:00:05.497006 yid_langchain_extensions-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:00:05.497006 yid_langchain_extensions-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:00:05.497006 yid_langchain_extensions-0.4.5/yid_langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:00:05.497006 yid_langchain_extensions-0.4.5/yid_langchain_extensions/output_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions/output_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions/output_parser/action_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions/output_parser/class_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions/output_parser/direct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions/output_parser/thoughts_json_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:00:05.497006 yid_langchain_extensions-0.4.5/yid_langchain_extensions/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions/tools/agent_as_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 17:59:46.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:00:05.497006 yid_langchain_extensions-0.4.5/yid_langchain_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 18:00:05.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-17 18:00:05.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:00:05.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-17 18:00:05.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-17 18:00:05.000000 yid_langchain_extensions-0.4.5/yid_langchain_extensions.egg-info/top_level.txt
```

### Comparing `yid_langchain_extensions-0.4.4/LICENSE` & `yid_langchain_extensions-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.4/PKG-INFO` & `yid_langchain_extensions-0.4.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid_langchain_extensions
-Version: 0.4.4
+Version: 0.4.5
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.4.4/setup.py` & `yid_langchain_extensions-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='yid_langchain_extensions',
-    version='0.4.4',
+    version='0.4.5',
     author='Dmitrii Rashchenko',
     author_email='dimitree54@gmail.com',
     packages=find_packages(),
     description='Useful classes extending langchain library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dimitree54/yid_langchain_extensions',
```

### Comparing `yid_langchain_extensions-0.4.4/tests/test_parser.py` & `yid_langchain_extensions-0.4.5/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.4/yid_langchain_extensions/output_parser/action_parser.py` & `yid_langchain_extensions-0.4.5/yid_langchain_extensions/output_parser/action_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.4/yid_langchain_extensions/output_parser/class_parser.py` & `yid_langchain_extensions-0.4.5/yid_langchain_extensions/output_parser/class_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.4/yid_langchain_extensions/output_parser/thoughts_json_parser.py` & `yid_langchain_extensions-0.4.5/yid_langchain_extensions/output_parser/thoughts_json_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.4/yid_langchain_extensions/tools/agent_as_tool.py` & `yid_langchain_extensions-0.4.5/yid_langchain_extensions/tools/agent_as_tool.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.4.4/yid_langchain_extensions.egg-info/PKG-INFO` & `yid_langchain_extensions-0.4.5/yid_langchain_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid-langchain-extensions
-Version: 0.4.4
+Version: 0.4.5
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.4.4/yid_langchain_extensions.egg-info/SOURCES.txt` & `yid_langchain_extensions-0.4.5/yid_langchain_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

