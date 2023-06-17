# Comparing `tmp/micropython-dps310-0.1.0.tar.gz` & `tmp/micropython-dps310-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-dps310-0.1.0.tar", last modified: Wed Apr 19 16:45:28 2023, max compression
+gzip compressed data, was "micropython-dps310-0.1.1.tar", last modified: Sat Jun 17 15:23:28 2023, max compression
```

## Comparing `micropython-dps310-0.1.0.tar` & `micropython-dps310-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:28.266741 micropython-dps310-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:28.262741 micropython-dps310-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:28.262741 micropython-dps310-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-19 16:45:28.266741 micropython-dps310-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:28.266741 micropython-dps310-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:28.266741 micropython-dps310-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:28.266741 micropython-dps310-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-19 16:45:18.000000 micropython-dps310-0.1.0/examples/dps310_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:28.266741 micropython-dps310-0.1.0/micropython_dps310/
--rw-r--r--   0 runner    (1001) docker     (123)    21936 2023-04-19 16:45:18.000000 micropython-dps310-0.1.0/micropython_dps310/dps310.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-19 16:45:18.000000 micropython-dps310-0.1.0/micropython_dps310/i2c_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:45:28.266741 micropython-dps310-0.1.0/micropython_dps310.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-19 16:45:28.000000 micropython-dps310-0.1.0/micropython_dps310.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-19 16:45:28.000000 micropython-dps310-0.1.0/micropython_dps310.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:45:28.000000 micropython-dps310-0.1.0/micropython_dps310.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 16:45:28.000000 micropython-dps310-0.1.0/micropython_dps310.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 16:45:28.000000 micropython-dps310-0.1.0/micropython_dps310.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-19 16:45:18.000000 micropython-dps310-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-19 16:45:06.000000 micropython-dps310-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:45:28.266741 micropython-dps310-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.080263 micropython-dps310-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.072263 micropython-dps310-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/examples/dps310_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/examples/dps310_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/examples/dps310_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/micropython_dps310/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/micropython_dps310/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23255 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/micropython_dps310/dps310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/micropython_dps310/i2c_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:23:28.076263 micropython-dps310-0.1.1/micropython_dps310.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 15:23:28.000000 micropython-dps310-0.1.1/micropython_dps310.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-17 15:23:20.000000 micropython-dps310-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:23:11.000000 micropython-dps310-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:23:28.080263 micropython-dps310-0.1.1/setup.cfg
```

### Comparing `micropython-dps310-0.1.0/.gitignore` & `micropython-dps310-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-dps310-0.1.0/.pre-commit-config.yaml` & `micropython-dps310-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-dps310-0.1.0/.pylintrc` & `micropython-dps310-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-dps310-0.1.0/LICENSE` & `micropython-dps310-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-dps310-0.1.0/micropython_dps310/dps310.py` & `micropython-dps310-0.1.1/micropython_dps310/dps310.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,23 +27,17 @@
 from micropython_dps310.i2c_helpers import CBits, RegisterStruct
 
 try:
     import struct
 except ImportError:
     import ustruct as struct
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/MicroPython_DPS310.git"
 
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
-
-
 _REG_WHOAMI = const(0x77)
 _DEVICE_ID = const(0x0D)
 _PRS_CFG = const(0x06)
 _TMP_CFG = const(0x07)
 _MEAS_CFG = const(0x08)
 _CFGREG = const(0x09)
 _RESET = const(0x0C)
@@ -180,24 +174,14 @@
         2: 8.4,
         3: 14.8,
         4: 27.6,
         5: 53.2,
         6: 104.4,
         7: 206.8,
     }
-    _oversample_scalefactor = (
-        524288,
-        1572864,
-        3670016,
-        7864320,
-        253952,
-        516096,
-        1040384,
-        2088960,
-    )
 
     _calib_coeff_temp_src_bit = CBits(1, _TMPCOEFSRCE, 7)
 
     _soft_reset = CBits(4, 0x0C, 0)
 
     def __init__(self, i2c, address=_REG_WHOAMI):
         self._i2c = i2c
@@ -231,32 +215,38 @@
 
         self._wait_temperature_ready()
         self._wait_pressure_ready()
 
     @property
     def pressure_oversample(self):
         """
+        Pressure Oversample. In order to achieve a higher precision, the sensor DPS310
+        will read multiple times ( oversampling ), and combine the readings into one result.
+        This increases the current consumption and also the measurement time, reducing the
+        maximum possible measurement rate. It is necessary to balance the accuracy and data rate
+        required for each application with the allowable current consumption.
+
         +------------------------------------------+-------------------------------------------------------------------+
         | Mode                                     | Value                                                             |
         +==========================================+===================================================================+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_1`   | :py:const:`const(0b000)  # 1 time (Pressure Low Precision)`       |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_1`   | :py:const:`0b000`  # 1 time (Pressure Low Precision)              |
         +------------------------------------------+-------------------------------------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_2`   | :py:const:`const(0b001)  # 2 times (Pressure Low Power)`          |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_2`   | :py:const:`0b001`  # 2 times (Pressure Low Power)                 |
         +------------------------------------------+-------------------------------------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_4`   | :py:const:`const(0b010)  # 4 times`                               |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_4`   | :py:const:`0b010`  # 4 times                                      |
         +------------------------------------------+-------------------------------------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_8`   | :py:const:`const(0b011)  # 8 times`                               |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_8`   | :py:const:`0b011`  # 8 times                                      |
         +------------------------------------------+-------------------------------------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_16`  | :py:const:`const(0b100)  # 16 times (Pressure Standard).**`       |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_16`  | :py:const:`0b100`  # 16 times (Pressure Standard).**              |
         +------------------------------------------+-------------------------------------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_32`  | :py:const:`const(0b101)  # 32 times **`                           |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_32`  | :py:const:`0b101`  # 32 times **                                  |
         +------------------------------------------+-------------------------------------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_64`  | :py:const:`const(0b110)  # 64 times (Pressure High Precision) **` |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_64`  | :py:const:`0b110`  # 64 times (Pressure High Precision) **        |
         +------------------------------------------+-------------------------------------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_128` | :py:const:`const(0b111)  # 128 times **`                          |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_128` | :py:const:`0b111`  # 128 times **                                 |
         +------------------------------------------+-------------------------------------------------------------------+
         """
 
         oversamples = {
             0: "SAMPLE_PER_SECOND_1",
             1: "SAMPLE_PER_SECOND_2",
             2: "SAMPLE_PER_SECOND_4",
@@ -278,29 +268,29 @@
 
     @property
     def pressure_rate(self):
         """
         +--------------------------------+--------------------------+
         | Mode                           | Value                    |
         +================================+==========================+
-        | :py:const:`dps310.RATE_1_HZ`   | :py:const:`const(0b000)` |
+        | :py:const:`dps310.RATE_1_HZ`   | :py:const:`0b000`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_2_HZ`   | :py:const:`const(0b001)` |
+        | :py:const:`dps310.RATE_2_HZ`   | :py:const:`0b001`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_4_HZ`   | :py:const:`const(0b010)` |
+        | :py:const:`dps310.RATE_4_HZ`   | :py:const:`0b010`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_8_HZ`   | :py:const:`const(0b011)` |
+        | :py:const:`dps310.RATE_8_HZ`   | :py:const:`0b011`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_16_HZ`  | :py:const:`const(0b100)` |
+        | :py:const:`dps310.RATE_16_HZ`  | :py:const:`0b100`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_32_HZ`  | :py:const:`const(0b101)` |
+        | :py:const:`dps310.RATE_32_HZ`  | :py:const:`0b101`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_64_HZ`  | :py:const:`const(0b110)` |
+        | :py:const:`dps310.RATE_64_HZ`  | :py:const:`0b110`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_128_HZ` | :py:const:`const(0b111)` |
+        | :py:const:`dps310.RATE_128_HZ` | :py:const:`0b111`        |
         +--------------------------------+--------------------------+
         """
 
         rates = {
             0: "RATE_1_HZ",
             1: "RATE_2_HZ",
             2: "RATE_4_HZ",
@@ -317,32 +307,38 @@
         if value not in rates_values:
             raise ValueError("Value must be a valid rate setting")
         self._pressure_rate = value
 
     @property
     def temperature_oversample(self):
         """
+        Temperature Oversample. In order to achieve a higher precision, the sensor DPS310
+        will read multiple times ( oversampling ), and combine the readings into one result.
+        This increases the current consumption and also the measurement time, reducing the
+        maximum possible measurement rate. It is necessary to balance the accuracy and data rate
+        required for each application with the allowable current consumption.
+
         +------------------------------------------+---------------------------------------+
         | Mode                                     | Value                                 |
         +==========================================+=======================================+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_1`   | :py:const:`const(0b000)  # 1 time`    |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_1`   | :py:const:`0b000`  # 1 time           |
         +------------------------------------------+---------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_2`   | :py:const:`const(0b001)  # 2 times`   |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_2`   | :py:const:`0b001`  # 2 times          |
         +------------------------------------------+---------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_4`   | :py:const:`const(0b010)  # 4 times`   |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_4`   | :py:const:`0b010`  # 4 times          |
         +------------------------------------------+---------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_8`   | :py:const:`const(0b011)  # 8 times`   |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_8`   | :py:const:`0b011`  # 8 times          |
         +------------------------------------------+---------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_16`  | :py:const:`const(0b100)  # 16 times`  |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_16`  | :py:const:`0b100`  # 16 times         |
         +------------------------------------------+---------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_32`  | :py:const:`const(0b101)  # 32 times`  |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_32`  | :py:const:`0b101`  # 32 times         |
         +------------------------------------------+---------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_64`  | :py:const:`const(0b110)  # 64 times`  |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_64`  | :py:const:`0b110`  # 64 times         |
         +------------------------------------------+---------------------------------------+
-        | :py:const:`dps310.SAMPLE_PER_SECOND_128` | :py:const:`const(0b111)  # 128 times` |
+        | :py:const:`dps310.SAMPLE_PER_SECOND_128` | :py:const:`0b111`  # 128 times        |
         +------------------------------------------+---------------------------------------+
         """
         return oversamples_values[self._temperature_oversample]
 
     @temperature_oversample.setter
     def temperature_oversample(self, value: int):
         if value not in oversamples_values:
@@ -353,29 +349,29 @@
 
     @property
     def temperature_rate(self):
         """
         +--------------------------------+--------------------------+
         | Mode                           | Value                    |
         +================================+==========================+
-        | :py:const:`dps310.RATE_1_HZ`   | :py:const:`const(0b000)` |
+        | :py:const:`dps310.RATE_1_HZ`   | :py:const:`0b000`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_2_HZ`   | :py:const:`const(0b001)` |
+        | :py:const:`dps310.RATE_2_HZ`   | :py:const:`0b001`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_4_HZ`   | :py:const:`const(0b010)` |
+        | :py:const:`dps310.RATE_4_HZ`   | :py:const:`0b010`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_8_HZ`   | :py:const:`const(0b011)` |
+        | :py:const:`dps310.RATE_8_HZ`   | :py:const:`0b011`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_16_HZ`  | :py:const:`const(0b100)` |
+        | :py:const:`dps310.RATE_16_HZ`  | :py:const:`0b100`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_32_HZ`  | :py:const:`const(0b101)` |
+        | :py:const:`dps310.RATE_32_HZ`  | :py:const:`0b101`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_64_HZ`  | :py:const:`const(0b110)` |
+        | :py:const:`dps310.RATE_64_HZ`  | :py:const:`0b110`        |
         +--------------------------------+--------------------------+
-        | :py:const:`dps310.RATE_128_HZ` | :py:const:`const(0b111)` |
+        | :py:const:`dps310.RATE_128_HZ` | :py:const:`0b111`        |
         +--------------------------------+--------------------------+
         """
         rates = {
             0: "RATE_1_HZ",
             1: "RATE_2_HZ",
             2: "RATE_4_HZ",
             3: "RATE_8_HZ",
@@ -527,7 +523,25 @@
         """The altitude in meters based on the sea level pressure
         (:attr:`sea_level_pressure`) - which you must enter
         ahead of time
         """
         return 44330 * (
             1.0 - math.pow(self.pressure / self._sea_level_pressure, 0.1903)
         )
+
+    @property
+    def temperature(self) -> float:
+        """The current temperature reading in Celsius"""
+        scaled_rawtemp = self._raw_temperature / self._temp_scale
+        temp = scaled_rawtemp * self._c1 + self._c0 / 2.0
+        return temp
+
+    @property
+    def sea_level_pressure(self) -> float:
+        """The local sea level pressure in hectoPascals (aka millibars). This is used
+        for calculation of :attr:`altitude`. Values are typically in the range
+        980 - 1030."""
+        return self._sea_level_pressure
+
+    @sea_level_pressure.setter
+    def sea_level_pressure(self, value: float) -> None:
+        self._sea_level_pressure = value
```

### Comparing `micropython-dps310-0.1.0/micropython_dps310/i2c_helpers.py` & `micropython-dps310-0.1.1/micropython_dps310/i2c_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,7 +132,17 @@
                 ),
             )
         return value
 
     def __set__(self, obj, value):
         mem_value = value.to_bytes(self.lenght, "big")
         obj._i2c.writeto_mem(obj._address, self.register, mem_value)
+
+
+def twos_complement(val: int, bits: int) -> int:
+    """
+    Two complements
+    """
+    if val & (1 << (bits - 1)):
+        val -= 1 << bits
+
+    return val
```

### Comparing `micropython-dps310-0.1.0/pyproject.toml` & `micropython-dps310-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-dps310"
 description = "MicroPython Driver for the DPS310 sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "dps310@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/MicroPython_dps310"}
 keywords = [
     "micropython",
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
 packages = ["micropython_dps310"]
 
 [tool.setuptools.dynamic]
```

