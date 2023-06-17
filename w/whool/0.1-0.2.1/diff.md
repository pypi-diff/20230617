# Comparing `tmp/whool-0.1.tar.gz` & `tmp/whool-0.2.1.tar.gz`

## Comparing `whool-0.1.tar` & `whool-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 whool-0.1/.flake8
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 whool-0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 whool-0.1/TODO
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 whool-0.1/tox.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whool-0.1/src/whool/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 whool-0.1/src/whool/__main__.py
--rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 whool-0.1/src/whool/buildapi.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 whool-0.1/src/whool/cli.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 whool-0.1/src/whool/dependencies.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 whool-0.1/src/whool/init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whool-0.1/src/whool/py.typed
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 whool-0.1/src/whool/version.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 whool-0.1/tests/conftest.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whool-0.1/tests/test_build_sdist.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 whool-0.1/tests/test_build_wheel.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 whool-0.1/tests/test_init.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 whool-0.1/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 whool-0.1/LICENSE
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 whool-0.1/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 whool-0.1/pyproject.toml
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 whool-0.1/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 whool-0.2.1/.flake8
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 whool-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 whool-0.2.1/TODO
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 whool-0.2.1/tox.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/__main__.py
+-rw-r--r--   0        0        0     7430 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/buildapi.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/cli.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/compat.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/dependencies.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/py.typed
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 whool-0.2.1/src/whool/version.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 whool-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 whool-0.2.1/tests/test_build_sdist.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 whool-0.2.1/tests/test_build_wheel.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 whool-0.2.1/tests/test_init.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 whool-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 whool-0.2.1/LICENSE
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 whool-0.2.1/README.md
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 whool-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 whool-0.2.1/PKG-INFO
```

### Comparing `whool-0.1/.pre-commit-config.yaml` & `whool-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `whool-0.1/tox.ini` & `whool-0.2.1/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [gh-actions]
 python =
     3.6: py36
     3.7: py37
     3.8: py38, typing
     3.9: py39, typing
-    3.10: py310, typing, pypi-description
+    3.10: py310, typing
+    3.11: py311, typing, pypi-description
     pypy3: pypy3
 
 [tox]
 isolated_build = True
 envlist =
     py36
     py37
     py38
     py39
     py310
+    py311
     pypy3
     lint
     typing
     docs
     pypi-description
 
 [testenv]
```

### Comparing `whool-0.1/src/whool/buildapi.py` & `whool-0.2.1/src/whool/buildapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 import re
 import shutil
 import subprocess
-import sys
 import tarfile
 import tempfile
 from email.generator import Generator
 from email.message import Message
 from email.parser import HeaderParser
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from manifestoo_core.metadata import metadata_from_addon_dir
 
-if sys.version_info < (3, 11):
-    import tomli as tomllib
-else:
-    import tomllib
-
 # TODO WheelFile is not a public API of wheel
 from wheel.wheelfile import WheelFile  # type: ignore
 
+from .compat import tomllib
 from .version import version as whool_version
 
 TAG = "py3-none-any"
 METADATA_NAME_RE = re.compile(r"^odoo(\d*)-addon-(?P<addon_name>.*)$")
 
 
 class UnsupportedOperation(NotImplementedError):
```

### Comparing `whool-0.1/src/whool/cli.py` & `whool-0.2.1/src/whool/cli.py`

 * *Files identical despite different names*

### Comparing `whool-0.1/src/whool/dependencies.py` & `whool-0.2.1/src/whool/dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
             addon_dir,
             options={"post_version_strategy_override": POST_VERSION_STRATEGY_NONE},
         )
     except ManifestooException as e:
         _logger.debug("Could not load metadata for %s: %s", addon_dir, e)
         return []
     else:
-        return metadata.get_all("Requires-Dist")
+        return metadata.get_all("Requires-Dist") or []
```

### Comparing `whool-0.1/src/whool/init.py` & `whool-0.2.1/src/whool/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from pathlib import Path
 from typing import Sequence
 
-import tomli
+from .compat import tomllib
 
 _logger = logging.getLogger(__name__)
 
 BUILD_SYSTEM_TOML = b"""\
 [build-system]
 requires = ["whool"]
 build-backend = "whool.buildapi"
@@ -18,15 +18,15 @@
         return False
     pyproject_toml_path = addon_dir / "pyproject.toml"
     if not pyproject_toml_path.exists():
         with open(pyproject_toml_path, "wb") as f:
             f.write(BUILD_SYSTEM_TOML)
     else:
         with open(pyproject_toml_path, "rb") as f:
-            pyproject_toml = tomli.load(f)
+            pyproject_toml = tomllib.load(f)
         if "build-system" in pyproject_toml:
             if (
                 pyproject_toml.get("build-system", {}).get("build-backend")
                 != "whool.buildapi"
             ):
                 _logger.debug(
                     f"Did not initialize Whool build-system in {pyproject_toml_path} "
```

### Comparing `whool-0.1/tests/conftest.py` & `whool-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `whool-0.1/tests/test_build_sdist.py` & `whool-0.2.1/tests/test_build_sdist.py`

 * *Files identical despite different names*

### Comparing `whool-0.1/tests/test_build_wheel.py` & `whool-0.2.1/tests/test_build_wheel.py`

 * *Files identical despite different names*

### Comparing `whool-0.1/tests/test_init.py` & `whool-0.2.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `whool-0.1/.gitignore` & `whool-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `whool-0.1/LICENSE` & `whool-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whool-0.1/pyproject.toml` & `whool-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "License :: OSI Approved :: MIT License",
     "Framework :: Odoo",
 ]
 requires-python = ">=3.6"
 dependencies = [
     "manifestoo-core[metadata]>=0.8",
     "tomli; python_version<'3.11'",
-    "wheel==0.37.1",  # pin because we use an undocumented feature
+    "wheel<0.41",  # pin because we use an undocumented feature
     "importlib_metadata; python_version<'3.8'",
 ]
 scripts = {whool = "whool.cli:main"}
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
```

### Comparing `whool-0.1/PKG-INFO` & `whool-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 Metadata-Version: 2.1
 Name: whool
-Version: 0.1
+Version: 0.2.1
 Summary: whool - build backend for Odoo addons
 Project-URL: Homepage, https://github.com/acsone/whool
 Project-URL: Documentation, https://whool.readthedocs.io/en/stable/
 Project-URL: Changelog, https://whool.readthedocs.io/en/stable/changelog.html
 Project-URL: Source, https://github.com/acsone/whool
 Author-email: Stéphane Bidoul <stephane.bidoul@acsone.eu>
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Odoo
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: manifestoo-core[metadata]>=0.8
 Requires-Dist: tomli; python_version < '3.11'
-Requires-Dist: wheel==0.37.1
+Requires-Dist: wheel<0.41
 Provides-Extra: doc
 Requires-Dist: furo; extra == 'doc'
 Requires-Dist: myst-parser; extra == 'doc'
 Requires-Dist: sphinx; extra == 'doc'
 Requires-Dist: sphinxcontrib-towncrier; extra == 'doc'
 Requires-Dist: towncrier; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: coverage[toml]; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # whool - Package Odoo Addons as Python Wheels
 
-!!! pre-alpha work in progress...
+This project is the successor of
+[setuptools-odoo](https://pypi.org/project/setuptools-odoo/), as a standard-compliant
+Python build backend.
 
-This project is the successor of setuptools-odoo, as a PEP 517 build backend.
+It also provides a CLI to initialize `pyproject.toml` in an addon directory,
+and list Python dependencies of an addon.
 
-It also provides a convenience CLI to build and install addons, although
-this can also be achieved with regular Python packaging ecosystem tools
-such as `pip` and `build`.
+The main expected benefit is that the the setup directory is replaced by a
+`pyproject.toml` file at the root of each addon. So it's less intrusive, and does not
+need symbolic links for regular operation.
 
-Main expected benefit: the setup directory is replaced by
-a `pyproject.toml` file at the root of each addon. So it's less intrusive,
-and does not need symbolic links so it works better on platforms where
-symlinks are problematic.
+## Configuration
 
-It currently depends on `setuptools-odoo` where the logic to extract
-Python Package Metadata from Odoo Addon Manifests resides.
+The following options can be set in `pyproject.toml`:
+
+... TODO
+
+## Development
+
+To release and publish to PyPI, go to GitHub and create a release.
```

