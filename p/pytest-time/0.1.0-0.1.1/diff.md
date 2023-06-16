# Comparing `tmp/pytest_time-0.1.0.tar.gz` & `tmp/pytest_time-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_time-0.1.0.tar", last modified: Thu Jun 15 05:13:26 2023, max compression
+gzip compressed data, was "pytest_time-0.1.1.tar", last modified: Fri Jun 16 21:56:11 2023, max compression
```

## Comparing `pytest_time-0.1.0.tar` & `pytest_time-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.337528 pytest_time-0.1.0/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      723 2023-03-01 18:11:13.000000 pytest_time-0.1.0/.editorconfig
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.337528 pytest_time-0.1.0/.github/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      179 2023-03-01 18:11:13.000000 pytest_time-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      362 2023-06-15 05:03:00.000000 pytest_time-0.1.0/.github/release-drafter.yml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     3504 2023-05-22 16:14:08.000000 pytest_time-0.1.0/.github/renovate.json5
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.337528 pytest_time-0.1.0/.github/workflows/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      347 2023-06-08 02:02:37.000000 pytest_time-0.1.0/.github/workflows/release-drafter.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     2500 2023-06-11 20:35:38.000000 pytest_time-0.1.0/.github/workflows/tests.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4827 2023-06-15 04:05:36.000000 pytest_time-0.1.0/.gitignore
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      921 2023-05-22 16:14:08.000000 pytest_time-0.1.0/.pre-commit-config.yaml
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     7652 2023-06-15 05:04:51.000000 pytest_time-0.1.0/COPYING
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1017 2023-06-15 05:13:26.337528 pytest_time-0.1.0/PKG-INFO
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      153 2023-06-15 00:24:20.000000 pytest_time-0.1.0/README.rst
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     6744 2023-06-15 05:07:57.000000 pytest_time-0.1.0/pyproject.toml
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.337528 pytest_time-0.1.0/pytester/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       31 2023-06-15 04:59:41.000000 pytest_time-0.1.0/pytester/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1091 2023-06-15 04:59:15.000000 pytest_time-0.1.0/pytester/test_instant_sleep.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       38 2023-06-15 05:13:26.337528 pytest_time-0.1.0/setup.cfg
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.333528 pytest_time-0.1.0/src/
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.337528 pytest_time-0.1.0/src/pytest_time/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      229 2023-06-15 04:52:37.000000 pytest_time-0.1.0/src/pytest_time/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      160 2023-06-15 05:13:26.000000 pytest_time-0.1.0/src/pytest_time/_version.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      311 2023-06-15 05:00:24.000000 pytest_time-0.1.0/src/pytest_time/conftest.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1897 2023-06-15 04:52:37.000000 pytest_time-0.1.0/src/pytest_time/fake_time.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      962 2023-06-15 05:01:03.000000 pytest_time-0.1.0/src/pytest_time/instant_sleep.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 03:51:25.000000 pytest_time-0.1.0/src/pytest_time/py.typed
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      221 2023-06-15 04:06:50.000000 pytest_time-0.1.0/src/pytest_time/real_time.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.337528 pytest_time-0.1.0/src/pytest_time.egg-info/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1017 2023-06-15 05:13:26.000000 pytest_time-0.1.0/src/pytest_time.egg-info/PKG-INFO
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      921 2023-06-15 05:13:26.000000 pytest_time-0.1.0/src/pytest_time.egg-info/SOURCES.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        1 2023-06-15 05:13:26.000000 pytest_time-0.1.0/src/pytest_time.egg-info/dependency_links.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       46 2023-06-15 05:13:26.000000 pytest_time-0.1.0/src/pytest_time.egg-info/entry_points.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      254 2023-06-15 05:13:26.000000 pytest_time-0.1.0/src/pytest_time.egg-info/requires.txt
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       12 2023-06-15 05:13:26.000000 pytest_time-0.1.0/src/pytest_time.egg-info/top_level.txt
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.337528 pytest_time-0.1.0/tests/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 02:52:45.000000 pytest_time-0.1.0/tests/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)       30 2023-06-15 04:52:37.000000 pytest_time-0.1.0/tests/conftest.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.337528 pytest_time-0.1.0/tests/integration/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 04:17:24.000000 pytest_time-0.1.0/tests/integration/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)      227 2023-06-15 04:52:37.000000 pytest_time-0.1.0/tests/integration/test_instant_sleep.py
-drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-15 05:13:26.337528 pytest_time-0.1.0/tests/unit/
--rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 04:07:43.000000 pytest_time-0.1.0/tests/unit/__init__.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1517 2023-06-15 04:46:29.000000 pytest_time-0.1.0/tests/unit/test_fake_time.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     1979 2023-06-15 03:49:44.000000 pytest_time-0.1.0/tests/unit/test_instant_sleep.py
--rw-rw-r--   0 lengau    (1000) lengau    (1000)     4714 2023-06-15 05:03:00.000000 pytest_time-0.1.0/tox.ini
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.455371 pytest_time-0.1.1/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      723 2023-03-01 18:11:13.000000 pytest_time-0.1.1/.editorconfig
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.447372 pytest_time-0.1.1/.github/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      179 2023-03-01 18:11:13.000000 pytest_time-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      362 2023-06-15 05:03:00.000000 pytest_time-0.1.1/.github/release-drafter.yml
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     3504 2023-05-22 16:14:08.000000 pytest_time-0.1.1/.github/renovate.json5
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.451372 pytest_time-0.1.1/.github/workflows/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      347 2023-06-08 02:02:37.000000 pytest_time-0.1.1/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     2500 2023-06-11 20:35:38.000000 pytest_time-0.1.1/.github/workflows/tests.yaml
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     4827 2023-06-15 04:05:36.000000 pytest_time-0.1.1/.gitignore
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      921 2023-05-22 16:14:08.000000 pytest_time-0.1.1/.pre-commit-config.yaml
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     7652 2023-06-15 05:04:51.000000 pytest_time-0.1.1/COPYING
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1017 2023-06-16 21:56:11.455371 pytest_time-0.1.1/PKG-INFO
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      153 2023-06-15 00:24:20.000000 pytest_time-0.1.1/README.rst
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     6731 2023-06-16 21:53:25.000000 pytest_time-0.1.1/pyproject.toml
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.451372 pytest_time-0.1.1/pytester/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       31 2023-06-15 04:59:41.000000 pytest_time-0.1.1/pytester/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1091 2023-06-15 04:59:15.000000 pytest_time-0.1.1/pytester/test_instant_sleep.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       38 2023-06-16 21:56:11.455371 pytest_time-0.1.1/setup.cfg
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.447372 pytest_time-0.1.1/src/
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.451372 pytest_time-0.1.1/src/pytest_time/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      129 2023-06-16 21:53:10.000000 pytest_time-0.1.1/src/pytest_time/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      160 2023-06-16 21:56:11.000000 pytest_time-0.1.1/src/pytest_time/_version.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1897 2023-06-15 04:52:37.000000 pytest_time-0.1.1/src/pytest_time/fake_time.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1191 2023-06-16 21:52:50.000000 pytest_time-0.1.1/src/pytest_time/instant_sleep.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 03:51:25.000000 pytest_time-0.1.1/src/pytest_time/py.typed
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      221 2023-06-15 04:06:50.000000 pytest_time-0.1.1/src/pytest_time/real_time.py
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.451372 pytest_time-0.1.1/src/pytest_time.egg-info/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1017 2023-06-16 21:56:11.000000 pytest_time-0.1.1/src/pytest_time.egg-info/PKG-INFO
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      893 2023-06-16 21:56:11.000000 pytest_time-0.1.1/src/pytest_time.egg-info/SOURCES.txt
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)        1 2023-06-16 21:56:11.000000 pytest_time-0.1.1/src/pytest_time.egg-info/dependency_links.txt
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       39 2023-06-16 21:56:11.000000 pytest_time-0.1.1/src/pytest_time.egg-info/entry_points.txt
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      254 2023-06-16 21:56:11.000000 pytest_time-0.1.1/src/pytest_time.egg-info/requires.txt
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       12 2023-06-16 21:56:11.000000 pytest_time-0.1.1/src/pytest_time.egg-info/top_level.txt
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.451372 pytest_time-0.1.1/tests/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 02:52:45.000000 pytest_time-0.1.1/tests/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)       30 2023-06-15 04:52:37.000000 pytest_time-0.1.1/tests/conftest.py
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.451372 pytest_time-0.1.1/tests/integration/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 04:17:24.000000 pytest_time-0.1.1/tests/integration/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)      227 2023-06-15 04:52:37.000000 pytest_time-0.1.1/tests/integration/test_instant_sleep.py
+drwxrwxr-x   0 lengau    (1000) lengau    (1000)        0 2023-06-16 21:56:11.455371 pytest_time-0.1.1/tests/unit/
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)        0 2023-06-15 04:07:43.000000 pytest_time-0.1.1/tests/unit/__init__.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1517 2023-06-15 04:46:29.000000 pytest_time-0.1.1/tests/unit/test_fake_time.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     1979 2023-06-15 03:49:44.000000 pytest_time-0.1.1/tests/unit/test_instant_sleep.py
+-rw-rw-r--   0 lengau    (1000) lengau    (1000)     4714 2023-06-15 05:03:00.000000 pytest_time-0.1.1/tox.ini
```

### Comparing `pytest_time-0.1.0/.editorconfig` & `pytest_time-0.1.1/.editorconfig`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/.github/renovate.json5` & `pytest_time-0.1.1/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/.github/workflows/tests.yaml` & `pytest_time-0.1.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/.gitignore` & `pytest_time-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/.pre-commit-config.yaml` & `pytest_time-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/COPYING` & `pytest_time-0.1.1/COPYING`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/PKG-INFO` & `pytest_time-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_time
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pytest_time-0.1.0/pyproject.toml` & `pytest_time-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Testing :: Unit",
 ]
 requires-python = ">=3.8"
 
-[project.entry-points]
-pytest11 = {"pytest_time" = "pytest_time.conftest"}
+[project.entry-points.pytest11]
+instant_sleep = "pytest_time"
 
 [project.optional-dependencies]
 dev = [
     "coverage[toml]==7.2.7",
     "hypothesis>=6.78",
     "pytest==7.3.1",
     "pytest-check",
```

### Comparing `pytest_time-0.1.0/pytester/test_instant_sleep.py` & `pytest_time-0.1.1/pytester/test_instant_sleep.py`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/src/pytest_time/fake_time.py` & `pytest_time-0.1.1/src/pytest_time/fake_time.py`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/src/pytest_time/instant_sleep.py` & `pytest_time-0.1.1/src/pytest_time/instant_sleep.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """A pytest fixture for making time.sleep instant with proper side effects."""
 from __future__ import annotations
 
 from typing import cast
 
+import pytest
+
 from pytest_time import fake_time
 
 
 class InstantSleep(fake_time.FakeTime):
     """A time faker that makes sleep instant, adjusting time values accordingly.
 
     This uses the real system clock, but adjusts the values from `time` after
@@ -26,7 +28,15 @@
     def time_ns(self) -> int:
         """Get time.time_ns."""
         return cast(int, self._time.time_ns() + self.offset_ns)
 
     def monotonic_ns(self) -> int:
         """Get time.monotonic_ns."""
         return cast(int, self._time.monotonic_ns() + self.offset_ns)
+
+
+@pytest.fixture()
+def instant_sleep(monkeypatch: pytest.MonkeyPatch) -> InstantSleep:
+    """Fixture for speeding through time.sleep."""
+    sleep = InstantSleep()
+    sleep.install(monkeypatch)
+    return sleep
```

### Comparing `pytest_time-0.1.0/src/pytest_time.egg-info/PKG-INFO` & `pytest_time-0.1.1/src/pytest_time.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-time
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pytest_time-0.1.0/src/pytest_time.egg-info/SOURCES.txt` & `pytest_time-0.1.1/src/pytest_time.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 .github/renovate.json5
 .github/workflows/release-drafter.yaml
 .github/workflows/tests.yaml
 pytester/__init__.py
 pytester/test_instant_sleep.py
 src/pytest_time/__init__.py
 src/pytest_time/_version.py
-src/pytest_time/conftest.py
 src/pytest_time/fake_time.py
 src/pytest_time/instant_sleep.py
 src/pytest_time/py.typed
 src/pytest_time/real_time.py
 src/pytest_time.egg-info/PKG-INFO
 src/pytest_time.egg-info/SOURCES.txt
 src/pytest_time.egg-info/dependency_links.txt
```

### Comparing `pytest_time-0.1.0/tests/unit/test_fake_time.py` & `pytest_time-0.1.1/tests/unit/test_fake_time.py`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/tests/unit/test_instant_sleep.py` & `pytest_time-0.1.1/tests/unit/test_instant_sleep.py`

 * *Files identical despite different names*

### Comparing `pytest_time-0.1.0/tox.ini` & `pytest_time-0.1.1/tox.ini`

 * *Files identical despite different names*

