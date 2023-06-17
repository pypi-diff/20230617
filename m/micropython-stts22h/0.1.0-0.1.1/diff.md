# Comparing `tmp/micropython-stts22h-0.1.0.tar.gz` & `tmp/micropython-stts22h-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-stts22h-0.1.0.tar", last modified: Sat Jun 10 02:11:06 2023, max compression
+gzip compressed data, was "micropython-stts22h-0.1.1.tar", last modified: Sat Jun 17 14:44:39 2023, max compression
```

## Comparing `micropython-stts22h-0.1.0.tar` & `micropython-stts22h-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:11:06.036611 micropython-stts22h-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:11:06.032611 micropython-stts22h-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:11:06.032611 micropython-stts22h-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-10 02:11:06.036611 micropython-stts22h-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:11:06.032611 micropython-stts22h-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:11:06.032611 micropython-stts22h-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:11:06.032611 micropython-stts22h-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-10 02:10:58.000000 micropython-stts22h-0.1.0/examples/stts22h_output_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-10 02:10:58.000000 micropython-stts22h-0.1.0/examples/stts22h_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:11:06.032611 micropython-stts22h-0.1.0/micropython_stts22h/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 02:10:58.000000 micropython-stts22h-0.1.0/micropython_stts22h/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-10 02:10:58.000000 micropython-stts22h-0.1.0/micropython_stts22h/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-10 02:10:58.000000 micropython-stts22h-0.1.0/micropython_stts22h/stts22h.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 02:11:06.032611 micropython-stts22h-0.1.0/micropython_stts22h.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-10 02:11:06.000000 micropython-stts22h-0.1.0/micropython_stts22h.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-10 02:11:06.000000 micropython-stts22h-0.1.0/micropython_stts22h.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 02:11:06.000000 micropython-stts22h-0.1.0/micropython_stts22h.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-10 02:11:06.000000 micropython-stts22h-0.1.0/micropython_stts22h.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 02:11:06.000000 micropython-stts22h-0.1.0/micropython_stts22h.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-10 02:10:58.000000 micropython-stts22h-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-10 02:10:51.000000 micropython-stts22h-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 02:11:06.036611 micropython-stts22h-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.682183 micropython-stts22h-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.674183 micropython-stts22h-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/examples/stts22h_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/examples/stts22h_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/micropython_stts22h/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/micropython_stts22h/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/micropython_stts22h/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/micropython_stts22h/stts22h.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:44:39.678183 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 14:44:39.000000 micropython-stts22h-0.1.1/micropython_stts22h.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-17 14:44:32.000000 micropython-stts22h-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:44:24.000000 micropython-stts22h-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:44:39.682183 micropython-stts22h-0.1.1/setup.cfg
```

### Comparing `micropython-stts22h-0.1.0/.gitignore` & `micropython-stts22h-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.0/.pre-commit-config.yaml` & `micropython-stts22h-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.0/.pylintrc` & `micropython-stts22h-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.0/LICENSE` & `micropython-stts22h-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.0/PKG-INFO` & `micropython-stts22h-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-stts22h
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the STTS22H Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_STTS22H
 Keywords: sensor,micropython,stts22h,temperature,sensor,stts22h,st,micropython,celsius
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
 .. image:: https://readthedocs.org/projects/micropython-stts22h/badge/?version=latest
     :target: https://micropython-stts22h.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-stts22h.svg
     :alt: latest version on PyPI
@@ -34,15 +38,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the STTS22H Temperature Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_STTS22H
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_STTS22H
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_STTS22H/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
 
+    mip install github:jposada202020/MicroPython_STTS22H/examples.json
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-stts22h/>`_.
 To install for current user:
```

### Comparing `micropython-stts22h-0.1.0/README.rst` & `micropython-stts22h-0.1.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-stts22h/badge/?version=latest
     :target: https://micropython-stts22h.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-stts22h.svg
     :alt: latest version on PyPI
@@ -17,15 +21,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the STTS22H Temperature Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_STTS22H
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_STTS22H
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_STTS22H/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
 
+    mip install github:jposada202020/MicroPython_STTS22H/examples.json
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-stts22h/>`_.
 To install for current user:
```

### Comparing `micropython-stts22h-0.1.0/docs/_static/Logo.png` & `micropython-stts22h-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.0/docs/_static/favicon.ico` & `micropython-stts22h-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.0/docs/conf.py` & `micropython-stts22h-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.0/examples/stts22h_output_data_rate.py` & `micropython-stts22h-0.1.1/examples/stts22h_output_data_rate.py`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.0/micropython_stts22h/i2c_helpers.py` & `micropython-stts22h-0.1.1/micropython_stts22h/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-stts22h-0.1.0/micropython_stts22h/stts22h.py` & `micropython-stts22h-0.1.1/micropython_stts22h/stts22h.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """
 
 from micropython import const
 from micropython_stts22h.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_STTS22H.git"
 
 _REG_WHOAMI = const(0x01)
 _CTRL = const(0x04)
 
 
 ODR_25_HZ = const(0b00)
```

### Comparing `micropython-stts22h-0.1.0/micropython_stts22h.egg-info/PKG-INFO` & `micropython-stts22h-0.1.1/micropython_stts22h.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-stts22h
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the STTS22H Temperature Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_STTS22H
 Keywords: sensor,micropython,stts22h,temperature,sensor,stts22h,st,micropython,celsius
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
 .. image:: https://readthedocs.org/projects/micropython-stts22h/badge/?version=latest
     :target: https://micropython-stts22h.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-stts22h.svg
     :alt: latest version on PyPI
@@ -34,15 +38,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the STTS22H Temperature Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_STTS22H
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_STTS22H
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_STTS22H/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
 
+    mip install github:jposada202020/MicroPython_STTS22H/examples.json
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-stts22h/>`_.
 To install for current user:
```

### Comparing `micropython-stts22h-0.1.0/micropython_stts22h.egg-info/SOURCES.txt` & `micropython-stts22h-0.1.1/micropython_stts22h.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

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

### Comparing `micropython-stts22h-0.1.0/pyproject.toml` & `micropython-stts22h-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-stts22h"
 description = "MicroPython Driver for the STTS22H Temperature Sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_STTS22H"}
 keywords = [
     "sensor",
@@ -32,15 +32,15 @@
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
 py-modules = ["stts22h"]
 
 [tool.setuptools.dynamic]
```

