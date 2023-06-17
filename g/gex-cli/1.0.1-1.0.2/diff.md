# Comparing `tmp/gex_cli-1.0.1.tar.gz` & `tmp/gex_cli-1.0.2.tar.gz`

## Comparing `gex_cli-1.0.1.tar` & `gex_cli-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/__init__.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/__main__.py
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/cli.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/config.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/logger.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/utils.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 gex_cli-1.0.1/.gitignore
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 gex_cli-1.0.1/README.md
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 gex_cli-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 gex_cli-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/__main__.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/cli.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/config.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/logger.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 gex_cli-1.0.2/gexpy/utils.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 gex_cli-1.0.2/.gitignore
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 gex_cli-1.0.2/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 gex_cli-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 gex_cli-1.0.2/PKG-INFO
```

### Comparing `gex_cli-1.0.1/gexpy/cli.py` & `gex_cli-1.0.2/gexpy/cli.py`

 * *Files identical despite different names*

### Comparing `gex_cli-1.0.1/.gitignore` & `gex_cli-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gex_cli-1.0.1/pyproject.toml` & `gex_cli-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gex_cli-1.0.1/PKG-INFO` & `gex_cli-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gex-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: Command-line project generator using git repo.
 Project-URL: Documentation, https://github.com/woidzero/gex-cli#readme
 Project-URL: Issues, https://github.com/woidzero/gex-cli/issues
 Project-URL: Source, https://github.com/woidzero/gex-cli
 Author-email: woidzero <woidzerov@gmail.com>
 License-Expression: MIT
 Keywords: cli,command-line,console,generator,project managment
@@ -26,18 +26,22 @@
 Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # gex-cli
 
 Generate projects using built-in or custom templates via command-line.
 
+[![PyPI - Version](https://img.shields.io/pypi/v/gex-cli.svg)](https://pypi.org/project/gex-cli)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/gex-cli)](https://pypi.org/project/gex-cli)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/gex-cli.svg)](https://pypi.org/project/gex-cli)
+
 
 ## Installation
 
-```
+```bash
  pip install gex-cli
 ```
 
 ## Usage
 
 ```bash
   gex g web -n MyWebsite
@@ -45,8 +49,8 @@
 
 ## Support
 
 For support, email <a href="mailto://woidzeroo@gmail.com">woidzeroo@gmail.com</a>
 
 ## License
 
-`mcfc` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
+`gex-cli` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gex-cli Version: 1.0.1 Summary: Command-line
+Metadata-Version: 2.1 Name: gex-cli Version: 1.0.2 Summary: Command-line
 project generator using git repo. Project-URL: Documentation, https://
 github.com/woidzero/gex-cli#readme Project-URL: Issues, https://github.com/
 woidzero/gex-cli/issues Project-URL: Source, https://github.com/woidzero/gex-
 cli Author-email: woidzero
 gmail.com> License-Expression: MIT Keywords: cli,command-
 line,console,generator,project managment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: License :: OSI
@@ -10,12 +10,16 @@
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7 Requires-Dist: click Requires-Dist: gitpython Requires-
 Dist: mcfc Requires-Dist: rich Description-Content-Type: text/markdown # gex-
-cli Generate projects using built-in or custom templates via command-line. ##
-Installation ``` pip install gex-cli ``` ## Usage ```bash gex g web -
+cli Generate projects using built-in or custom templates via command-line. [!
+[PyPI - Version](https://img.shields.io/pypi/v/gex-cli.svg)](https://pypi.org/
+project/gex-cli) [![PyPI - Downloads](https://img.shields.io/pypi/dm/gex-cli)]
+(https://pypi.org/project/gex-cli) [![PyPI - Python Version](https://
+img.shields.io/pypi/pyversions/gex-cli.svg)](https://pypi.org/project/gex-cli)
+## Installation ```bash pip install gex-cli ``` ## Usage ```bash gex g web -
 n MyWebsite ``` ## Support For support, email woidzeroo@gmail.com ## License
-`mcfc` is distributed under the terms of the [MIT](https://spdx.org/licenses/
-MIT.html) license.
+`gex-cli` is distributed under the terms of the [MIT](https://spdx.org/
+licenses/MIT.html) license.
```

