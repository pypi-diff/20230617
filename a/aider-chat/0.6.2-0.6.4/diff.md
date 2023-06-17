# Comparing `tmp/aider-chat-0.6.2.tar.gz` & `tmp/aider-chat-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aider-chat-0.6.2.tar", last modified: Sat Jun 17 13:47:56 2023, max compression
+gzip compressed data, was "aider-chat-0.6.4.tar", last modified: Sat Jun 17 14:09:26 2023, max compression
```

## Comparing `aider-chat-0.6.2.tar` & `aider-chat-0.6.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.684814 aider-chat-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-17 13:47:46.000000 aider-chat-0.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 13:47:46.000000 aider-chat-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 13:47:56.684814 aider-chat-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-17 13:47:46.000000 aider-chat-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.680814 aider-chat-0.6.2/aider/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27031 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/diffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-06-17 13:47:46.000000 aider-chat-0.6.2/aider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.680814 aider-chat-0.6.2/aider_chat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 13:47:56.000000 aider-chat-0.6.2/aider_chat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-17 13:47:46.000000 aider-chat-0.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:47:56.684814 aider-chat-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-17 13:47:46.000000 aider-chat-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:56.684814 aider-chat-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_repomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-17 13:47:46.000000 aider-chat-0.6.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:09:26.562494 aider-chat-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-17 14:09:17.000000 aider-chat-0.6.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 14:09:17.000000 aider-chat-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 14:09:26.562494 aider-chat-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-06-17 14:09:17.000000 aider-chat-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:09:26.562494 aider-chat-0.6.4/aider/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27031 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-06-17 14:09:17.000000 aider-chat-0.6.4/aider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:09:26.562494 aider-chat-0.6.4/aider_chat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-06-17 14:09:26.000000 aider-chat-0.6.4/aider_chat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-17 14:09:26.000000 aider-chat-0.6.4/aider_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:09:26.000000 aider-chat-0.6.4/aider_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 14:09:26.000000 aider-chat-0.6.4/aider_chat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-17 14:09:26.000000 aider-chat-0.6.4/aider_chat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 14:09:26.000000 aider-chat-0.6.4/aider_chat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-17 14:09:17.000000 aider-chat-0.6.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:09:26.562494 aider-chat-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-17 14:09:17.000000 aider-chat-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:09:26.562494 aider-chat-0.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:09:17.000000 aider-chat-0.6.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-17 14:09:17.000000 aider-chat-0.6.4/tests/test_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-17 14:09:17.000000 aider-chat-0.6.4/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-17 14:09:17.000000 aider-chat-0.6.4/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-06-17 14:09:17.000000 aider-chat-0.6.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-17 14:09:17.000000 aider-chat-0.6.4/tests/test_repomap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-17 14:09:17.000000 aider-chat-0.6.4/tests/test_utils.py
```

### Comparing `aider-chat-0.6.2/LICENSE.txt` & `aider-chat-0.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/PKG-INFO` & `aider-chat-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.6.2
+Version: 0.6.4
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
```

### Comparing `aider-chat-0.6.2/README.md` & `aider-chat-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider/coder.py` & `aider-chat-0.6.4/aider/coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider/commands.py` & `aider-chat-0.6.4/aider/commands.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider/diffs.py` & `aider-chat-0.6.4/aider/diffs.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider/dump.py` & `aider-chat-0.6.4/aider/dump.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider/io.py` & `aider-chat-0.6.4/aider/io.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider/main.py` & `aider-chat-0.6.4/aider/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 
 import configargparse
 import git
 
-from aider import models
+from aider import models, __version__
 from aider.coder import Coder
 from aider.io import InputOutput
 
 
 def get_git_root():
     try:
         repo = git.Repo(search_parent_directories=True)
@@ -26,22 +26,26 @@
     default_config_files = [
         os.path.expanduser("~/.aider.conf.yml"),
     ]
     if git_root:
         default_config_files.insert(0, os.path.join(git_root, ".aider.conf.yml"))
 
     parser = configargparse.ArgumentParser(
-        description="aider - chat with GPT about your code",
+        description="aider is GPT powered coding in your terminal",
         add_config_file_help=True,
         default_config_files=default_config_files,
         config_file_parser_class=configargparse.YAMLConfigFileParser,
         auto_env_var_prefix="AIDER_",
     )
 
     parser.add_argument(
+        "--version", action="version", version=f"%(prog)s {__version__}", help="Show the version number and exit"
+    )
+
+    parser.add_argument(
         "-c",
         "--config",
         is_config_file=True,
         metavar="CONFIG_FILE",
         help=(
             "Specify the config file (default: search for .aider.conf.yml in git root or home"
             " directory)"
```

### Comparing `aider-chat-0.6.2/aider/models.py` & `aider-chat-0.6.4/aider/models.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider/prompts.py` & `aider-chat-0.6.4/aider/prompts.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider/repomap.py` & `aider-chat-0.6.4/aider/repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider/utils.py` & `aider-chat-0.6.4/aider/utils.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/aider_chat.egg-info/PKG-INFO` & `aider-chat-0.6.4/aider_chat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aider-chat
-Version: 0.6.2
+Version: 0.6.4
 Summary: aider is GPT powered coding in your terminal
 Home-page: https://github.com/paul-gauthier/aider
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # aider is GPT powered coding in your terminal
```

### Comparing `aider-chat-0.6.2/aider_chat.egg-info/SOURCES.txt` & `aider-chat-0.6.4/aider_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/setup.py` & `aider-chat-0.6.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import re
+
 from setuptools import find_packages, setup
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
-import re
+from aider import __version__
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
     long_description = re.sub(r"\n!\[.*\]\(.*\)", "", long_description)
     long_description = re.sub(r"\n- \[.*\]\(#.*\)", "", long_description)
 
 setup(
     name="aider-chat",
-    version="0.6.2",
+    version=__version__,
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "aider = aider.main:main",
         ],
```

### Comparing `aider-chat-0.6.2/tests/test_coder.py` & `aider-chat-0.6.4/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/tests/test_commands.py` & `aider-chat-0.6.4/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/tests/test_main.py` & `aider-chat-0.6.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/tests/test_repomap.py` & `aider-chat-0.6.4/tests/test_repomap.py`

 * *Files identical despite different names*

### Comparing `aider-chat-0.6.2/tests/test_utils.py` & `aider-chat-0.6.4/tests/test_utils.py`

 * *Files identical despite different names*

