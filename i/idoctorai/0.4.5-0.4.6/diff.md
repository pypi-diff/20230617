# Comparing `tmp/idoctorai-0.4.5.tar.gz` & `tmp/idoctorai-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.4.5.tar", max compression
+gzip compressed data, was "idoctorai-0.4.6.tar", max compression
```

## Comparing `idoctorai-0.4.5.tar` & `idoctorai-0.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.5/LICENSE
--rw-r--r--   0        0        0    20215 2023-06-17 06:51:20.807942 idoctorai-0.4.5/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.5/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.5/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.5/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.5/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.5/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.5/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.5/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.5/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.5/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.5/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.5/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.5/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.5/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.5/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.5/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.5/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3271 2023-06-17 01:00:10.732858 idoctorai-0.4.5/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.5/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.5/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.5/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.5/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.5/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1732 2023-06-17 06:36:26.292817 idoctorai-0.4.5/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.5/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1597 2023-06-17 06:36:37.045220 idoctorai-0.4.5/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1449 2023-06-17 06:45:05.595148 idoctorai-0.4.5/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.5/README.md
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 idoctorai-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.6/LICENSE
+-rw-r--r--   0        0        0    20480 2023-06-17 07:12:56.545739 idoctorai-0.4.6/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.6/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.6/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.6/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.6/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.6/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.6/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.6/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.6/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.6/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.6/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.6/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.6/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.6/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.6/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.6/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.6/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3271 2023-06-17 01:00:10.732858 idoctorai-0.4.6/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.6/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.6/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.6/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.6/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.6/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1732 2023-06-17 06:36:26.292817 idoctorai-0.4.6/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.6/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1597 2023-06-17 06:36:37.045220 idoctorai-0.4.6/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1449 2023-06-17 07:13:58.217321 idoctorai-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.6/README.md
+-rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 idoctorai-0.4.6/PKG-INFO
```

### Comparing `idoctorai-0.4.5/LICENSE` & `idoctorai-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/__init__.py` & `idoctorai-0.4.6/pandasai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 from .prompts.correct_error_prompt import CorrectErrorPrompt
 from .prompts.correct_multiples_prompt import CorrectMultipleDataframesErrorPrompt
 from .prompts.generate_python_code import GeneratePythonCodePrompt
 from .prompts.generate_response import GenerateResponsePrompt
 from .prompts.multiple_dataframes import MultipleDataframesPrompt
 
 import toml
+import os
 
 
 # pylint: disable=too-many-instance-attributes disable=too-many-arguments
 class PandasAI:
     """
     PandasAI is a wrapper around a LLM to make dataframes conversational.
 
@@ -557,12 +558,17 @@
     def last_prompt_id(self) -> str:
         """Return the id of the last prompt that was run."""
         if self._prompt_id is None:
             raise ValueError("Pandas AI has not been run yet.")
         return self._prompt_id
     
     def output_version(self) -> str:
-        with open('pyproject.toml') as f:
-            pyproject_toml = toml.load(f)
+        # 优先从pyproject.toml.orig获取,如果不存在则从pyproject.toml获取
+        orig_file = 'pyproject.toml.orig'
+        if os.path.exists(orig_file):
+            with open(orig_file) as f:
+                pyproject_toml = toml.load(f)
+        else:
+            with open('pyproject.toml') as f:
+                pyproject_toml = toml.load(f)
         version = pyproject_toml['tool']['poetry']['version']
-        # print(version)
         return version
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `idoctorai-0.4.5/pandasai/constants.py` & `idoctorai-0.4.6/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/exceptions.py` & `idoctorai-0.4.6/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/helpers/_optional.py` & `idoctorai-0.4.6/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/helpers/anonymizer.py` & `idoctorai-0.4.6/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/helpers/cache.py` & `idoctorai-0.4.6/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/helpers/from_excel.py` & `idoctorai-0.4.6/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/helpers/notebook.py` & `idoctorai-0.4.6/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/helpers/save_chart.py` & `idoctorai-0.4.6/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/langchain/__init__.py` & `idoctorai-0.4.6/pandasai/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/llm/azure_openai.py` & `idoctorai-0.4.6/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/llm/base.py` & `idoctorai-0.4.6/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/llm/fake.py` & `idoctorai-0.4.6/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/llm/google_palm.py` & `idoctorai-0.4.6/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/llm/open_assistant.py` & `idoctorai-0.4.6/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/llm/openai.py` & `idoctorai-0.4.6/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/llm/starcoder.py` & `idoctorai-0.4.6/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/prompts/base.py` & `idoctorai-0.4.6/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.4.6/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.4.6/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/prompts/generate_python_code.py` & `idoctorai-0.4.6/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/prompts/generate_response.py` & `idoctorai-0.4.6/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.4.6/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.5/pyproject.toml` & `idoctorai-0.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.4.5"
+version = "0.4.6"
 description = "idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
```

### Comparing `idoctorai-0.4.5/PKG-INFO` & `idoctorai-0.4.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.4.5
+Version: 0.4.6
 Summary: idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

