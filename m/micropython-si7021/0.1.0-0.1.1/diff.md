# Comparing `tmp/micropython-si7021-0.1.0.tar.gz` & `tmp/micropython-si7021-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-si7021-0.1.0.tar", last modified: Mon Apr 17 18:13:00 2023, max compression
+gzip compressed data, was "micropython-si7021-0.1.1.tar", last modified: Sat Jun 17 14:47:58 2023, max compression
```

## Comparing `micropython-si7021-0.1.0.tar` & `micropython-si7021-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:13:00.632722 micropython-si7021-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:13:00.624722 micropython-si7021-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:13:00.628722 micropython-si7021-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-17 18:13:00.632722 micropython-si7021-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:13:00.628722 micropython-si7021-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:13:00.632722 micropython-si7021-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:13:00.632722 micropython-si7021-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-17 18:12:51.000000 micropython-si7021-0.1.0/examples/micropython_si7021_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:13:00.632722 micropython-si7021-0.1.0/micropython_si7021.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-17 18:13:00.000000 micropython-si7021-0.1.0/micropython_si7021.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-17 18:13:00.000000 micropython-si7021-0.1.0/micropython_si7021.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:13:00.000000 micropython-si7021-0.1.0/micropython_si7021.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-17 18:13:00.000000 micropython-si7021-0.1.0/micropython_si7021.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-17 18:13:00.000000 micropython-si7021-0.1.0/micropython_si7021.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-04-17 18:12:51.000000 micropython-si7021-0.1.0/micropython_si7021.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-17 18:12:51.000000 micropython-si7021-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-17 18:12:39.000000 micropython-si7021-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:13:00.632722 micropython-si7021-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.747110 micropython-si7021-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 14:47:51.000000 micropython-si7021-0.1.1/examples/si7021_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/micropython_si7021/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:51.000000 micropython-si7021-0.1.1/micropython_si7021/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-06-17 14:47:51.000000 micropython-si7021-0.1.1/micropython_si7021/si7021.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:47:58.743111 micropython-si7021-0.1.1/micropython_si7021.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 14:47:58.000000 micropython-si7021-0.1.1/micropython_si7021.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-17 14:47:51.000000 micropython-si7021-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:47:43.000000 micropython-si7021-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:47:58.747110 micropython-si7021-0.1.1/setup.cfg
```

### Comparing `micropython-si7021-0.1.0/.gitignore` & `micropython-si7021-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-si7021-0.1.0/.pre-commit-config.yaml` & `micropython-si7021-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-si7021-0.1.0/.pylintrc` & `micropython-si7021-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-si7021-0.1.0/LICENSE` & `micropython-si7021-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-si7021-0.1.0/PKG-INFO` & `micropython-si7021-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,88 @@
 Metadata-Version: 2.1
 Name: micropython-si7021
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Library for the the Temperature and Humidity SI7021 Sensor
 Author-email: "Jose D. Montoya" <si7021@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_SI7021
 Keywords: micropython,micropython_si7021,sensor,temperature,humidity
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
 Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-si7021/badge/?version=latest
     :target: https://micropython-si7021.readthedocs.io/
     :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/v/micropython-si7021.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/micropython-si7021
+
+.. image:: https://static.pepy.tech/personalized-badge/micropython-si7021?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-si7021
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Library for the the Temperature and Humidity SI7021 Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_SI7021
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_SI7021
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_SI7021/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_SI7021/examples.json
+
+
+
+
+Installation
+=============
+
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-si7021/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install micropython-si7021
```

### Comparing `micropython-si7021-0.1.0/micropython_si7021.egg-info/PKG-INFO` & `micropython-si7021-0.1.1/micropython_si7021.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,88 @@
 Metadata-Version: 2.1
 Name: micropython-si7021
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Library for the the Temperature and Humidity SI7021 Sensor
 Author-email: "Jose D. Montoya" <si7021@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_SI7021
 Keywords: micropython,micropython_si7021,sensor,temperature,humidity
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
 Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-si7021/badge/?version=latest
     :target: https://micropython-si7021.readthedocs.io/
     :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/v/micropython-si7021.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/micropython-si7021
+
+.. image:: https://static.pepy.tech/personalized-badge/micropython-si7021?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-si7021
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Library for the the Temperature and Humidity SI7021 Sensor
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_SI7021
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_SI7021
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_SI7021/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_SI7021/examples.json
+
+
+
+
+Installation
+=============
+
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-si7021/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install micropython-si7021
```

### Comparing `micropython-si7021-0.1.0/micropython_si7021.py` & `micropython-si7021-0.1.1/micropython_si7021/si7021.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from micropython import const
 
 try:
     import struct
 except ImportError:
     import ustruct as struct
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_SI7021.git"
 
 
 class RegisterStructRW:
     """
     Register Struct
     """
```

### Comparing `micropython-si7021-0.1.0/pyproject.toml` & `micropython-si7021-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-si7021"
 description = "MicroPython Library for the the Temperature and Humidity SI7021 Sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "si7021@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_SI7021"}
 keywords = [
     "micropython",
@@ -28,15 +28,15 @@
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
 py-modules = ["micropython_si7021"]
 
 [tool.setuptools.dynamic]
```

