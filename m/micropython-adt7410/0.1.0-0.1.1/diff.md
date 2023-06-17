# Comparing `tmp/micropython-adt7410-0.1.0.tar.gz` & `tmp/micropython-adt7410-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-adt7410-0.1.0.tar", last modified: Mon Jun 12 17:33:44 2023, max compression
+gzip compressed data, was "micropython-adt7410-0.1.1.tar", last modified: Sat Jun 17 15:38:21 2023, max compression
```

## Comparing `micropython-adt7410-0.1.0.tar` & `micropython-adt7410-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:33:44.419547 micropython-adt7410-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:33:44.407547 micropython-adt7410-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:33:44.411547 micropython-adt7410-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-12 17:33:44.419547 micropython-adt7410-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:33:44.415547 micropython-adt7410-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:33:44.415547 micropython-adt7410-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:33:44.415547 micropython-adt7410-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-12 17:33:34.000000 micropython-adt7410-0.1.0/examples/adt7410_operation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-12 17:33:34.000000 micropython-adt7410-0.1.0/examples/adt7410_resolution_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-12 17:33:34.000000 micropython-adt7410-0.1.0/examples/adt7410_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-12 17:33:34.000000 micropython-adt7410-0.1.0/examples/adt7410_temp_limits.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:33:44.419547 micropython-adt7410-0.1.0/micropython_adt7410/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:33:34.000000 micropython-adt7410-0.1.0/micropython_adt7410/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-12 17:33:34.000000 micropython-adt7410-0.1.0/micropython_adt7410/adt7410.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-12 17:33:34.000000 micropython-adt7410-0.1.0/micropython_adt7410/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:33:44.419547 micropython-adt7410-0.1.0/micropython_adt7410.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-12 17:33:44.000000 micropython-adt7410-0.1.0/micropython_adt7410.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-12 17:33:44.000000 micropython-adt7410-0.1.0/micropython_adt7410.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:33:44.000000 micropython-adt7410-0.1.0/micropython_adt7410.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-12 17:33:44.000000 micropython-adt7410-0.1.0/micropython_adt7410.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 17:33:44.000000 micropython-adt7410-0.1.0/micropython_adt7410.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-12 17:33:34.000000 micropython-adt7410-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-12 17:33:17.000000 micropython-adt7410-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:33:44.419547 micropython-adt7410-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.207476 micropython-adt7410-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/examples/adt7410_operation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/examples/adt7410_resolution_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/examples/adt7410_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/examples/adt7410_temp_limits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/micropython_adt7410/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/micropython_adt7410/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/micropython_adt7410/adt7410.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/micropython_adt7410/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 15:38:21.000000 micropython-adt7410-0.1.1/micropython_adt7410.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-17 15:38:13.000000 micropython-adt7410-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:38:02.000000 micropython-adt7410-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:38:21.211476 micropython-adt7410-0.1.1/setup.cfg
```

### Comparing `micropython-adt7410-0.1.0/.gitignore` & `micropython-adt7410-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/.pre-commit-config.yaml` & `micropython-adt7410-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/.pylintrc` & `micropython-adt7410-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/LICENSE` & `micropython-adt7410-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/PKG-INFO` & `micropython-adt7410-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-adt7410
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Analog Devices ADT7410 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADT7410
 Keywords: sensor,micropython,adt7410,temperature,adt7410,sensor,driver,micropython
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
 .. image:: https://readthedocs.org/projects/micropython-adt7410/badge/?version=latest
     :target: https://micropython-adt7410.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-adt7410.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-adt7410-0.1.0/README.rst` & `micropython-adt7410-0.1.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-adt7410/badge/?version=latest
     :target: https://micropython-adt7410.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-adt7410.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-adt7410-0.1.0/docs/_static/Logo.png` & `micropython-adt7410-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/docs/_static/favicon.ico` & `micropython-adt7410-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/docs/conf.py` & `micropython-adt7410-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/docs/examples.rst` & `micropython-adt7410-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/examples/adt7410_operation_mode.py` & `micropython-adt7410-0.1.1/examples/adt7410_operation_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/examples/adt7410_resolution_mode.py` & `micropython-adt7410-0.1.1/examples/adt7410_resolution_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/examples/adt7410_temp_limits.py` & `micropython-adt7410-0.1.1/examples/adt7410_temp_limits.py`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/examples.json` & `micropython-adt7410-0.1.1/examples.json`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/micropython_adt7410/adt7410.py` & `micropython-adt7410-0.1.1/micropython_adt7410/adt7410.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import time
 from collections import namedtuple
 from micropython import const
 from micropython_adt7410.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_ADT7410.git"
 
 
 _REG_WHOAMI = const(0xB)
 _TEMP = const(0x00)
 _STATUS = const(0x02)
 _CONFIGURATION = const(0x03)
```

### Comparing `micropython-adt7410-0.1.0/micropython_adt7410/i2c_helpers.py` & `micropython-adt7410-0.1.1/micropython_adt7410/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/micropython_adt7410.egg-info/PKG-INFO` & `micropython-adt7410-0.1.1/micropython_adt7410.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-adt7410
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Analog Devices ADT7410 Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ADT7410
 Keywords: sensor,micropython,adt7410,temperature,adt7410,sensor,driver,micropython
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
 .. image:: https://readthedocs.org/projects/micropython-adt7410/badge/?version=latest
     :target: https://micropython-adt7410.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-adt7410.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-adt7410-0.1.0/micropython_adt7410.egg-info/SOURCES.txt` & `micropython-adt7410-0.1.1/micropython_adt7410.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micropython-adt7410-0.1.0/pyproject.toml` & `micropython-adt7410-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-adt7410"
 description = "MicroPython Driver for the Analog Devices ADT7410 Temperature Sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_ADT7410"}
 keywords = [
     "sensor",
@@ -31,15 +31,15 @@
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
 py-modules = ["adt7410"]
 
 [tool.setuptools.dynamic]
```

