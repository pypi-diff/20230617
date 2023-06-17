# Comparing `tmp/micropython-bmi160-0.1.0.tar.gz` & `tmp/micropython-bmi160-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-bmi160-0.1.0.tar", last modified: Sat Jun 10 21:07:40 2023, max compression
+gzip compressed data, was "micropython-bmi160-0.1.1.tar", last modified: Sat Jun 17 15:33:04 2023, max compression
```

## Comparing `micropython-bmi160-0.1.0.tar` & `micropython-bmi160-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:07:40.667527 micropython-bmi160-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:07:40.659527 micropython-bmi160-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:07:40.659527 micropython-bmi160-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-10 21:07:40.667527 micropython-bmi160-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:07:40.663527 micropython-bmi160-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:07:40.663527 micropython-bmi160-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:07:40.663527 micropython-bmi160-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/examples/bmi160_acc_datarate.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/examples/bmi160_acce_datarange.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/examples/bmi160_gyro_datarate.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/examples/bmi160_gyro_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/examples/bmi160_gyro_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/examples/bmi160_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/examples/bmi160_temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:07:40.667527 micropython-bmi160-0.1.0/micropython_bmi160/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/micropython_bmi160/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/micropython_bmi160/bmi160.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/micropython_bmi160/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 21:07:40.667527 micropython-bmi160-0.1.0/micropython_bmi160.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-10 21:07:40.000000 micropython-bmi160-0.1.0/micropython_bmi160.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-10 21:07:40.000000 micropython-bmi160-0.1.0/micropython_bmi160.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 21:07:40.000000 micropython-bmi160-0.1.0/micropython_bmi160.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-10 21:07:40.000000 micropython-bmi160-0.1.0/micropython_bmi160.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-10 21:07:40.000000 micropython-bmi160-0.1.0/micropython_bmi160.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-10 21:07:30.000000 micropython-bmi160-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-10 21:07:20.000000 micropython-bmi160-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 21:07:40.667527 micropython-bmi160-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.712855 micropython-bmi160-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.704855 micropython-bmi160-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-17 15:33:04.712855 micropython-bmi160-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_acc_datarate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_acce_datarange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_gyro_datarate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_gyro_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_gyro_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/examples/bmi160_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.708855 micropython-bmi160-0.1.1/micropython_bmi160/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/micropython_bmi160/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26971 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/micropython_bmi160/bmi160.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/micropython_bmi160/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:33:04.712855 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 15:33:04.000000 micropython-bmi160-0.1.1/micropython_bmi160.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-17 15:32:57.000000 micropython-bmi160-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:32:49.000000 micropython-bmi160-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:33:04.712855 micropython-bmi160-0.1.1/setup.cfg
```

### Comparing `micropython-bmi160-0.1.0/.gitignore` & `micropython-bmi160-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/.pre-commit-config.yaml` & `micropython-bmi160-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/.pylintrc` & `micropython-bmi160-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/LICENSE` & `micropython-bmi160-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/PKG-INFO` & `micropython-bmi160-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-bmi160
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Bosch BMI160 Acc/Gyro Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMI160
 Keywords: sensor,micropython,bmi160,gyro,acceleration,accelerometer,temperature,vector,gravity,micropython,rotation
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
 .. image:: https://readthedocs.org/projects/micropython-bmi160/badge/?version=latest
     :target: https://micropython-bmi160.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-bmi160.svg
     :alt: latest version on PyPI
@@ -34,14 +38,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Bosch BMI160 Acc/Gyro Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_BMI160
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_BMI160
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_BMI160/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_BMI160/examples.json
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-bmi160/>`_.
@@ -71,8 +105,7 @@
 =============
 
 Take a look at the examples directory
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://micropython-bmi160.readthedocs.io/en/latest/>`_.
-
```

### Comparing `micropython-bmi160-0.1.0/README.rst` & `micropython-bmi160-0.1.1/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-bmi160/badge/?version=latest
     :target: https://micropython-bmi160.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-bmi160.svg
     :alt: latest version on PyPI
@@ -17,14 +21,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Bosch BMI160 Acc/Gyro Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_BMI160
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_BMI160
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_BMI160/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_BMI160/examples.json
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-bmi160/>`_.
@@ -54,8 +88,7 @@
 =============
 
 Take a look at the examples directory
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://micropython-bmi160.readthedocs.io/en/latest/>`_.
-
```

### Comparing `micropython-bmi160-0.1.0/docs/_static/Logo.png` & `micropython-bmi160-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/docs/_static/favicon.ico` & `micropython-bmi160-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/docs/conf.py` & `micropython-bmi160-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/docs/examples.rst` & `micropython-bmi160-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/examples/bmi160_acc_datarate.py` & `micropython-bmi160-0.1.1/examples/bmi160_acc_datarate.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 from machine import Pin, I2C
 from micropython_bmi160 import bmi160
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 bmi = bmi160.BMI160(i2c)
 
-bmi.acceleration_output_data_rate = BMI160.BANDWIDTH_25_32
+bmi.acceleration_output_data_rate = bmi160.BANDWIDTH_25_32
 
 while True:
-    for data_rate in BMI160.bandwidth_values:
+    for data_rate in bmi160.bandwidth_values:
         print("Current Acceleration Data Rate: ", bmi.acceleration_output_data_rate)
         for _ in range(10):
             accx, accy, accz = bmi.acceleration
             print("x:{:.2f}m/s2, y:{:.2f}m/s2, z{:.2f}m/s2".format(accx, accy, accz))
             time.sleep(0.5)
         bmi.acceleration_output_data_rate = data_rate
```

### Comparing `micropython-bmi160-0.1.0/examples/bmi160_acce_datarange.py` & `micropython-bmi160-0.1.1/examples/bmi160_acce_datarange.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 from machine import Pin, I2C
 from micropython_bmi160 import bmi160
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 bmi = bmi160.BMI160(i2c)
 
-bmi.acceleration_range = BMI160.ACCEL_RANGE_4G
+bmi.acceleration_range = bmi160.ACCEL_RANGE_4G
 
 while True:
-    for data_range in BMI160.acc_range_values:
+    for data_range in bmi160.acc_range_values:
         print("Current Acceleration Data Rate: ", bmi.acceleration_range)
         for _ in range(10):
             accx, accy, accz = bmi.acceleration
             print("x:{:.2f}m/s2, y:{:.2f}m/s2, z{:.2f}m/s2".format(accx, accy, accz))
             time.sleep(0.5)
         bmi.acceleration_range = data_range
```

### Comparing `micropython-bmi160-0.1.0/examples/bmi160_gyro_datarate.py` & `micropython-bmi160-0.1.1/examples/bmi160_gyro_datarate.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 from machine import Pin, I2C
 from micropython_bmi160 import bmi160
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 bmi = bmi160.BMI160(i2c)
 
-bmi.gyro_output_data_rate = BMI160.BANDWIDTH_200
+bmi.gyro_output_data_rate = bmi160.BANDWIDTH_200
 
 while True:
-    for data_rate in BMI160.gyro_bandwidth_values:
+    for data_rate in bmi160.gyro_bandwidth_values:
         print("Current Gyro Data Range: ", bmi.gyro_output_data_rate)
         for _ in range(10):
             gyrox, gyroy, gyroz = bmi.gyro
             print("x:{:.2f}°/s, y:{:.2f}°/s, z{:.2f}°/s".format(gyrox, gyroy, gyroz))
             time.sleep(0.5)
         bmi.gyro_output_data_rate = data_rate
```

### Comparing `micropython-bmi160-0.1.0/examples/bmi160_gyro_range.py` & `micropython-bmi160-0.1.1/examples/bmi160_gyro_range.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 from machine import Pin, I2C
 from micropython_bmi160 import bmi160
 
 i2c = I2C(1, sda=Pin(2), scl=Pin(3))  # Correct I2C pins for RP2040
 bmi = bmi160.BMI160(i2c)
 
-bmi.gyro_range = BMI160.GYRO_RANGE_500
+bmi.gyro_range = bmi160.GYRO_RANGE_500
 
 while True:
-    for data_range in BMI160.gyro_values:
+    for data_range in bmi160.gyro_values:
         print("Current Gyro Data Range: ", bmi.gyro_range)
         for _ in range(10):
             gyrox, gyroy, gyroz = bmi.gyro
             print("x:{:.2f}°/s, y:{:.2f}°/s, z{:.2f}°/s".format(gyrox, gyroy, gyroz))
             time.sleep(0.5)
         bmi.gyro_range = data_range
```

### Comparing `micropython-bmi160-0.1.0/examples/bmi160_simpletest.py` & `micropython-bmi160-0.1.1/examples/bmi160_simpletest.py`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/micropython_bmi160/bmi160.py` & `micropython-bmi160-0.1.1/micropython_bmi160/bmi160.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_BMI160.git"
 
 
 _I2C_ADDR = const(0x69)
 _REG_WHOAMI = const(0x00)
 _ERROR_CODE = const(0x02)
 _COMMAND = const(0x7E)
@@ -299,17 +299,17 @@
         it will change to normal mode. If the acc_us is set to ‘0’ and a
         command to enter low-power mode is sent to the Register (0x7E) CMD,
         this command is ignored.
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
-        | :py:const:`BMI160.NO_UNDERSAMPLE`      | :py:const:`0`           |
+        | :py:const:`bmi160.NO_UNDERSAMPLE`      | :py:const:`0`           |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.UNDERSAMPLE`         | :py:const:`1`           |
+        | :py:const:`bmi160.UNDERSAMPLE`         | :py:const:`1`           |
         +----------------------------------------+-------------------------+
 
         """
         sample_values = ("NO_UNDERSAMPLE", "UNDERSAMPLE")
         return sample_values[self._acc_us]
 
     @acceleration_undersample.setter
@@ -323,17 +323,17 @@
         """
         Determines filter configuration (acc_us=0) and averaging for
         undersampling mode (acc_us=1).
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
-        | :py:const:`BMI160.FILTER`              | :py:const:`0`           |
+        | :py:const:`bmi160.FILTER`              | :py:const:`0`           |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.AVERAGING`           | :py:const:`1`           |
+        | :py:const:`bmi160.AVERAGING`           | :py:const:`1`           |
         +----------------------------------------+-------------------------+
 
         """
         values = ("FILTER", "AVERAGING")
         return values[self._acc_bwp]
 
     @acceleration_bandwidth_parameter.setter
@@ -352,37 +352,37 @@
         result in an error code in the Register (0x02) ERR_REG.
 
         At startup this is setup at 100 Hz
 
         +----------------------------------------+---------------------------------+
         | Mode                                   | Value                           |
         +========================================+=================================+
-        | :py:const:`BMI160.BANDWIDTH_25_32`     | :py:const:`0b0001` 25/32 Hz     |
+        | :py:const:`bmi160.BANDWIDTH_25_32`     | :py:const:`0b0001` 25/32 Hz     |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_25_16`     | :py:const:`0b0010` 25/16 Hz     |
+        | :py:const:`bmi160.BANDWIDTH_25_16`     | :py:const:`0b0010` 25/16 Hz     |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_25_8`      | :py:const:`0b0011` 25/8 Hz      |
+        | :py:const:`bmi160.BANDWIDTH_25_8`      | :py:const:`0b0011` 25/8 Hz      |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_25_4`      | :py:const:`0b0100` 25/4 Hz      |
+        | :py:const:`bmi160.BANDWIDTH_25_4`      | :py:const:`0b0100` 25/4 Hz      |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_25_2`      | :py:const:`0b0101` 25/2 Hz      |
+        | :py:const:`bmi160.BANDWIDTH_25_2`      | :py:const:`0b0101` 25/2 Hz      |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_25`        | :py:const:`0b0110` 25 Hz        |
+        | :py:const:`bmi160.BANDWIDTH_25`        | :py:const:`0b0110` 25 Hz        |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_50`        | :py:const:`0b0111` 50 Hz        |
+        | :py:const:`bmi160.BANDWIDTH_50`        | :py:const:`0b0111` 50 Hz        |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_100`       | :py:const:`0b1000` 100 Hz       |
+        | :py:const:`bmi160.BANDWIDTH_100`       | :py:const:`0b1000` 100 Hz       |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_200`       | :py:const:`0b1001` 200 Hz       |
+        | :py:const:`bmi160.BANDWIDTH_200`       | :py:const:`0b1001` 200 Hz       |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_400`       | :py:const:`0b1010` 400 Hz       |
+        | :py:const:`bmi160.BANDWIDTH_400`       | :py:const:`0b1010` 400 Hz       |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_800`       | :py:const:`0b1011` 800 Hz       |
+        | :py:const:`bmi160.BANDWIDTH_800`       | :py:const:`0b1011` 800 Hz       |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_1600`      | :py:const:`0b1100` 1600 Hz      |
+        | :py:const:`bmi160.BANDWIDTH_1600`      | :py:const:`0b1100` 1600 Hz      |
         +----------------------------------------+---------------------------------+
 
         """
         values = (
             "BANDWIDTH_25_32",
             "BANDWIDTH_25_16",
             "BANDWIDTH_25_8",
@@ -413,21 +413,21 @@
         ready bit in the Register (0x1B) STATUS. It is recommended to
         read the Register (0x04-0x17) DATA after the range change to
         remove a stall data ready bit from before the range change.
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
-        | :py:const:`BMI160.ACCEL_RANGE_2G`      | :py:const:`0b0011`      |
+        | :py:const:`bmi160.ACCEL_RANGE_2G`      | :py:const:`0b0011`      |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.ACCEL_RANGE_4G`      | :py:const:`0b0101`      |
+        | :py:const:`bmi160.ACCEL_RANGE_4G`      | :py:const:`0b0101`      |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.ACCEL_RANGE_8G`      | :py:const:`0b1000`      |
+        | :py:const:`bmi160.ACCEL_RANGE_8G`      | :py:const:`0b1000`      |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.ACCEL_RANGE_16G`     | :py:const:`0b1100`      |
+        | :py:const:`bmi160.ACCEL_RANGE_16G`     | :py:const:`0b1100`      |
         +----------------------------------------+-------------------------+
 
         """
         values = {
             3: "ACCEL_RANGE_2G",
             5: "ACCEL_RANGE_4G",
             8: "ACCEL_RANGE_8G",
@@ -439,23 +439,29 @@
     def acceleration_range(self, value: int) -> None:
         if value not in acc_range_values:
             raise ValueError("Value must be a valid Acceleration Range setting")
         self._acc_range = value
 
     @property
     def acceleration(self) -> Tuple[int, int, int]:
+        """
+        Sensor Acceleration
+        """
 
         factor = self.acceleration_scale[self.acceleration_range]
 
         x = self._acc_data_x / factor
         y = self._acc_data_y / factor
         z = self._acc_data_z / factor
         return x, y, z
 
     def power_mode_status(self) -> None:
+        """
+        Returns Power mode status
+        """
         values = self._power_mode
 
         acc_pmu_status = (values & 0x18) >> 4
         gyr_pmu_status = (values & 0xC) >> 2
         mag_pmu_status = values & 0x03
 
         acc_pmu_codes = {0: "Suspend", 1: "Normal", 2: "Low Power"}
@@ -467,19 +473,19 @@
         print("Mag Power Mode", mag_pmu_codes[mag_pmu_status])
 
     def acc_power_mode(self, value: int) -> None:
         """
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
-        | :py:const:`BMI160.ACC_POWER_SUSPEND`   | :py:const:`0x10`        |
+        | :py:const:`bmi160.ACC_POWER_SUSPEND`   | :py:const:`0x10`        |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.ACC_POWER_NORMAL`    | :py:const:`0x11`        |
+        | :py:const:`bmi160.ACC_POWER_NORMAL`    | :py:const:`0x11`        |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.POWER_LOWPOWER`      | :py:const:`0x12`        |
+        | :py:const:`bmi160.POWER_LOWPOWER`      | :py:const:`0x12`        |
         +----------------------------------------+-------------------------+
 
         """
         if value not in acc_power_mode_values:
             raise ValueError("Value must be a valid Acceleration Power Mode Setting")
         self._read = value
         time.sleep(0.1)
@@ -497,14 +503,17 @@
         :return: int
         """
 
         return (self._temp_data * 1 / 2**9) + 23
 
     @property
     def gyro(self) -> Tuple[int, int, int]:
+        """
+        Gyro values
+        """
 
         factor = self.gyro_scale[self.gyro_range]
 
         x = self._gyro_data_x / factor
         y = self._gyro_data_y / factor
         z = self._gyro_data_z / factor
         return x, y, z
@@ -523,29 +532,29 @@
             in an error code in Register (0x02) ERR_REG.
 
         At startup this is setup at 100 Hz
 
         +----------------------------------------+---------------------------------+
         | Mode                                   | Value                           |
         +========================================+=================================+
-        | :py:const:`BMI160.BANDWIDTH_25`        | :py:const:`0b0110` 25 Hz        |
+        | :py:const:`bmi160.BANDWIDTH_25`        | :py:const:`0b0110` 25 Hz        |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_50`        | :py:const:`0b0111` 50 Hz        |
+        | :py:const:`bmi160.BANDWIDTH_50`        | :py:const:`0b0111` 50 Hz        |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_100`       | :py:const:`0b1000` 100 Hz       |
+        | :py:const:`bmi160.BANDWIDTH_100`       | :py:const:`0b1000` 100 Hz       |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_200`       | :py:const:`0b1001` 200 Hz       |
+        | :py:const:`bmi160.BANDWIDTH_200`       | :py:const:`0b1001` 200 Hz       |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_400`       | :py:const:`0b1010` 400 Hz       |
+        | :py:const:`bmi160.BANDWIDTH_400`       | :py:const:`0b1010` 400 Hz       |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_800`       | :py:const:`0b1011` 800 Hz       |
+        | :py:const:`bmi160.BANDWIDTH_800`       | :py:const:`0b1011` 800 Hz       |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_1600`      | :py:const:`0b1100` 1600 Hz      |
+        | :py:const:`bmi160.BANDWIDTH_1600`      | :py:const:`0b1100` 1600 Hz      |
         +----------------------------------------+---------------------------------+
-        | :py:const:`BMI160.BANDWIDTH_3200`      | :py:const:`0b1101` 3200 Hz      |
+        | :py:const:`bmi160.BANDWIDTH_3200`      | :py:const:`0b1101` 3200 Hz      |
         +----------------------------------------+---------------------------------+
 
         """
         values = (
             "BANDWIDTH_25",
             "BANDWIDTH_50",
             "BANDWIDTH_100",
@@ -593,19 +602,19 @@
         the filter bandwidth will be approximately 4 times smaller than the
         bandwidth achieved for the same ODR in the normal filter mode.
         For example, for ODR=50Hz we will have a 3dB cutoff frequency of 5.06Hz.
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
-        | :py:const:`BMI160.GYRO_NORMAL`         | :py:const:`0b10`        |
+        | :py:const:`bmi160.GYRO_NORMAL`         | :py:const:`0b10`        |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.GYRO_OSR2`           | :py:const:`0b01`        |
+        | :py:const:`bmi160.GYRO_OSR2`           | :py:const:`0b01`        |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.GYRO_OSR4`           | :py:const:`0b00`        |
+        | :py:const:`bmi160.GYRO_OSR4`           | :py:const:`0b00`        |
         +----------------------------------------+-------------------------+
 
         """
         values = ("GYRO_OSR4", "GYRO_OSR2", "GYRO_NORMAL")
         return values[self._gyro_bwp]
 
     @gyro_bandwidth_parameter.setter
@@ -616,19 +625,19 @@
 
     @property
     def gyro_power_mode(self) -> str:
         """
         +-------------------------------------------+-------------------------+
         | Mode                                      | Value                   |
         +===========================================+=========================+
-        | :py:const:`BMI160.GYRO_POWER_SUSPEND`     | :py:const:`0x14`        |
+        | :py:const:`bmi160.GYRO_POWER_SUSPEND`     | :py:const:`0x14`        |
         +-------------------------------------------+-------------------------+
-        | :py:const:`BMI160.GYRO_POWER_NORMAL`      | :py:const:`0x15`        |
+        | :py:const:`bmi160.GYRO_POWER_NORMAL`      | :py:const:`0x15`        |
         +-------------------------------------------+-------------------------+
-        | :py:const:`BMI160.GYRO_POWER_FASTSTARTUP` | :py:const:`0x17`        |
+        | :py:const:`bmi160.GYRO_POWER_FASTSTARTUP` | :py:const:`0x17`        |
         +-------------------------------------------+-------------------------+
 
         """
         g_power_modes = {
             0x14: "GYRO_POWER_SUSPEND",
             0x15: "GYRO_POWER_NORMAL",
             0x17: "GYRO_POWER_FASTSTARTUP",
@@ -652,23 +661,23 @@
         ready bit in the Register (0x1B) STATUS. It is recommended to
         read the Register (0x04-0x17) DATA after the range change to
         remove a stall data ready bit from before the range change.
 
         +----------------------------------------+-------------------------+
         | Mode                                   | Value                   |
         +========================================+=========================+
-        | :py:const:`BMI160.GYRO_RANGE_2000`     | :py:const:`0b000`       |
+        | :py:const:`bmi160.GYRO_RANGE_2000`     | :py:const:`0b000`       |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.GYRO_RANGE_1000`     | :py:const:`0b001`       |
+        | :py:const:`bmi160.GYRO_RANGE_1000`     | :py:const:`0b001`       |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.GYRO_RANGE_500`      | :py:const:`0b010`       |
+        | :py:const:`bmi160.GYRO_RANGE_500`      | :py:const:`0b010`       |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.GYRO_RANGE_250`      | :py:const:`0b011`       |
+        | :py:const:`bmi160.GYRO_RANGE_250`      | :py:const:`0b011`       |
         +----------------------------------------+-------------------------+
-        | :py:const:`BMI160.GYRO_RANGE_125`      | :py:const:`0b100`       |
+        | :py:const:`bmi160.GYRO_RANGE_125`      | :py:const:`0b100`       |
         +----------------------------------------+-------------------------+
 
         """
         g_values = (
             "GYRO_RANGE_125",
             "GYRO_RANGE_250",
             "GYRO_RANGE_500",
```

### Comparing `micropython-bmi160-0.1.0/micropython_bmi160/i2c_helpers.py` & `micropython-bmi160-0.1.1/micropython_bmi160/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-bmi160-0.1.0/micropython_bmi160.egg-info/PKG-INFO` & `micropython-bmi160-0.1.1/micropython_bmi160.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-bmi160
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the Bosch BMI160 Acc/Gyro Sensor
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_BMI160
 Keywords: sensor,micropython,bmi160,gyro,acceleration,accelerometer,temperature,vector,gravity,micropython,rotation
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
 .. image:: https://readthedocs.org/projects/micropython-bmi160/badge/?version=latest
     :target: https://micropython-bmi160.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-bmi160.svg
     :alt: latest version on PyPI
@@ -34,14 +38,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Bosch BMI160 Acc/Gyro Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_BMI160
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_BMI160
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_BMI160/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_BMI160/examples.json
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-bmi160/>`_.
@@ -71,8 +105,7 @@
 =============
 
 Take a look at the examples directory
 
 Documentation
 =============
 API documentation for this library can be found on `Read the Docs <https://micropython-bmi160.readthedocs.io/en/latest/>`_.
-
```

### Comparing `micropython-bmi160-0.1.0/micropython_bmi160.egg-info/SOURCES.txt` & `micropython-bmi160-0.1.1/micropython_bmi160.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

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

### Comparing `micropython-bmi160-0.1.0/pyproject.toml` & `micropython-bmi160-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-bmi160"
 description = "MicroPython Driver for the Bosch BMI160 Acc/Gyro Sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_BMI160"}
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
 py-modules = ["bmi160"]
 
 [tool.setuptools.dynamic]
```

