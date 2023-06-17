# Comparing `tmp/micropython-mc3479-0.4.0.tar.gz` & `tmp/micropython-mc3479-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-mc3479-0.4.0.tar", last modified: Mon Apr 10 15:24:23 2023, max compression
+gzip compressed data, was "micropython-mc3479-0.4.1.tar", last modified: Sat Jun 17 14:59:10 2023, max compression
```

## Comparing `micropython-mc3479-0.4.0.tar` & `micropython-mc3479-0.4.1.tar`

### file list

```diff
@@ -1,40 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:24:23.394124 micropython-mc3479-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-10 15:24:16.000000 micropython-mc3479-0.4.0/examples/mc3479_acceleration_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-10 15:24:16.000000 micropython-mc3479-0.4.0/examples/mc3479_datarate.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-10 15:24:16.000000 micropython-mc3479-0.4.0/examples/mc3479_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/micropython_mc3479/
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-10 15:24:16.000000 micropython-mc3479-0.4.0/micropython_mc3479/i2c_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-04-10 15:24:16.000000 micropython-mc3479-0.4.0/micropython_mc3479/mc3479.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/micropython_mc3479.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-10 15:24:23.000000 micropython-mc3479-0.4.0/micropython_mc3479.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-10 15:24:23.000000 micropython-mc3479-0.4.0/micropython_mc3479.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 15:24:23.000000 micropython-mc3479-0.4.0/micropython_mc3479.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-10 15:24:23.000000 micropython-mc3479-0.4.0/micropython_mc3479.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-10 15:24:23.000000 micropython-mc3479-0.4.0/micropython_mc3479.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-10 15:24:16.000000 micropython-mc3479-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-10 15:24:09.000000 micropython-mc3479-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 15:24:23.398124 micropython-mc3479-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.721902 micropython-mc3479-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.709901 micropython-mc3479-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.713901 micropython-mc3479-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.713901 micropython-mc3479-0.4.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-17 14:59:10.721902 micropython-mc3479-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.717901 micropython-mc3479-0.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.717901 micropython-mc3479-0.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.717901 micropython-mc3479-0.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/examples/mc3479_acceleration_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/examples/mc3479_datarate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/examples/mc3479_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.717901 micropython-mc3479-0.4.1/micropython_mc3479/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/micropython_mc3479/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/micropython_mc3479/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/micropython_mc3479/mc3479.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:59:10.721902 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 14:59:10.000000 micropython-mc3479-0.4.1/micropython_mc3479.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-17 14:59:03.000000 micropython-mc3479-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:58:55.000000 micropython-mc3479-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:59:10.721902 micropython-mc3479-0.4.1/setup.cfg
```

### Comparing `micropython-mc3479-0.4.0/.gitignore` & `micropython-mc3479-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/.pre-commit-config.yaml` & `micropython-mc3479-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/.pylintrc` & `micropython-mc3479-0.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/LICENSE` & `micropython-mc3479-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/LICENSES/CC-BY-4.0.txt` & `micropython-mc3479-0.4.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/LICENSES/MIT.txt` & `micropython-mc3479-0.4.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/LICENSES/Unlicense.txt` & `micropython-mc3479-0.4.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/docs/examples.rst` & `micropython-mc3479-0.4.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/examples/mc3479_acceleration_range.py` & `micropython-mc3479-0.4.1/examples/mc3479_acceleration_range.py`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/examples/mc3479_datarate.py` & `micropython-mc3479-0.4.1/examples/mc3479_datarate.py`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/micropython_mc3479/i2c_helpers.py` & `micropython-mc3479-0.4.1/micropython_mc3479/i2c_helpers.py`

 * *Files identical despite different names*

### Comparing `micropython-mc3479-0.4.0/micropython_mc3479/mc3479.py` & `micropython-mc3479-0.4.1/micropython_mc3479/mc3479.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 * Author(s): Jose D. Montoya
 
 
 """
 
 from micropython import const
-from  micropython_mc3479.i2c_helpers import CBits, RegisterStruct
+from micropython_mc3479.i2c_helpers import CBits, RegisterStruct
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_MC3479.git"
 
 _I2C_ADDR = const(0x4C)
 _REG_WHOAMI = const(0x98)
 _SENSOR_STATUS_REG = const(0x05)
 _MODE_REG = const(0x07)
 _ACC_RANGE = const(0x20)
@@ -67,15 +67,15 @@
 # pylint: disable= invalid-name, too-many-instance-attributes, missing-function-docstring
 # pylint: disable=too-few-public-methods
 
 
 class MC3479:
     """Driver for the MC3479 Sensor connected over I2C.
 
-    :param ~machine.I2C i2c_bus: The I2C bus the MC3479 is connected to.
+    :param ~machine.I2C i2c: The I2C bus the MC3479 is connected to.
     :param int address: The I2C device address. Defaults to :const:`0x4C`
 
     :raises RuntimeError: if the sensor is not found
 
     **Quickstart: Importing and using the device**
 
     Here is an example of using the :class:`micropython_mc3479.MC3479` class.
```

### Comparing `micropython-mc3479-0.4.0/micropython_mc3479.egg-info/SOURCES.txt` & `micropython-mc3479-0.4.1/micropython_mc3479.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,34 @@
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
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 docs/api.rst
 docs/conf.py
 docs/examples.rst
 docs/index.rst
 docs/requirements.txt
+docs/_static/Logo.png
+docs/_static/extra_css.css
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/mc3479_acceleration_range.py
 examples/mc3479_datarate.py
 examples/mc3479_simpletest.py
+micropython_mc3479/__init__.py
 micropython_mc3479/i2c_helpers.py
 micropython_mc3479/mc3479.py
 micropython_mc3479.egg-info/PKG-INFO
 micropython_mc3479.egg-info/SOURCES.txt
 micropython_mc3479.egg-info/dependency_links.txt
 micropython_mc3479.egg-info/requires.txt
 micropython_mc3479.egg-info/top_level.txt
```

### Comparing `micropython-mc3479-0.4.0/pyproject.toml` & `micropython-mc3479-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-mc3479"
 description = "MicroPython Driver for the MC3479 Accelerometer"
-version = "0.4.0"
+version = "0.4.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "mc3479@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_MC3479"}
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
 packages = ["micropython_mc3479"]
 
 [tool.setuptools.dynamic]
```

