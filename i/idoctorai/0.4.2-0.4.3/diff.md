# Comparing `tmp/idoctorai-0.4.2.tar.gz` & `tmp/idoctorai-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.4.2.tar", max compression
+gzip compressed data, was "idoctorai-0.4.3.tar", max compression
```

## Comparing `idoctorai-0.4.2.tar` & `idoctorai-0.4.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.2/LICENSE
--rw-r--r--   0        0        0    19866 2023-06-16 12:09:41.726411 idoctorai-0.4.2/pandasai/__init__.py
--rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.2/pandasai/constants.py
--rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.2/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.2/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.2/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.2/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.2/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.2/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.2/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.2/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.2/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.2/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.2/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.2/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.2/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.2/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.2/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3269 2023-06-14 13:05:20.642518 idoctorai-0.4.2/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.2/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.2/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.2/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.2/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.2/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1695 2023-06-16 12:19:29.617354 idoctorai-0.4.2/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.2/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1560 2023-06-16 12:19:34.652736 idoctorai-0.4.2/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1431 2023-06-16 12:30:59.218118 idoctorai-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.2/README.md
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 idoctorai-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.4.3/LICENSE
+-rw-r--r--   0        0        0    19920 2023-06-17 01:10:51.962642 idoctorai-0.4.3/pandasai/__init__.py
+-rw-r--r--   0        0        0     1776 2023-06-07 12:25:21.034963 idoctorai-0.4.3/pandasai/constants.py
+-rw-r--r--   0        0        0     1566 2023-06-07 12:25:21.034963 idoctorai-0.4.3/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.4.3/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3898 2023-06-07 12:25:21.035961 idoctorai-0.4.3/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5529 2023-05-31 07:10:59.363572 idoctorai-0.4.3/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1898 2023-06-07 12:25:21.035961 idoctorai-0.4.3/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.4.3/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1537 2023-05-31 07:10:59.363572 idoctorai-0.4.3/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3140 2023-06-07 12:25:21.036958 idoctorai-0.4.3/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     2994 2023-06-16 09:50:05.591027 idoctorai-0.4.3/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.4.3/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4456 2023-05-31 07:10:59.365592 idoctorai-0.4.3/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    11321 2023-06-10 09:23:05.843239 idoctorai-0.4.3/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.4.3/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1913 2023-05-31 07:10:59.366593 idoctorai-0.4.3/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1535 2023-05-31 07:10:59.367662 idoctorai-0.4.3/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3271 2023-06-17 01:00:10.732858 idoctorai-0.4.3/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.4.3/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.4.3/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      764 2023-05-31 07:10:59.368559 idoctorai-0.4.3/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1876 2023-06-16 10:04:42.471079 idoctorai-0.4.3/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1381 2023-05-31 07:10:59.369581 idoctorai-0.4.3/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1695 2023-06-16 12:19:29.617354 idoctorai-0.4.3/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      528 2023-05-31 07:10:59.370561 idoctorai-0.4.3/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1560 2023-06-16 12:19:34.652736 idoctorai-0.4.3/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1431 2023-06-17 01:13:34.308981 idoctorai-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      108 2023-06-09 13:02:50.798856 idoctorai-0.4.3/README.md
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 idoctorai-0.4.3/PKG-INFO
```

### Comparing `idoctorai-0.4.2/LICENSE` & `idoctorai-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/__init__.py` & `idoctorai-0.4.3/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
                         Code generated:
                         ```
                         {code}
                         ```
                     """
                 )
 
-                self._cache.set(prompt, code)
+                
 
             if show_code and self._in_notebook:
                 self.notebook.create_new_cell(code)
 
             answer = self.run_code(
                 code,
                 data_frame,
@@ -295,14 +295,17 @@
             self.log(f"Answer: {answer}")
 
             if is_conversational_answer is None:
                 is_conversational_answer = self._is_conversational_answer
             if is_conversational_answer:
                 answer = self.conversational_answer(prompt, answer)
                 self.log(f"Conversational answer: {answer}")
+
+            ## add code to cache    
+            self._cache.set(prompt, code)
             return answer
         except Exception as exception:  # pylint: disable=broad-except
             self.last_error = str(exception)
             return (
                 "Unfortunately, I was not able to answer your question, "
                 "because of the following error:\n"
                 f"\n{exception}\n"
```

### Comparing `idoctorai-0.4.2/pandasai/constants.py` & `idoctorai-0.4.3/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/exceptions.py` & `idoctorai-0.4.3/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/helpers/_optional.py` & `idoctorai-0.4.3/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/helpers/anonymizer.py` & `idoctorai-0.4.3/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/helpers/cache.py` & `idoctorai-0.4.3/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/helpers/from_excel.py` & `idoctorai-0.4.3/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/helpers/notebook.py` & `idoctorai-0.4.3/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/helpers/save_chart.py` & `idoctorai-0.4.3/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/langchain/__init__.py` & `idoctorai-0.4.3/pandasai/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/llm/azure_openai.py` & `idoctorai-0.4.3/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/llm/base.py` & `idoctorai-0.4.3/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/llm/fake.py` & `idoctorai-0.4.3/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/llm/google_palm.py` & `idoctorai-0.4.3/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/llm/open_assistant.py` & `idoctorai-0.4.3/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/llm/openai.py` & `idoctorai-0.4.3/pandasai/llm/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         self.last_prompt = str(instruction) + str(value)
 
         if self.model in self._supported_completion_models:
             response = self.completion(str(instruction) + str(value) + suffix)
         elif self.model in self._supported_chat_models:
             # response = self.chat_completion(str(instruction) + str(value) + suffix)
             response = self.langchain_input(str(instruction) + str(value) + suffix, history)
-            print(response)
+            # print(response)
         else:
             raise UnsupportedOpenAIModelError("Unsupported model")
 
         return response
 
     @property
     def type(self) -> str:
```

### Comparing `idoctorai-0.4.2/pandasai/llm/starcoder.py` & `idoctorai-0.4.3/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/prompts/base.py` & `idoctorai-0.4.3/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.4.3/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.4.3/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/prompts/generate_python_code.py` & `idoctorai-0.4.3/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/prompts/generate_response.py` & `idoctorai-0.4.3/pandasai/prompts/generate_response.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.4.3/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.4.2/pyproject.toml` & `idoctorai-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.4.2"
+version = "0.4.3"
 description = "idoctorai"
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
```

### Comparing `idoctorai-0.4.2/PKG-INFO` & `idoctorai-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.4.2
+Version: 0.4.3
 Summary: idoctorai
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

