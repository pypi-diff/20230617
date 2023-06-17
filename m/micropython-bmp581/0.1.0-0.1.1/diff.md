# Comparing `tmp/micropython-bmp581-0.1.0.tar.gz` & `tmp/micropython-bmp581-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-bmp581-0.1.0.tar", last modified: Mon Jun 12 01:42:16 2023, max compression
+gzip compressed data, was "micropython-bmp581-0.1.1.tar", last modified: Sat Jun 17 15:28:30 2023, max compression
```

## Comparing `micropython-bmp581-0.1.0.tar` & `micropython-bmp581-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:42:16.068493 micropython-bmp581-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:42:16.064493 micropython-bmp581-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:42:16.064493 micropython-bmp581-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-12 01:42:16.068493 micropython-bmp581-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:42:16.064493 micropython-bmp581-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:42:16.068493 micropython-bmp581-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:42:16.068493 micropython-bmp581-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/examples/bmp581_output_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/examples/bmp581_power_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/examples/bmp581_pressure_oversample_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/examples/bmp581_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/examples/bmp581_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/examples/bmp581_temperature_oversample_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:42:16.068493 micropython-bmp581-0.1.0/micropython_bmp581/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/micropython_bmp581/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/micropython_bmp581/bmp581.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/micropython_bmp581/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:42:16.068493 micropython-bmp581-0.1.0/micropython_bmp581.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-12 01:42:16.000000 micropython-bmp581-0.1.0/micropython_bmp581.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-12 01:42:16.000000 micropython-bmp581-0.1.0/micropython_bmp581.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 01:42:16.000000 micropython-bmp581-0.1.0/micropython_bmp581.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 01:42:16.000000 micropython-bmp581-0.1.0/micropython_bmp581.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 01:42:16.000000 micropython-bmp581-0.1.0/micropython_bmp581.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-12 01:42:08.000000 micropython-bmp581-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 01:42:01.000000 micropython-bmp581-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 01:42:16.068493 micropython-bmp581-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.499702 micropython-bmp581-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.503702 micropython-bmp581-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.503702 micropython-bmp581-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.503702 micropython-bmp581-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_power_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_pressure_oversample_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/examples/bmp581_temperature_oversample_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/micropython_bmp581/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/micropython_bmp581/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/micropython_bmp581/bmp581.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/micropython_bmp581/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 15:28:30.000000 micropython-bmp581-0.1.1/micropython_bmp581.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-17 15:28:20.000000 micropython-bmp581-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:28:05.000000 micropython-bmp581-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:28:30.507702 micropython-bmp581-0.1.1/setup.cfg
```

### Comparing `micropython-bmp581-0.1.0/.gitignore` & `micropython-bmp581-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/.pre-commit-config.yaml` & `micropython-bmp581-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/.pylintrc` & `micropython-bmp581-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/LICENSE` & `micropython-bmp581-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/PKG-INFO` & `micropython-bmp581-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-bmp581
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Bosch BMP581 pressure sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMP581
 Keywords: sensor,micropython,bmp581,pressure,altitude,bosch,bmp581,micropython,sensor,pressure,altitude
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
 .. image:: https://readthedocs.org/projects/micropython-bmp581/badge/?version=latest
     :target: https://micropython-bmp581.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-bmp581.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-bmp581-0.1.0/README.rst` & `micropython-bmp581-0.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-bmp581/badge/?version=latest
     :target: https://micropython-bmp581.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-bmp581.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-bmp581-0.1.0/docs/_static/Logo.png` & `micropython-bmp581-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/docs/_static/favicon.ico` & `micropython-bmp581-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/docs/conf.py` & `micropython-bmp581-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/docs/examples.rst` & `micropython-bmp581-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/examples/bmp581_output_data_rate.py` & `micropython-bmp581-0.1.1/examples/bmp581_output_data_rate.py`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/examples/bmp581_power_mode.py` & `micropython-bmp581-0.1.1/examples/bmp581_power_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/examples/bmp581_pressure_oversample_rate.py` & `micropython-bmp581-0.1.1/examples/bmp581_pressure_oversample_rate.py`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/examples/bmp581_temperature_oversample_rate.py` & `micropython-bmp581-0.1.1/examples/bmp581_temperature_oversample_rate.py`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/examples.json` & `micropython-bmp581-0.1.1/examples.json`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/micropython_bmp581/bmp581.py` & `micropython-bmp581-0.1.1/micropython_bmp581/bmp581.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """
 
 from micropython import const
 from micropython_bmp581.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMP581.git"
 
 _REG_WHOAMI = const(0x01)
 _OSR_CONF = const(0x36)
 _ODR_CONFIG = const(0x37)
```

### Comparing `micropython-bmp581-0.1.0/micropython_bmp581/i2c_helpers.py` & `micropython-bmp581-0.1.1/micropython_bmp581/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/micropython_bmp581.egg-info/PKG-INFO` & `micropython-bmp581-0.1.1/micropython_bmp581.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-bmp581
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Bosch BMP581 pressure sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMP581
 Keywords: sensor,micropython,bmp581,pressure,altitude,bosch,bmp581,micropython,sensor,pressure,altitude
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
 .. image:: https://readthedocs.org/projects/micropython-bmp581/badge/?version=latest
     :target: https://micropython-bmp581.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-bmp581.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-bmp581-0.1.0/micropython_bmp581.egg-info/SOURCES.txt` & `micropython-bmp581-0.1.1/micropython_bmp581.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micropython-bmp581-0.1.0/pyproject.toml` & `micropython-bmp581-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-bmp581"
 description = "MicroPython Driver for the Bosch BMP581 pressure sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_BMP581"}
 keywords = [
     "sensor",
@@ -34,15 +34,15 @@
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
 py-modules = ["bmp581"]
 
 [tool.setuptools.dynamic]
```

