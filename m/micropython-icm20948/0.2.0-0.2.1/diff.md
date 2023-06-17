# Comparing `tmp/micropython-icm20948-0.2.0.tar.gz` & `tmp/micropython-icm20948-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-icm20948-0.2.0.tar", last modified: Thu Apr 27 00:11:46 2023, max compression
+gzip compressed data, was "micropython-icm20948-0.2.1.tar", last modified: Sat Jun 17 15:13:32 2023, max compression
```

## Comparing `micropython-icm20948-0.2.0.tar` & `micropython-icm20948-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.951321 micropython-icm20948-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.939321 micropython-icm20948-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.943321 micropython-icm20948-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-27 00:11:46.951321 micropython-icm20948-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.947321 micropython-icm20948-0.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.947321 micropython-icm20948-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.947321 micropython-icm20948-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-27 00:11:38.000000 micropython-icm20948-0.2.0/examples/icm20948_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.947321 micropython-icm20948-0.2.0/micropython_icm20948/
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-27 00:11:38.000000 micropython-icm20948-0.2.0/micropython_icm20948/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23466 2023-04-27 00:11:38.000000 micropython-icm20948-0.2.0/micropython_icm20948/icm20948.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:11:46.951321 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 00:11:46.000000 micropython-icm20948-0.2.0/micropython_icm20948.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-27 00:11:38.000000 micropython-icm20948-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-27 00:11:26.000000 micropython-icm20948-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:11:46.951321 micropython-icm20948-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.918759 micropython-icm20948-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.918759 micropython-icm20948-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/examples/icm20948_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/micropython_icm20948/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/micropython_icm20948/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/micropython_icm20948/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/micropython_icm20948/icm20948.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 15:13:32.000000 micropython-icm20948-0.2.1/micropython_icm20948.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-17 15:13:25.000000 micropython-icm20948-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:13:18.000000 micropython-icm20948-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:13:32.922759 micropython-icm20948-0.2.1/setup.cfg
```

### Comparing `micropython-icm20948-0.2.0/.gitignore` & `micropython-icm20948-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.0/.pre-commit-config.yaml` & `micropython-icm20948-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.0/.pylintrc` & `micropython-icm20948-0.2.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.0/LICENSE` & `micropython-icm20948-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.0/PKG-INFO` & `micropython-icm20948-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-icm20948
-Version: 0.2.0
+Version: 0.2.1
 Summary: MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
 Author-email: "Jose D. Montoya" <icm20948@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ICM20948
 Keywords: micropython,icm20948,gyro,accelerometer,acceleration,sensor
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
 .. image:: https://readthedocs.org/projects/micropython-icm20948/badge/?version=latest
     :target: https://micropython-icm20948.readthedocs.io/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-icm20948.svg
     :target: https://pypi.python.org/pypi/micropython-icm20948
@@ -34,14 +38,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ICM20948
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ICM20948
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ICM20948/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ICM20948/examples.json
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-icm20948/>`_.
```

### Comparing `micropython-icm20948-0.2.0/README.rst` & `micropython-icm20948-0.2.1/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-icm20948/badge/?version=latest
     :target: https://micropython-icm20948.readthedocs.io/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-icm20948.svg
     :target: https://pypi.python.org/pypi/micropython-icm20948
@@ -17,14 +21,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ICM20948
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ICM20948
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ICM20948/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ICM20948/examples.json
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-icm20948/>`_.
```

### Comparing `micropython-icm20948-0.2.0/docs/_static/Logo.png` & `micropython-icm20948-0.2.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.0/docs/_static/favicon.ico` & `micropython-icm20948-0.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.0/docs/conf.py` & `micropython-icm20948-0.2.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     "sphinx.ext.todo",
     "sphinx.ext.viewcode",
     "sphinx_immaterial",
 ]
 
 autodoc_preserve_defaults = True
 
-
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "MicroPython": ("https://docs.micropython.org/en/latest/", None),
 }
 
 autoclass_content = "both"
 templates_path = ["_templates"]
@@ -177,15 +176,15 @@
 }
 
 object_description_options = [
     ("py:.*", dict(generate_synopses="first_sentence")),
 ]
 
 # Set link name generated in the top bar.
-html_title = "MicroPython MC3479"
+html_title = "MicroPython ICM20948"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # These paths are either relative to html_static_path
```

### Comparing `micropython-icm20948-0.2.0/micropython_icm20948/i2c_helpers.py` & `micropython-icm20948-0.2.1/micropython_icm20948/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-icm20948-0.2.0/micropython_icm20948/icm20948.py` & `micropython-icm20948-0.2.1/micropython_icm20948/icm20948.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 """
 
 # pylint: disable=too-many-arguments, line-too-long, too-many-instance-attributes
 
 from time import sleep
 from micropython import const
-from i2c_helpers import CBits, RegisterStruct
+from micropython_icm20948.i2c_helpers import CBits, RegisterStruct
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_ICM20948.git"
 
 _REG_WHOAMI = const(0x69)
 _DEVICE_ID = const(0x00)
 
 _PWR_MGMT_1 = const(0x06)
 _PWR_MGMT_2 = const(0x07)
```

### Comparing `micropython-icm20948-0.2.0/micropython_icm20948.egg-info/PKG-INFO` & `micropython-icm20948-0.2.1/micropython_icm20948.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-icm20948
-Version: 0.2.0
+Version: 0.2.1
 Summary: MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
 Author-email: "Jose D. Montoya" <icm20948@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_ICM20948
 Keywords: micropython,icm20948,gyro,accelerometer,acceleration,sensor
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
 .. image:: https://readthedocs.org/projects/micropython-icm20948/badge/?version=latest
     :target: https://micropython-icm20948.readthedocs.io/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-icm20948.svg
     :target: https://pypi.python.org/pypi/micropython-icm20948
@@ -34,14 +38,44 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ICM20948
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ICM20948
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_ICM20948/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_ICM20948/examples.json
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-icm20948/>`_.
```

### Comparing `micropython-icm20948-0.2.0/micropython_icm20948.egg-info/SOURCES.txt` & `micropython-icm20948-0.2.1/micropython_icm20948.egg-info/SOURCES.txt`

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
@@ -15,14 +17,15 @@
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/icm20948_simpletest.py
+micropython_icm20948/__init__.py
 micropython_icm20948/i2c_helpers.py
 micropython_icm20948/icm20948.py
 micropython_icm20948.egg-info/PKG-INFO
 micropython_icm20948.egg-info/SOURCES.txt
 micropython_icm20948.egg-info/dependency_links.txt
 micropython_icm20948.egg-info/requires.txt
 micropython_icm20948.egg-info/top_level.txt
```

### Comparing `micropython-icm20948-0.2.0/pyproject.toml` & `micropython-icm20948-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-icm20948"
 description = "MicroPython Driver for the Accelerometer and Gyro ICM20948 Sensor"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "icm20948@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_ICM20948"}
 keywords = [
     "micropython",
@@ -29,15 +29,15 @@
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
 packages = ["micropython_icm20948"]
 
 [tool.setuptools.dynamic]
```

