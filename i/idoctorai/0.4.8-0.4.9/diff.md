# Comparing `tmp/idoctorai-0.4.8.tar.gz` & `tmp/idoctorai-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.4.8.tar", max compression
+gzip compressed data, was "idoctorai-0.4.9.tar", max compression
```

## Comparing `idoctorai-0.4.8.tar` & `idoctorai-0.4.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.8/LICENSE
--rw-r--r--   0        0        0    20556 2023-06-17 08:29:15.902169 idoctorai-0.4.8/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.8/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.8/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.8/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.8/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.8/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.8/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.8/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.8/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.8/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.8/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.8/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.8/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.8/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.8/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.8/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.8/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3271 2023-06-17 01:00:10.732858 idoctorai-0.4.8/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.8/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.8/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.8/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.8/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.8/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1732 2023-06-17 06:36:26.292817 idoctorai-0.4.8/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.8/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1597 2023-06-17 06:36:37.045220 idoctorai-0.4.8/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1480 2023-06-17 08:29:34.224788 idoctorai-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.8/README.md
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 idoctorai-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.9/LICENSE
+-rw-r--r--   0        0        0    20610 2023-06-17 08:34:36.128691 idoctorai-0.4.9/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.9/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.9/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.9/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.9/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.9/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.9/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.9/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.9/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.9/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.9/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.9/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.9/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.9/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.9/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.9/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.9/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3271 2023-06-17 01:00:10.732858 idoctorai-0.4.9/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.9/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.9/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.9/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.9/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.9/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1732 2023-06-17 06:36:26.292817 idoctorai-0.4.9/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.9/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1597 2023-06-17 06:36:37.045220 idoctorai-0.4.9/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1480 2023-06-17 08:34:41.459497 idoctorai-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.9/README.md
+-rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 idoctorai-0.4.9/PKG-INFO
```

### Comparing `idoctorai-0.4.8/LICENSE` & `idoctorai-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/__init__.py` & `idoctorai-0.4.9/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,12 +564,13 @@
     def output_version(self) -> str:
         # 优先从pyproject.toml.orig获取,如果不存在则从pyproject.toml获取
         orig_file = 'pyproject.toml.orig'
         if os.path.exists(orig_file):
             with open(orig_file) as f:
                 pyproject_toml = toml.load(f)
         else:
-            file_path = os.path.join(os.path.dirname(__file__), 'pyproject.toml')
+            parent_dir = os.path.dirname(os.path.dirname(__file__))
+            file_path = os.path.join(parent_dir, 'pyproject.toml')
             with open(file_path) as f:
                 pyproject_toml = toml.load(f)
         version = pyproject_toml['tool']['poetry']['version']
         return version
```

### Comparing `idoctorai-0.4.8/pandasai/constants.py` & `idoctorai-0.4.9/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/exceptions.py` & `idoctorai-0.4.9/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/helpers/_optional.py` & `idoctorai-0.4.9/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/helpers/anonymizer.py` & `idoctorai-0.4.9/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/helpers/cache.py` & `idoctorai-0.4.9/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/helpers/from_excel.py` & `idoctorai-0.4.9/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/helpers/notebook.py` & `idoctorai-0.4.9/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/helpers/save_chart.py` & `idoctorai-0.4.9/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/langchain/__init__.py` & `idoctorai-0.4.9/pandasai/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/llm/azure_openai.py` & `idoctorai-0.4.9/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/llm/base.py` & `idoctorai-0.4.9/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/llm/fake.py` & `idoctorai-0.4.9/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/llm/google_palm.py` & `idoctorai-0.4.9/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/llm/open_assistant.py` & `idoctorai-0.4.9/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/llm/openai.py` & `idoctorai-0.4.9/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/llm/starcoder.py` & `idoctorai-0.4.9/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/prompts/base.py` & `idoctorai-0.4.9/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.4.9/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.4.9/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/prompts/generate_python_code.py` & `idoctorai-0.4.9/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/prompts/generate_response.py` & `idoctorai-0.4.9/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.4.9/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.8/pyproject.toml` & `idoctorai-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.4.8"
+version = "0.4.9"
 description = "idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"},{include="pyproject.toml"}]
```

### Comparing `idoctorai-0.4.8/PKG-INFO` & `idoctorai-0.4.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.4.8
+Version: 0.4.9
 Summary: idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

