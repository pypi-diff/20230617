# Comparing `tmp/gex_cli-1.0.0.tar.gz` & `tmp/gex_cli-1.0.1.tar.gz`

## Comparing `gex_cli-1.0.0.tar` & `gex_cli-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gex_cli-1.0.0/src/gexpy/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 gex_cli-1.0.0/src/gexpy/__main__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 gex_cli-1.0.0/src/gexpy/cli.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gex_cli-1.0.0/src/gexpy/config.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gex_cli-1.0.0/src/gexpy/logger.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 gex_cli-1.0.0/src/gexpy/utils.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 gex_cli-1.0.0/.gitignore
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 gex_cli-1.0.0/README.md
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 gex_cli-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 gex_cli-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/__init__.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/__main__.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/cli.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/config.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/logger.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 gex_cli-1.0.1/gexpy/utils.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 gex_cli-1.0.1/.gitignore
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 gex_cli-1.0.1/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 gex_cli-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 gex_cli-1.0.1/PKG-INFO
```

### Comparing `gex_cli-1.0.0/src/gexpy/cli.py` & `gex_cli-1.0.1/gexpy/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import click
 import git
 import github3
 from rich.console import Console
 from rich.table import Table
 
-from gexpy import __name__, __version__
+from . import __name__, __version__
 from gexpy.config import Config
 from gexpy.logger import success, error, info, warn
 from gexpy.utils import rmtree
 
 
 @click.group(context_settings={'help_option_names': ['-h', '--help'],})
 @click.version_option(version=__version__, prog_name=__name__)
```

### Comparing `gex_cli-1.0.0/.gitignore` & `gex_cli-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gex_cli-1.0.0/pyproject.toml` & `gex_cli-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 
 [project.urls]
 Documentation = "https://github.com/woidzero/gex-cli#readme"
 Issues = "https://github.com/woidzero/gex-cli/issues"
 Source = "https://github.com/woidzero/gex-cli"
 
 [project.scripts]
-gex = "src.gexpy.__main__:main"
+gex = "gexpy.__main__:main"
 
 [tool.hatch.version]
-path = "src/gexpy/__init__.py"
+path = "gexpy/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "/src/gexpy/",
+    "gexpy/",
 ]
```

### Comparing `gex_cli-1.0.0/PKG-INFO` & `gex_cli-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gex-cli
-Version: 1.0.0
+Version: 1.0.1
 Summary: Command-line project generator using git repo.
 Project-URL: Documentation, https://github.com/woidzero/gex-cli#readme
 Project-URL: Issues, https://github.com/woidzero/gex-cli/issues
 Project-URL: Source, https://github.com/woidzero/gex-cli
 Author-email: woidzero <woidzerov@gmail.com>
 License-Expression: MIT
 Keywords: cli,command-line,console,generator,project managment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gex-cli Version: 1.0.0 Summary: Command-line
+Metadata-Version: 2.1 Name: gex-cli Version: 1.0.1 Summary: Command-line
 project generator using git repo. Project-URL: Documentation, https://
 github.com/woidzero/gex-cli#readme Project-URL: Issues, https://github.com/
 woidzero/gex-cli/issues Project-URL: Source, https://github.com/woidzero/gex-
 cli Author-email: woidzero
 gmail.com> License-Expression: MIT Keywords: cli,command-
 line,console,generator,project managment Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: License :: OSI
```

