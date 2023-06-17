# Comparing `tmp/micropython-mlx90393-0.1.0.tar.gz` & `tmp/micropython-mlx90393-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-mlx90393-0.1.0.tar", last modified: Sun Apr 16 23:04:04 2023, max compression
+gzip compressed data, was "micropython-mlx90393-0.1.1.tar", last modified: Sat Jun 17 14:55:34 2023, max compression
```

## Comparing `micropython-mlx90393-0.1.0.tar` & `micropython-mlx90393-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:04:04.420139 micropython-mlx90393-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:04:04.416139 micropython-mlx90393-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:04:04.420139 micropython-mlx90393-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-16 23:04:04.420139 micropython-mlx90393-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:04:04.420139 micropython-mlx90393-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:04:04.420139 micropython-mlx90393-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:04:04.420139 micropython-mlx90393-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-16 23:03:57.000000 micropython-mlx90393-0.1.0/examples/micropython_mlx90393_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:04:04.420139 micropython-mlx90393-0.1.0/micropython_mlx90393/
--rw-r--r--   0 runner    (1001) docker     (123)    18033 2023-04-16 23:03:57.000000 micropython-mlx90393-0.1.0/micropython_mlx90393/mlx90393.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 23:04:04.420139 micropython-mlx90393-0.1.0/micropython_mlx90393.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-16 23:04:04.000000 micropython-mlx90393-0.1.0/micropython_mlx90393.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-16 23:04:04.000000 micropython-mlx90393-0.1.0/micropython_mlx90393.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 23:04:04.000000 micropython-mlx90393-0.1.0/micropython_mlx90393.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-16 23:04:04.000000 micropython-mlx90393-0.1.0/micropython_mlx90393.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 23:04:04.000000 micropython-mlx90393-0.1.0/micropython_mlx90393.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-16 23:03:57.000000 micropython-mlx90393-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-16 23:03:47.000000 micropython-mlx90393-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 23:04:04.420139 micropython-mlx90393-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.200568 micropython-mlx90393-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.200568 micropython-mlx90393-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-17 14:55:25.000000 micropython-mlx90393-0.1.1/examples/micropython_mlx90393_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/micropython_mlx90393/
+-rw-r--r--   0 runner    (1001) docker     (123)    18031 2023-06-17 14:55:25.000000 micropython-mlx90393-0.1.1/micropython_mlx90393/mlx90393.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 14:55:34.000000 micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-17 14:55:25.000000 micropython-mlx90393-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:55:16.000000 micropython-mlx90393-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:55:34.204568 micropython-mlx90393-0.1.1/setup.cfg
```

### Comparing `micropython-mlx90393-0.1.0/.gitignore` & `micropython-mlx90393-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-mlx90393-0.1.0/.pre-commit-config.yaml` & `micropython-mlx90393-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-mlx90393-0.1.0/.pylintrc` & `micropython-mlx90393-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-mlx90393-0.1.0/LICENSE` & `micropython-mlx90393-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-mlx90393-0.1.0/PKG-INFO` & `micropython-mlx90393-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,89 @@
 Metadata-Version: 2.1
 Name: micropython-mlx90393
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the MLX90393 Sensor
 Author-email: "Jose D. Montoya" <mlx90393@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MLX90393
 Keywords: micropython,micropython_mlx90393,MicroPython,Sensor,Magnetic,magnetometer
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
 .. image:: https://readthedocs.org/projects/micropython-mlx90393/badge/?version=latest
     :target: https://micropython-mlx90393.readthedocs.io/
     :alt: Documentation Status
 
 
+.. image:: https://img.shields.io/pypi/v/micropython-mlx90393.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/micropython-mlx90393
+
+.. image:: https://static.pepy.tech/personalized-badge/micropython-mlx90393?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-mlx90393
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the MLX90393 Sensor
 
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_MLX90393
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_MLX90393
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_MLX90393/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_MLX90393/examples.json
+
+
+
+Installation
+==============
+
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-mlx90393/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install micropython-mlx90393
```

### Comparing `micropython-mlx90393-0.1.0/README.rst` & `micropython-mlx90393-0.1.1/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,71 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-mlx90393/badge/?version=latest
     :target: https://micropython-mlx90393.readthedocs.io/
     :alt: Documentation Status
 
 
+.. image:: https://img.shields.io/pypi/v/micropython-mlx90393.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/micropython-mlx90393
+
+.. image:: https://static.pepy.tech/personalized-badge/micropython-mlx90393?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-mlx90393
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the MLX90393 Sensor
 
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_MLX90393
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_MLX90393
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_MLX90393/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_MLX90393/examples.json
+
+
+
+Installation
+==============
+
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-mlx90393/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install micropython-mlx90393
```

### Comparing `micropython-mlx90393-0.1.0/micropython_mlx90393/mlx90393.py` & `micropython-mlx90393-0.1.1/micropython_mlx90393/mlx90393.py`

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
 __repo__ = "https://github.com/jposada202020/MicroPython_MLX90393.git"
 
 
 class CBits:
     """
     Changes bits from a byte register
     """
@@ -478,16 +478,16 @@
     def oversampling(self):
         """
         Temperature sensor ADC oversampling ratio
 
         .. note::
             The MLX90393 provides configurable filters to adjust the tradeoff
             between current consumption, noise, and conversion time. See section
-             15.1.5 for details on selecting the conversion time by adjusting
-             `oversampling` and `digital_filter`
+            15.1.5 for details on selecting the conversion time by adjusting
+            `oversampling` and `digital_filter`
 
         +----------------------------+-----------------+
         | Mode                       | Value           |
         +============================+=================+
         | :py:const:`mlx90393.OSR_0` | :py:const:`0x0` |
         +----------------------------+-----------------+
         | :py:const:`mlx90393.OSR_1` | :py:const:`0x1` |
```

### Comparing `micropython-mlx90393-0.1.0/micropython_mlx90393.egg-info/PKG-INFO` & `micropython-mlx90393-0.1.1/micropython_mlx90393.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,89 @@
 Metadata-Version: 2.1
 Name: micropython-mlx90393
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the MLX90393 Sensor
 Author-email: "Jose D. Montoya" <mlx90393@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_MLX90393
 Keywords: micropython,micropython_mlx90393,MicroPython,Sensor,Magnetic,magnetometer
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
 .. image:: https://readthedocs.org/projects/micropython-mlx90393/badge/?version=latest
     :target: https://micropython-mlx90393.readthedocs.io/
     :alt: Documentation Status
 
 
+.. image:: https://img.shields.io/pypi/v/micropython-mlx90393.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/micropython-mlx90393
+
+.. image:: https://static.pepy.tech/personalized-badge/micropython-mlx90393?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-mlx90393
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the MLX90393 Sensor
 
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_MLX90393
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_MLX90393
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_MLX90393/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_MLX90393/examples.json
+
+
+
+Installation
+==============
+
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-mlx90393/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install micropython-mlx90393
```

### Comparing `micropython-mlx90393-0.1.0/pyproject.toml` & `micropython-mlx90393-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-mlx90393"
 description = "MicroPython Driver for the MLX90393 Sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "mlx90393@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_MLX90393"}
 keywords = [
     "micropython",
@@ -30,15 +30,15 @@
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
 packages = ["micropython_mlx90393"]
 
 [tool.setuptools.dynamic]
```

