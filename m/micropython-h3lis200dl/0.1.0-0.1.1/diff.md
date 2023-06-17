# Comparing `tmp/micropython-h3lis200dl-0.1.0.tar.gz` & `tmp/micropython-h3lis200dl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-h3lis200dl-0.1.0.tar", last modified: Fri Jun  9 23:25:33 2023, max compression
+gzip compressed data, was "micropython-h3lis200dl-0.1.1.tar", last modified: Sat Jun 17 15:17:13 2023, max compression
```

## Comparing `micropython-h3lis200dl-0.1.0.tar` & `micropython-h3lis200dl-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:25:33.162364 micropython-h3lis200dl-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:25:33.146364 micropython-h3lis200dl-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:25:33.150364 micropython-h3lis200dl-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-09 23:25:33.162364 micropython-h3lis200dl-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:25:33.154364 micropython-h3lis200dl-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:25:33.154364 micropython-h3lis200dl-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:25:33.158364 micropython-h3lis200dl-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/examples/h3lis200dl_data_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/examples/h3lis200dl_full_scale_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/examples/h3lis200dl_high_pass_filter_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/examples/h3lis200dl_interrupt_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/examples/h3lis200dl_operation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/examples/h3lis200dl_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:25:33.162364 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21195 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl/h3lis200dl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 23:25:33.162364 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-09 23:25:33.000000 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-09 23:25:33.000000 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 23:25:33.000000 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 23:25:33.000000 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 23:25:33.000000 micropython-h3lis200dl-0.1.0/micropython_h3lis200dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-09 23:25:23.000000 micropython-h3lis200dl-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 23:25:13.000000 micropython-h3lis200dl-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 23:25:33.162364 micropython-h3lis200dl-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.286739 micropython-h3lis200dl-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.278739 micropython-h3lis200dl-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-17 15:17:13.286739 micropython-h3lis200dl-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_full_scale_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_high_pass_filter_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_interrupt_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_operation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/examples/h3lis200dl_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.282739 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21195 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/h3lis200dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:17:13.286739 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 15:17:13.000000 micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-17 15:17:05.000000 micropython-h3lis200dl-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:16:58.000000 micropython-h3lis200dl-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:17:13.286739 micropython-h3lis200dl-0.1.1/setup.cfg
```

### Comparing `micropython-h3lis200dl-0.1.0/.gitignore` & `micropython-h3lis200dl-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/.pre-commit-config.yaml` & `micropython-h3lis200dl-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/.pylintrc` & `micropython-h3lis200dl-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/LICENSE` & `micropython-h3lis200dl-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/PKG-INFO` & `micropython-h3lis200dl-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-h3lis200dl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Micropython Driver for the ST H3LIS200DL Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_H3LIS200DL
 Keywords: sensor,micropython,h3lis200dl,aceleration,Micropython,gravity,accelerometer,H3LIS200DL
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
 .. image:: https://readthedocs.org/projects/micropython-h3lis200dl/badge/?version=latest
     :target: https://micropython-h3lis200dl.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-h3lis200dl.svg
     :alt: latest version on PyPI
@@ -34,14 +38,45 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Micropython Driver for the ST H3LIS200DL Accelerometer
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_H3LIS200DL
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_H3LIS200DL
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_H3LIS200DL/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_H3LIS200DL/examples.json
+
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-h3lis200dl/>`_.
```

### Comparing `micropython-h3lis200dl-0.1.0/README.rst` & `micropython-h3lis200dl-0.1.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-h3lis200dl/badge/?version=latest
     :target: https://micropython-h3lis200dl.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-h3lis200dl.svg
     :alt: latest version on PyPI
@@ -17,14 +21,45 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Micropython Driver for the ST H3LIS200DL Accelerometer
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_H3LIS200DL
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_H3LIS200DL
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_H3LIS200DL/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_H3LIS200DL/examples.json
+
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-h3lis200dl/>`_.
```

### Comparing `micropython-h3lis200dl-0.1.0/docs/_static/Logo.png` & `micropython-h3lis200dl-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/docs/_static/favicon.ico` & `micropython-h3lis200dl-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/docs/conf.py` & `micropython-h3lis200dl-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/docs/examples.rst` & `micropython-h3lis200dl-0.1.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/examples/h3lis200dl_data_rate.py` & `micropython-h3lis200dl-0.1.1/examples/h3lis200dl_data_rate.py`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/examples/h3lis200dl_full_scale_selection.py` & `micropython-h3lis200dl-0.1.1/examples/h3lis200dl_full_scale_selection.py`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/examples/h3lis200dl_high_pass_filter_cutoff.py` & `micropython-h3lis200dl-0.1.1/examples/h3lis200dl_high_pass_filter_cutoff.py`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/examples/h3lis200dl_interrupt_example.py` & `micropython-h3lis200dl-0.1.1/examples/h3lis200dl_interrupt_example.py`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/examples/h3lis200dl_operation_mode.py` & `micropython-h3lis200dl-0.1.1/examples/h3lis200dl_operation_mode.py`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/micropython_h3lis200dl/h3lis200dl.py` & `micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/h3lis200dl.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_H3LIS200DL.git"
 
 _REG_WHOAMI = const(0x0F)
 _CTRL_REG1 = const(0x20)
 _CTRL_REG2 = const(0x21)
 _CTRL_REG3 = const(0x22)
 _CTRL_REG4 = const(0x23)
```

### Comparing `micropython-h3lis200dl-0.1.0/micropython_h3lis200dl/i2c_helpers.py` & `micropython-h3lis200dl-0.1.1/micropython_h3lis200dl/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-h3lis200dl-0.1.0/micropython_h3lis200dl.egg-info/PKG-INFO` & `micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-h3lis200dl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Micropython Driver for the ST H3LIS200DL Accelerometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_H3LIS200DL
 Keywords: sensor,micropython,h3lis200dl,aceleration,Micropython,gravity,accelerometer,H3LIS200DL
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
 .. image:: https://readthedocs.org/projects/micropython-h3lis200dl/badge/?version=latest
     :target: https://micropython-h3lis200dl.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-h3lis200dl.svg
     :alt: latest version on PyPI
@@ -34,14 +38,45 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 Micropython Driver for the ST H3LIS200DL Accelerometer
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_H3LIS200DL
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_H3LIS200DL
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_H3LIS200DL/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_H3LIS200DL/examples.json
+
 
 
 Installing from PyPI
 =====================
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-h3lis200dl/>`_.
```

### Comparing `micropython-h3lis200dl-0.1.0/micropython_h3lis200dl.egg-info/SOURCES.txt` & `micropython-h3lis200dl-0.1.1/micropython_h3lis200dl.egg-info/SOURCES.txt`

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

### Comparing `micropython-h3lis200dl-0.1.0/pyproject.toml` & `micropython-h3lis200dl-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-h3lis200dl"
 description = "Micropython Driver for the ST H3LIS200DL Accelerometer"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_H3LIS200DL"}
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
 py-modules = ["h3lis200dl"]
 
 [tool.setuptools.dynamic]
```

