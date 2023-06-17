# Comparing `tmp/atksh-utils-0.0.3.tar.gz` & `tmp/atksh-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.0.3.tar", last modified: Sat Jun 17 02:58:27 2023, max compression
+gzip compressed data, was "atksh-utils-0.0.4.tar", last modified: Sat Jun 17 06:30:49 2023, max compression
```

## Comparing `atksh-utils-0.0.3.tar` & `atksh-utils-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.765316 atksh-utils-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 02:58:27.000000 atksh-utils-0.0.3/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:58:27.769316 atksh-utils-0.0.3/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-17 02:58:17.000000 atksh-utils-0.0.3/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.665572 atksh-utils-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.669572 atksh-utils-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.665572 atksh-utils-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.669572 atksh-utils-0.0.4/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/src/atksh_utils/openai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 06:30:49.000000 atksh-utils-0.0.4/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.669572 atksh-utils-0.0.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 06:30:49.673572 atksh-utils-0.0.4/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-17 06:30:39.000000 atksh-utils-0.0.4/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.0.3/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.0.4/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.3/.gitignore` & `atksh-utils-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.3/LICENSE` & `atksh-utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.3/PKG-INFO` & `atksh-utils-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.0.3/README.md` & `atksh-utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.3/pyproject.toml` & `atksh-utils-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.3/src/atksh_utils/openai/api.py` & `atksh-utils-0.0.4/src/atksh_utils/openai/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from collections import defaultdict
-from typing import Any, Dict, Generator, List, Optional, Tuple
+from typing import Any, Dict, Generator, List, Optional, Tuple, Union
 
 from .functional import FunctionWrapper, function_info
+from .prompt import generate_prompt
 
 
 class OpenAI:
     """
     A class for interacting with the OpenAI API.
 
     Args:
@@ -38,15 +39,15 @@
         self.openai = openai
         self.openai.api_key = api_key
         self.model_name = model_name
         self.temperature = temperature
         self.top_p = top_p
         self.functions: List[FunctionWrapper] = []
 
-        self.system_prompt = "You are ChatGPT with external functions given by a user."
+        self.system_prompt = generate_prompt()
 
     def set_function(self, func):
         """
         Adds a function to the list of functions that can be called by the OpenAI API.
 
         Args:
             func: The function to add.
@@ -58,22 +59,26 @@
         Returns a list of information about the functions that can be called by the OpenAI API.
 
         Returns:
             List[Dict[str, Any]]: A list of information about the functions.
         """
         return [f.info for f in self.functions]
 
-    def set_system_prompt(self, prompt: str):
+    def add_instructions(self, instructions: Union[str, List[str]]):
         """
-        Sets the system prompt for the OpenAI API.
+        Adds instructions to the system prompt.
 
         Args:
             prompt (str): The system prompt to set.
         """
-        self.system_prompt = prompt
+        if isinstance(instructions, str):
+            instructions = [instructions]
+        instructions = list(map(lambda x: x.strip(), instructions))
+        more = "\n" + "\n- ".join(instructions) + "\n"
+        self.system_prompt = generate_prompt(more)
 
     def step(self, message, delta):
         for k, v in delta.items():
             if message[k] is None:
                 message[k] = v
             elif isinstance(message[k], dict):
                 self.step(message[k], v)
```

### Comparing `atksh-utils-0.0.3/src/atksh_utils/openai/functional.py` & `atksh-utils-0.0.4/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.3/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.0.4/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.0.3/tests/openai/test_api.py` & `atksh-utils-0.0.4/tests/openai/test_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,17 +30,14 @@
     """
     return a + b
 
 
 def test_openai_init(openai_instance):
     assert openai_instance.model_name == "test_model"
     assert openai_instance.functions == []
-    assert (
-        openai_instance.system_prompt == "You are ChatGPT with external functions given by a user."
-    )
 
 
 def test_set_function(openai_instance):
     openai_instance.set_function(example_function)
     assert len(openai_instance.functions) == 1
     assert isinstance(openai_instance.functions[0], FunctionWrapper)
 
@@ -48,17 +45,17 @@
 def test_get_functions(openai_instance):
     openai_instance.set_function(example_function)
     functions = openai_instance.get_functions()
     assert len(functions) == 1
     assert functions[0]["name"] == "example_function"
 
 
-def test_set_system_prompt(openai_instance):
-    openai_instance.set_system_prompt("New system prompt.")
-    assert openai_instance.system_prompt == "New system prompt."
+def test_add_instructions(openai_instance):
+    openai_instance.add_instructions(["This is a test."])
+    assert "This is a test." in openai_instance.system_prompt
 
 
 def test_call_without_function_call(openai_instance, openai_mock):
     user_prompt = "What is the weather like today?"
     openai_mock.ChatCompletion.create.return_value = {
         "choices": [{"message": {"role": "assistant", "content": "It is sunny today."}}]
     }
```

### Comparing `atksh-utils-0.0.3/tests/openai/test_functional.py` & `atksh-utils-0.0.4/tests/openai/test_functional.py`

 * *Files identical despite different names*

