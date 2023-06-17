# Comparing `tmp/gorilla-cli-0.0.2.tar.gz` & `tmp/gorilla-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gorilla-cli-0.0.2.tar", last modified: Sat Jun 17 09:40:44 2023, max compression
+gzip compressed data, was "gorilla-cli-0.0.3.tar", last modified: Sat Jun 17 10:15:50 2023, max compression
```

## Comparing `gorilla-cli-0.0.2.tar` & `gorilla-cli-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 09:40:44.034073 gorilla-cli-0.0.2/
--rw-r--r--   0 shishir    (501) staff       (20)      448 2023-06-17 09:40:44.033904 gorilla-cli-0.0.2/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)     1496 2023-06-17 09:15:04.000000 gorilla-cli-0.0.2/README.md
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 09:40:44.031810 gorilla-cli-0.0.2/go_questionary/
--rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-17 08:04:28.000000 gorilla-cli-0.0.2/go_questionary/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-17 08:04:14.000000 gorilla-cli-0.0.2/go_questionary/constants.py
--rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-17 08:04:06.000000 gorilla-cli-0.0.2/go_questionary/form.py
--rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-17 08:03:53.000000 gorilla-cli-0.0.2/go_questionary/prompt.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 09:40:44.032980 gorilla-cli-0.0.2/go_questionary/prompts/
--rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-17 08:05:56.000000 gorilla-cli-0.0.2/go_questionary/prompts/__init__.py
--rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-17 08:05:47.000000 gorilla-cli-0.0.2/go_questionary/prompts/autocomplete.py
--rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-17 08:05:40.000000 gorilla-cli-0.0.2/go_questionary/prompts/checkbox.py
--rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-17 08:05:32.000000 gorilla-cli-0.0.2/go_questionary/prompts/common.py
--rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-17 08:05:20.000000 gorilla-cli-0.0.2/go_questionary/prompts/confirm.py
--rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-17 08:05:13.000000 gorilla-cli-0.0.2/go_questionary/prompts/password.py
--rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-17 08:05:05.000000 gorilla-cli-0.0.2/go_questionary/prompts/path.py
--rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-17 08:04:57.000000 gorilla-cli-0.0.2/go_questionary/prompts/rawselect.py
--rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-17 08:04:50.000000 gorilla-cli-0.0.2/go_questionary/prompts/select.py
--rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-17 08:04:41.000000 gorilla-cli-0.0.2/go_questionary/prompts/text.py
--rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-17 08:09:12.000000 gorilla-cli-0.0.2/go_questionary/question.py
--rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-17 07:49:52.000000 gorilla-cli-0.0.2/go_questionary/utils.py
--rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-17 07:49:52.000000 gorilla-cli-0.0.2/go_questionary/version.py
-drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 09:40:44.033701 gorilla-cli-0.0.2/gorilla_cli.egg-info/
--rw-r--r--   0 shishir    (501) staff       (20)      448 2023-06-17 09:40:44.000000 gorilla-cli-0.0.2/gorilla_cli.egg-info/PKG-INFO
--rw-r--r--   0 shishir    (501) staff       (20)      752 2023-06-17 09:40:44.000000 gorilla-cli-0.0.2/gorilla_cli.egg-info/SOURCES.txt
--rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-17 09:40:44.000000 gorilla-cli-0.0.2/gorilla_cli.egg-info/dependency_links.txt
--rw-r--r--   0 shishir    (501) staff       (20)       36 2023-06-17 09:40:44.000000 gorilla-cli-0.0.2/gorilla_cli.egg-info/entry_points.txt
--rw-r--r--   0 shishir    (501) staff       (20)       14 2023-06-17 09:40:44.000000 gorilla-cli-0.0.2/gorilla_cli.egg-info/requires.txt
--rw-r--r--   0 shishir    (501) staff       (20)       15 2023-06-17 09:40:44.000000 gorilla-cli-0.0.2/gorilla_cli.egg-info/top_level.txt
--rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-17 09:40:44.034189 gorilla-cli-0.0.2/setup.cfg
--rw-r--r--   0 shishir    (501) staff       (20)      728 2023-06-17 09:27:09.000000 gorilla-cli-0.0.2/setup.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 10:15:50.765204 gorilla-cli-0.0.3/
+-rw-r--r--   0 shishir    (501) staff       (20)    11357 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/LICENSE
+-rw-r--r--   0 shishir    (501) staff       (20)     2162 2023-06-17 10:15:50.765004 gorilla-cli-0.0.3/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)     1656 2023-06-17 09:55:31.000000 gorilla-cli-0.0.3/README.md
+-rw-r--r--   0 shishir    (501) staff       (20)     2623 2023-06-17 10:15:33.000000 gorilla-cli-0.0.3/go_cli.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 10:15:50.762411 gorilla-cli-0.0.3/go_questionary/
+-rw-r--r--   0 shishir    (501) staff       (20)     1442 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1674 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/constants.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3300 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/form.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7429 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompt.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 10:15:50.764070 gorilla-cli-0.0.3/go_questionary/prompts/
+-rw-r--r--   0 shishir    (501) staff       (20)      820 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/__init__.py
+-rw-r--r--   0 shishir    (501) staff       (20)     7045 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/autocomplete.py
+-rw-r--r--   0 shishir    (501) staff       (20)     9210 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/checkbox.py
+-rw-r--r--   0 shishir    (501) staff       (20)    17026 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/common.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3721 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/confirm.py
+-rw-r--r--   0 shishir    (501) staff       (20)     1999 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/password.py
+-rw-r--r--   0 shishir    (501) staff       (20)     6606 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/path.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2399 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/rawselect.py
+-rw-r--r--   0 shishir    (501) staff       (20)     8818 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/select.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3285 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/prompts/text.py
+-rw-r--r--   0 shishir    (501) staff       (20)     3982 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/question.py
+-rw-r--r--   0 shishir    (501) staff       (20)     2217 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/utils.py
+-rw-r--r--   0 shishir    (501) staff       (20)       23 2023-06-17 09:51:12.000000 gorilla-cli-0.0.3/go_questionary/version.py
+drwxr-xr-x   0 shishir    (501) staff       (20)        0 2023-06-17 10:15:50.764797 gorilla-cli-0.0.3/gorilla_cli.egg-info/
+-rw-r--r--   0 shishir    (501) staff       (20)     2162 2023-06-17 10:15:50.000000 gorilla-cli-0.0.3/gorilla_cli.egg-info/PKG-INFO
+-rw-r--r--   0 shishir    (501) staff       (20)      770 2023-06-17 10:15:50.000000 gorilla-cli-0.0.3/gorilla_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 shishir    (501) staff       (20)        1 2023-06-17 10:15:50.000000 gorilla-cli-0.0.3/gorilla_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       36 2023-06-17 10:15:50.000000 gorilla-cli-0.0.3/gorilla_cli.egg-info/entry_points.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       14 2023-06-17 10:15:50.000000 gorilla-cli-0.0.3/gorilla_cli.egg-info/requires.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       22 2023-06-17 10:15:50.000000 gorilla-cli-0.0.3/gorilla_cli.egg-info/top_level.txt
+-rw-r--r--   0 shishir    (501) staff       (20)       38 2023-06-17 10:15:50.765256 gorilla-cli-0.0.3/setup.cfg
+-rw-r--r--   0 shishir    (501) staff       (20)      879 2023-06-17 10:15:23.000000 gorilla-cli-0.0.3/setup.py
```

### Comparing `gorilla-cli-0.0.2/README.md` & `gorilla-cli-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 
 Gorilla CLI is a user-friendly command-line interface (CLI) tool that helps you to interact with your system using natural language. Just tell Gorilla CLI what you want to do, and it will suggest possible commands for you. No need to memorize complex command line arguments!
 
 ## Get Started
 
 Gorilla CLI can be installed via pip. 
 
-```
+```bash
 pip install gorilla-cli
 ```
 
 ## Usage
 
 Using Gorilla CLI is as simple as typing `go` followed by your command in plain English.
 
 For example, if you want to list all files in the current directory, simply type:
 
-```
-go I want to list all files in the current directory
+```bash
+$go I want to list all files in the current directory
 ```
 
 Gorilla CLI will then suggest possible commands, which you can select using the arrow keys and then press enter to execute the command. 
 
 ```
 🦍  Welcome to Gorilla. Use arrows to select
  » ls
    ls -l
    ls -al
 ```
 
 ## How It Works
 
-Gorilla CLI is tool that combines the power of [Gorilla LLM](https://github.com/ShishirPatil/gorilla/), and other LLMs including OpenAI's GPT-4, Claude v1, to provide a user-friendly interface to the command line. It then presents these commands to you, and you can select the one that suits your needs.
+Gorilla CLI is tool that combines the power of [Gorilla LLM](https://github.com/ShishirPatil/gorilla/), and other LLMs including OpenAI's GPT-4, Claude v1, to provide a user-friendly interface to the command line. You can now tell your command line what task you want it to execute, and it then presents a few possible commands for you to choose from and execute.
+
+Gorilla will NOT execute any command without the user explicitly executing it themselves.
 
 ## Contributions
 
 Contributions to Gorilla CLI are welcome. Please submit a pull request on GitHub if you have made improvements to the tool. 
 
 ## License
```

### Comparing `gorilla-cli-0.0.2/go_questionary/__init__.py` & `gorilla-cli-0.0.3/go_questionary/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/constants.py` & `gorilla-cli-0.0.3/go_questionary/constants.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/form.py` & `gorilla-cli-0.0.3/go_questionary/form.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompt.py` & `gorilla-cli-0.0.3/go_questionary/prompt.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/__init__.py` & `gorilla-cli-0.0.3/go_questionary/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/autocomplete.py` & `gorilla-cli-0.0.3/go_questionary/prompts/autocomplete.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/checkbox.py` & `gorilla-cli-0.0.3/go_questionary/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/common.py` & `gorilla-cli-0.0.3/go_questionary/prompts/common.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/confirm.py` & `gorilla-cli-0.0.3/go_questionary/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/password.py` & `gorilla-cli-0.0.3/go_questionary/prompts/password.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/path.py` & `gorilla-cli-0.0.3/go_questionary/prompts/path.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/rawselect.py` & `gorilla-cli-0.0.3/go_questionary/prompts/rawselect.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/select.py` & `gorilla-cli-0.0.3/go_questionary/prompts/select.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/prompts/text.py` & `gorilla-cli-0.0.3/go_questionary/prompts/text.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/question.py` & `gorilla-cli-0.0.3/go_questionary/question.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/go_questionary/utils.py` & `gorilla-cli-0.0.3/go_questionary/utils.py`

 * *Files identical despite different names*

### Comparing `gorilla-cli-0.0.2/gorilla_cli.egg-info/SOURCES.txt` & `gorilla-cli-0.0.3/gorilla_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+LICENSE
 README.md
+go_cli.py
 setup.py
 go_questionary/__init__.py
 go_questionary/constants.py
 go_questionary/form.py
 go_questionary/prompt.py
 go_questionary/question.py
 go_questionary/utils.py
```

### Comparing `gorilla-cli-0.0.2/setup.py` & `gorilla-cli-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gorilla-cli',
-    version='0.0.2',
+    version='0.0.3',
     url='https://github.com/gorilla-llm/gorilla-cli',
     author='Shishir Patil, Tianjun Zhang',
     author_email='sgp@berkeley.edu, tianjunz@berkeley.edu',
     description='LLMs for CLI',
+    long_description=open('README.md').read(),
+    long_description_content_type="text/markdown",
+    py_modules=['go_cli'],
     packages=find_packages(include=['*', 'go_questionary.*']),    
     install_requires=[
         'requests',
         'halo',
     ],
     entry_points={
         'console_scripts': [
@@ -18,9 +21,10 @@
         ],
     },
     classifiers=[  
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
+    license='Apache 2.0',
     python_requires='>=3.6',
 )
```

