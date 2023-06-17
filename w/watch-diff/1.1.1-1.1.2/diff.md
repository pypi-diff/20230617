# Comparing `tmp/watch-diff-1.1.1.tar.gz` & `tmp/watch-diff-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watch-diff-1.1.1.tar", last modified: Sun Mar  5 14:50:46 2023, max compression
+gzip compressed data, was "watch-diff-1.1.2.tar", last modified: Sat Jun 17 15:17:58 2023, max compression
```

## Comparing `watch-diff-1.1.1.tar` & `watch-diff-1.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-03-05 14:50:46.160310 watch-diff-1.1.1/
--rw-r--r--   0 berfr     (1000) berfr     (1000)     1086 2023-03-05 14:46:00.000000 watch-diff-1.1.1/LICENSE
--rw-r--r--   0 berfr     (1000) berfr     (1000)     2004 2023-03-05 14:50:46.160310 watch-diff-1.1.1/PKG-INFO
--rw-r--r--   0 berfr     (1000) berfr     (1000)     1654 2023-03-05 14:50:03.000000 watch-diff-1.1.1/README.md
--rw-r--r--   0 berfr     (1000) berfr     (1000)       38 2023-03-05 14:50:46.160310 watch-diff-1.1.1/setup.cfg
--rw-r--r--   0 berfr     (1000) berfr     (1000)      990 2023-03-05 14:46:00.000000 watch-diff-1.1.1/setup.py
-drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-03-05 14:50:46.157310 watch-diff-1.1.1/tests/
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     1272 2021-06-12 21:44:03.000000 watch-diff-1.1.1/tests/test_watch_diff.py
-drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-03-05 14:50:46.158310 watch-diff-1.1.1/watch_diff/
--rw-r--r--   0 berfr     (1000) berfr     (1000)      198 2023-03-05 14:50:33.000000 watch-diff-1.1.1/watch_diff/__init__.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     3112 2021-06-12 21:44:05.000000 watch-diff-1.1.1/watch_diff/__main__.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     1051 2021-06-12 21:44:05.000000 watch-diff-1.1.1/watch_diff/command.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     1477 2021-06-12 21:44:05.000000 watch-diff-1.1.1/watch_diff/diff.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     2759 2021-06-12 21:44:05.000000 watch-diff-1.1.1/watch_diff/email.py
--rw-rw-r--   0 berfr     (1000) berfr     (1000)     1353 2021-06-12 21:44:05.000000 watch-diff-1.1.1/watch_diff/format.py
-drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-03-05 14:50:46.159310 watch-diff-1.1.1/watch_diff.egg-info/
--rw-r--r--   0 berfr     (1000) berfr     (1000)     2004 2023-03-05 14:50:46.000000 watch-diff-1.1.1/watch_diff.egg-info/PKG-INFO
--rw-r--r--   0 berfr     (1000) berfr     (1000)      385 2023-03-05 14:50:46.000000 watch-diff-1.1.1/watch_diff.egg-info/SOURCES.txt
--rw-r--r--   0 berfr     (1000) berfr     (1000)        1 2023-03-05 14:50:46.000000 watch-diff-1.1.1/watch_diff.egg-info/dependency_links.txt
--rw-r--r--   0 berfr     (1000) berfr     (1000)       56 2023-03-05 14:50:46.000000 watch-diff-1.1.1/watch_diff.egg-info/entry_points.txt
--rw-r--r--   0 berfr     (1000) berfr     (1000)       78 2023-03-05 14:50:46.000000 watch-diff-1.1.1/watch_diff.egg-info/requires.txt
--rw-r--r--   0 berfr     (1000) berfr     (1000)       11 2023-03-05 14:50:46.000000 watch-diff-1.1.1/watch_diff.egg-info/top_level.txt
+drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:17:58.312111 watch-diff-1.1.2/
+-rw-r--r--   0 berfr     (1000) berfr     (1000)     1086 2023-03-05 14:46:00.000000 watch-diff-1.1.2/LICENSE
+-rw-r--r--   0 berfr     (1000) berfr     (1000)     2003 2023-06-17 15:17:58.312111 watch-diff-1.1.2/PKG-INFO
+-rw-r--r--   0 berfr     (1000) berfr     (1000)     1653 2023-06-17 15:13:15.000000 watch-diff-1.1.2/README.md
+-rw-r--r--   0 berfr     (1000) berfr     (1000)       38 2023-06-17 15:17:58.312111 watch-diff-1.1.2/setup.cfg
+-rw-r--r--   0 berfr     (1000) berfr     (1000)      990 2023-03-05 14:46:00.000000 watch-diff-1.1.2/setup.py
+drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:17:58.309111 watch-diff-1.1.2/tests/
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     1272 2021-06-12 21:44:03.000000 watch-diff-1.1.2/tests/test_watch_diff.py
+drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:17:58.310111 watch-diff-1.1.2/watch_diff/
+-rw-r--r--   0 berfr     (1000) berfr     (1000)      198 2023-06-17 15:14:10.000000 watch-diff-1.1.2/watch_diff/__init__.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     3112 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/__main__.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     1051 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/command.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     1477 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/diff.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     2759 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/email.py
+-rw-rw-r--   0 berfr     (1000) berfr     (1000)     1353 2021-06-12 21:44:05.000000 watch-diff-1.1.2/watch_diff/format.py
+drwxr-xr-x   0 berfr     (1000) berfr     (1000)        0 2023-06-17 15:17:58.312111 watch-diff-1.1.2/watch_diff.egg-info/
+-rw-r--r--   0 berfr     (1000) berfr     (1000)     2003 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/PKG-INFO
+-rw-r--r--   0 berfr     (1000) berfr     (1000)      385 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/SOURCES.txt
+-rw-r--r--   0 berfr     (1000) berfr     (1000)        1 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/dependency_links.txt
+-rw-r--r--   0 berfr     (1000) berfr     (1000)       56 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/entry_points.txt
+-rw-r--r--   0 berfr     (1000) berfr     (1000)       78 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/requires.txt
+-rw-r--r--   0 berfr     (1000) berfr     (1000)       11 2023-06-17 15:17:58.000000 watch-diff-1.1.2/watch_diff.egg-info/top_level.txt
```

### Comparing `watch-diff-1.1.1/LICENSE` & `watch-diff-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.1/PKG-INFO` & `watch-diff-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watch-diff
-Version: 1.1.1
+Version: 1.1.2
 Summary: Watch command output and get notified on changes
 Home-page: https://github.com/francisbergin/watch-diff
 Author: francisbergin
 Author-email: francisbergin.dev@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -14,30 +14,30 @@
 # watch-diff
 
 [![Main workflow](https://github.com/francisbergin/watch-diff/workflows/Main%20workflow/badge.svg)](https://github.com/francisbergin/watch-diff/actions?query=workflow%3A%22Main+workflow%22)
 [![PyPI](https://img.shields.io/pypi/v/watch-diff)](https://pypi.org/project/watch-diff)
 
 Periodically run a command and receive nice diff styled emails on output changes.
 
-See https://francisbergin.github.io/posts/watch-diff/ for more info.
+See https://francisbergin.github.io/posts/watch-diff for more info.
 
-## setup
+## Setup
 
 ```shell
 pip install watch-diff
 ```
 
-## features
+## Features
 
 - supports Python >= 3.7
 - uses only Python Standard Library
 - sends email diff in both text and html form
 - uses `Message-ID` and `In-Reply-To` to group email threads
 
-## usage
+## Usage
 
 ```console
 $ watch-diff --help
 usage: watch-diff [-h] [-v | -d] [-i SECONDS] [-r RECIPIENT] command
 
 Watch command output and get notified on changes
 
@@ -52,25 +52,25 @@
                         send email to recipient
 
 logging level:
   -v, --verbose         enable verbose output
   -d, --debug           show debugging statements
 ```
 
-## credentials
+## Credentials
 
 ```shell
 export SMTP_HOST=qwer.ty
 export SMTP_PORT=1234
 export SMTP_USER=qwer@qwer.ty
 read -s -p "SMTP_PASS: " SMTP_PASS
 export SMTP_PASS
 ```
 
-## development
+## Development
 
 ```shell
 # setup
 python3 -m venv venv && . venv/bin/activate
 
 # editable install
 pip install -e .[dev]
```

### Comparing `watch-diff-1.1.1/README.md` & `watch-diff-1.1.2/watch_diff.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,43 @@
+Metadata-Version: 2.1
+Name: watch-diff
+Version: 1.1.2
+Summary: Watch command output and get notified on changes
+Home-page: https://github.com/francisbergin/watch-diff
+Author: francisbergin
+Author-email: francisbergin.dev@gmail.com
+License: MIT
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # watch-diff
 
 [![Main workflow](https://github.com/francisbergin/watch-diff/workflows/Main%20workflow/badge.svg)](https://github.com/francisbergin/watch-diff/actions?query=workflow%3A%22Main+workflow%22)
 [![PyPI](https://img.shields.io/pypi/v/watch-diff)](https://pypi.org/project/watch-diff)
 
 Periodically run a command and receive nice diff styled emails on output changes.
 
-See https://francisbergin.github.io/posts/watch-diff/ for more info.
+See https://francisbergin.github.io/posts/watch-diff for more info.
 
-## setup
+## Setup
 
 ```shell
 pip install watch-diff
 ```
 
-## features
+## Features
 
 - supports Python >= 3.7
 - uses only Python Standard Library
 - sends email diff in both text and html form
 - uses `Message-ID` and `In-Reply-To` to group email threads
 
-## usage
+## Usage
 
 ```console
 $ watch-diff --help
 usage: watch-diff [-h] [-v | -d] [-i SECONDS] [-r RECIPIENT] command
 
 Watch command output and get notified on changes
 
@@ -39,25 +52,25 @@
                         send email to recipient
 
 logging level:
   -v, --verbose         enable verbose output
   -d, --debug           show debugging statements
 ```
 
-## credentials
+## Credentials
 
 ```shell
 export SMTP_HOST=qwer.ty
 export SMTP_PORT=1234
 export SMTP_USER=qwer@qwer.ty
 read -s -p "SMTP_PASS: " SMTP_PASS
 export SMTP_PASS
 ```
 
-## development
+## Development
 
 ```shell
 # setup
 python3 -m venv venv && . venv/bin/activate
 
 # editable install
 pip install -e .[dev]
```

### Comparing `watch-diff-1.1.1/setup.py` & `watch-diff-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.1/tests/test_watch_diff.py` & `watch-diff-1.1.2/tests/test_watch_diff.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.1/watch_diff/__main__.py` & `watch-diff-1.1.2/watch_diff/__main__.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.1/watch_diff/command.py` & `watch-diff-1.1.2/watch_diff/command.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.1/watch_diff/diff.py` & `watch-diff-1.1.2/watch_diff/diff.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.1/watch_diff/email.py` & `watch-diff-1.1.2/watch_diff/email.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.1/watch_diff/format.py` & `watch-diff-1.1.2/watch_diff/format.py`

 * *Files identical despite different names*

### Comparing `watch-diff-1.1.1/watch_diff.egg-info/PKG-INFO` & `watch-diff-1.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,30 @@
-Metadata-Version: 2.1
-Name: watch-diff
-Version: 1.1.1
-Summary: Watch command output and get notified on changes
-Home-page: https://github.com/francisbergin/watch-diff
-Author: francisbergin
-Author-email: francisbergin.dev@gmail.com
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # watch-diff
 
 [![Main workflow](https://github.com/francisbergin/watch-diff/workflows/Main%20workflow/badge.svg)](https://github.com/francisbergin/watch-diff/actions?query=workflow%3A%22Main+workflow%22)
 [![PyPI](https://img.shields.io/pypi/v/watch-diff)](https://pypi.org/project/watch-diff)
 
 Periodically run a command and receive nice diff styled emails on output changes.
 
-See https://francisbergin.github.io/posts/watch-diff/ for more info.
+See https://francisbergin.github.io/posts/watch-diff for more info.
 
-## setup
+## Setup
 
 ```shell
 pip install watch-diff
 ```
 
-## features
+## Features
 
 - supports Python >= 3.7
 - uses only Python Standard Library
 - sends email diff in both text and html form
 - uses `Message-ID` and `In-Reply-To` to group email threads
 
-## usage
+## Usage
 
 ```console
 $ watch-diff --help
 usage: watch-diff [-h] [-v | -d] [-i SECONDS] [-r RECIPIENT] command
 
 Watch command output and get notified on changes
 
@@ -52,25 +39,25 @@
                         send email to recipient
 
 logging level:
   -v, --verbose         enable verbose output
   -d, --debug           show debugging statements
 ```
 
-## credentials
+## Credentials
 
 ```shell
 export SMTP_HOST=qwer.ty
 export SMTP_PORT=1234
 export SMTP_USER=qwer@qwer.ty
 read -s -p "SMTP_PASS: " SMTP_PASS
 export SMTP_PASS
 ```
 
-## development
+## Development
 
 ```shell
 # setup
 python3 -m venv venv && . venv/bin/activate
 
 # editable install
 pip install -e .[dev]
```

