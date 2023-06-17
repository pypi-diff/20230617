# Comparing `tmp/CallingGPT-0.0.0.1.tar.gz` & `tmp/CallingGPT-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CallingGPT-0.0.0.1.tar", last modified: Sat Jun 17 12:22:08 2023, max compression
+gzip compressed data, was "CallingGPT-0.0.0.2.tar", last modified: Sat Jun 17 12:38:15 2023, max compression
```

## Comparing `CallingGPT-0.0.0.1.tar` & `CallingGPT-0.0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:22:08.120108 CallingGPT-0.0.0.1/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:22:08.096107 CallingGPT-0.0.0.1/CallingGPT/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:22:08.108107 CallingGPT-0.0.0.1/CallingGPT/CallingGPT.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1861 2023-06-17 12:22:08.000000 CallingGPT-0.0.0.1/CallingGPT/CallingGPT.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      395 2023-06-17 12:22:08.000000 CallingGPT-0.0.0.1/CallingGPT/CallingGPT.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-17 12:22:08.000000 CallingGPT-0.0.0.1/CallingGPT/CallingGPT.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-17 12:22:08.000000 CallingGPT-0.0.0.1/CallingGPT/CallingGPT.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-17 12:22:08.000000 CallingGPT-0.0.0.1/CallingGPT/CallingGPT.egg-info/top_level.txt
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:22:08.108107 CallingGPT-0.0.0.1/CallingGPT/cli/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      933 2023-06-17 08:44:54.000000 CallingGPT-0.0.0.1/CallingGPT/cli/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:22:08.116107 CallingGPT-0.0.0.1/CallingGPT/entities/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.1/CallingGPT/entities/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4420 2023-06-17 08:49:00.000000 CallingGPT-0.0.0.1/CallingGPT/entities/namespace.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:22:08.120108 CallingGPT-0.0.0.1/CallingGPT/session/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.1/CallingGPT/session/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2244 2023-06-17 08:49:49.000000 CallingGPT-0.0.0.1/CallingGPT/session/session.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1861 2023-06-17 12:22:08.120108 CallingGPT-0.0.0.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1497 2023-06-17 08:56:13.000000 CallingGPT-0.0.0.1/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-17 12:22:08.120108 CallingGPT-0.0.0.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      697 2023-06-17 12:21:59.000000 CallingGPT-0.0.0.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.744107 CallingGPT-0.0.0.2/CallingGPT/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.748108 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3277 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      395 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       21 2023-06-17 12:38:15.000000 CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.748108 CallingGPT-0.0.0.2/CallingGPT/cli/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      933 2023-06-17 08:44:54.000000 CallingGPT-0.0.0.2/CallingGPT/cli/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/CallingGPT/entities/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 06:09:28.000000 CallingGPT-0.0.0.2/CallingGPT/entities/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4420 2023-06-17 08:49:00.000000 CallingGPT-0.0.0.2/CallingGPT/entities/namespace.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/CallingGPT/session/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-17 07:58:52.000000 CallingGPT-0.0.0.2/CallingGPT/session/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2244 2023-06-17 08:49:49.000000 CallingGPT-0.0.0.2/CallingGPT/session/session.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3277 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2873 2023-06-17 12:37:52.000000 CallingGPT-0.0.0.2/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-17 12:38:15.752107 CallingGPT-0.0.0.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      748 2023-06-17 12:37:52.000000 CallingGPT-0.0.0.2/setup.py
```

### Comparing `CallingGPT-0.0.0.1/CallingGPT/CallingGPT.egg-info/PKG-INFO` & `CallingGPT-0.0.0.2/CallingGPT/CallingGPT.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
 
 # CallingGPT
 
 GPT's Function Calling - the proof-of-concept.  
 
 > Read this guide before you start: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
 
 ## Abstract
 
-OpenAI's GPT models provide a function calling feature, so we can easily create `ChatGPT Plugins` like tools. This repository is a proof-of-concept of the function calling feature.  
+OpenAI's GPT models provide a function calling feature, so we can easily create `ChatGPT-Plugins-like` tools. This repository is a proof-of-concept of the function calling feature.  
 In this experiment, we defined the `Plugin` as `Namespace` which contains a serial of functions. While user performing a conversation, the functions in `Namespace` will be called by the API and return the result to the user.
 
 ## Usage
 
 1. Clone this repository and install the dependencies.
 
     ```bash
@@ -60,7 +61,64 @@
 <<< Hello! I am an AI assistant here to help you. How may I assist you today?
 >>> say hello to Rock
 func<examples.greet.greet>: Hello, Rock!
 >>> and to Alice
 func<examples.greet.greet>: Hello, Alice!
 >>> 
 ```
+
+## For Code
+
+1. Install the package
+
+    ```bash
+    pip install --upgrade CallingGPT
+    ```
+
+2. Create your own functions in modules(these modules can also be used in the CLI mode)
+
+    ```python
+    # your_module_a.py
+    def func_a(prompt: str) -> str:  # Type hint of EACH argument and return value is REQUIRED.
+        """
+        The description of this func a, will be provided to the api.
+
+        Args:
+            prompt(str): The prompt of the function.
+
+        Returns:
+            The result of the function.
+        """
+        # Google style docstring is REQUIRED, it will be split into `description` and `params`(required if there are args) and `returns`(optional), `\n\n` between each part.
+        return "func_a: " + prompt
+    ```
+
+    ```python
+    # your_module_b.py
+    def adder(a: int, b: int) -> int:
+        """
+        Add two numbers.
+
+        Args:
+            a: The first number.
+            b: The second number.
+
+        Returns:
+            The sum of a and b.
+        """
+        # Type hints of args in docstring is optional.
+        return a + b
+    ```
+
+3. Call the wrapper
+
+    ```python
+    from CallingGPT.session.session import Session
+
+    import your_module_a, your_module_b
+
+    session = Session([your_module_a, your_module_b])
+
+    session.ask("your prompt")
+    ```
+
+    `Session` will automatically manage context for you.
```

### Comparing `CallingGPT-0.0.0.1/CallingGPT/cli/__init__.py` & `CallingGPT-0.0.0.2/CallingGPT/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.1/CallingGPT/entities/namespace.py` & `CallingGPT-0.0.0.2/CallingGPT/entities/namespace.py`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.1/CallingGPT/session/session.py` & `CallingGPT-0.0.0.2/CallingGPT/session/session.py`

 * *Files identical despite different names*

### Comparing `CallingGPT-0.0.0.1/PKG-INFO` & `CallingGPT-0.0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: CallingGPT
-Version: 0.0.0.1
+Version: 0.0.0.2
 Summary: GPT's function calling feature wrapper
 Home-page: https://github.com/RockChinQ/CallingGPT
 Author: RockChinQ
 Author-email: 1010553892@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
 
 # CallingGPT
 
 GPT's Function Calling - the proof-of-concept.  
 
 > Read this guide before you start: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
 
 ## Abstract
 
-OpenAI's GPT models provide a function calling feature, so we can easily create `ChatGPT Plugins` like tools. This repository is a proof-of-concept of the function calling feature.  
+OpenAI's GPT models provide a function calling feature, so we can easily create `ChatGPT-Plugins-like` tools. This repository is a proof-of-concept of the function calling feature.  
 In this experiment, we defined the `Plugin` as `Namespace` which contains a serial of functions. While user performing a conversation, the functions in `Namespace` will be called by the API and return the result to the user.
 
 ## Usage
 
 1. Clone this repository and install the dependencies.
 
     ```bash
@@ -60,7 +61,64 @@
 <<< Hello! I am an AI assistant here to help you. How may I assist you today?
 >>> say hello to Rock
 func<examples.greet.greet>: Hello, Rock!
 >>> and to Alice
 func<examples.greet.greet>: Hello, Alice!
 >>> 
 ```
+
+## For Code
+
+1. Install the package
+
+    ```bash
+    pip install --upgrade CallingGPT
+    ```
+
+2. Create your own functions in modules(these modules can also be used in the CLI mode)
+
+    ```python
+    # your_module_a.py
+    def func_a(prompt: str) -> str:  # Type hint of EACH argument and return value is REQUIRED.
+        """
+        The description of this func a, will be provided to the api.
+
+        Args:
+            prompt(str): The prompt of the function.
+
+        Returns:
+            The result of the function.
+        """
+        # Google style docstring is REQUIRED, it will be split into `description` and `params`(required if there are args) and `returns`(optional), `\n\n` between each part.
+        return "func_a: " + prompt
+    ```
+
+    ```python
+    # your_module_b.py
+    def adder(a: int, b: int) -> int:
+        """
+        Add two numbers.
+
+        Args:
+            a: The first number.
+            b: The second number.
+
+        Returns:
+            The sum of a and b.
+        """
+        # Type hints of args in docstring is optional.
+        return a + b
+    ```
+
+3. Call the wrapper
+
+    ```python
+    from CallingGPT.session.session import Session
+
+    import your_module_a, your_module_b
+
+    session = Session([your_module_a, your_module_b])
+
+    session.ask("your prompt")
+    ```
+
+    `Session` will automatically manage context for you.
```

### Comparing `CallingGPT-0.0.0.1/README.md` & `CallingGPT-0.0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 GPT's Function Calling - the proof-of-concept.  
 
 > Read this guide before you start: [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling)
 
 ## Abstract
 
-OpenAI's GPT models provide a function calling feature, so we can easily create `ChatGPT Plugins` like tools. This repository is a proof-of-concept of the function calling feature.  
+OpenAI's GPT models provide a function calling feature, so we can easily create `ChatGPT-Plugins-like` tools. This repository is a proof-of-concept of the function calling feature.  
 In this experiment, we defined the `Plugin` as `Namespace` which contains a serial of functions. While user performing a conversation, the functions in `Namespace` will be called by the API and return the result to the user.
 
 ## Usage
 
 1. Clone this repository and install the dependencies.
 
     ```bash
@@ -49,7 +49,64 @@
 <<< Hello! I am an AI assistant here to help you. How may I assist you today?
 >>> say hello to Rock
 func<examples.greet.greet>: Hello, Rock!
 >>> and to Alice
 func<examples.greet.greet>: Hello, Alice!
 >>> 
 ```
+
+## For Code
+
+1. Install the package
+
+    ```bash
+    pip install --upgrade CallingGPT
+    ```
+
+2. Create your own functions in modules(these modules can also be used in the CLI mode)
+
+    ```python
+    # your_module_a.py
+    def func_a(prompt: str) -> str:  # Type hint of EACH argument and return value is REQUIRED.
+        """
+        The description of this func a, will be provided to the api.
+
+        Args:
+            prompt(str): The prompt of the function.
+
+        Returns:
+            The result of the function.
+        """
+        # Google style docstring is REQUIRED, it will be split into `description` and `params`(required if there are args) and `returns`(optional), `\n\n` between each part.
+        return "func_a: " + prompt
+    ```
+
+    ```python
+    # your_module_b.py
+    def adder(a: int, b: int) -> int:
+        """
+        Add two numbers.
+
+        Args:
+            a: The first number.
+            b: The second number.
+
+        Returns:
+            The sum of a and b.
+        """
+        # Type hints of args in docstring is optional.
+        return a + b
+    ```
+
+3. Call the wrapper
+
+    ```python
+    from CallingGPT.session.session import Session
+
+    import your_module_a, your_module_b
+
+    session = Session([your_module_a, your_module_b])
+
+    session.ask("your prompt")
+    ```
+
+    `Session` will automatically manage context for you.
```

### Comparing `CallingGPT-0.0.0.1/setup.py` & `CallingGPT-0.0.0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CallingGPT',
-    version='0.0.0.1',
+    version='0.0.0.2',
     description="GPT's function calling feature wrapper",
     long_description=open('README.md', encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
     install_requires=[
         'openai',
     ],
     author='RockChinQ',
     author_email="1010553892@qq.com",
     url="https://github.com/RockChinQ/CallingGPT",
     classifiers=[
```

