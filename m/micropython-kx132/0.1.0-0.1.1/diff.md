# Comparing `tmp/micropython-kx132-0.1.0.tar.gz` & `tmp/micropython-kx132-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-kx132-0.1.0.tar", last modified: Fri Jun  9 13:57:17 2023, max compression
+gzip compressed data, was "micropython-kx132-0.1.1.tar", last modified: Sat Jun 17 15:07:29 2023, max compression
```

## Comparing `micropython-kx132-0.1.0.tar` & `micropython-kx132-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:57:17.831655 micropython-kx132-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:57:17.827655 micropython-kx132-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:57:17.831655 micropython-kx132-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-09 13:57:17.831655 micropython-kx132-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:57:17.831655 micropython-kx132-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:57:17.831655 micropython-kx132-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:57:17.831655 micropython-kx132-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-09 13:57:09.000000 micropython-kx132-0.1.0/examples/kx132_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:57:17.831655 micropython-kx132-0.1.0/micropython_kx132/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:57:09.000000 micropython-kx132-0.1.0/micropython_kx132/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-09 13:57:09.000000 micropython-kx132-0.1.0/micropython_kx132/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-06-09 13:57:09.000000 micropython-kx132-0.1.0/micropython_kx132/kx132.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:57:17.831655 micropython-kx132-0.1.0/micropython_kx132.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-09 13:57:17.000000 micropython-kx132-0.1.0/micropython_kx132.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-09 13:57:17.000000 micropython-kx132-0.1.0/micropython_kx132.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:57:17.000000 micropython-kx132-0.1.0/micropython_kx132.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 13:57:17.000000 micropython-kx132-0.1.0/micropython_kx132.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 13:57:17.000000 micropython-kx132-0.1.0/micropython_kx132.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-09 13:57:09.000000 micropython-kx132-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 13:56:56.000000 micropython-kx132-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:57:17.831655 micropython-kx132-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.891171 micropython-kx132-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.895171 micropython-kx132-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.899171 micropython-kx132-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.899171 micropython-kx132-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.903171 micropython-kx132-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_acc_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_adp_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_previous_tilt_position_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_tap_doubletap_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/examples/kx132_tilt_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/micropython_kx132/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/micropython_kx132/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/micropython_kx132/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/micropython_kx132/kx132.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/micropython_kx132.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 15:07:29.000000 micropython-kx132-0.1.1/micropython_kx132.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-17 15:07:22.000000 micropython-kx132-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:07:15.000000 micropython-kx132-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:07:29.907171 micropython-kx132-0.1.1/setup.cfg
```

### Comparing `micropython-kx132-0.1.0/.gitignore` & `micropython-kx132-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.0/.pre-commit-config.yaml` & `micropython-kx132-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.0/.pylintrc` & `micropython-kx132-0.1.1/.pylintrc`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 jobs=1
 load-plugins=pylint.extensions.no_self_use
 persistent=yes
 unsafe-load-any-extension=no
 
 [MESSAGES CONTROL]
 confidence=
-disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
 disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 enable=
 
 [REPORTS]
 evaluation=10.0 - ((float(5 * error + warning + refactor + convention) / statement) * 10)
 #msg-template=
 output-format=text
```

### Comparing `micropython-kx132-0.1.0/LICENSE` & `micropython-kx132-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.0/PKG-INFO` & `micropython-kx132-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-kx132
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Kionix KX132 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_KX132
 Keywords: sensor,micropython,kx132,acceleration
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
 .. image:: https://readthedocs.org/projects/micropython-kx132/badge/?version=latest
     :target: https://micropython-kx132.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-kx132.svg
     :alt: latest version on PyPI
@@ -34,14 +38,45 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Kionix KX132 Accelerometer
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_KX132
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_KX132
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_KX132/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_KX132/examples.json
+
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-kx132/>`_.
@@ -71,8 +106,7 @@
 =============
 
 Take a look at the examples directory
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://micropython-kx132.readthedocs.io/>`_.
-
```

### Comparing `micropython-kx132-0.1.0/README.rst` & `micropython-kx132-0.1.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-kx132/badge/?version=latest
     :target: https://micropython-kx132.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-kx132.svg
     :alt: latest version on PyPI
@@ -17,14 +21,45 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Kionix KX132 Accelerometer
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_KX132
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_KX132
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_KX132/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_KX132/examples.json
+
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-kx132/>`_.
@@ -54,8 +89,7 @@
 =============
 
 Take a look at the examples directory
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://micropython-kx132.readthedocs.io/>`_.
-
```

### Comparing `micropython-kx132-0.1.0/docs/_static/Logo.png` & `micropython-kx132-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.0/docs/_static/favicon.ico` & `micropython-kx132-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.0/docs/conf.py` & `micropython-kx132-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.0/micropython_kx132/i2c_helpers.py` & `micropython-kx132-0.1.1/micropython_kx132/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-kx132-0.1.0/micropython_kx132/kx132.py` & `micropython-kx132-0.1.1/micropython_kx132/kx132.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 
 
 * Author(s): Jose D. Montoya
 
 
 """
 
+import time
 from micropython import const
 from micropython_kx132.i2c_helpers import CBits, RegisterStruct
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_KX132.git"
 
 _ADP = const(0x02)
 _ACC = const(0x08)
 _REG_WHOAMI = const(0x13)
 _TILT_POSITION = const(0x14)
 _PREVIOUS_TILT_POSITION = const(0x15)
@@ -88,15 +89,15 @@
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
         import kx132
 
-    Once this is done you can define your `board.I2C` object and define your sensor object
+    Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
         i2c = I2C(sda=Pin28), scl=Pin(3))
         kx132 = kx132.KX132(i2c)
 
     Now you have access to the attributes
@@ -131,15 +132,15 @@
     _adp_enabled = CBits(1, _CNTL5, 4)
     _free_fall_enabled = CBits(1, _FFCNTL, 7)
 
     # Register ODCNTL (0x21)
     # |IIR_BYPASS|LPRO|FSTUP|----|OSA3|OSA2|OSA1|OSA0|
     _output_data_rate = CBits(4, _ODCNTL, 0)
 
-    def __init__(self, i2c: I2C, address: int = 0x1F) -> None:
+    def __init__(self, i2c, address: int = 0x1F) -> None:
         self._i2c = i2c
         self._address = address
 
         if self._device_id != 0x3D:
             raise RuntimeError("Failed to find KX132")
 
         self._operating_mode = NORMAL_MODE
```

### Comparing `micropython-kx132-0.1.0/micropython_kx132.egg-info/PKG-INFO` & `micropython-kx132-0.1.1/micropython_kx132.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-kx132
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Kionix KX132 Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_KX132
 Keywords: sensor,micropython,kx132,acceleration
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
 .. image:: https://readthedocs.org/projects/micropython-kx132/badge/?version=latest
     :target: https://micropython-kx132.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-kx132.svg
     :alt: latest version on PyPI
@@ -34,14 +38,45 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Kionix KX132 Accelerometer
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_KX132
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_KX132
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_KX132/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_KX132/examples.json
+
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-kx132/>`_.
@@ -71,8 +106,7 @@
 =============
 
 Take a look at the examples directory
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://micropython-kx132.readthedocs.io/>`_.
-
```

### Comparing `micropython-kx132-0.1.0/pyproject.toml` & `micropython-kx132-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-kx132"
 description = "MicroPython Driver for the Kionix KX132 Accelerometer"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_KX132"}
 keywords = [
     "sensor",
@@ -27,16 +27,16 @@
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
-py-modules = ["kx132"]
+packages = ["micropython_kx132"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

