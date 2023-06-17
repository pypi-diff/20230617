# Comparing `tmp/micropython-bma220-0.1.0.tar.gz` & `tmp/micropython-bma220-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-bma220-0.1.0.tar", last modified: Thu Jun 15 17:17:14 2023, max compression
+gzip compressed data, was "micropython-bma220-0.1.1.tar", last modified: Sat Jun 17 14:00:39 2023, max compression
```

## Comparing `micropython-bma220-0.1.0.tar` & `micropython-bma220-0.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:17:13.995916 micropython-bma220-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:17:13.987916 micropython-bma220-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:17:13.987916 micropython-bma220-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-15 17:17:13.991916 micropython-bma220-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:17:13.987916 micropython-bma220-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:17:13.991916 micropython-bma220-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:17:13.991916 micropython-bma220-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_acc_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_double_tap_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_filter_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_latched_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_lowg_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_sleep_duration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_slope_slope_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/examples/bma220_slope_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:17:13.991916 micropython-bma220-0.1.0/micropython_bma220/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/micropython_bma220/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/micropython_bma220/bma220.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/micropython_bma220/bma220_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/micropython_bma220/bma220_lowg_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/micropython_bma220/bma220_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/micropython_bma220/bma220_slope.py
--rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/micropython_bma220/bma220_tap_sensing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/micropython_bma220/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 17:17:13.991916 micropython-bma220-0.1.0/micropython_bma220.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-15 17:17:13.000000 micropython-bma220-0.1.0/micropython_bma220.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-15 17:17:13.000000 micropython-bma220-0.1.0/micropython_bma220.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 17:17:13.000000 micropython-bma220-0.1.0/micropython_bma220.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 17:17:13.000000 micropython-bma220-0.1.0/micropython_bma220.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 17:17:13.000000 micropython-bma220-0.1.0/micropython_bma220.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/packages.json
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-15 17:17:05.000000 micropython-bma220-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-15 17:16:55.000000 micropython-bma220-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 17:17:13.995916 micropython-bma220-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.151820 micropython-bma220-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.139820 micropython-bma220-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.143820 micropython-bma220-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-17 14:00:39.151820 micropython-bma220-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.143820 micropython-bma220-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.143820 micropython-bma220-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.147820 micropython-bma220-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_double_tap_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_filter_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_latched_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_lowg_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_sleep_duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_slope_slope_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/examples/bma220_slope_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.147820 micropython-bma220-0.1.1/micropython_bma220/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_lowg_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_slope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13350 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/bma220_tap_sensing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/micropython_bma220/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:00:39.151820 micropython-bma220-0.1.1/micropython_bma220.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 14:00:39.000000 micropython-bma220-0.1.1/micropython_bma220.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-17 14:00:28.000000 micropython-bma220-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:00:16.000000 micropython-bma220-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:00:39.151820 micropython-bma220-0.1.1/setup.cfg
```

### Comparing `micropython-bma220-0.1.0/.gitignore` & `micropython-bma220-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/.pre-commit-config.yaml` & `micropython-bma220-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/.pylintrc` & `micropython-bma220-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/LICENSE` & `micropython-bma220-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/PKG-INFO` & `micropython-bma220-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: micropython-bma220
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Bosch BMA220 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMA220
 Keywords: sensor,micropython,bma220,acceleration,driver,bosch,bma220,accelerometer,gravity,slope,tap,orientation
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
 .. image:: https://readthedocs.org/projects/micropython-bma220/badge/?version=latest
     :target: https://micropython-bma220.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-
 .. image:: https://img.shields.io/pypi/v/micropython-bma220.svg
     :alt: latest version on PyPI
     :target: https://pypi.python.org/pypi/micropython-bma220
 
 .. image:: https://static.pepy.tech/personalized-badge/micropython-bma220?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
     :alt: Total PyPI downloads
     :target: https://pepy.tech/project/micropython-bma220
```

### Comparing `micropython-bma220-0.1.0/README.rst` & `micropython-bma220-0.1.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-bma220/badge/?version=latest
     :target: https://micropython-bma220.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-
 .. image:: https://img.shields.io/pypi/v/micropython-bma220.svg
     :alt: latest version on PyPI
     :target: https://pypi.python.org/pypi/micropython-bma220
 
 .. image:: https://static.pepy.tech/personalized-badge/micropython-bma220?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
     :alt: Total PyPI downloads
     :target: https://pepy.tech/project/micropython-bma220
```

### Comparing `micropython-bma220-0.1.0/docs/_static/Logo.png` & `micropython-bma220-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/docs/_static/favicon.ico` & `micropython-bma220-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/docs/conf.py` & `micropython-bma220-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/docs/examples.rst` & `micropython-bma220-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/examples/bma220_acc_range.py` & `micropython-bma220-0.1.1/examples/bma220_acc_range.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/examples/bma220_double_tap_test.py` & `micropython-bma220-0.1.1/examples/bma220_double_tap_test.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/examples/bma220_filter_bandwidth.py` & `micropython-bma220-0.1.1/examples/bma220_filter_bandwidth.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/examples/bma220_latched_mode.py` & `micropython-bma220-0.1.1/examples/bma220_latched_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/examples/bma220_orientation.py` & `micropython-bma220-0.1.1/examples/bma220_orientation.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/examples/bma220_sleep_duration.py` & `micropython-bma220-0.1.1/examples/bma220_sleep_duration.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/examples/bma220_slope_slope_sign.py` & `micropython-bma220-0.1.1/examples/bma220_slope_slope_sign.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/examples/bma220_slope_test.py` & `micropython-bma220-0.1.1/examples/bma220_slope_test.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/examples.json` & `micropython-bma220-0.1.1/examples.json`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/micropython_bma220/bma220.py` & `micropython-bma220-0.1.1/micropython_bma220/bma220.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _REG_WHOAMI = const(0x00)
 _FILTER_CONF = const(0x20)
 _ACC_RANGE = const(0x22)
 _SLEEP_CONF = const(0x0F)
 _LATCH_CONF = const(0x1C)
```

### Comparing `micropython-bma220-0.1.0/micropython_bma220/bma220_const.py` & `micropython-bma220-0.1.1/micropython_bma220/bma220_const.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * Author(s): Jose D. Montoya
 
 
 """
 
 from micropython import const
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 # pylint: disable=duplicate-code
 # Acceleration range
 ACC_RANGE_2 = const(0b00)
 ACC_RANGE_4 = const(0b01)
 ACC_RANGE_8 = const(0b10)
```

### Comparing `micropython-bma220-0.1.0/micropython_bma220/bma220_lowg_detection.py` & `micropython-bma220-0.1.1/micropython_bma220/bma220_lowg_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # pylint: disable=useless-parent-delegation,no-name-in-module
 
 from micropython import const
 from micropython_bma220.i2c_helpers import CBits
 from micropython_bma220.bma220 import BMA220
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _CONF = const(0x1A)
 _LG_CONF = const(0x1C)
 _LG_CONF2 = const(0x0E)
 _LG_CONF3 = const(0x0C)
 _INTERRUPTS = const(0x18)
```

### Comparing `micropython-bma220-0.1.0/micropython_bma220/bma220_orientation.py` & `micropython-bma220-0.1.1/micropython_bma220/bma220_orientation.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 from micropython import const
 from micropython_bma220.i2c_helpers import CBits
 from micropython_bma220.bma220 import BMA220
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _CONF = const(0x1A)
 _ORIENT_EX = const(0x12)
 _INTERRUPTS = const(0x16)
 
 # Orientation Enabled
```

### Comparing `micropython-bma220-0.1.0/micropython_bma220/bma220_slope.py` & `micropython-bma220-0.1.1/micropython_bma220/bma220_slope.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from micropython_bma220.bma220 import BMA220
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _CONF = const(0x1A)
 _SLOPE_INFO = const(0x12)
 _SLOPE_INFO2 = const(0x16)
 _INTERRUPTS = const(0x18)
```

### Comparing `micropython-bma220-0.1.0/micropython_bma220/bma220_tap_sensing.py` & `micropython-bma220-0.1.1/micropython_bma220/bma220_tap_sensing.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from micropython_bma220.bma220 import BMA220
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMA220.git"
 
 _CONF = const(0x1A)
 _TT_INFO = const(0x10)
 _TT_INFO2 = const(0x16)
 _INTERRUPTS = const(0x18)
```

### Comparing `micropython-bma220-0.1.0/micropython_bma220/i2c_helpers.py` & `micropython-bma220-0.1.1/micropython_bma220/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/micropython_bma220.egg-info/PKG-INFO` & `micropython-bma220-0.1.1/micropython_bma220.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: micropython-bma220
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Bosch BMA220 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMA220
 Keywords: sensor,micropython,bma220,acceleration,driver,bosch,bma220,accelerometer,gravity,slope,tap,orientation
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
 .. image:: https://readthedocs.org/projects/micropython-bma220/badge/?version=latest
     :target: https://micropython-bma220.readthedocs.io/en/latest/
     :alt: Documentation Status
 
-
 .. image:: https://img.shields.io/pypi/v/micropython-bma220.svg
     :alt: latest version on PyPI
     :target: https://pypi.python.org/pypi/micropython-bma220
 
 .. image:: https://static.pepy.tech/personalized-badge/micropython-bma220?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
     :alt: Total PyPI downloads
     :target: https://pepy.tech/project/micropython-bma220
```

### Comparing `micropython-bma220-0.1.0/micropython_bma220.egg-info/SOURCES.txt` & `micropython-bma220-0.1.1/micropython_bma220.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/packages.json` & `micropython-bma220-0.1.1/packages.json`

 * *Files identical despite different names*

### Comparing `micropython-bma220-0.1.0/pyproject.toml` & `micropython-bma220-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-bma220"
 description = "MicroPython Driver for the Bosch BMA220 Accelerometer"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_BMA220"}
 keywords = [
     "sensor",
@@ -35,15 +35,15 @@
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
 py-modules = ["bma220"]
 
 [tool.setuptools.dynamic]
```

