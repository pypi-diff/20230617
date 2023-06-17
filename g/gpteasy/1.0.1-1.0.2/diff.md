# Comparing `tmp/gpteasy-1.0.1.tar.gz` & `tmp/gpteasy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpteasy-1.0.1.tar", last modified: Sat Jun 17 13:37:38 2023, max compression
+gzip compressed data, was "gpteasy-1.0.2.tar", last modified: Sat Jun 17 14:06:51 2023, max compression
```

## Comparing `gpteasy-1.0.1.tar` & `gpteasy-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 13:37:38.532147 gpteasy-1.0.1/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.0.1/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 13:37:38.531856 gpteasy-1.0.1/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 13:37:30.000000 gpteasy-1.0.1/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 13:37:38.529192 gpteasy-1.0.1/gpteasy/
--rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.0.1/gpteasy/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4457 2023-06-17 13:35:36.000000 gpteasy-1.0.1/gpteasy/commands.py
--rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.0.1/gpteasy/display.py
--rw-r--r--   0 hp         (501) staff       (20)    12654 2023-06-17 13:35:36.000000 gpteasy-1.0.1/gpteasy/gpt.py
--rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.0.1/gpteasy/repl.py
--rw-r--r--   0 hp         (501) staff       (20)     3757 2023-06-16 09:08:00.000000 gpteasy-1.0.1/gpteasy/settings.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 13:37:38.531459 gpteasy-1.0.1/gpteasy.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      296 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)       52 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 13:37:38.000000 gpteasy-1.0.1/gpteasy.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)     1052 2023-06-17 13:37:30.000000 gpteasy-1.0.1/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 13:37:38.532229 gpteasy-1.0.1/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 14:06:51.134625 gpteasy-1.0.2/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-1.0.2/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 14:06:51.134264 gpteasy-1.0.2/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 14:06:42.000000 gpteasy-1.0.2/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 14:06:51.131125 gpteasy-1.0.2/gpteasy/
+-rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-1.0.2/gpteasy/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4457 2023-06-17 13:35:36.000000 gpteasy-1.0.2/gpteasy/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-1.0.2/gpteasy/display.py
+-rw-r--r--   0 hp         (501) staff       (20)    12654 2023-06-17 13:35:36.000000 gpteasy-1.0.2/gpteasy/gpt.py
+-rw-r--r--   0 hp         (501) staff       (20)     1193 2023-06-17 13:35:36.000000 gpteasy-1.0.2/gpteasy/repl.py
+-rw-r--r--   0 hp         (501) staff       (20)     3757 2023-06-16 09:08:00.000000 gpteasy-1.0.2/gpteasy/settings.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 14:06:51.133672 gpteasy-1.0.2/gpteasy.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 14:06:51.000000 gpteasy-1.0.2/gpteasy.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      296 2023-06-17 14:06:51.000000 gpteasy-1.0.2/gpteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 14:06:51.000000 gpteasy-1.0.2/gpteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      105 2023-06-17 14:06:51.000000 gpteasy-1.0.2/gpteasy.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 14:06:51.000000 gpteasy-1.0.2/gpteasy.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)     1146 2023-06-17 14:06:42.000000 gpteasy-1.0.2/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 14:06:51.134753 gpteasy-1.0.2/setup.cfg
```

### Comparing `gpteasy-1.0.1/LICENSE` & `gpteasy-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.1/PKG-INFO` & `gpteasy-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.0.1
+Current version: 1.0.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.0.1/README.md` & `gpteasy-1.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.0.1
+Current version: 1.0.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.0.1/gpteasy/commands.py` & `gpteasy-1.0.2/gpteasy/commands.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.1/gpteasy/display.py` & `gpteasy-1.0.2/gpteasy/display.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.1/gpteasy/gpt.py` & `gpteasy-1.0.2/gpteasy/gpt.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.1/gpteasy/repl.py` & `gpteasy-1.0.2/gpteasy/repl.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.1/gpteasy/settings.py` & `gpteasy-1.0.2/gpteasy/settings.py`

 * *Files identical despite different names*

### Comparing `gpteasy-1.0.1/gpteasy.egg-info/PKG-INFO` & `gpteasy-1.0.2/gpteasy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpteasy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Makes working with OpenAi's GPT API super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -38,15 +38,15 @@
 License-File: LICENSE
 
 # GPT Easy
 
 Package to make working with the OpenAI GPT API in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 1.0.1
+Current version: 1.0.2
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install gpteasy
 ~~~~
 2. Create an OpenAI acccount [here](https://platform.openai.com/))
```

### Comparing `gpteasy-1.0.1/pyproject.toml` & `gpteasy-1.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpteasy"
-version = "1.0.1"
+version = "1.0.2"
 description = "Makes working with OpenAi's GPT API super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["ChatGPT", "GPT4", "GPT3.5", "api"]
 dependencies = [
+    "openai",
+    "tenacity",
     "python-dateutil",
+    "python-dotenv",
+    "rich",
+    "tenacity",
+    "requests"
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black", "pytest", "build", "twine", "nox"]
 
 [project.urls]
```

