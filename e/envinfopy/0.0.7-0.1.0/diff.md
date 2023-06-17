# Comparing `tmp/envinfopy-0.0.7.tar.gz` & `tmp/envinfopy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/envinfopy-0.0.7.tar", last modified: Sun Jun 13 14:59:35 2021, max compression
+gzip compressed data, was "envinfopy-0.1.0.tar", last modified: Sat Jun 17 16:19:40 2023, max compression
```

## Comparing `envinfopy-0.0.7.tar` & `envinfopy-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-13 14:59:35.232534 envinfopy-0.0.7/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:13:59.000000 envinfopy-0.0.7/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      222 2021-03-20 04:13:59.000000 envinfopy-0.0.7/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     4719 2021-06-13 14:59:35.232534 envinfopy-0.0.7/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     3149 2021-06-13 14:52:17.000000 envinfopy-0.0.7/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-13 14:59:35.232534 envinfopy-0.0.7/envinfopy/
--rw-r--r--   0 toor      (1000) toor      (1000)     4289 2021-06-13 14:34:07.000000 envinfopy-0.0.7/envinfopy/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1158 2021-06-13 14:49:07.000000 envinfopy-0.0.7/envinfopy/__main__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2021-06-13 13:48:35.000000 envinfopy-0.0.7/envinfopy/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:13:59.000000 envinfopy-0.0.7/envinfopy/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-13 14:59:35.232534 envinfopy-0.0.7/envinfopy.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     4719 2021-06-13 14:59:35.000000 envinfopy-0.0.7/envinfopy.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      451 2021-06-13 14:59:35.000000 envinfopy-0.0.7/envinfopy.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2021-06-13 14:59:35.000000 envinfopy-0.0.7/envinfopy.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2021-06-13 14:59:22.000000 envinfopy-0.0.7/envinfopy.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      221 2021-06-13 14:59:35.000000 envinfopy-0.0.7/envinfopy.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       10 2021-06-13 14:59:35.000000 envinfopy-0.0.7/envinfopy.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1108 2021-06-13 13:46:58.000000 envinfopy-0.0.7/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-13 14:59:35.232534 envinfopy-0.0.7/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:13:59.000000 envinfopy-0.0.7/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       82 2021-03-20 04:13:59.000000 envinfopy-0.0.7/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2021-06-13 14:59:35.232534 envinfopy-0.0.7/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2981 2021-06-02 13:01:00.000000 envinfopy-0.0.7/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2021-06-13 14:59:35.232534 envinfopy-0.0.7/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)      886 2021-06-13 13:58:39.000000 envinfopy-0.0.7/tests/test_cli.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2979 2021-06-13 14:33:04.000000 envinfopy-0.0.7/tests/test_envinfo.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1065 2021-06-13 14:33:18.000000 envinfopy-0.0.7/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:13:59.000000 envinfopy-0.1.0/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      222 2021-03-20 04:13:59.000000 envinfopy-0.1.0/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     5190 2023-06-17 16:19:40.261482 envinfopy-0.1.0/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     3600 2023-06-17 15:53:45.000000 envinfopy-0.1.0/README.rst
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/envinfopy/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5568 2023-06-17 11:43:43.000000 envinfopy-0.1.0/envinfopy/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1145 2023-06-17 11:04:59.000000 envinfopy-0.1.0/envinfopy/__main__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-06-17 11:46:07.000000 envinfopy-0.1.0/envinfopy/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      392 2023-06-17 11:40:05.000000 envinfopy-0.1.0/envinfopy/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:13:59.000000 envinfopy-0.1.0/envinfopy/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/envinfopy.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5190 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      471 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-06-17 16:19:21.000000 envinfopy-0.1.0/envinfopy.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)      314 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       10 2023-06-17 16:19:40.000000 envinfopy-0.1.0/envinfopy.egg-info/top_level.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1205 2023-06-17 09:03:58.000000 envinfopy-0.1.0/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:13:59.000000 envinfopy-0.1.0/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       79 2023-06-17 05:03:58.000000 envinfopy-0.1.0/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-06-17 16:19:40.261482 envinfopy-0.1.0/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     3121 2023-06-17 15:49:42.000000 envinfopy-0.1.0/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-06-17 16:19:40.261482 envinfopy-0.1.0/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)      878 2023-06-17 04:56:36.000000 envinfopy-0.1.0/tests/test_cli.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3747 2023-06-17 10:04:15.000000 envinfopy-0.1.0/tests/test_envinfo.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      954 2023-06-17 16:19:08.000000 envinfopy-0.1.0/tox.ini
```

### Comparing `envinfopy-0.0.7/LICENSE` & `envinfopy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `envinfopy-0.0.7/PKG-INFO` & `envinfopy-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: envinfopy
-Version: 0.0.7
+Version: 0.1.0
 Summary: envinfopy is a Python Library to get execution environment information.
 Home-page: https://github.com/thombashi/envinfopy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/envinfopy
 Project-URL: Tracker, https://github.com/thombashi/envinfopy/issues
 Keywords: environment,uname,version,markdown
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Terminals
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: all
+Provides-Extra: cli
+Provides-Extra: dev
 Provides-Extra: distro
 Provides-Extra: markdown
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **envinfopy**
    :backlinks: top
@@ -66,77 +67,86 @@
 envinfopy is a Python Library to get execution environment information.
 
 
 Installation
 ============================================
 ::
 
-    pip3 install envinfopy
+    python3 -m pip install envinfopy
 
 
 Usage
 ============================================
 
 Library usage
 --------------------------------------------
+
+Get execution environment information as a dictionary:
+
+.. code-block:: python
+
+    >>> import envinfopy
+    >>> envinfopy.get_envinfo()
+    {'uname': 'Linux', 'python_implementation': 'CPython', 'python_version': '3.11.4', 'platform': 'Ubuntu 22.04.2 LTS'}
+
+Get execution environment information and specific package version information:
+
 .. code-block:: python
 
     >>> import envinfopy
     >>> envinfopy.get_envinfo(["envinfopy"])
-    {'uname': 'Linux', 'python_implementation': 'CPython', 'python_version': '3.8.5', 'platform': 'Ubuntu 18.04', 'envinfopy': '0.0.4'}
+    {'uname': 'Linux', 'python_implementation': 'CPython', 'python_version': '3.11.4', 'platform': 'Ubuntu 22.04.2 LTS', 'envinfopy': '0.1.0'}
 
 Get environment information as Markdown:
 
 ::
 
-    pip3 install envinfopy[all]  # install optional dependencies
+    python3 -m pip install envinfopy[markdown]  # install optional dependencies
 
 .. code-block:: python
 
     >>> import envinfopy
     >>> print(envinfopy.dumps(["envinfopy"], format="markdown"))
-    |  Module   |    Version    |
-    | --------- | ------------- |
-    | uname     | Linux         |
-    | Python    | CPython 3.8.5 |
-    | platform  | Ubuntu 18.04  |
-    | envinfopy | 0.0.4         |
+    |  Module   |      Version       |
+    | --------- | ------------------ |
+    | uname     | Linux              |
+    | Python    | CPython 3.11.4     |
+    | platform  | Ubuntu 22.04.2 LTS |
+    | envinfopy | 0.1.0              |
 
 CLI usage
 --------------------------------------------
 ::
 
-    $ pip3 install envinfopy[all]  # install optional dependencies
+    $ python3 -m install envinfopy[cli]  # install optional dependencies
 
     $ python3 -m envinfopy envinfopy setuptools --format markdown
-    |   Module   |              Version              |
-    | ---------- | --------------------------------- |
-    | uname      | Linux 4.19.104-microsoft-standard |
-    | Python     | CPython 3.8.5                     |
-    | platform   | Ubuntu 18.04                      |
-    | envinfopy  | 0.0.4                             |
-    | setuptools | 57.0.0                            |
+    |   Module   |                 Version                 |
+    | ---------- | --------------------------------------- |
+    | uname      | Linux 5.15.90.1-microsoft-standard-WSL2 |
+    | Python     | CPython 3.11.4                          |
+    | platform   | Ubuntu 22.04.2 LTS                      |
+    | envinfopy  | 0.0.7                                   |
+    | setuptools | 67.8.0                                  |
 
 Command help
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 ::
 
-    usage: __main__.py [-h] [-V] [-v] [--format {text,markdown,json,itemize}] packages [packages ...]
+    usage: __main__.py [-h] [-V] [-v] [--format {text,markdown,md,json,itemize}] packages [packages ...]
 
     positional arguments:
-      packages              package names to extract versions
+      packages              PyPI package names to extract versions
 
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       -V, --version         show program's version number and exit
       -v, --verbose
-      --format {text,markdown,json,itemize}
+      --format {text,markdown,md,json,itemize}
                             output format
 
     Issue tracker: https://github.com/thombashi/envinfopy/issues
 
 
 Dependencies
 ============================================
-Python 3.6+
-
-
+Python 3.7+
```

### Comparing `envinfopy-0.0.7/README.rst` & `envinfopy-0.1.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -28,75 +28,86 @@
 envinfopy is a Python Library to get execution environment information.
 
 
 Installation
 ============================================
 ::
 
-    pip3 install envinfopy
+    python3 -m pip install envinfopy
 
 
 Usage
 ============================================
 
 Library usage
 --------------------------------------------
+
+Get execution environment information as a dictionary:
+
+.. code-block:: python
+
+    >>> import envinfopy
+    >>> envinfopy.get_envinfo()
+    {'uname': 'Linux', 'python_implementation': 'CPython', 'python_version': '3.11.4', 'platform': 'Ubuntu 22.04.2 LTS'}
+
+Get execution environment information and specific package version information:
+
 .. code-block:: python
 
     >>> import envinfopy
     >>> envinfopy.get_envinfo(["envinfopy"])
-    {'uname': 'Linux', 'python_implementation': 'CPython', 'python_version': '3.8.5', 'platform': 'Ubuntu 18.04', 'envinfopy': '0.0.4'}
+    {'uname': 'Linux', 'python_implementation': 'CPython', 'python_version': '3.11.4', 'platform': 'Ubuntu 22.04.2 LTS', 'envinfopy': '0.1.0'}
 
 Get environment information as Markdown:
 
 ::
 
-    pip3 install envinfopy[all]  # install optional dependencies
+    python3 -m pip install envinfopy[markdown]  # install optional dependencies
 
 .. code-block:: python
 
     >>> import envinfopy
     >>> print(envinfopy.dumps(["envinfopy"], format="markdown"))
-    |  Module   |    Version    |
-    | --------- | ------------- |
-    | uname     | Linux         |
-    | Python    | CPython 3.8.5 |
-    | platform  | Ubuntu 18.04  |
-    | envinfopy | 0.0.4         |
+    |  Module   |      Version       |
+    | --------- | ------------------ |
+    | uname     | Linux              |
+    | Python    | CPython 3.11.4     |
+    | platform  | Ubuntu 22.04.2 LTS |
+    | envinfopy | 0.1.0              |
 
 CLI usage
 --------------------------------------------
 ::
 
-    $ pip3 install envinfopy[all]  # install optional dependencies
+    $ python3 -m install envinfopy[cli]  # install optional dependencies
 
     $ python3 -m envinfopy envinfopy setuptools --format markdown
-    |   Module   |              Version              |
-    | ---------- | --------------------------------- |
-    | uname      | Linux 4.19.104-microsoft-standard |
-    | Python     | CPython 3.8.5                     |
-    | platform   | Ubuntu 18.04                      |
-    | envinfopy  | 0.0.4                             |
-    | setuptools | 57.0.0                            |
+    |   Module   |                 Version                 |
+    | ---------- | --------------------------------------- |
+    | uname      | Linux 5.15.90.1-microsoft-standard-WSL2 |
+    | Python     | CPython 3.11.4                          |
+    | platform   | Ubuntu 22.04.2 LTS                      |
+    | envinfopy  | 0.0.7                                   |
+    | setuptools | 67.8.0                                  |
 
 Command help
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 ::
 
-    usage: __main__.py [-h] [-V] [-v] [--format {text,markdown,json,itemize}] packages [packages ...]
+    usage: __main__.py [-h] [-V] [-v] [--format {text,markdown,md,json,itemize}] packages [packages ...]
 
     positional arguments:
-      packages              package names to extract versions
+      packages              PyPI package names to extract versions
 
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       -V, --version         show program's version number and exit
       -v, --verbose
-      --format {text,markdown,json,itemize}
+      --format {text,markdown,md,json,itemize}
                             output format
 
     Issue tracker: https://github.com/thombashi/envinfopy/issues
 
 
 Dependencies
 ============================================
-Python 3.6+
+Python 3.7+
```

### Comparing `envinfopy-0.0.7/envinfopy/__main__.py` & `envinfopy-0.1.0/envinfopy/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python3
-
 """
 .. codeauthor:: Tsuyoshi Hombashi <tsuyoshi.hombashi@gmail.com>
 """
 
 import argparse
 from textwrap import dedent
 
@@ -22,19 +20,19 @@
     )
     parser.add_argument("-V", "--version", action="version", version=f"%(prog)s {__version__}")
     parser.add_argument("-v", "--verbose", dest="verbosity_level", action="count", default=1)
 
     parser.add_argument(
         "packages",
         nargs="+",
-        help="package names to extract versions",
+        help="PyPI package names to extract versions",
     )
     parser.add_argument(
         "--format",
-        choices=["text", "markdown", "json", "itemize"],
+        choices=["text", "markdown", "md", "json", "itemize"],
         default="text",
         help="output format",
     )
 
     return parser.parse_args()
```

### Comparing `envinfopy-0.0.7/envinfopy.egg-info/PKG-INFO` & `envinfopy-0.1.0/envinfopy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: envinfopy
-Version: 0.0.7
+Version: 0.1.0
 Summary: envinfopy is a Python Library to get execution environment information.
 Home-page: https://github.com/thombashi/envinfopy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/envinfopy
 Project-URL: Tracker, https://github.com/thombashi/envinfopy/issues
 Keywords: environment,uname,version,markdown
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Terminals
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: all
+Provides-Extra: cli
+Provides-Extra: dev
 Provides-Extra: distro
 Provides-Extra: markdown
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **envinfopy**
    :backlinks: top
@@ -66,77 +67,86 @@
 envinfopy is a Python Library to get execution environment information.
 
 
 Installation
 ============================================
 ::
 
-    pip3 install envinfopy
+    python3 -m pip install envinfopy
 
 
 Usage
 ============================================
 
 Library usage
 --------------------------------------------
+
+Get execution environment information as a dictionary:
+
+.. code-block:: python
+
+    >>> import envinfopy
+    >>> envinfopy.get_envinfo()
+    {'uname': 'Linux', 'python_implementation': 'CPython', 'python_version': '3.11.4', 'platform': 'Ubuntu 22.04.2 LTS'}
+
+Get execution environment information and specific package version information:
+
 .. code-block:: python
 
     >>> import envinfopy
     >>> envinfopy.get_envinfo(["envinfopy"])
-    {'uname': 'Linux', 'python_implementation': 'CPython', 'python_version': '3.8.5', 'platform': 'Ubuntu 18.04', 'envinfopy': '0.0.4'}
+    {'uname': 'Linux', 'python_implementation': 'CPython', 'python_version': '3.11.4', 'platform': 'Ubuntu 22.04.2 LTS', 'envinfopy': '0.1.0'}
 
 Get environment information as Markdown:
 
 ::
 
-    pip3 install envinfopy[all]  # install optional dependencies
+    python3 -m pip install envinfopy[markdown]  # install optional dependencies
 
 .. code-block:: python
 
     >>> import envinfopy
     >>> print(envinfopy.dumps(["envinfopy"], format="markdown"))
-    |  Module   |    Version    |
-    | --------- | ------------- |
-    | uname     | Linux         |
-    | Python    | CPython 3.8.5 |
-    | platform  | Ubuntu 18.04  |
-    | envinfopy | 0.0.4         |
+    |  Module   |      Version       |
+    | --------- | ------------------ |
+    | uname     | Linux              |
+    | Python    | CPython 3.11.4     |
+    | platform  | Ubuntu 22.04.2 LTS |
+    | envinfopy | 0.1.0              |
 
 CLI usage
 --------------------------------------------
 ::
 
-    $ pip3 install envinfopy[all]  # install optional dependencies
+    $ python3 -m install envinfopy[cli]  # install optional dependencies
 
     $ python3 -m envinfopy envinfopy setuptools --format markdown
-    |   Module   |              Version              |
-    | ---------- | --------------------------------- |
-    | uname      | Linux 4.19.104-microsoft-standard |
-    | Python     | CPython 3.8.5                     |
-    | platform   | Ubuntu 18.04                      |
-    | envinfopy  | 0.0.4                             |
-    | setuptools | 57.0.0                            |
+    |   Module   |                 Version                 |
+    | ---------- | --------------------------------------- |
+    | uname      | Linux 5.15.90.1-microsoft-standard-WSL2 |
+    | Python     | CPython 3.11.4                          |
+    | platform   | Ubuntu 22.04.2 LTS                      |
+    | envinfopy  | 0.0.7                                   |
+    | setuptools | 67.8.0                                  |
 
 Command help
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 ::
 
-    usage: __main__.py [-h] [-V] [-v] [--format {text,markdown,json,itemize}] packages [packages ...]
+    usage: __main__.py [-h] [-V] [-v] [--format {text,markdown,md,json,itemize}] packages [packages ...]
 
     positional arguments:
-      packages              package names to extract versions
+      packages              PyPI package names to extract versions
 
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       -V, --version         show program's version number and exit
       -v, --verbose
-      --format {text,markdown,json,itemize}
+      --format {text,markdown,md,json,itemize}
                             output format
 
     Issue tracker: https://github.com/thombashi/envinfopy/issues
 
 
 Dependencies
 ============================================
-Python 3.6+
-
-
+Python 3.7+
```

### Comparing `envinfopy-0.0.7/pyproject.toml` & `envinfopy-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
@@ -14,14 +15,15 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.coverage.run]
 source = ['envinfopy']
 branch = true
 
 [tool.coverage.report]
 show_missing = true
@@ -49,15 +51,15 @@
     '*/.eggs/*',
     '*/.pytype/*',
     '*/.tox/*',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.6
+python_version = 3.7
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 warn_unused_configs = true
```

### Comparing `envinfopy-0.0.7/setup.py` & `envinfopy-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "envinfopy"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
-pkg_info = {}  # type: Dict[str, str]
+pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -31,16 +31,18 @@
     INSTALL_REQUIRES = [line.strip() for line in f if line.strip()]
 
 with open(os.path.join(REQUIREMENT_DIR, "test_requirements.txt")) as f:
     TESTS_REQUIRES = [line.strip() for line in f if line.strip()]
 
 
 markdown_requires = ["pytablewriter>=0.59.0,<2"]
+dev_requires = ["releasecmd>=0.9"]
 distro_requires = ["distro<2"]
-all_requires = markdown_requires + distro_requires
+cli_requires = markdown_requires + distro_requires
+all_requires = cli_requires + dev_requires
 
 setuptools.setup(
     name=MODULE_NAME,
     version=pkg_info["__version__"],
     url=REPOSITORY_URL,
     author=pkg_info["__author__"],
     author_email=pkg_info["__email__"],
@@ -52,35 +54,37 @@
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["tests*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=INSTALL_REQUIRES,
     extras_require={
         "all": all_requires,
+        "cli": cli_requires,
+        "dev": dev_requires,
         "distro": distro_requires,
         "markdown": markdown_requires,
         "test": set(TESTS_REQUIRES + all_requires),
     },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Terminals",
     ],
```

### Comparing `envinfopy-0.0.7/tests/test_cli.py` & `envinfopy-0.1.0/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from subprocrunner import SubprocessRunner
 
 
 RE_VERSION = re.compile(r"[0-9]\.[0-9]+\.[0-9]+", re.MULTILINE)
 
 
 class Test_cli:
-    def test_help(self, tmpdir):
+    def test_help(self):
         runner = SubprocessRunner([sys.executable, "-m", "envinfopy", "-h"])
         runner.run()
         assert runner.returncode == 0
 
     @pytest.mark.parametrize(
         ["format"],
         [
```

### Comparing `envinfopy-0.0.7/tests/test_envinfo.py` & `envinfopy-0.1.0/tests/test_envinfo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,47 @@
 import re
 import sys
 from itertools import combinations
 
 import pytest
 
 import envinfopy
-from envinfopy import Key
+from envinfopy import Key, _normalize_format
+from envinfopy._const import OutputFormat
 
 
 RE_VERSION = re.compile(r"[0-9]\.[0-9]+\.[0-9]+", re.MULTILINE)
 
 
+class Test_normalize_format:
+    @pytest.mark.parametrize(
+        ["format", "expected"],
+        [
+            ["", OutputFormat.TEXT],
+            ["markdown", OutputFormat.MARKDOWN],
+            ["markdown ", OutputFormat.MARKDOWN],
+            ["md", OutputFormat.MARKDOWN],
+            ["json", OutputFormat.JSON],
+            ["itemize", OutputFormat.ITEMIZE],
+        ],
+    )
+    def test_normal(self, format, expected):
+        assert _normalize_format(format) == expected
+
+    @pytest.mark.parametrize(
+        ["format"],
+        [
+            ["unknown"],
+        ],
+    )
+    def test_abnormal(self, format):
+        with pytest.raises(ValueError):
+            _normalize_format(format)
+
+
 class Test_get_uname:
     def test_normal(self):
         value_v0 = envinfopy.get_uname(verbosity_level=0)
         assert len(value_v0) > 0
 
         value_v1 = envinfopy.get_uname(verbosity_level=1)
         assert len(value_v1) > len(value_v0)
@@ -29,27 +56,27 @@
         print(envinfo)
 
         assert len(envinfo["uname"]) > 0
         assert RE_VERSION.search(envinfo[Key.PYTHON_VERSION])
         assert RE_VERSION.search(envinfo["pytest"])
         assert RE_VERSION.search(envinfo["envinfopy"])
 
+    def test_normal_no_packages(self):
+        envinfo = envinfopy.get_envinfo([""])
+
+        assert envinfo == envinfopy.get_envinfo()
+
     def test_abnormal_not_installed(self):
         envinfo = envinfopy.get_envinfo(["not-installed-pkg"])
         print(envinfo)
 
         assert len(envinfo["uname"]) > 0
         assert RE_VERSION.search(envinfo[Key.PYTHON_VERSION])
         assert envinfo["not-installed-pkg"] == "not installed"
 
-    def test_abnormal_empty(self):
-        envinfo = envinfopy.get_envinfo([""])
-
-        assert envinfo == envinfopy.get_envinfo()
-
 
 class Test_dumps:
     @pytest.mark.parametrize(
         ["format"],
         [
             ["text"],
             ["itemize"],
```

### Comparing `envinfopy-0.0.7/tox.ini` & `envinfopy-0.1.0/tox.ini`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,64 @@
 [tox]
 envlist =
-    py{36,37,38,39,310}
+    py{37,38,39,310,311}
     pypy3
     build
-    clean
     cov
     fmt
     lint
 
 [testenv]
 passenv = *
-deps =
-    .[test]
+extras =
+    test
 commands =
     pytest {posargs}
 
 [testenv:build]
-basepython = python3.8
 deps =
+    build>=0.10
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*.whl dist/*.tar.gz
-    python setup.py clean --all
 
 [testenv:clean]
 skip_install = true
 deps =
-    cleanpy>=0.2
+    cleanpy>=0.4
 commands =
-    cleanpy --force --all --exclude-envs .
+    cleanpy --all --exclude-envs .
 
 [testenv:cov]
 passenv = *
+extras =
+    test
 deps =
-    .[test]
     coverage[toml]>=5
 commands =
     coverage run -m pytest {posargs:-vv}
     coverage report -m
 
 [testenv:fmt]
-basepython = python3.8
 skip_install = true
 deps =
-    autoflake
-    black
+    autoflake>=2
+    black>=23.1
     isort>=5
 commands =
-    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    autoflake --in-place --recursive --remove-all-unused-imports .
     isort .
     black setup.py tests envinfopy
 
 [testenv:lint]
-basepython = python3.8
 skip_install = true
 deps =
-    mypy>=0.902
-    pylama
+    mypy>=1
+    pylama>=8.4.1
     types-pkg_resources
+    types-setuptools
 commands =
     python setup.py check
     mypy envinfopy setup.py
     pylama
```

