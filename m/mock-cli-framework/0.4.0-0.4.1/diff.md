# Comparing `tmp/mock-cli-framework-0.4.0.tar.gz` & `tmp/mock-cli-framework-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock-cli-framework-0.4.0.tar", last modified: Tue Mar 14 04:03:02 2023, max compression
+gzip compressed data, was "mock-cli-framework-0.4.1.tar", last modified: Fri Jun 16 22:54:58 2023, max compression
```

## Comparing `mock-cli-framework-0.4.0.tar` & `mock-cli-framework-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-14 04:03:02.657380 mock-cli-framework-0.4.0/
--rw-r--r--   0 zach       (502) staff       (20)     1071 2020-12-02 02:55:12.000000 mock-cli-framework-0.4.0/LICENSE
--rw-r--r--   0 zach       (502) staff       (20)     9581 2023-03-14 04:03:02.657475 mock-cli-framework-0.4.0/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)     9143 2021-02-19 21:07:02.000000 mock-cli-framework-0.4.0/README.md
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-14 04:03:02.656470 mock-cli-framework-0.4.0/mock_cli/
--rw-r--r--   0 zach       (502) staff       (20)      541 2023-03-14 04:02:06.000000 mock-cli-framework-0.4.0/mock_cli/__about__.py
--rw-r--r--   0 zach       (502) staff       (20)      417 2023-03-14 03:59:29.000000 mock-cli-framework-0.4.0/mock_cli/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      147 2021-02-04 03:22:02.000000 mock-cli-framework-0.4.0/mock_cli/about.py
--rw-r--r--   0 zach       (502) staff       (20)      759 2021-02-05 21:58:29.000000 mock-cli-framework-0.4.0/mock_cli/argv_conversion.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-14 04:03:02.656748 mock-cli-framework-0.4.0/mock_cli/data/
--rw-r--r--   0 zach       (502) staff       (20)       87 2022-09-12 01:48:18.000000 mock-cli-framework-0.4.0/mock_cli/data/__init__.py
--rw-r--r--   0 zach       (502) staff       (20)      357 2023-02-17 23:11:41.000000 mock-cli-framework-0.4.0/mock_cli/hashing.py
--rw-r--r--   0 zach       (502) staff       (20)     2507 2023-03-14 04:00:13.000000 mock-cli-framework-0.4.0/mock_cli/mock_cmd.py
--rw-r--r--   0 zach       (502) staff       (20)     5494 2023-02-22 23:25:34.000000 mock-cli-framework-0.4.0/mock_cli/mock_cmd_state.py
--rw-r--r--   0 zach       (502) staff       (20)     1013 2021-02-03 00:37:32.000000 mock-cli-framework-0.4.0/mock_cli/path.py
--rw-r--r--   0 zach       (502) staff       (20)      161 2022-09-12 00:48:54.000000 mock-cli-framework-0.4.0/mock_cli/pkg_resources.py
--rw-r--r--   0 zach       (502) staff       (20)     8928 2023-03-14 03:44:06.000000 mock-cli-framework-0.4.0/mock_cli/responses.py
-drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-03-14 04:03:02.657270 mock-cli-framework-0.4.0/mock_cli_framework.egg-info/
--rw-r--r--   0 zach       (502) staff       (20)     9581 2023-03-14 04:03:02.000000 mock-cli-framework-0.4.0/mock_cli_framework.egg-info/PKG-INFO
--rw-r--r--   0 zach       (502) staff       (20)      452 2023-03-14 04:03:02.000000 mock-cli-framework-0.4.0/mock_cli_framework.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (502) staff       (20)        1 2023-03-14 04:03:02.000000 mock-cli-framework-0.4.0/mock_cli_framework.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (502) staff       (20)        9 2023-03-14 04:03:02.000000 mock-cli-framework-0.4.0/mock_cli_framework.egg-info/top_level.txt
--rw-r--r--   0 zach       (502) staff       (20)      156 2023-03-14 04:03:02.657697 mock-cli-framework-0.4.0/setup.cfg
--rw-r--r--   0 zach       (502) staff       (20)      708 2021-02-05 23:19:45.000000 mock-cli-framework-0.4.0/setup.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-16 22:54:58.964267 mock-cli-framework-0.4.1/
+-rw-r--r--   0 zach       (502) staff       (20)     1071 2020-12-02 02:55:12.000000 mock-cli-framework-0.4.1/LICENSE
+-rw-r--r--   0 zach       (502) staff       (20)     9581 2023-06-16 22:54:58.964327 mock-cli-framework-0.4.1/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)     9143 2021-02-19 21:07:02.000000 mock-cli-framework-0.4.1/README.md
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-16 22:54:58.963505 mock-cli-framework-0.4.1/mock_cli/
+-rw-r--r--   0 zach       (502) staff       (20)      541 2023-06-16 22:53:18.000000 mock-cli-framework-0.4.1/mock_cli/__about__.py
+-rw-r--r--   0 zach       (502) staff       (20)      417 2023-03-14 03:59:29.000000 mock-cli-framework-0.4.1/mock_cli/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      147 2021-02-04 03:22:02.000000 mock-cli-framework-0.4.1/mock_cli/about.py
+-rw-r--r--   0 zach       (502) staff       (20)      791 2023-06-16 22:37:28.000000 mock-cli-framework-0.4.1/mock_cli/argv_conversion.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-16 22:54:58.963641 mock-cli-framework-0.4.1/mock_cli/data/
+-rw-r--r--   0 zach       (502) staff       (20)       87 2022-09-12 01:48:18.000000 mock-cli-framework-0.4.1/mock_cli/data/__init__.py
+-rw-r--r--   0 zach       (502) staff       (20)      357 2023-02-17 23:11:41.000000 mock-cli-framework-0.4.1/mock_cli/hashing.py
+-rw-r--r--   0 zach       (502) staff       (20)     2507 2023-03-14 04:00:13.000000 mock-cli-framework-0.4.1/mock_cli/mock_cmd.py
+-rw-r--r--   0 zach       (502) staff       (20)     5494 2023-02-22 23:25:34.000000 mock-cli-framework-0.4.1/mock_cli/mock_cmd_state.py
+-rw-r--r--   0 zach       (502) staff       (20)     1013 2021-02-03 00:37:32.000000 mock-cli-framework-0.4.1/mock_cli/path.py
+-rw-r--r--   0 zach       (502) staff       (20)      161 2022-09-12 00:48:54.000000 mock-cli-framework-0.4.1/mock_cli/pkg_resources.py
+-rw-r--r--   0 zach       (502) staff       (20)     8928 2023-03-14 03:44:06.000000 mock-cli-framework-0.4.1/mock_cli/responses.py
+drwxr-xr-x   0 zach       (502) staff       (20)        0 2023-06-16 22:54:58.964144 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/
+-rw-r--r--   0 zach       (502) staff       (20)     9581 2023-06-16 22:54:58.000000 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (502) staff       (20)      452 2023-06-16 22:54:58.000000 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (502) staff       (20)        1 2023-06-16 22:54:58.000000 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (502) staff       (20)        9 2023-06-16 22:54:58.000000 mock-cli-framework-0.4.1/mock_cli_framework.egg-info/top_level.txt
+-rw-r--r--   0 zach       (502) staff       (20)      156 2023-06-16 22:54:58.964514 mock-cli-framework-0.4.1/setup.cfg
+-rw-r--r--   0 zach       (502) staff       (20)      708 2021-02-05 23:19:45.000000 mock-cli-framework-0.4.1/setup.py
```

### Comparing `mock-cli-framework-0.4.0/LICENSE` & `mock-cli-framework-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.0/PKG-INFO` & `mock-cli-framework-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-cli-framework
-Version: 0.4.0
+Version: 0.4.1
 Summary: A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests.
 Home-page: https://github.com/zcutlip/mock-cli-framework.git
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mock-cli-framework-0.4.0/README.md` & `mock-cli-framework-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.0/mock_cli/__about__.py` & `mock-cli-framework-0.4.1/mock_cli/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = "Mock CLI Framework"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __summary__ = """A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests."""
 
 """
 See PEP 440 for version scheme
 https://www.python.org/dev/peps/pep-0440/#examples-of-compliant-version-schemes
 Examples:
```

### Comparing `mock-cli-framework-0.4.0/mock_cli/mock_cmd.py` & `mock-cli-framework-0.4.1/mock_cli/mock_cmd.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.0/mock_cli/mock_cmd_state.py` & `mock-cli-framework-0.4.1/mock_cli/mock_cmd_state.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.0/mock_cli/path.py` & `mock-cli-framework-0.4.1/mock_cli/path.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.0/mock_cli/responses.py` & `mock-cli-framework-0.4.1/mock_cli/responses.py`

 * *Files identical despite different names*

### Comparing `mock-cli-framework-0.4.0/mock_cli_framework.egg-info/PKG-INFO` & `mock-cli-framework-0.4.1/mock_cli_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mock-cli-framework
-Version: 0.4.0
+Version: 0.4.1
 Summary: A framework for creating stand-ins for CLI tools that pretend to be the real thing for when "the real thing" isn't suitable, such as in automated tests.
 Home-page: https://github.com/zcutlip/mock-cli-framework.git
 Author: Zachary Cutlip
 Author-email: uid000@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mock-cli-framework-0.4.0/setup.py` & `mock-cli-framework-0.4.1/setup.py`

 * *Files identical despite different names*

