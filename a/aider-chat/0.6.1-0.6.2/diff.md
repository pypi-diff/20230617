# Comparing `tmp/aider-chat-0.6.1.tar.gz` & `tmp/aider-chat-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aider-chat-0.6.1.tar", last modified: Sat Jun 17 13:47:56 2023, max compression
+gzip compressed data, was "aider-chat-0.6.2.tar", last modified: Sat Jun 17 13:47:56 2023, max compression
```

## Comparing `aider-chat-0.6.1.tar` & `aider-chat-0.6.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.025391 aider-chat-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-17 13:47:44.000000 aider-chat-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 13:47:44.000000 aider-chat-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 13:47:56.025391 aider-chat-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-17 13:47:44.000000 aider-chat-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.025391 aider-chat-0.6.1/aider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27031 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-06-17 13:47:44.000000 aider-chat-0.6.1/aider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.025391 aider-chat-0.6.1/aider_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 13:47:55.000000 aider-chat-0.6.1/aider_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-17 13:47:55.000000 aider-chat-0.6.1/aider_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:47:55.000000 aider-chat-0.6.1/aider_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 13:47:55.000000 aider-chat-0.6.1/aider_chat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-17 13:47:55.000000 aider-chat-0.6.1/aider_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 13:47:55.000000 aider-chat-0.6.1/aider_chat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-17 13:47:44.000000 aider-chat-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:47:56.025391 aider-chat-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-17 13:47:44.000000 aider-chat-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.025391 aider-chat-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:44.000000 aider-chat-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-17 13:47:44.000000 aider-chat-0.6.1/tests/test_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-17 13:47:44.000000 aider-chat-0.6.1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-17 13:47:44.000000 aider-chat-0.6.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-17 13:47:44.000000 aider-chat-0.6.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-17 13:47:44.000000 aider-chat-0.6.1/tests/test_repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-17 13:47:44.000000 aider-chat-0.6.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.684814 aider-chat-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-17 13:47:46.000000 aider-chat-0.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 13:47:46.000000 aider-chat-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 13:47:56.684814 aider-chat-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-17 13:47:46.000000 aider-chat-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.680814 aider-chat-0.6.2/aider/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27031 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.680814 aider-chat-0.6.2/aider_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-17 13:47:46.000000 aider-chat-0.6.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:47:56.684814 aider-chat-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-17 13:47:46.000000 aider-chat-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.684814 aider-chat-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_utils.py
```

### Comparing `aider-chat-0.6.1/LICENSE.txt` & `aider-chat-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/PKG-INFO` & `aider-chat-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.6.1
+Version: 0.6.2
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
```

### Comparing `aider-chat-0.6.1/README.md` & `aider-chat-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/coder.py` & `aider-chat-0.6.2/aider/coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/commands.py` & `aider-chat-0.6.2/aider/commands.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/diffs.py` & `aider-chat-0.6.2/aider/diffs.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/dump.py` & `aider-chat-0.6.2/aider/dump.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/io.py` & `aider-chat-0.6.2/aider/io.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/main.py` & `aider-chat-0.6.2/aider/main.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/models.py` & `aider-chat-0.6.2/aider/models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/prompts.py` & `aider-chat-0.6.2/aider/prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/repomap.py` & `aider-chat-0.6.2/aider/repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider/utils.py` & `aider-chat-0.6.2/aider/utils.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/aider_chat.egg-info/PKG-INFO` & `aider-chat-0.6.2/aider_chat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.6.1
+Version: 0.6.2
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
```

### Comparing `aider-chat-0.6.1/aider_chat.egg-info/SOURCES.txt` & `aider-chat-0.6.2/aider_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/setup.py` & `aider-chat-0.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     long_description = re.sub(r"\n!\[.*\]\(.*\)", "", long_description)
     long_description = re.sub(r"\n- \[.*\]\(#.*\)", "", long_description)
 
 setup(
     name="aider-chat",
-    version="0.6.1",
+    version="0.6.2",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "aider = aider.main:main",
         ],
```

### Comparing `aider-chat-0.6.1/tests/test_coder.py` & `aider-chat-0.6.2/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/tests/test_commands.py` & `aider-chat-0.6.2/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/tests/test_main.py` & `aider-chat-0.6.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/tests/test_repomap.py` & `aider-chat-0.6.2/tests/test_repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.1/tests/test_utils.py` & `aider-chat-0.6.2/tests/test_utils.py`

 * *Files identical despite different names*

