# Comparing `tmp/CacheToolsUtils-6.0.tar.gz` & `tmp/CacheToolsUtils-7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CacheToolsUtils-6.0.tar", last modified: Sun Mar 19 08:31:02 2023, max compression
+gzip compressed data, was "CacheToolsUtils-7.0.tar", last modified: Sat Jun 17 07:18:40 2023, max compression
```

## Comparing `CacheToolsUtils-6.0.tar` & `CacheToolsUtils-7.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-03-19 08:31:02.907572 CacheToolsUtils-6.0/
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-03-19 08:31:02.907572 CacheToolsUtils-6.0/CacheToolsUtils.egg-info/
--rw-------   0 fabien    (1001) fabien    (1001)     9896 2023-03-19 08:31:02.000000 CacheToolsUtils-6.0/CacheToolsUtils.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)      285 2023-03-19 08:31:02.000000 CacheToolsUtils-6.0/CacheToolsUtils.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2023-03-19 08:31:02.000000 CacheToolsUtils-6.0/CacheToolsUtils.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)       11 2023-03-19 08:31:02.000000 CacheToolsUtils-6.0/CacheToolsUtils.egg-info/requires.txt
--rw-------   0 fabien    (1001) fabien    (1001)       16 2023-03-19 08:31:02.000000 CacheToolsUtils-6.0/CacheToolsUtils.egg-info/top_level.txt
--rwx------   0 fabien    (1001) fabien    (1001)     8214 2022-09-07 13:39:49.000000 CacheToolsUtils-6.0/CacheToolsUtils.py
--rw-------   0 fabien    (1001) fabien    (1001)       33 2022-01-27 13:44:32.000000 CacheToolsUtils-6.0/LICENSE
--rw-------   0 fabien    (1001) fabien    (1001)       17 2022-01-29 07:50:51.000000 CacheToolsUtils-6.0/MANIFEST.in
--rw-------   0 fabien    (1001) fabien    (1001)     1784 2022-09-11 09:25:44.000000 CacheToolsUtils-6.0/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)     9896 2023-03-19 08:31:02.907572 CacheToolsUtils-6.0/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)     9036 2023-03-19 08:24:03.000000 CacheToolsUtils-6.0/README.md
--rw-------   0 fabien    (1001) fabien    (1001)      218 2023-03-19 08:22:29.000000 CacheToolsUtils-6.0/pyproject.toml
--rw-------   0 fabien    (1001) fabien    (1001)      877 2023-03-19 08:31:02.907572 CacheToolsUtils-6.0/setup.cfg
--rw-------   0 fabien    (1001) fabien    (1001)       89 2022-01-27 13:49:40.000000 CacheToolsUtils-6.0/setup.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-17 07:18:40.862618 CacheToolsUtils-7.0/
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-17 07:18:40.862618 CacheToolsUtils-7.0/CacheToolsUtils.egg-info/
+-rw-------   0 fabien    (1001) fabien    (1001)     9997 2023-06-17 07:18:40.000000 CacheToolsUtils-7.0/CacheToolsUtils.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)      266 2023-06-17 07:18:40.000000 CacheToolsUtils-7.0/CacheToolsUtils.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2023-06-17 07:18:40.000000 CacheToolsUtils-7.0/CacheToolsUtils.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)      146 2023-06-17 07:18:40.000000 CacheToolsUtils-7.0/CacheToolsUtils.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)       16 2023-06-17 07:18:40.000000 CacheToolsUtils-7.0/CacheToolsUtils.egg-info/top_level.txt
+-rwx------   0 fabien    (1001) fabien    (1001)     8196 2023-06-16 11:07:47.000000 CacheToolsUtils-7.0/CacheToolsUtils.py
+-rw-------   0 fabien    (1001) fabien    (1001)       33 2023-05-14 12:34:09.000000 CacheToolsUtils-7.0/LICENSE
+-rw-------   0 fabien    (1001) fabien    (1001)       17 2023-05-14 12:34:09.000000 CacheToolsUtils-7.0/MANIFEST.in
+-rw-------   0 fabien    (1001) fabien    (1001)     1711 2023-06-17 07:10:27.000000 CacheToolsUtils-7.0/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     9997 2023-06-17 07:18:40.862618 CacheToolsUtils-7.0/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)     9130 2023-06-17 07:09:39.000000 CacheToolsUtils-7.0/README.md
+-rw-------   0 fabien    (1001) fabien    (1001)     1150 2023-06-17 07:06:57.000000 CacheToolsUtils-7.0/pyproject.toml
+-rw-------   0 fabien    (1001) fabien    (1001)       38 2023-06-17 07:18:40.862618 CacheToolsUtils-7.0/setup.cfg
```

### Comparing `CacheToolsUtils-6.0/CacheToolsUtils.egg-info/PKG-INFO` & `CacheToolsUtils-7.0/CacheToolsUtils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: CacheToolsUtils
-Version: 6.0
+Version: 7.0
 Summary: Cachetools Utilities
-Home-page: https://github.com/zx80/cachetools-utils
-Author: Fabien Coelho
-Author-email: cachetools.utils@coelho.net
-License: UNKNOWN
-Project-URL: Documentation, https://zx80.github.io/cachetools-utils/
-Project-URL: Issues, https://github.com/zx80/cachetools-utils/issues
-Project-URL: Package, https://pypi.org/project/CacheToolsUtils/
-Project-URL: Sources, https://github.com/zx80/cachetools-utils
-Platform: UNKNOWN
+Author-email: Fabien Coelho <cachetools.utils@coelho.net>
+License: CC0
+Project-URL: repository, https://github.com/zx80/cachetools-utils
+Project-URL: documentation, https://zx80.github.io/cachetools-utils/
+Project-URL: issues, https://github.com/zx80/cachetools-utils/issues
+Project-URL: package, https://pypi.org/project/CacheToolsUtils/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: tests
+Provides-Extra: pub
 License-File: LICENSE
 
 # cachetools-utils
 
 Classes to add key prefix and stats to
 [cachetools](https://pypi.org/project/cachetools/) classes and use
 [redis](https://redis.io/) and
@@ -235,14 +236,19 @@
 [Sources](https://github.com/zx80/cachetools-utils),
 [documentation](https://zx80.github.io/cachetools-utils/) and
 [issues](https://github.com/zx80/cachetools-utils/issues)
 are hosted on [GitHub](https://github.com).
 Install [package](https://pypi.org/project/CacheToolsUtils/) from
 [PyPI](https://pypi.org/).
 
+### 7.0 on 2023-06-17
+
+Switch to `pyproject.toml`.
+Require Python *3.10+* for easier typing.
+
 ### 6.0 on 2023-03-19
 
 Improved documentation for `github.io`.
 Add a `pyproject.toml` (stupid) file.
 
 ### 5.1 on 2022-11-12
 
@@ -306,9 +312,7 @@
 Initial version extracted from another project.
 
 ## TODO
 
 - add a `close`?
 - rename `hits`  `hit_rate`?
 - add other efficiency statistics?
-
-
```

### Comparing `CacheToolsUtils-6.0/CacheToolsUtils.py` & `CacheToolsUtils-7.0/CacheToolsUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
 CacheTools Utilities
 
 This code is public domain.
 """
 
-from typing import Any, Callable, Union, MutableMapping as MutMap
+from typing import Any, Callable, MutableMapping as MutMap
 
 import cachetools
 import json
 
-import pkg_resources as pkg  # type: ignore
-
-__version__ = pkg.require("CacheToolsUtils")[0].version
+from importlib.metadata import version as pkg_version
+__version__ = pkg_version("CacheToolsUtils")
 
 import logging
-
 log = logging.getLogger(__name__)
 
 
 #
 # UTILS
 #
 
@@ -67,15 +65,15 @@
 # CACHETOOLS EXTENSIONS
 #
 
 
 class PrefixedCache(KeyMutMapMix, MutMap):
     """Cache class to add a key prefix."""
 
-    def __init__(self, cache: MutMap, prefix: Union[str, bytes] = ""):
+    def __init__(self, cache: MutMap, prefix: str|bytes = ""):
         self._prefix = prefix
         self._cache = cache
 
     def _key(self, key):
         return self._prefix + str(key)
```

### Comparing `CacheToolsUtils-6.0/Makefile` & `CacheToolsUtils-7.0/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -21,35 +21,34 @@
 # venv for local testing
 PYTHON	= python
 PIP		= venv/bin/pip
 
 venv:
 	$(PYTHON) -m venv venv
 	$(PIP) install --upgrade pip
-	$(PIP) install -e .
-	$(PIP) install -r dev-requirements.txt
+	$(PIP) install -e .[dev,pub,tests]
 
 #
 # Tests
 #
 PYTEST	= pytest --log-level=debug --capture=tee-sys
 PYTOPT	=
 
 .PHONY: check
-check: check.mypy check.flake8 check.black check.pytest check.coverage check.pymarkdown
+check: check.mypy check.flake8 check.pytest check.coverage check.pymarkdown
 
 .PHONY: check.mypy
 check.mypy:
 	. venv/bin/activate
 	mypy $(MODULE).py
 
 .PHONY: check.flake8
 check.flake8:
 	. venv/bin/activate
-	flake8 --ignore=E501 $(MODULE).py
+	flake8 --ignore=E227,E501 $(MODULE).py
 
 .PHONY: check.black
 check.black:
 	. venv/bin/activate
 	black --check $(MODULE).py
 
 .PHONY: check.pytest
@@ -74,19 +73,19 @@
 	type $(PYTHON)
 
 $(MODULE).egg-info: venv
 	$(PIP) install -e .
 
 # generate source and built distribution
 dist:
-	$(PYTHON) setup.py sdist bdist_wheel
+	$(PYTHON) -m build
 
 .PHONY: publish
 publish: dist
 	# provide pypi login/pw or token somewhere…
-	echo twine upload --repository $(MODULE) dist/*
+	echo twine upload dist/*
 
 # generate pdf doc
 MD2PDF  = pandoc -f markdown -t latex -V papersize:a4 -V geometry:hmargin=2.5cm -V geometry:vmargin=3cm
 
 %.pdf: %.md
 	$(MD2PDF) -o $@ $<
```

### Comparing `CacheToolsUtils-6.0/PKG-INFO` & `CacheToolsUtils-7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: CacheToolsUtils
-Version: 6.0
+Version: 7.0
 Summary: Cachetools Utilities
-Home-page: https://github.com/zx80/cachetools-utils
-Author: Fabien Coelho
-Author-email: cachetools.utils@coelho.net
-License: UNKNOWN
-Project-URL: Documentation, https://zx80.github.io/cachetools-utils/
-Project-URL: Issues, https://github.com/zx80/cachetools-utils/issues
-Project-URL: Package, https://pypi.org/project/CacheToolsUtils/
-Project-URL: Sources, https://github.com/zx80/cachetools-utils
-Platform: UNKNOWN
+Author-email: Fabien Coelho <cachetools.utils@coelho.net>
+License: CC0
+Project-URL: repository, https://github.com/zx80/cachetools-utils
+Project-URL: documentation, https://zx80.github.io/cachetools-utils/
+Project-URL: issues, https://github.com/zx80/cachetools-utils/issues
+Project-URL: package, https://pypi.org/project/CacheToolsUtils/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: tests
+Provides-Extra: pub
 License-File: LICENSE
 
 # cachetools-utils
 
 Classes to add key prefix and stats to
 [cachetools](https://pypi.org/project/cachetools/) classes and use
 [redis](https://redis.io/) and
@@ -235,14 +236,19 @@
 [Sources](https://github.com/zx80/cachetools-utils),
 [documentation](https://zx80.github.io/cachetools-utils/) and
 [issues](https://github.com/zx80/cachetools-utils/issues)
 are hosted on [GitHub](https://github.com).
 Install [package](https://pypi.org/project/CacheToolsUtils/) from
 [PyPI](https://pypi.org/).
 
+### 7.0 on 2023-06-17
+
+Switch to `pyproject.toml`.
+Require Python *3.10+* for easier typing.
+
 ### 6.0 on 2023-03-19
 
 Improved documentation for `github.io`.
 Add a `pyproject.toml` (stupid) file.
 
 ### 5.1 on 2022-11-12
 
@@ -306,9 +312,7 @@
 Initial version extracted from another project.
 
 ## TODO
 
 - add a `close`?
 - rename `hits`  `hit_rate`?
 - add other efficiency statistics?
-
-
```

### Comparing `CacheToolsUtils-6.0/README.md` & `CacheToolsUtils-7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -214,14 +214,19 @@
 [Sources](https://github.com/zx80/cachetools-utils),
 [documentation](https://zx80.github.io/cachetools-utils/) and
 [issues](https://github.com/zx80/cachetools-utils/issues)
 are hosted on [GitHub](https://github.com).
 Install [package](https://pypi.org/project/CacheToolsUtils/) from
 [PyPI](https://pypi.org/).
 
+### 7.0 on 2023-06-17
+
+Switch to `pyproject.toml`.
+Require Python *3.10+* for easier typing.
+
 ### 6.0 on 2023-03-19
 
 Improved documentation for `github.io`.
 Add a `pyproject.toml` (stupid) file.
 
 ### 5.1 on 2022-11-12
```

