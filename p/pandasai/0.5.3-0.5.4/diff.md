# Comparing `tmp/pandasai-0.5.3.tar.gz` & `tmp/pandasai-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.5.3.tar", max compression
+gzip compressed data, was "pandasai-0.5.4.tar", max compression
```

## Comparing `pandasai-0.5.3.tar` & `pandasai-0.5.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1055 2023-06-15 10:45:52.718959 pandasai-0.5.3/LICENSE
--rw-r--r--   0        0        0     7123 2023-06-15 10:45:52.718959 pandasai-0.5.3/README.md
--rw-r--r--   0        0        0    20746 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/__init__.py
--rw-r--r--   0        0        0     1423 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3787 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5434 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1825 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1493 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3252 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4354 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10885 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1213 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     1828 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      841 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     1482 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2932 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      558 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      595 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      647 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1697 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1262 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1514 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1343 2023-06-15 10:45:52.726959 pandasai-0.5.3/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1636 2023-06-15 10:45:52.730959 pandasai-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     8140 1970-01-01 00:00:00.000000 pandasai-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-16 12:43:59.958135 pandasai-0.5.4/LICENSE
+-rw-r--r--   0        0        0     7123 2023-06-16 12:43:59.958135 pandasai-0.5.4/README.md
+-rw-r--r--   0        0        0    20850 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/__init__.py
+-rw-r--r--   0        0        0     1423 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3787 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5434 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1493 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3252 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4354 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10885 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1828 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      841 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1482 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2932 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      558 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      595 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1697 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1262 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1514 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1343 2023-06-16 12:43:59.962135 pandasai-0.5.4/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1636 2023-06-16 12:43:59.966135 pandasai-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     8140 1970-01-01 00:00:00.000000 pandasai-0.5.4/PKG-INFO
```

### Comparing `pandasai-0.5.3/LICENSE` & `pandasai-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/README.md` & `pandasai-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/__init__.py` & `pandasai-0.5.4/pandasai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,16 @@
         _max_retries (int, optional): max no. of tries to generate code on failure.
         Default to 3
         _is_notebook (bool, optional): Whether to run code in notebook. Default to False
         _original_instructions (dict, optional): The dict of instruction to run. Default
         to None
         last_code_generated (str, optional): Pass last Code if generated. Default to
         None
-        last_run_code (str, optional): Pass the last execution / run. Default to None
+        last_code_executed (str, optional): Pass the last execution / run. Default to
+        None
         code_output (str, optional): The code output if any. Default to None
         last_error (str, optional): Error of running code last time. Default to None
         prompt_id (str, optional): Unique ID to differentiate calls. Default to None
 
 
     Returns (str): Response to a Question related to Data
 
@@ -118,15 +119,15 @@
     _cache: Cache = Cache()
     _enable_cache: bool = True
     _prompt_id: Optional[str] = None
     _middlewares: List[Middleware] = [ChartsMiddleware()]
     _additional_dependencies: List[dict] = []
     _custom_whitelisted_dependencies: List[str] = []
     last_code_generated: Optional[str] = None
-    last_run_code: Optional[str] = None
+    last_code_executed: Optional[str] = None
     code_output: Optional[str] = None
     last_error: Optional[str] = None
 
     def __init__(
         self,
         llm=None,
         conversational=False,
@@ -231,26 +232,26 @@
             return answer
 
         instruction = GenerateResponsePrompt(question=question, answer=answer)
         return self._llm.call(instruction, "")
 
     def run(
         self,
-        data_frame: pd.DataFrame,
+        data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
         use_error_correction_framework: bool = True,
     ) -> Union[str, pd.DataFrame]:
         """
         Run the PandasAI to make Dataframes Conversational.
 
         Args:
-            data_frame (pd.Dataframe): A pandas Dataframe
+            data_frame (Union[pd.DataFrame, List[pd.DataFrame]]): A pandas Dataframe
             prompt (str): A prompt to query about the Dataframe
             is_conversational_answer (bool): Whether to return answer in conversational
             form. Default to False
             show_code (bool): To show the intermediate python code generated on the
             prompt. Default to False
             anonymize_df (bool): Running the code with Sensitive Data. Default to True
             use_error_correction_framework (bool): Turn on Error Correction mechanism.
@@ -369,15 +370,15 @@
         """
         Clears the cache of the PandasAI instance.
         """
         self._cache.clear()
 
     def __call__(
         self,
-        data_frame: pd.DataFrame,
+        data_frame: Union[pd.DataFrame, List[pd.DataFrame]],
         prompt: str,
         is_conversational_answer: bool = None,
         show_code: bool = False,
         anonymize_df: bool = True,
         use_error_correction_framework: bool = True,
     ) -> Union[str, pd.DataFrame]:
         """
@@ -510,15 +511,15 @@
 
         # Add save chart code
         if self._save_charts:
             code = add_save_chart(code, self._prompt_id, not self._verbose)
 
         # Get the code to run removing unsafe imports and df overwrites
         code_to_run = self._clean_code(code)
-        self.last_run_code = code_to_run
+        self.last_code_executed = code_to_run
         self.log(
             f"""
 Code running:
 ```
 {code_to_run}
 ```"""
         )
```

### Comparing `pandasai-0.5.3/pandasai/constants.py` & `pandasai-0.5.4/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/exceptions.py` & `pandasai-0.5.4/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/helpers/_optional.py` & `pandasai-0.5.4/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/helpers/anonymizer.py` & `pandasai-0.5.4/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/helpers/cache.py` & `pandasai-0.5.4/pandasai/helpers/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 """Cache module for caching queries."""
 import glob
 import os
 import shelve
-from os.path import dirname
+from pathlib import Path
 
 
 class Cache:
     """Cache class for caching queries. It is used to cache queries
     to save time and money.
 
     Args:
         filename (str): filename to store the cache.
     """
 
     def __init__(self, filename="cache"):
         # define cache directory and create directory if it does not exist
-        project_root = dirname(dirname(dirname(__file__)))
-        cache_dir = os.path.join(project_root, "cache")
-        if not os.path.exists(cache_dir):
-            os.makedirs(cache_dir)
+        cache_dir = os.path.join(Path.cwd(), "cache")
+        os.makedirs(cache_dir, mode=0o777, exist_ok=True)
 
         self.filepath = os.path.join(cache_dir, filename)
         self.cache = shelve.open(self.filepath)
 
     def set(self, key: str, value: str) -> None:
         """Set a key value pair in the cache.
```

### Comparing `pandasai-0.5.3/pandasai/helpers/from_excel.py` & `pandasai-0.5.4/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/helpers/notebook.py` & `pandasai-0.5.4/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/helpers/save_chart.py` & `pandasai-0.5.4/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/llm/azure_openai.py` & `pandasai-0.5.4/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/llm/base.py` & `pandasai-0.5.4/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/llm/fake.py` & `pandasai-0.5.4/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/llm/falcon.py` & `pandasai-0.5.4/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/llm/google_palm.py` & `pandasai-0.5.4/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/llm/langchain.py` & `pandasai-0.5.4/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/llm/open_assistant.py` & `pandasai-0.5.4/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/llm/openai.py` & `pandasai-0.5.4/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/llm/starcoder.py` & `pandasai-0.5.4/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/middlewares/base.py` & `pandasai-0.5.4/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/middlewares/charts.py` & `pandasai-0.5.4/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/middlewares/streamlit.py` & `pandasai-0.5.4/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/prompts/base.py` & `pandasai-0.5.4/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.5.4/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.5.4/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/prompts/generate_python_code.py` & `pandasai-0.5.4/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.5.4/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.5.3/pyproject.toml` & `pandasai-0.5.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.5.3"
+version = "0.5.4"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.5.3/PKG-INFO` & `pandasai-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.5.3
+Version: 0.5.4
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

