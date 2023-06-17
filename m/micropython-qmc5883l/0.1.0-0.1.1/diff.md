# Comparing `tmp/micropython-qmc5883l-0.1.0.tar.gz` & `tmp/micropython-qmc5883l-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-qmc5883l-0.1.0.tar", last modified: Sun Jun 11 00:42:23 2023, max compression
+gzip compressed data, was "micropython-qmc5883l-0.1.1.tar", last modified: Sat Jun 17 14:51:06 2023, max compression
```

## Comparing `micropython-qmc5883l-0.1.0.tar` & `micropython-qmc5883l-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:42:23.423462 micropython-qmc5883l-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:42:23.419462 micropython-qmc5883l-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:42:23.423462 micropython-qmc5883l-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-11 00:42:23.423462 micropython-qmc5883l-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:42:23.423462 micropython-qmc5883l-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:42:23.423462 micropython-qmc5883l-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:42:23.423462 micropython-qmc5883l-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/examples/qmc5883l_advanced_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/examples/qmc5883l_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/examples/qmc5883l_field_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/examples/qmc5883l_magnetic_compass.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/examples/qmc5883l_oversample.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/examples/qmc5883l_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:42:23.423462 micropython-qmc5883l-0.1.0/micropython_qmc5883l/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/micropython_qmc5883l/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/micropython_qmc5883l/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/micropython_qmc5883l/qmc5883l.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 00:42:23.423462 micropython-qmc5883l-0.1.0/micropython_qmc5883l.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-11 00:42:23.000000 micropython-qmc5883l-0.1.0/micropython_qmc5883l.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-11 00:42:23.000000 micropython-qmc5883l-0.1.0/micropython_qmc5883l.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 00:42:23.000000 micropython-qmc5883l-0.1.0/micropython_qmc5883l.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-11 00:42:23.000000 micropython-qmc5883l-0.1.0/micropython_qmc5883l.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-11 00:42:23.000000 micropython-qmc5883l-0.1.0/micropython_qmc5883l.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-11 00:42:16.000000 micropython-qmc5883l-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-11 00:42:08.000000 micropython-qmc5883l-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 00:42:23.423462 micropython-qmc5883l-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.542938 micropython-qmc5883l-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-17 14:51:06.542938 micropython-qmc5883l-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_advanced_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_field_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_magnetic_compass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_oversample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/examples/qmc5883l_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.538938 micropython-qmc5883l-0.1.1/micropython_qmc5883l/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10661 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l/qmc5883l.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:51:06.542938 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 14:51:06.000000 micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-17 14:50:58.000000 micropython-qmc5883l-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:50:50.000000 micropython-qmc5883l-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:51:06.542938 micropython-qmc5883l-0.1.1/setup.cfg
```

### Comparing `micropython-qmc5883l-0.1.0/.gitignore` & `micropython-qmc5883l-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/.pre-commit-config.yaml` & `micropython-qmc5883l-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/.pylintrc` & `micropython-qmc5883l-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/LICENSE` & `micropython-qmc5883l-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/PKG-INFO` & `micropython-qmc5883l-0.1.1/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-Metadata-Version: 2.1
-Name: micropython-qmc5883l
-Version: 0.1.0
-Summary: MicroPython Driver for the QMC5883L Accelerometer
-Author-email: JDM <xxyx@mailmeto.mozmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/jposada202020/MicroPython_QMC5883L
-Keywords: sensor,micropython,qmc5883l,acceleration,heading,driver,sensor,gravity,micropython,accelerometer
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Embedded Systems
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-qmc5883l/badge/?version=latest
     :target: https://micropython-qmc5883l.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-qmc5883l.svg
     :alt: latest version on PyPI
@@ -34,14 +21,45 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the QMC5883L Accelerometer
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_QMC5883L
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_QMC5883L
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_QMC5883L/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_QMC5883L/examples.json
+
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-qmc5883l/>`_.
```

### Comparing `micropython-qmc5883l-0.1.0/docs/_static/Logo.png` & `micropython-qmc5883l-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/docs/_static/favicon.ico` & `micropython-qmc5883l-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/docs/conf.py` & `micropython-qmc5883l-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/docs/examples.rst` & `micropython-qmc5883l-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/examples/qmc5883l_advanced_settings.py` & `micropython-qmc5883l-0.1.1/examples/qmc5883l_advanced_settings.py`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/examples/qmc5883l_data_rate.py` & `micropython-qmc5883l-0.1.1/examples/qmc5883l_data_rate.py`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/examples/qmc5883l_field_range.py` & `micropython-qmc5883l-0.1.1/examples/qmc5883l_field_range.py`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/examples/qmc5883l_magnetic_compass.py` & `micropython-qmc5883l-0.1.1/examples/qmc5883l_magnetic_compass.py`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/examples/qmc5883l_oversample.py` & `micropython-qmc5883l-0.1.1/examples/qmc5883l_oversample.py`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/micropython_qmc5883l/i2c_helpers.py` & `micropython-qmc5883l-0.1.1/micropython_qmc5883l/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-qmc5883l-0.1.0/micropython_qmc5883l/qmc5883l.py` & `micropython-qmc5883l-0.1.1/micropython_qmc5883l/qmc5883l.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """
 
 import time
 from micropython import const
 from micropython_qmc5883l.i2c_helpers import CBits, RegisterStruct
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_QMC5883L.git"
 
 _REG_WHOAMI = const(0x0D)
 _REG_SET_RESET = const(0x0B)
 _REG_OPERATION_MODE = const(0x09)
 _REG_STATUS = const(0x06)
```

### Comparing `micropython-qmc5883l-0.1.0/micropython_qmc5883l.egg-info/PKG-INFO` & `micropython-qmc5883l-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-qmc5883l
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the QMC5883L Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_QMC5883L
 Keywords: sensor,micropython,qmc5883l,acceleration,heading,driver,sensor,gravity,micropython,accelerometer
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
 .. image:: https://readthedocs.org/projects/micropython-qmc5883l/badge/?version=latest
     :target: https://micropython-qmc5883l.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-qmc5883l.svg
     :alt: latest version on PyPI
@@ -34,14 +38,45 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the QMC5883L Accelerometer
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_QMC5883L
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_QMC5883L
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_QMC5883L/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_QMC5883L/examples.json
+
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-qmc5883l/>`_.
```

### Comparing `micropython-qmc5883l-0.1.0/micropython_qmc5883l.egg-info/SOURCES.txt` & `micropython-qmc5883l-0.1.1/micropython_qmc5883l.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 LICENSE
 README.rst
+examples.json
+packages.json
 pyproject.toml
 requirements.txt
 .github/workflows/release_pypi.yml
 docs/api.rst
 docs/conf.py
 docs/examples.rst
 docs/index.rst
```

### Comparing `micropython-qmc5883l-0.1.0/pyproject.toml` & `micropython-qmc5883l-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-qmc5883l"
 description = "MicroPython Driver for the QMC5883L Accelerometer"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_QMC5883L"}
 keywords = [
     "sensor",
@@ -33,15 +33,15 @@
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
 py-modules = ["qmc5883l"]
 
 [tool.setuptools.dynamic]
```

