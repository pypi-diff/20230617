# Comparing `tmp/pytest-fluentbit-0.1.4.tar.gz` & `tmp/pytest-fluentbit-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ml/newpytfluent-bit/pytfluent/pytest-fluentbit/dist/.tmp-kidzru0w/pytest-fluentbit-0.1.4.tar", last modified: Fri Jun 16 21:45:09 2023, max compression
+gzip compressed data, was "/home/ml/newpytfluent-bit/pytfluent/pytest-fluentbit/dist/.tmp-40pc9a6y/pytest-fluentbit-0.1.5.tar", last modified: Fri Jun 16 22:04:59 2023, max compression
```

## Comparing `pytest-fluentbit-0.1.4.tar` & `pytest-fluentbit-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/
--rw-r--r--   0 root         (0) root         (0)     2108 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/.gitignore
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)     1086 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9666 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8478 2023-06-16 21:42:03.000000 pytest-fluentbit-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/docs/
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-16 20:21:54.000000 pytest-fluentbit-0.1.4/docs/api.md
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/docs/changelog.md
--rw-r--r--   0 root         (0) root         (0)      861 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       79 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/docs/contributing.md
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/docs/index.md
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/docs/installation.md
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/docs/usage.md
--rw-r--r--   0 root         (0) root         (0)     1879 2023-06-16 21:43:32.000000 pytest-fluentbit-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/requirements-dev.txt
--rw-r--r--   0 root         (0) root         (0)      305 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit/
--rw-r--r--   0 root         (0) root         (0)      552 2023-06-16 21:43:15.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit/__init__.py
--rw-r--r--   0 root         (0) root         (0)      837 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit/additional_information.py
--rw-r--r--   0 root         (0) root         (0)    13041 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit/plugin.py
--rw-r--r--   0 root         (0) root         (0)     4750 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit/test_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9666 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      854 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/src/pytest_fluentbit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:45:09.000000 pytest-fluentbit-0.1.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1511 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tests/test_additional_information.py
--rw-r--r--   0 root         (0) root         (0)     1785 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tests/test_addoptions.py
--rw-r--r--   0 root         (0) root         (0)     1703 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tests/test_docstrings.py
--rw-r--r--   0 root         (0) root         (0)     1324 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tests/test_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tests/test_ini_configuration.py
--rw-r--r--   0 root         (0) root         (0)     4279 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tests/test_reporting.py
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tests/utility.py
--rw-r--r--   0 root         (0) root         (0)     3912 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.4/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9666 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8478 2023-06-16 21:42:03.000000 pytest-fluentbit-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/docs/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-16 20:21:54.000000 pytest-fluentbit-0.1.5/docs/api.md
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/docs/changelog.md
+-rw-r--r--   0 root         (0) root         (0)      861 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/docs/contributing.md
+-rw-r--r--   0 root         (0) root         (0)      140 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/docs/index.md
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/docs/installation.md
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/docs/usage.md
+-rw-r--r--   0 root         (0) root         (0)     1879 2023-06-16 22:03:40.000000 pytest-fluentbit-0.1.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/requirements-dev.txt
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit/
+-rw-r--r--   0 root         (0) root         (0)      555 2023-06-16 22:03:20.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      837 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit/additional_information.py
+-rw-r--r--   0 root         (0) root         (0)    13041 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit/plugin.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit/test_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9666 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      854 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/src/pytest_fluentbit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:04:59.000000 pytest-fluentbit-0.1.5/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)      824 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/tests/test_additional_information.py
+-rw-r--r--   0 root         (0) root         (0)     1785 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/tests/test_addoptions.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/tests/test_docstrings.py
+-rw-r--r--   0 root         (0) root         (0)     1324 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/tests/test_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     3894 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/tests/test_ini_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/tests/test_reporting.py
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-16 19:58:12.000000 pytest-fluentbit-0.1.5/tests/utility.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-06-16 22:01:45.000000 pytest-fluentbit-0.1.5/tox.ini
```

### Comparing `pytest-fluentbit-0.1.4/.gitignore` & `pytest-fluentbit-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/.readthedocs.yaml` & `pytest-fluentbit-0.1.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/LICENSE` & `pytest-fluentbit-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/PKG-INFO` & `pytest-fluentbit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-fluentbit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A pytest plugin in order to provide logs via fluentbit
 Author-email: Sujay Kanungo <sujay.kanungo@gmail.com>
 License: MIT
 Project-URL: project, https://github.com/sujay2002/pytest-fluentbit
 Keywords: pytest,logging,fluent
 Platform: Unix
 Platform: Linux
```

### Comparing `pytest-fluentbit-0.1.4/README.md` & `pytest-fluentbit-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/docs/conf.py` & `pytest-fluentbit-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/pyproject.toml` & `pytest-fluentbit-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 dependencies = [
     "pytest>=7.0.0",
     "msgpack",
     "six",
     "fluent-logger"
 ]
 
-version = "0.1.4"
+version = "0.1.5"
 
 
 [project.urls]
 project = "https://github.com/sujay2002/pytest-fluentbit"
 
 [project.optional-dependencies]
 docs = [
```

### Comparing `pytest-fluentbit-0.1.4/src/pytest_fluentbit/__init__.py` & `pytest-fluentbit-0.1.5/src/pytest_fluentbit/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-"""pytest-fluent-logging."""
+"""pytest-fluentbit-logging."""
 
 from importlib_metadata import PackageNotFoundError, version
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
 try:
     __version__ = version(__name__)
 except PackageNotFoundError:
     # package is not installed
     pass
```

### Comparing `pytest-fluentbit-0.1.4/src/pytest_fluentbit/additional_information.py` & `pytest-fluentbit-0.1.5/src/pytest_fluentbit/additional_information.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/src/pytest_fluentbit/plugin.py` & `pytest-fluentbit-0.1.5/src/pytest_fluentbit/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/src/pytest_fluentbit/test_report.py` & `pytest-fluentbit-0.1.5/src/pytest_fluentbit/test_report.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/src/pytest_fluentbit.egg-info/PKG-INFO` & `pytest-fluentbit-0.1.5/src/pytest_fluentbit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-fluentbit
-Version: 0.1.4
+Version: 0.1.5
 Summary: A pytest plugin in order to provide logs via fluentbit
 Author-email: Sujay Kanungo <sujay.kanungo@gmail.com>
 License: MIT
 Project-URL: project, https://github.com/sujay2002/pytest-fluentbit
 Keywords: pytest,logging,fluent
 Platform: Unix
 Platform: Linux
```

### Comparing `pytest-fluentbit-0.1.4/src/pytest_fluentbit.egg-info/SOURCES.txt` & `pytest-fluentbit-0.1.5/src/pytest_fluentbit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/tests/conftest.py` & `pytest-fluentbit-0.1.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/tests/test_additional_information.py` & `pytest-fluentbit-0.1.5/tests/test_additional_information.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/tests/test_addoptions.py` & `pytest-fluentbit-0.1.5/tests/test_addoptions.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/tests/test_docstrings.py` & `pytest-fluentbit-0.1.5/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/tests/test_fixtures.py` & `pytest-fluentbit-0.1.5/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/tests/test_ini_configuration.py` & `pytest-fluentbit-0.1.5/tests/test_ini_configuration.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/tests/test_reporting.py` & `pytest-fluentbit-0.1.5/tests/test_reporting.py`

 * *Files identical despite different names*

### Comparing `pytest-fluentbit-0.1.4/tox.ini` & `pytest-fluentbit-0.1.5/tox.ini`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
 [testenv:pylint]
 description = Find errors with static code analysis.
 envdir = {toxworkdir}/lint
 deps =
     pylint
 commands =    
-    pylint --output-format=colorized --errors-only src/pytest_fluent
+    pylint --output-format=colorized --errors-only src/pytest_fluentbit
 
 [testenv:errors]
 description = Find errors with static code analysis.
 envdir = {toxworkdir}/lint
 deps =
     {[testenv:flake]deps}
     {[testenv:pylint]deps}
```

