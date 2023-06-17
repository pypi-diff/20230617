# Comparing `tmp/pytest_gitconfig-0.1.0.tar.gz` & `tmp/pytest_gitconfig-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_gitconfig-0.1.0.tar", last modified: Fri Jun 16 14:57:59 2023, max compression
+gzip compressed data, was "pytest_gitconfig-0.1.1.tar", last modified: Sat Jun 17 01:12:59 2023, max compression
```

## Comparing `pytest_gitconfig-0.1.0.tar` & `pytest_gitconfig-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-06-16 09:32:31.548634 pytest_gitconfig-0.1.0/LICENSE
--rw-r--r--   0        0        0      823 2023-06-16 13:23:04.119535 pytest_gitconfig-0.1.0/README.md
--rw-r--r--   0        0        0     3683 2023-06-16 14:57:59.484985 pytest_gitconfig-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-16 09:32:31.539634 pytest_gitconfig-0.1.0/src/pytest_gitconfig/__init__.py
--rw-r--r--   0        0        0       62 2023-06-16 13:18:04.260801 pytest_gitconfig-0.1.0/src/pytest_gitconfig/_version.py
--rw-r--r--   0        0        0     2863 2023-06-16 13:21:58.308562 pytest_gitconfig-0.1.0/src/pytest_gitconfig/plugin.py
--rw-r--r--   0        0        0        0 2023-06-16 09:32:31.537634 pytest_gitconfig-0.1.0/src/pytest_gitconfig/py.typed
--rw-r--r--   0        0        0       64 2023-06-16 13:10:10.760439 pytest_gitconfig-0.1.0/tests/conftests.py
--rw-r--r--   0        0        0      633 2023-06-16 13:11:36.083976 pytest_gitconfig-0.1.0/tests/test_override_defaults.py
--rw-r--r--   0        0        0      788 2023-06-16 13:11:35.517979 pytest_gitconfig-0.1.0/tests/test_pytest_gitconfig.py
--rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 pytest_gitconfig-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-16 09:32:31.548634 pytest_gitconfig-0.1.1/LICENSE
+-rw-r--r--   0        0        0      823 2023-06-16 13:23:04.119535 pytest_gitconfig-0.1.1/README.md
+-rw-r--r--   0        0        0     3479 2023-06-17 01:12:59.043561 pytest_gitconfig-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-16 09:32:31.539634 pytest_gitconfig-0.1.1/src/pytest_gitconfig/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-16 13:18:04.260801 pytest_gitconfig-0.1.1/src/pytest_gitconfig/_version.py
+-rw-r--r--   0        0        0     2863 2023-06-16 13:21:58.308562 pytest_gitconfig-0.1.1/src/pytest_gitconfig/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-16 09:32:31.537634 pytest_gitconfig-0.1.1/src/pytest_gitconfig/py.typed
+-rw-r--r--   0        0        0       64 2023-06-16 13:10:10.760439 pytest_gitconfig-0.1.1/tests/conftests.py
+-rw-r--r--   0        0        0      633 2023-06-16 13:11:36.083976 pytest_gitconfig-0.1.1/tests/test_override_defaults.py
+-rw-r--r--   0        0        0      788 2023-06-16 13:11:35.517979 pytest_gitconfig-0.1.1/tests/test_pytest_gitconfig.py
+-rw-r--r--   0        0        0     1907 1970-01-01 00:00:00.000000 pytest_gitconfig-0.1.1/PKG-INFO
```

### Comparing `pytest_gitconfig-0.1.0/LICENSE` & `pytest_gitconfig-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_gitconfig-0.1.0/README.md` & `pytest_gitconfig-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_gitconfig-0.1.0/pyproject.toml` & `pytest_gitconfig-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,45 +17,44 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Typing :: Typed",
 ]
-dependencies = []
-version = "0.1.0"
+dependencies = [
+    "pytest>=7.1.2",
+]
+version = "0.1.1"
 
 [project.license]
 text = "MIT"
 
-[project.optional-dependencies]
-
 [project.urls]
 Homepage = "https://github.com/noirbizarre/pytest-gitconfig"
-Documentation = "https://pytest-gitconfig.rtfd.io"
+Documentation = "https://github.com/noirbizarre/pytest-gitconfig#readme"
 Repository = "https://github.com/noirbizarre/pytest-gitconfig"
 Issues = "https://github.com/noirbizarre/pytest-gitconfig/issues"
 
 [project.entry-points.pytest11]
-myplugin = "pytest_gitconfig.plugin"
+gitconfig = "pytest_gitconfig.plugin"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.version]
 source = "scm"
 write_to = "src/pytest_gitconfig/_version.py"
 write_template = "__version__ = \"{}\""
 
 [tool.pdm.dev-dependencies]
 test = [
-    "pytest>=7.1.2",
     "pytest-sugar>=0.9.5",
     "pytest-cov>=3.0.0",
 ]
 lint = [
     "black>=23.3.0",
     "mypy>=1.3.0",
     "ruff>=0.0.270",
@@ -66,15 +65,15 @@
 ]
 release = [
     "emotional",
 ]
 
 [tool.pdm.scripts]
 pre_cover = "coverage erase"
-"pre_cover:tox" = "coverage erase"
+"pre_cover:all" = "coverage erase"
 
 [tool.pdm.scripts.test]
 help = "Run the test suite"
 cmd = "pytest"
 
 [tool.pdm.scripts.lint]
 help = "Lint all tracked files using pre-commit"
@@ -91,27 +90,20 @@
 [tool.pdm.scripts.typing]
 help = "Full typing linting (includes imported packages and uncommmited files)"
 cmd = "mypy src tests --warn-unused-ignores"
 
 [tool.pdm.scripts.cover]
 help = "Run the test suite with coverage"
 composite = [
-    "  test\n    --cov-report=term\n    --cov=pytest_gitconfig\n    --cov-report=html:reports/coverage\n    --cov-report=xml:reports/coverage.xml\n    --no-cov-on-fail\n    --junitxml=reports/tests.xml\n  ",
+    "  test\n    --cov\n    --cov-report=term\n    --cov-report=html:reports/coverage\n    --cov-report=xml:reports/coverage.xml\n    --no-cov-on-fail\n    --junitxml=reports/tests.xml\n  ",
 ]
 
-[tool.pdm.scripts."cover:tox"]
+[tool.pdm.scripts."cover:all"]
 help = "Run the test suite against all supported Python version"
-composite = [
-    "echo '🚦 Tests'",
-    "tox -p",
-    "echo '\n📸 Coverage'",
-    "coverage report",
-    "coverage xml -o reports/tox/coverage.xml",
-    "coverage html -d reports/tox/coverage",
-]
+cmd = "tox --parallel"
 
 [tool.pdm.scripts.changelog]
 help = "Update the changelog"
 cmd = "cz changelog"
 
 [tool.pdm.ide]
 linters = [
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytest_gitconfig-0.1.0/src/pytest_gitconfig/plugin.py` & `pytest_gitconfig-0.1.1/src/pytest_gitconfig/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_gitconfig-0.1.0/tests/test_override_defaults.py` & `pytest_gitconfig-0.1.1/tests/test_override_defaults.py`

 * *Files identical despite different names*

### Comparing `pytest_gitconfig-0.1.0/tests/test_pytest_gitconfig.py` & `pytest_gitconfig-0.1.1/tests/test_pytest_gitconfig.py`

 * *Files identical despite different names*

### Comparing `pytest_gitconfig-0.1.0/PKG-INFO` & `pytest_gitconfig-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-gitconfig
-Version: 0.1.0
+Version: 0.1.1
 Summary: Provide a gitconfig sandbox for testing
 Author-Email: Axel Haustant <noirbizarre@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -12,18 +12,19 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Project-URL: Homepage, https://github.com/noirbizarre/pytest-gitconfig
-Project-URL: Documentation, https://pytest-gitconfig.rtfd.io
+Project-URL: Documentation, https://github.com/noirbizarre/pytest-gitconfig#readme
 Project-URL: Repository, https://github.com/noirbizarre/pytest-gitconfig
 Project-URL: Issues, https://github.com/noirbizarre/pytest-gitconfig/issues
 Requires-Python: >=3.7
+Requires-Dist: pytest>=7.1.2
 Description-Content-Type: text/markdown
 
 # pytest-gitconfig
 
 [![CI](https://github.com/noirbizarre/pytest-gitconfig/actions/workflows/ci.yml/badge.svg)](https://github.com/noirbizarre/pytest-gitconfig/actions/workflows/ci.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/noirbizarre/pytest-gitconfig/main.svg)](https://results.pre-commit.ci/latest/github/noirbizarre/pytest-gitconfig/main)
 [![PyPI](https://img.shields.io/pypi/v/pytest-gitconfig)](https://pypi.org/project/pytest-gitconfig/)
```

