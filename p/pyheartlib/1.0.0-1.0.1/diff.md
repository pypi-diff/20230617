# Comparing `tmp/pyheartlib-1.0.0.tar.gz` & `tmp/pyheartlib-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyheartlib-1.0.0.tar", max compression
+gzip compressed data, was "pyheartlib-1.0.1.tar", max compression
```

## Comparing `pyheartlib-1.0.0.tar` & `pyheartlib-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    34522 2023-06-17 15:46:50.319715 pyheartlib-1.0.0/LICENSE
--rw-r--r--   0        0        0     2648 2023-06-17 15:46:50.319715 pyheartlib-1.0.0/README.md
--rw-r--r--   0        0        0     1593 2023-06-17 15:48:13.280544 pyheartlib-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      113 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/__init__.py
--rw-r--r--   0        0        0       54 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/archs/__init__.py
--rw-r--r--   0        0        0    18449 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/beat_info.py
--rw-r--r--   0        0        0     1179 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/config.yaml
--rw-r--r--   0        0        0     5491 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/data.py
--rw-r--r--   0        0        0     9217 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/data_arrhythmia.py
--rw-r--r--   0        0        0    24741 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/data_beat.py
--rw-r--r--   0        0        0     9480 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/data_rpeak.py
--rw-r--r--   0        0        0       39 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/extra/__init__.py
--rw-r--r--   0        0        0     3841 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/extra/pqrst.py
--rw-r--r--   0        0        0     2979 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/extra/report.py
--rw-r--r--   0        0        0     6063 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/extra/utils.py
--rw-r--r--   0        0        0     6150 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/features.py
--rw-r--r--   0        0        0     2579 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/io.py
--rw-r--r--   0        0        0     5773 2023-06-17 15:46:50.327715 pyheartlib-1.0.0/src/pyheartlib/processing.py
--rw-r--r--   0        0        0     3579 1970-01-01 00:00:00.000000 pyheartlib-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    34522 2023-06-17 16:34:56.667933 pyheartlib-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2648 2023-06-17 16:34:56.667933 pyheartlib-1.0.1/README.md
+-rw-r--r--   0        0        0     1620 2023-06-17 16:36:43.093351 pyheartlib-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/archs/__init__.py
+-rw-r--r--   0        0        0    18449 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/beat_info.py
+-rw-r--r--   0        0        0     1179 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/config.yaml
+-rw-r--r--   0        0        0     5491 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/data.py
+-rw-r--r--   0        0        0     9217 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/data_arrhythmia.py
+-rw-r--r--   0        0        0    24741 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/data_beat.py
+-rw-r--r--   0        0        0     9480 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/data_rpeak.py
+-rw-r--r--   0        0        0       39 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/extra/__init__.py
+-rw-r--r--   0        0        0     3841 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/extra/pqrst.py
+-rw-r--r--   0        0        0     2979 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/extra/report.py
+-rw-r--r--   0        0        0     6063 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/extra/utils.py
+-rw-r--r--   0        0        0     6150 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/features.py
+-rw-r--r--   0        0        0     2579 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/io.py
+-rw-r--r--   0        0        0     5773 2023-06-17 16:34:56.675933 pyheartlib-1.0.1/src/pyheartlib/processing.py
+-rw-r--r--   0        0        0     3645 1970-01-01 00:00:00.000000 pyheartlib-1.0.1/PKG-INFO
```

### Comparing `pyheartlib-1.0.0/LICENSE` & `pyheartlib-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/README.md` & `pyheartlib-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/pyproject.toml` & `pyheartlib-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "pyheartlib"
-version = "1.0.0"
+version = "1.0.1"
 description = "A Python package for processing electrocardiogram signals"
-authors = ["devnums"]
-license = "Proprietary"
+authors = ["devnums <devnums.code@gmail.com>"]
+license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/devnums/pyheartlib"
 documentation = "https://pyheartlib.readthedocs.io"
 keywords = ["electrocardiogram", "ECG"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `pyheartlib-1.0.0/src/pyheartlib/beat_info.py` & `pyheartlib-1.0.1/src/pyheartlib/beat_info.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/config.yaml` & `pyheartlib-1.0.1/src/pyheartlib/config.yaml`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/data.py` & `pyheartlib-1.0.1/src/pyheartlib/data.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/data_arrhythmia.py` & `pyheartlib-1.0.1/src/pyheartlib/data_arrhythmia.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/data_beat.py` & `pyheartlib-1.0.1/src/pyheartlib/data_beat.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/data_rpeak.py` & `pyheartlib-1.0.1/src/pyheartlib/data_rpeak.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/extra/pqrst.py` & `pyheartlib-1.0.1/src/pyheartlib/extra/pqrst.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/extra/report.py` & `pyheartlib-1.0.1/src/pyheartlib/extra/report.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/extra/utils.py` & `pyheartlib-1.0.1/src/pyheartlib/extra/utils.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/features.py` & `pyheartlib-1.0.1/src/pyheartlib/features.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/io.py` & `pyheartlib-1.0.1/src/pyheartlib/io.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/src/pyheartlib/processing.py` & `pyheartlib-1.0.1/src/pyheartlib/processing.py`

 * *Files identical despite different names*

### Comparing `pyheartlib-1.0.0/PKG-INFO` & `pyheartlib-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pyheartlib
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package for processing electrocardiogram signals
 Home-page: https://github.com/devnums/pyheartlib
-License: Proprietary
+License: AGPL-3.0-only
 Keywords: electrocardiogram,ECG
 Author: devnums
+Author-email: devnums.code@gmail.com
 Requires-Python: >=3.10,<3.12
-Classifier: License :: Other/Proprietary License
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3.5.2)
 Requires-Dist: numpy (>=1.22.0)
 Requires-Dist: pandas (>=1.4.0)
 Requires-Dist: pyyaml (>=6.0)
```

