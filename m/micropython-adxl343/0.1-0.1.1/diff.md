# Comparing `tmp/micropython-adxl343-0.1.tar.gz` & `tmp/micropython-adxl343-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-adxl343-0.1.tar", last modified: Wed Jun 14 19:41:23 2023, max compression
+gzip compressed data, was "micropython-adxl343-0.1.1.tar", last modified: Sat Jun 17 14:35:04 2023, max compression
```

## Comparing `micropython-adxl343-0.1.tar` & `micropython-adxl343-0.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:41:23.756220 micropython-adxl343-0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:41:23.748219 micropython-adxl343-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:41:23.752220 micropython-adxl343-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-14 19:41:23.756220 micropython-adxl343-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:41:23.752220 micropython-adxl343-0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:41:23.752220 micropython-adxl343-0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:41:23.756220 micropython-adxl343-0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/examples/adxl343_acceleration_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/examples/adxl343_activity_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/examples/adxl343_double_tap_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/examples/adxl343_inactivity_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/examples/adxl343_resolution_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/examples/adxl343_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/examples/adxl343_single_tap_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:41:23.756220 micropython-adxl343-0.1/micropython_adxl343/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/micropython_adxl343/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15861 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/micropython_adxl343/adxl343.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/micropython_adxl343/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 19:41:23.756220 micropython-adxl343-0.1/micropython_adxl343.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-14 19:41:23.000000 micropython-adxl343-0.1/micropython_adxl343.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-14 19:41:23.000000 micropython-adxl343-0.1/micropython_adxl343.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 19:41:23.000000 micropython-adxl343-0.1/micropython_adxl343.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-14 19:41:23.000000 micropython-adxl343-0.1/micropython_adxl343.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-14 19:41:23.000000 micropython-adxl343-0.1/micropython_adxl343.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-14 19:41:14.000000 micropython-adxl343-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-14 19:41:01.000000 micropython-adxl343-0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 19:41:23.756220 micropython-adxl343-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.574675 micropython-adxl343-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.574675 micropython-adxl343-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.574675 micropython-adxl343-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_acceleration_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_activity_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_double_tap_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_inactivity_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_resolution_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/examples/adxl343_single_tap_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/micropython_adxl343/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/micropython_adxl343/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/micropython_adxl343/adxl343.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/micropython_adxl343/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 14:35:04.000000 micropython-adxl343-0.1.1/micropython_adxl343.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-17 14:34:55.000000 micropython-adxl343-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:34:47.000000 micropython-adxl343-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:35:04.578675 micropython-adxl343-0.1.1/setup.cfg
```

### Comparing `micropython-adxl343-0.1/.gitignore` & `micropython-adxl343-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/.pre-commit-config.yaml` & `micropython-adxl343-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/.pylintrc` & `micropython-adxl343-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/LICENSE` & `micropython-adxl343-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/PKG-INFO` & `micropython-adxl343-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-adxl343
-Version: 0.1
+Version: 0.1.1
 Summary: MicroPython Driver for the Analog Devices ADXL343 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADXL343
 Keywords: sensor,micropython,adxl343,tap,double,activity,acceleration,accelerometer,adxl343,micropython,gravity,sensor,driver
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-adxl343/badge/?version=latest
     :target: https://micropython-adxl343.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-adxl343.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-adxl343-0.1/README.rst` & `micropython-adxl343-0.1.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-adxl343/badge/?version=latest
     :target: https://micropython-adxl343.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-adxl343.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-adxl343-0.1/docs/_static/Logo.png` & `micropython-adxl343-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/docs/_static/favicon.ico` & `micropython-adxl343-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/docs/conf.py` & `micropython-adxl343-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/docs/examples.rst` & `micropython-adxl343-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/examples/adxl343_acceleration_range.py` & `micropython-adxl343-0.1.1/examples/adxl343_acceleration_range.py`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/examples/adxl343_double_tap_mode.py` & `micropython-adxl343-0.1.1/examples/adxl343_double_tap_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/examples/adxl343_resolution_mode.py` & `micropython-adxl343-0.1.1/examples/adxl343_resolution_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/examples.json` & `micropython-adxl343-0.1.1/examples.json`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/micropython_adxl343/adxl343.py` & `micropython-adxl343-0.1.1/micropython_adxl343/adxl343.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 #
 # SPDX-License-Identifier: MIT
+
 """
 `adxl343`
 ================================================================================
 
 MicroPython Driver for the Analog Devices ADXL343 Accelerometer
 
 
@@ -18,15 +19,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_ADXL343.git"
 
 _STANDARD_GRAVITY = 9.80665
 _REG_WHOAMI = const(0x00)
 _POWER_CTL = const(0x2D)
 _DATA_FORMAT = const(0x31)
 _ACC = const(0x32)
```

### Comparing `micropython-adxl343-0.1/micropython_adxl343/i2c_helpers.py` & `micropython-adxl343-0.1.1/micropython_adxl343/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/micropython_adxl343.egg-info/PKG-INFO` & `micropython-adxl343-0.1.1/micropython_adxl343.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-adxl343
-Version: 0.1
+Version: 0.1.1
 Summary: MicroPython Driver for the Analog Devices ADXL343 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADXL343
 Keywords: sensor,micropython,adxl343,tap,double,activity,acceleration,accelerometer,adxl343,micropython,gravity,sensor,driver
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-adxl343/badge/?version=latest
     :target: https://micropython-adxl343.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-adxl343.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-adxl343-0.1/micropython_adxl343.egg-info/SOURCES.txt` & `micropython-adxl343-0.1.1/micropython_adxl343.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micropython-adxl343-0.1/pyproject.toml` & `micropython-adxl343-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-adxl343"
 description = "MicroPython Driver for the Analog Devices ADXL343 Accelerometer"
-version = "0.1"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_ADXL343"}
 keywords = [
     "sensor",
@@ -36,15 +36,15 @@
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
 py-modules = ["adxl343"]
 
 [tool.setuptools.dynamic]
```

