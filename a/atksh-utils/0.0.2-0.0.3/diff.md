# Comparing `tmp/atksh-utils-0.0.2.tar.gz` & `tmp/atksh-utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.0.2.tar", last modified: Sat Jun 17 02:34:38 2023, max compression
+gzip compressed data, was "atksh-utils-0.0.3.tar", last modified: Sat Jun 17 02:58:27 2023, max compression
```

## Comparing `atksh-utils-0.0.2.tar` & `atksh-utils-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.765316 atksh-utils-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.0.2/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.0.3/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.2/.gitignore` & `atksh-utils-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.2/LICENSE` & `atksh-utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.2/PKG-INFO` & `atksh-utils-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.0.2/README.md` & `atksh-utils-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.2/pyproject.toml` & `atksh-utils-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.2/src/atksh_utils/openai/api.py` & `atksh-utils-0.0.3/src/atksh_utils/openai/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 from collections import defaultdict
-from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Dict, Generator, List, Optional, Tuple
 
 from .functional import FunctionWrapper, function_info
 
 
 class OpenAI:
     """
@@ -38,21 +37,17 @@
             import openai
         self.openai = openai
         self.openai.api_key = api_key
         self.model_name = model_name
         self.temperature = temperature
         self.top_p = top_p
         self.functions: List[FunctionWrapper] = []
-        self._callback_exe = ThreadPoolExecutor(max_workers=1)
 
         self.system_prompt = "You are ChatGPT with external functions given by a user."
 
-    def __del__(self):
-        self._callback_exe.shutdown(wait=False)
-
     def set_function(self, func):
         """
         Adds a function to the list of functions that can be called by the OpenAI API.
 
         Args:
             func: The function to add.
         """
@@ -127,17 +122,17 @@
                 top_p=self.top_p,
                 stream=stream_callback is not None,
             )
 
         if stream_callback is not None:
             message = defaultdict(lambda: None)
             for chunk in response:
-                self._callback_exe.submit(stream_callback, chunk.copy())
                 delta = chunk["choices"][0]["delta"]
                 self.step(message, delta)
+                stream_callback(chunk)
             message = dict(message)
         else:
             message = response["choices"][0]["message"]
         messages.append(message)
 
         if message.get("function_call"):
             function_name = message["function_call"]["name"]
```

### Comparing `atksh-utils-0.0.2/src/atksh_utils/openai/functional.py` & `atksh-utils-0.0.3/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.2/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.0.3/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.0.2/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.0.3/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.2/tests/openai/test_api.py` & `atksh-utils-0.0.3/tests/openai/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     """
     return a + b
 
 
 def test_openai_init(openai_instance):
     assert openai_instance.model_name == "test_model"
     assert openai_instance.functions == []
-    assert openai_instance.system_prompt == "You are FunctionChatGPT."
+    assert (
+        openai_instance.system_prompt == "You are ChatGPT with external functions given by a user."
+    )
 
 
 def test_set_function(openai_instance):
     openai_instance.set_function(example_function)
     assert len(openai_instance.functions) == 1
     assert isinstance(openai_instance.functions[0], FunctionWrapper)
```

### Comparing `atksh-utils-0.0.2/tests/openai/test_functional.py` & `atksh-utils-0.0.3/tests/openai/test_functional.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 def test_extract_function_info():
     func = function_info(my_function)
     info = func.info
 
     assert info["name"] == "my_function"
     assert info["description"] == "This is a test function."
     assert info["parameters"]["type"] == "object"
-    assert info["parameters"]["properties"]["x"]["type"] == "int"
+    assert info["parameters"]["properties"]["x"]["type"] == "integer"
     assert info["parameters"]["properties"]["x"]["description"] == "An integer."
-    assert info["parameters"]["properties"]["y"]["type"] == "str"
+    assert info["parameters"]["properties"]["y"]["type"] == "string"
     assert info["parameters"]["properties"]["y"]["description"] == "A string."
-    assert info["parameters"]["properties"]["flag"]["type"] == "bool, optional"
+    assert info["parameters"]["properties"]["flag"]["type"] == "boolean"
     assert (
         info["parameters"]["properties"]["flag"]["description"] == "A boolean. Defaults to False."
     )
     assert info["parameters"]["required"] == ["x", "y"]
-    assert info["return_type"] == "float"
+    assert info["return_type"] == "number"
```

