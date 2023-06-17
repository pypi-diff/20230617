# Comparing `tmp/yid_langchain_extensions-0.3.tar.gz` & `tmp/yid_langchain_extensions-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yid_langchain_extensions-0.3.tar", last modified: Sat Jun 17 11:58:26 2023, max compression
+gzip compressed data, was "yid_langchain_extensions-0.4.1.tar", last modified: Sat Jun 17 16:20:49 2023, max compression
```

## Comparing `yid_langchain_extensions-0.3.tar` & `yid_langchain_extensions-0.4.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.993059 yid_langchain_extensions-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-17 11:58:26.993059 yid_langchain_extensions-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 11:58:26.993059 yid_langchain_extensions-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.993059 yid_langchain_extensions-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.993059 yid_langchain_extensions-0.3/yid_langchain_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/yid_langchain_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.993059 yid_langchain_extensions-0.3/yid_langchain_extensions/output_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/yid_langchain_extensions/output_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/yid_langchain_extensions/output_parser/action_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/yid_langchain_extensions/output_parser/class_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/yid_langchain_extensions/output_parser/direct_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/yid_langchain_extensions/output_parser/thoughts_json_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.993059 yid_langchain_extensions-0.3/yid_langchain_extensions/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/yid_langchain_extensions/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/yid_langchain_extensions/tools/agent_as_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 11:58:17.000000 yid_langchain_extensions-0.3/yid_langchain_extensions/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.993059 yid_langchain_extensions-0.3/yid_langchain_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-17 11:58:26.000000 yid_langchain_extensions-0.3/yid_langchain_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-17 11:58:26.000000 yid_langchain_extensions-0.3/yid_langchain_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:58:26.000000 yid_langchain_extensions-0.3/yid_langchain_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-17 11:58:26.000000 yid_langchain_extensions-0.3/yid_langchain_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-17 11:58:26.000000 yid_langchain_extensions-0.3/yid_langchain_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:49.623192 yid_langchain_extensions-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 16:20:49.623192 yid_langchain_extensions-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 16:20:49.623192 yid_langchain_extensions-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 16:20:49.000000 yid_langchain_extensions-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:49.623192 yid_langchain_extensions-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:49.623192 yid_langchain_extensions-0.4.1/yid_langchain_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:49.623192 yid_langchain_extensions-0.4.1/yid_langchain_extensions/output_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions/output_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions/output_parser/action_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions/output_parser/class_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions/output_parser/direct_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions/output_parser/thoughts_json_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:49.623192 yid_langchain_extensions-0.4.1/yid_langchain_extensions/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions/tools/agent_as_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 16:20:39.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:20:49.623192 yid_langchain_extensions-0.4.1/yid_langchain_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 16:20:49.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-17 16:20:49.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:20:49.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-17 16:20:49.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-17 16:20:49.000000 yid_langchain_extensions-0.4.1/yid_langchain_extensions.egg-info/top_level.txt
```

### Comparing `yid_langchain_extensions-0.3/LICENSE` & `yid_langchain_extensions-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.3/PKG-INFO` & `yid_langchain_extensions-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid_langchain_extensions
-Version: 0.3
+Version: 0.4.1
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.3/setup.py` & `yid_langchain_extensions-0.4.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='yid_langchain_extensions',
-    version='0.3',
+    version='0.4.1',
     author='Dmitrii Rashchenko',
     author_email='dimitree54@gmail.com',
     packages=find_packages(),
     description='Useful classes extending langchain library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/dimitree54/yid_langchain_extensions',
```

### Comparing `yid_langchain_extensions-0.3/yid_langchain_extensions/output_parser/action_parser.py` & `yid_langchain_extensions-0.4.1/yid_langchain_extensions/output_parser/action_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.3/yid_langchain_extensions/output_parser/class_parser.py` & `yid_langchain_extensions-0.4.1/yid_langchain_extensions/output_parser/class_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,21 +14,21 @@
     result = ""
     for class_index, _class in enumerate(classes):
         result += f"> {class_index}: {_class.name}. {_class.description};\n"
     return result
 
 
 def get_classes_summary(classes: List[Class]) -> str:
-    return "; ".join([f"{class_index}({_class.name})" for class_index, _class in enumerate(classes)])
+    return "; ".join([f"{class_index} ({_class.name})" for class_index, _class in enumerate(classes)])
 
 
 class ClassParser(ThoughtsJSONParser):
     extra_thoughts: List[Thought] = []
     action_thoughts: List[Thought] = [
-        Thought(name="class_index", type=int, description="The class chosen. Must be one of [{classes_summary}]"),
+        Thought(name="class_index", type="int", description="The class chosen. Must be one of [{classes_summary}]"),
     ]
 
     @property
     def thoughts(self) -> List[Thought]:
         return self.action_thoughts + self.extra_thoughts
 
     def parse(self, text: str) -> int:
```

### Comparing `yid_langchain_extensions-0.3/yid_langchain_extensions/output_parser/thoughts_json_parser.py` & `yid_langchain_extensions-0.4.1/yid_langchain_extensions/output_parser/thoughts_json_parser.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.3/yid_langchain_extensions/tools/agent_as_tool.py` & `yid_langchain_extensions-0.4.1/yid_langchain_extensions/tools/agent_as_tool.py`

 * *Files identical despite different names*

### Comparing `yid_langchain_extensions-0.3/yid_langchain_extensions.egg-info/PKG-INFO` & `yid_langchain_extensions-0.4.1/yid_langchain_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yid-langchain-extensions
-Version: 0.3
+Version: 0.4.1
 Summary: Useful classes extending langchain library
 Home-page: https://github.com/dimitree54/yid_langchain_extensions
 Author: Dmitrii Rashchenko
 Author-email: dimitree54@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yid_langchain_extensions-0.3/yid_langchain_extensions.egg-info/SOURCES.txt` & `yid_langchain_extensions-0.4.1/yid_langchain_extensions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 tests/__init__.py
+tests/test_parser.py
 yid_langchain_extensions/__init__.py
 yid_langchain_extensions.egg-info/PKG-INFO
 yid_langchain_extensions.egg-info/SOURCES.txt
 yid_langchain_extensions.egg-info/dependency_links.txt
 yid_langchain_extensions.egg-info/requires.txt
 yid_langchain_extensions.egg-info/top_level.txt
 yid_langchain_extensions/output_parser/__init__.py
```

