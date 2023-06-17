# Comparing `tmp/llm-0.3.tar.gz` & `tmp/llm-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-0.3.tar", last modified: Wed May 17 21:15:02 2023, max compression
+gzip compressed data, was "llm-0.4.tar", last modified: Sat Jun 17 08:47:04 2023, max compression
```

## Comparing `llm-0.3.tar` & `llm-0.4.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:15:02.527603 llm-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 21:14:47.000000 llm-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-17 21:15:02.527603 llm-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-17 21:14:47.000000 llm-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:15:02.527603 llm-0.3/llm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 21:14:47.000000 llm-0.3/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-17 21:14:47.000000 llm-0.3/llm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-17 21:14:47.000000 llm-0.3/llm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:15:02.527603 llm-0.3/llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 21:15:02.000000 llm-0.3/llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 21:15:02.527603 llm-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-17 21:14:47.000000 llm-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 21:15:02.527603 llm-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-17 21:14:47.000000 llm-0.3/tests/test_llm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:47:04.872565 llm-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-17 08:46:44.000000 llm-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-17 08:47:04.872565 llm-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-17 08:46:44.000000 llm-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:47:04.872565 llm-0.4/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-17 08:46:44.000000 llm-0.4/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 08:46:44.000000 llm-0.4/llm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13100 2023-06-17 08:46:44.000000 llm-0.4/llm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-17 08:46:44.000000 llm-0.4/llm/migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:47:04.872565 llm-0.4/llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-17 08:47:04.000000 llm-0.4/llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 08:47:04.872565 llm-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-17 08:46:44.000000 llm-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 08:47:04.872565 llm-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-17 08:46:44.000000 llm-0.4/tests/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-17 08:46:44.000000 llm-0.4/tests/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-17 08:46:44.000000 llm-0.4/tests/test_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-17 08:46:44.000000 llm-0.4/tests/test_templates.py
```

### Comparing `llm-0.3/LICENSE` & `llm-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-0.3/setup.py` & `llm-0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.3"
+VERSION = "0.4"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -16,22 +16,30 @@
     name="llm",
     description="Access large language models from the command-line",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     author="Simon Willison",
     url="https://github.com/simonw/llm",
     project_urls={
+        "Documentation": "https://llm.datasette.io/",
         "Issues": "https://github.com/simonw/llm/issues",
         "CI": "https://github.com/simonw/llm/actions",
         "Changelog": "https://github.com/simonw/llm/releases",
     },
     license="Apache License, Version 2.0",
     version=VERSION,
     packages=["llm"],
     entry_points="""
         [console_scripts]
         llm=llm.cli:cli
     """,
-    install_requires=["click", "openai", "click-default-group-wheel", "sqlite-utils"],
-    extras_require={"test": ["pytest"]},
+    install_requires=[
+        "click",
+        "openai",
+        "click-default-group-wheel",
+        "sqlite-utils",
+        "pydantic",
+        "PyYAML",
+    ],
+    extras_require={"test": ["pytest", "requests-mock"]},
     python_requires=">=3.7",
 )
```

