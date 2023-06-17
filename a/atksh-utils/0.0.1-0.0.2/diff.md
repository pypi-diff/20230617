# Comparing `tmp/atksh-utils-0.0.1.tar.gz` & `tmp/atksh-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atksh-utils-0.0.1.tar", last modified: Sat Jun 17 01:45:46 2023, max compression
+gzip compressed data, was "atksh-utils-0.0.2.tar", last modified: Sat Jun 17 02:34:38 2023, max compression
```

## Comparing `atksh-utils-0.0.1.tar` & `atksh-utils-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:46.699148 atksh-utils-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:46.695148 atksh-utils-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:46.695148 atksh-utils-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/.github/workflows/publish_to_pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 01:45:46.699148 atksh-utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 01:45:46.699148 atksh-utils-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:46.695148 atksh-utils-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:46.695148 atksh-utils-0.0.1/src/atksh_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/src/atksh_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:46.699148 atksh-utils-0.0.1/src/atksh_utils/openai/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/src/atksh_utils/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/src/atksh_utils/openai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/src/atksh_utils/openai/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 01:45:46.000000 atksh-utils-0.0.1/src/atksh_utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:46.699148 atksh-utils-0.0.1/src/atksh_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 01:45:46.000000 atksh-utils-0.0.1/src/atksh_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-17 01:45:46.000000 atksh-utils-0.0.1/src/atksh_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:45:46.000000 atksh-utils-0.0.1/src/atksh_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 01:45:46.000000 atksh-utils-0.0.1/src/atksh_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 01:45:46.000000 atksh-utils-0.0.1/src/atksh_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:46.695148 atksh-utils-0.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:45:46.699148 atksh-utils-0.0.1/tests/openai/
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/tests/openai/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-17 01:45:36.000000 atksh-utils-0.0.1/tests/openai/test_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/.github/workflows/publish_to_pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/src/atksh_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/src/atksh_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/src/atksh_utils/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/src/atksh_utils/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/src/atksh_utils/openai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/src/atksh_utils/openai/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/src/atksh_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 02:34:38.000000 atksh-utils-0.0.2/src/atksh_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:34:38.168233 atksh-utils-0.0.2/tests/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/tests/openai/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-17 02:34:24.000000 atksh-utils-0.0.2/tests/openai/test_functional.py
```

### Comparing `atksh-utils-0.0.1/.github/workflows/publish_to_pypi.yaml` & `atksh-utils-0.0.2/.github/workflows/publish_to_pypi.yaml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.1/.gitignore` & `atksh-utils-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.1/LICENSE` & `atksh-utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.1/PKG-INFO` & `atksh-utils-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.0.1/README.md` & `atksh-utils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.1/pyproject.toml` & `atksh-utils-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.1/src/atksh_utils/openai/functional.py` & `atksh-utils-0.0.2/src/atksh_utils/openai/functional.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.1/src/atksh_utils.egg-info/PKG-INFO` & `atksh-utils-0.0.2/src/atksh_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atksh-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: atksh's utils
 Home-page: https://github.com/atksh/atksh_utils
 Author: atksh
 License: MIT License
         
         Copyright (c) 2023 atksh
```

### Comparing `atksh-utils-0.0.1/src/atksh_utils.egg-info/SOURCES.txt` & `atksh-utils-0.0.2/src/atksh_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.1/tests/openai/test_api.py` & `atksh-utils-0.0.2/tests/openai/test_api.py`

 * *Files identical despite different names*

### Comparing `atksh-utils-0.0.1/tests/openai/test_functional.py` & `atksh-utils-0.0.2/tests/openai/test_functional.py`

 * *Files identical despite different names*

