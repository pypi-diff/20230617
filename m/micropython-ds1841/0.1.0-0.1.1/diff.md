# Comparing `tmp/micropython-ds1841-0.1.0.tar.gz` & `tmp/micropython-ds1841-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-ds1841-0.1.0.tar", last modified: Fri Jun 16 19:51:41 2023, max compression
+gzip compressed data, was "micropython-ds1841-0.1.1.tar", last modified: Sat Jun 17 14:19:26 2023, max compression
```

## Comparing `micropython-ds1841-0.1.0.tar` & `micropython-ds1841-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:51:41.468896 micropython-ds1841-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:51:41.464896 micropython-ds1841-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:51:41.468896 micropython-ds1841-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-16 19:51:41.468896 micropython-ds1841-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:51:41.468896 micropython-ds1841-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:51:41.468896 micropython-ds1841-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:51:41.468896 micropython-ds1841-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-16 19:51:34.000000 micropython-ds1841-0.1.0/examples/ds1841_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/examples.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:51:41.468896 micropython-ds1841-0.1.0/micropython_ds1841/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 19:51:34.000000 micropython-ds1841-0.1.0/micropython_ds1841/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-16 19:51:34.000000 micropython-ds1841-0.1.0/micropython_ds1841/ds1841.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-16 19:51:34.000000 micropython-ds1841-0.1.0/micropython_ds1841/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 19:51:41.468896 micropython-ds1841-0.1.0/micropython_ds1841.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-16 19:51:41.000000 micropython-ds1841-0.1.0/micropython_ds1841.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-16 19:51:41.000000 micropython-ds1841-0.1.0/micropython_ds1841.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 19:51:41.000000 micropython-ds1841-0.1.0/micropython_ds1841.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 19:51:41.000000 micropython-ds1841-0.1.0/micropython_ds1841.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 19:51:41.000000 micropython-ds1841-0.1.0/micropython_ds1841.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-16 19:51:34.000000 micropython-ds1841-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 19:51:26.000000 micropython-ds1841-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 19:51:41.468896 micropython-ds1841-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.037050 micropython-ds1841-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/examples/ds1841_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/micropython_ds1841/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/micropython_ds1841/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/micropython_ds1841/ds1841.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/micropython_ds1841/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 14:19:26.000000 micropython-ds1841-0.1.1/micropython_ds1841.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-17 14:19:18.000000 micropython-ds1841-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:19:10.000000 micropython-ds1841-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:19:26.041051 micropython-ds1841-0.1.1/setup.cfg
```

### Comparing `micropython-ds1841-0.1.0/.gitignore` & `micropython-ds1841-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.0/.pre-commit-config.yaml` & `micropython-ds1841-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.0/.pylintrc` & `micropython-ds1841-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.0/LICENSE` & `micropython-ds1841-0.1.1/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,10 @@
 The MIT License (MIT)
 
 Copyright (c) 2020 Bryan Siepert for Adafruit Industries
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-The MIT License (MIT)
-
 Copyright (c) 2023 Jose D. Montoya
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
```

### Comparing `micropython-ds1841-0.1.0/PKG-INFO` & `micropython-ds1841-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-ds1841
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the DS1841 Potentiometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_DS1841
 Keywords: sensor,micropython,ds1841,micropython,driver,ds1841,potentiometer,analog,devices,resistance
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
 .. image:: https://readthedocs.org/projects/micropython-ds1841/badge/?version=latest
     :target: https://micropython-ds1841.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-ds1841.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-ds1841-0.1.0/README.rst` & `micropython-ds1841-0.1.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Introduction
 ============
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/micropython-ds1841/badge/?version=latest
     :target: https://micropython-ds1841.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-ds1841.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-ds1841-0.1.0/docs/_static/Logo.png` & `micropython-ds1841-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.0/docs/_static/favicon.ico` & `micropython-ds1841-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.0/docs/conf.py` & `micropython-ds1841-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.0/examples/ds1841_simpletest.py` & `micropython-ds1841-0.1.1/examples/ds1841_simpletest.py`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.0/micropython_ds1841/ds1841.py` & `micropython-ds1841-0.1.1/micropython_ds1841/ds1841.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 
 from time import sleep
 from micropython import const
 from micropython_ds1841.i2c_helpers import CBits, RegisterStruct
 
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_DS1841.git"
 
 _IVR = const(0x00)
 _CR0 = const(0x02)
 _CR1 = const(0x03)
 _LUTAR = const(0x08)
 _WR = const(0x09)
```

### Comparing `micropython-ds1841-0.1.0/micropython_ds1841/i2c_helpers.py` & `micropython-ds1841-0.1.1/micropython_ds1841/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.0/micropython_ds1841.egg-info/PKG-INFO` & `micropython-ds1841-0.1.1/micropython_ds1841.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 Metadata-Version: 2.1
 Name: micropython-ds1841
-Version: 0.1.0
+Version: 0.1.1
 Summary: MicroPython Driver for the DS1841 Potentiometer
 Author-email: JDM <xxyx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/MicroPython_DS1841
 Keywords: sensor,micropython,ds1841,micropython,driver,ds1841,potentiometer,analog,devices,resistance
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
 .. image:: https://readthedocs.org/projects/micropython-ds1841/badge/?version=latest
     :target: https://micropython-ds1841.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 
 .. image:: https://img.shields.io/pypi/v/micropython-ds1841.svg
     :alt: latest version on PyPI
```

### Comparing `micropython-ds1841-0.1.0/micropython_ds1841.egg-info/SOURCES.txt` & `micropython-ds1841-0.1.1/micropython_ds1841.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micropython-ds1841-0.1.0/pyproject.toml` & `micropython-ds1841-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-ds1841"
 description = "MicroPython Driver for the DS1841 Potentiometer"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxyx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_DS1841"}
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
 py-modules = ["ds1841"]
 
 [tool.setuptools.dynamic]
```

