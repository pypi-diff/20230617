# Comparing `tmp/micropython-isl29125-0.1.0.tar.gz` & `tmp/micropython-isl29125-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-isl29125-0.1.0.tar", last modified: Sat Jun 10 22:37:30 2023, max compression
+gzip compressed data, was "micropython-isl29125-0.1.1.tar", last modified: Sat Jun 17 15:10:49 2023, max compression
```

## Comparing `micropython-isl29125-0.1.0.tar` & `micropython-isl29125-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:37:30.498776 micropython-isl29125-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:37:30.494776 micropython-isl29125-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:37:30.494776 micropython-isl29125-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-10 22:37:30.498776 micropython-isl29125-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:37:30.494776 micropython-isl29125-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:37:30.494776 micropython-isl29125-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:37:30.494776 micropython-isl29125-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-10 22:37:22.000000 micropython-isl29125-0.1.0/examples/isl29125_ADC_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-10 22:37:22.000000 micropython-isl29125-0.1.0/examples/isl29125_operation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-10 22:37:22.000000 micropython-isl29125-0.1.0/examples/isl29125_rgb_sensing_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-10 22:37:22.000000 micropython-isl29125-0.1.0/examples/isl29125_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-10 22:37:22.000000 micropython-isl29125-0.1.0/examples/isl29125_threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:37:30.498776 micropython-isl29125-0.1.0/micropython_isl29125/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 22:37:22.000000 micropython-isl29125-0.1.0/micropython_isl29125/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-10 22:37:22.000000 micropython-isl29125-0.1.0/micropython_isl29125/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-06-10 22:37:22.000000 micropython-isl29125-0.1.0/micropython_isl29125/isl29125.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 22:37:30.498776 micropython-isl29125-0.1.0/micropython_isl29125.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-10 22:37:30.000000 micropython-isl29125-0.1.0/micropython_isl29125.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-10 22:37:30.000000 micropython-isl29125-0.1.0/micropython_isl29125.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 22:37:30.000000 micropython-isl29125-0.1.0/micropython_isl29125.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-10 22:37:30.000000 micropython-isl29125-0.1.0/micropython_isl29125.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 22:37:30.000000 micropython-isl29125-0.1.0/micropython_isl29125.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-10 22:37:22.000000 micropython-isl29125-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-10 22:37:07.000000 micropython-isl29125-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 22:37:30.498776 micropython-isl29125-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.070340 micropython-isl29125-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.070340 micropython-isl29125-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.070340 micropython-isl29125-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_ADC_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_operation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_rgb_sensing_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/examples/isl29125_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/micropython_isl29125/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/micropython_isl29125/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/micropython_isl29125/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/micropython_isl29125/isl29125.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 15:10:49.000000 micropython-isl29125-0.1.1/micropython_isl29125.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-17 15:10:39.000000 micropython-isl29125-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:10:26.000000 micropython-isl29125-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:10:49.074340 micropython-isl29125-0.1.1/setup.cfg
```

### Comparing `micropython-isl29125-0.1.0/.gitignore` & `micropython-isl29125-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/.pre-commit-config.yaml` & `micropython-isl29125-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/.pylintrc` & `micropython-isl29125-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/LICENSE` & `micropython-isl29125-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/PKG-INFO` & `micropython-isl29125-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-isl29125
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Intersil ISL29125 Color Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ISL29125
 Keywords: sensor,micropython,isl29125,color,sensor,intersil,RGB,mciropython,isl29125
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
 .. image:: https://readthedocs.org/projects/micropython-isl29125/badge/?version=latest
     :target: https://micropython-isl29125.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-isl29125.svg
     :alt: latest version on PyPI
@@ -34,14 +38,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Intersil ISL29125 Color Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ISL29125
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ISL29125
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ISL29125/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ISL29125/examples.json
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-isl29125/>`_.
```

### Comparing `micropython-isl29125-0.1.0/README.rst` & `micropython-isl29125-0.1.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-isl29125/badge/?version=latest
     :target: https://micropython-isl29125.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-isl29125.svg
     :alt: latest version on PyPI
@@ -17,14 +21,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Intersil ISL29125 Color Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ISL29125
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ISL29125
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ISL29125/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ISL29125/examples.json
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-isl29125/>`_.
```

### Comparing `micropython-isl29125-0.1.0/docs/_static/Logo.png` & `micropython-isl29125-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/docs/_static/favicon.ico` & `micropython-isl29125-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/docs/conf.py` & `micropython-isl29125-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/docs/examples.rst` & `micropython-isl29125-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/examples/isl29125_ADC_resolution.py` & `micropython-isl29125-0.1.1/examples/isl29125_ADC_resolution.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/examples/isl29125_operation_mode.py` & `micropython-isl29125-0.1.1/examples/isl29125_operation_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/examples/isl29125_rgb_sensing_range.py` & `micropython-isl29125-0.1.1/examples/isl29125_rgb_sensing_range.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/examples/isl29125_threshold.py` & `micropython-isl29125-0.1.1/examples/isl29125_threshold.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/micropython_isl29125/i2c_helpers.py` & `micropython-isl29125-0.1.1/micropython_isl29125/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-isl29125-0.1.0/micropython_isl29125/isl29125.py` & `micropython-isl29125-0.1.1/micropython_isl29125/isl29125.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 """
 
 from micropython import const
 from micropython_isl29125.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_ISL29125.git"
 
 _REG_WHOAMI = const(0x00)
 _CONFIG1 = const(0x01)
 _CONFIG2 = const(0x02)
 _CONFIG3 = const(0x03)
 _FLAG_REGISTER = const(0x08)
```

### Comparing `micropython-isl29125-0.1.0/micropython_isl29125.egg-info/PKG-INFO` & `micropython-isl29125-0.1.1/micropython_isl29125.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-isl29125
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Intersil ISL29125 Color Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ISL29125
 Keywords: sensor,micropython,isl29125,color,sensor,intersil,RGB,mciropython,isl29125
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
 .. image:: https://readthedocs.org/projects/micropython-isl29125/badge/?version=latest
     :target: https://micropython-isl29125.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-isl29125.svg
     :alt: latest version on PyPI
@@ -34,14 +38,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Intersil ISL29125 Color Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ISL29125
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ISL29125
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ISL29125/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ISL29125/examples.json
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-isl29125/>`_.
```

### Comparing `micropython-isl29125-0.1.0/micropython_isl29125.egg-info/SOURCES.txt` & `micropython-isl29125-0.1.1/micropython_isl29125.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

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

### Comparing `micropython-isl29125-0.1.0/pyproject.toml` & `micropython-isl29125-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-isl29125"
 description = "MicroPython Driver for the Intersil ISL29125 Color Sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_ISL29125"}
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
 py-modules = ["isl29125"]
 
 [tool.setuptools.dynamic]
```

