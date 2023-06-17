# Comparing `tmp/monalysa-0.0.6.tar.gz` & `tmp/monalysa-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monalysa-0.0.6.tar", max compression
+gzip compressed data, was "monalysa-0.0.7.tar", max compression
```

## Comparing `monalysa-0.0.6.tar` & `monalysa-0.0.7.tar`

### file list

```diff
@@ -1,29 +1,52 @@
--rw-r--r--   0        0        0     1082 2022-10-22 00:53:43.665720 monalysa-0.0.6/LICENSE
--rw-r--r--   0        0        0     1042 2022-10-26 03:39:52.744314 monalysa-0.0.6/README.md
--rw-r--r--   0        0        0     6148 2022-10-25 06:19:52.579292 monalysa-0.0.6/monalysa/.DS_Store
--rw-r--r--   0        0        0       47 2023-02-02 06:36:48.059401 monalysa-0.0.6/monalysa/.idea/.gitignore
--rw-r--r--   0        0        0      478 2023-02-02 06:36:48.059726 monalysa-0.0.6/monalysa/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-02-02 06:36:48.059929 monalysa-0.0.6/monalysa/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      192 2023-02-02 06:36:48.060142 monalysa-0.0.6/monalysa/.idea/misc.xml
--rw-r--r--   0        0        0      268 2023-02-02 06:36:48.060359 monalysa-0.0.6/monalysa/.idea/modules.xml
--rw-r--r--   0        0        0      443 2023-02-02 06:36:48.060569 monalysa-0.0.6/monalysa/.idea/monalysa.iml
--rw-r--r--   0        0        0      183 2023-02-02 06:36:48.060775 monalysa-0.0.6/monalysa/.idea/vcs.xml
--rw-r--r--   0        0        0     1624 2022-10-26 03:50:31.898961 monalysa-0.0.6/monalysa/README.md
--rw-r--r--   0        0        0      141 2022-10-26 06:33:00.428352 monalysa-0.0.6/monalysa/__init__.py
--rw-r--r--   0        0        0     1366 2022-10-25 10:02:49.405111 monalysa-0.0.6/monalysa/misc.py
--rw-r--r--   0        0        0        0 2022-10-23 07:09:30.198480 monalysa-0.0.6/monalysa/preprocess/__init__.py
--rw-r--r--   0        0        0        0 2022-10-23 07:10:00.538584 monalysa-0.0.6/monalysa/quality/__init__.py
--rw-r--r--   0        0        0     7453 2022-10-25 10:01:49.823522 monalysa-0.0.6/monalysa/readers.py
--rw-r--r--   0        0        0        0 2022-10-25 05:53:15.931456 monalysa-0.0.6/monalysa/tests/__init__.py
--rw-r--r--   0        0        0     1604 2022-10-26 06:32:29.378486 monalysa-0.0.6/monalysa/tests/test_misc.py
--rw-r--r--   0        0        0      629 2022-10-26 06:09:06.257416 monalysa-0.0.6/monalysa/tests/test_ulfunc.py
--rw-r--r--   0        0        0      383 2023-02-02 06:53:26.896946 monalysa-0.0.6/monalysa/todo.md
--rw-r--r--   0        0        0     6148 2022-10-25 06:19:57.616213 monalysa-0.0.6/monalysa/ulfunc/.DS_Store
--rw-r--r--   0        0        0       92 2022-10-26 06:03:58.851573 monalysa-0.0.6/monalysa/ulfunc/__init__.py
--rw-r--r--   0        0        0    12329 2023-02-02 06:53:26.897407 monalysa-0.0.6/monalysa/ulfunc/measures.py
--rw-r--r--   0        0        0     3890 2023-02-02 06:53:26.897973 monalysa-0.0.6/monalysa/ulfunc/ulint.py
--rw-r--r--   0        0        0     7783 2023-02-03 03:56:21.013659 monalysa-0.0.6/monalysa/ulfunc/uluse.py
--rw-r--r--   0        0        0        0 2022-10-26 05:56:31.325436 monalysa-0.0.6/monalysa/ulfunc/visualizations.py
--rw-r--r--   0        0        0      558 2023-02-03 04:58:08.062435 monalysa-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 monalysa-0.0.6/setup.py
--rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 monalysa-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-10-22 00:53:43.665720 monalysa-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1040 2023-06-13 10:59:45.465067 monalysa-0.0.7/README.md
+-rw-r--r--   0        0        0     6148 2022-10-25 06:19:52.579292 monalysa-0.0.7/monalysa/.DS_Store
+-rw-r--r--   0        0        0       47 2023-02-02 06:36:48.059401 monalysa-0.0.7/monalysa/.idea/.gitignore
+-rw-r--r--   0        0        0      478 2023-02-02 06:36:48.059726 monalysa-0.0.7/monalysa/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-02-02 06:36:48.059929 monalysa-0.0.7/monalysa/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      192 2023-02-02 06:36:48.060142 monalysa-0.0.7/monalysa/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2023-02-02 06:36:48.060359 monalysa-0.0.7/monalysa/.idea/modules.xml
+-rw-r--r--   0        0        0      443 2023-02-02 06:36:48.060569 monalysa-0.0.7/monalysa/.idea/monalysa.iml
+-rw-r--r--   0        0        0      183 2023-02-02 06:36:48.060775 monalysa-0.0.7/monalysa/.idea/vcs.xml
+-rw-r--r--   0        0        0       37 2022-10-25 06:57:35.628454 monalysa-0.0.7/monalysa/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-10-25 06:57:35.628525 monalysa-0.0.7/monalysa/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-10-25 06:57:35.628367 monalysa-0.0.7/monalysa/.pytest_cache/README.md
+-rw-r--r--   0        0        0      213 2022-10-26 04:26:12.613167 monalysa-0.0.7/monalysa/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      327 2022-10-26 04:27:01.645422 monalysa-0.0.7/monalysa/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-10-26 04:27:01.647487 monalysa-0.0.7/monalysa/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1624 2022-10-26 03:50:31.898961 monalysa-0.0.7/monalysa/README.md
+-rw-r--r--   0        0        0      167 2023-06-17 07:47:38.742131 monalysa-0.0.7/monalysa/__init__.py
+-rw-r--r--   0        0        0     1274 2023-06-17 06:31:40.892658 monalysa-0.0.7/monalysa/misc.py
+-rw-r--r--   0        0        0    10877 2023-06-17 07:16:21.095262 monalysa-0.0.7/monalysa/movements.py
+-rw-r--r--   0        0        0        0 2022-10-23 07:09:30.198480 monalysa-0.0.7/monalysa/preprocess/__init__.py
+-rw-r--r--   0        0        0      170 2022-10-23 07:14:33.644553 monalysa-0.0.7/monalysa/preprocess/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2022-10-23 07:10:00.538584 monalysa-0.0.7/monalysa/quality/__init__.py
+-rw-r--r--   0        0        0      167 2022-10-23 07:14:33.644259 monalysa-0.0.7/monalysa/quality/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13572 2023-06-17 07:10:09.110552 monalysa-0.0.7/monalysa/quality/__pycache__/smoothness.cpython-39.pyc
+-rw-r--r--   0        0        0    14823 2023-06-17 07:07:45.172172 monalysa-0.0.7/monalysa/quality/smoothness.py
+-rw-r--r--   0        0        0     7549 2023-06-17 07:09:54.658172 monalysa-0.0.7/monalysa/readers.py
+-rw-r--r--   0        0        0        0 2022-10-25 05:53:15.931456 monalysa-0.0.7/monalysa/tests/__init__.py
+-rw-r--r--   0        0        0      174 2022-10-25 06:57:34.579384 monalysa-0.0.7/monalysa/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2653 2022-10-25 06:57:34.582061 monalysa-0.0.7/monalysa/tests/__pycache__/test_basic.cpython-39-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0     5456 2022-10-26 06:32:30.680020 monalysa-0.0.7/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.1.pyc
+-rw-r--r--   0        0        0     5456 2022-10-26 06:10:01.482787 monalysa-0.0.7/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0     2878 2022-10-26 06:09:30.228921 monalysa-0.0.7/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.1.pyc
+-rw-r--r--   0        0        0     2878 2022-10-26 06:09:40.412593 monalysa-0.0.7/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0     1604 2022-10-26 06:32:29.378486 monalysa-0.0.7/monalysa/tests/test_misc.py
+-rw-r--r--   0        0        0      629 2022-10-26 06:09:06.257416 monalysa-0.0.7/monalysa/tests/test_ulfunc.py
+-rw-r--r--   0        0        0      383 2023-02-02 06:53:26.896946 monalysa-0.0.7/monalysa/todo.md
+-rw-r--r--   0        0        0     6148 2022-10-25 06:19:57.616213 monalysa-0.0.7/monalysa/ulfunc/.DS_Store
+-rw-r--r--   0        0        0       92 2022-10-26 06:03:58.851573 monalysa-0.0.7/monalysa/ulfunc/__init__.py
+-rw-r--r--   0        0        0      301 2022-10-26 06:04:05.162412 monalysa-0.0.7/monalysa/ulfunc/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6662 2023-06-17 05:52:52.196446 monalysa-0.0.7/monalysa/ulfunc/__pycache__/measures.cpython-39.pyc
+-rw-r--r--   0        0        0     6428 2022-10-23 07:30:14.065832 monalysa-0.0.7/monalysa/ulfunc/__pycache__/ulfunc.cpython-39.pyc
+-rw-r--r--   0        0        0     4154 2023-06-17 06:26:50.387422 monalysa-0.0.7/monalysa/ulfunc/__pycache__/ulint.cpython-39.pyc
+-rw-r--r--   0        0        0     7497 2023-06-17 06:15:39.748132 monalysa-0.0.7/monalysa/ulfunc/__pycache__/uluse.cpython-39.pyc
+-rw-r--r--   0        0        0      181 2023-06-15 08:16:11.174423 monalysa-0.0.7/monalysa/ulfunc/__pycache__/visualizations.cpython-39.pyc
+-rw-r--r--   0        0        0    12452 2023-06-17 05:52:21.294309 monalysa-0.0.7/monalysa/ulfunc/measures.py
+-rw-r--r--   0        0        0     4014 2023-06-17 06:26:26.797777 monalysa-0.0.7/monalysa/ulfunc/ulint.py
+-rw-r--r--   0        0        0     8067 2023-06-17 06:15:33.539036 monalysa-0.0.7/monalysa/ulfunc/uluse.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:15:23.254131 monalysa-0.0.7/monalysa/ulfunc/visualizations.py
+-rw-r--r--   0        0        0      559 2023-06-17 07:48:45.130332 monalysa-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 monalysa-0.0.7/setup.py
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 monalysa-0.0.7/PKG-INFO
```

### Comparing `monalysa-0.0.6/LICENSE` & `monalysa-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.6/README.md` & `monalysa-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # <span style="color:#555"><span style="color:#A62B17">**Mo**</span>vement  A<span style="color:#A62B17">**nalys**</span>is Libr<span style="color:#A62B17">**a**</span>ry (Monalysa)</span>
 
 Monalysa, _aka_ <u>**Mo**</u>ovement a<u>**nalys**</u>is libr<u>**a**</u>y, is a unified python library for the quantitative analysis of sensorimotor behavior. Monalysa provides a set of data structures, functions, and classes for representing, analyzing, and visualizing movement-related data from different technologies (motion capture, inertial measurement units, robots, force/torque sensors, force plates, etc.).
 
 ## Purpose of the library
-In the spirit of open science, the monalysa library provides open-source code for a set of commonly used methods, measures, and tools for analyzing movement data. Such a library would be a step towards the standardization of procedures used for movement analysis.
+In the spirit of open science, the monalysa library provides open-source code for a set of commonly used methods, measures, and tools for analyzing movement data. Such a library can be a step towards the standardization of procedures used for movement analysis.
 
 ## Who is this library for?
 This library is aimed at students, researchers, clinicians and industry professionals working with movement data.
```

### Comparing `monalysa-0.0.6/monalysa/.DS_Store` & `monalysa-0.0.7/monalysa/.DS_Store`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.6/monalysa/README.md` & `monalysa-0.0.7/monalysa/README.md`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.6/monalysa/misc.py` & `monalysa-0.0.7/monalysa/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 """
-misc.py is a module containing a set of additional useful functions for use by 
-other modules in monalysa.
+misc.py is a module containing a set of useful functions monalysa library.
 
-Author: Sivakumar Balasubramanian
-Email: siva82kb@gmail.com
-Date: 25 Oct 2022 
+----
 """
 
 from typing import Union
 import numpy as np
 
 
-def is_integer_num(n: Union[int, float]) -> bool:
+def is_integer_num(num: Union[int, float]) -> bool:
     """Checks if the given number is an integer.
 
     Parameters
     ----------
-    n : Union[int, float]
-        The number that is to be checked if it is an
-        integer.
+    num : Union[int, float]
+          The number that is to be checked if it is an
+          integer.
 
     Returns
     -------
     bool
         Bool indicating if the number is an integer. True if n is an
         integer, else its False
     """
-    if isinstance(n, int):
+    if isinstance(num, int):
         return True
-    if isinstance(n, float):
-        return n.is_integer()
+    if isinstance(num, float):
+        return num.is_integer()
     return False
 
 
 def is_binary_signal(sig: np.array, allownan=False) -> bool:
     """Indicates if the given input signal is a binary signal. Nan values can be allowed.
 
     Parameters
```

### Comparing `monalysa-0.0.6/monalysa/readers.py` & `monalysa-0.0.7/monalysa/readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 """
-readers.py is a module with classes and functions to read data from different
-wearable sensors that are commonly used for movement tracking applications.
+``readers.py`` is a module for reading data from different wearable sensors 
+that are commonly used for movement tracking applications.
+
+The current version supports the following sensor types:
+
+1. `ActiGraph <https://theactigraph.com/>`_ sensor.
+
+----
 """
 
 import pandas
 from pandas import DataFrame
 from pandas import Timestamp, Timedelta
 from datetime import datetime as dt
 import datetime
@@ -54,15 +60,15 @@
         
     @property
     def filename(self):
         return self._filename
     
     @property
     def id(self):
-        return self._devid
+        return self._id
     
     @property
     def head_str(self):
         return self._head_str
     
     @property
     def data(self):
```

### Comparing `monalysa-0.0.6/monalysa/tests/test_misc.py` & `monalysa-0.0.7/monalysa/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.6/monalysa/tests/test_ulfunc.py` & `monalysa-0.0.7/monalysa/tests/test_ulfunc.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.6/monalysa/ulfunc/.DS_Store` & `monalysa-0.0.7/monalysa/ulfunc/.DS_Store`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.6/monalysa/ulfunc/measures.py` & `monalysa-0.0.7/monalysa/ulfunc/measures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 """
-ulfunc.py contains functions and classes for implementing different measures
-for quantifying upper-limb functioning. 
+``ulfunc.py`` contains functions and classes for implementing different measures for quantifying upper-limb functioning. 
+
+----
 """
 
 from scipy import signal
 # from datetime import datetime as dt
 import numpy as np
 
 
-class ULUse(object):
-    """Class implementing different UL use measures as static functions.
-    """
-    @staticmethod
-    def from_activity_counts1(actcounts: np.array,
-                              threshold: float) -> np.array:
-        """A single threshold based algorithm for computing UL use
-        from activity counts.
-
-        Args:
-            actcounts (np.array): 1D numpy array containing the activity counts
-            time series.
-            threshold (float): Threshold for generating the binary UL use
-            output time series.
-
-        Returns:
-            np.array: 1D numpy array of the UL use signal, which is a binary
-            signal indicating the presence or absence of a "functional"
-            movement any time instant.
-        """
-        assert len(actcounts) > 0, "actcounts cannot be a of zero length."
-        assert min(actcounts) >= 0., "Activity count cannot be negative."
+# class ULUse(object):
+#     """Class implementing different UL use measures as static functions.
+#     """
+#     @staticmethod
+#     def from_activity_counts1(actcounts: np.array,
+#                               threshold: float) -> np.array:
+#         """A single threshold based algorithm for computing UL use
+#         from activity counts.
+
+#         Args:
+#             actcounts (np.array): 1D numpy array containing the activity counts
+#             time series.
+#             threshold (float): Threshold for generating the binary UL use
+#             output time series.
+
+#         Returns:
+#             np.array: 1D numpy array of the UL use signal, which is a binary
+#             signal indicating the presence or absence of a "functional"
+#             movement any time instant.
+#         """
+#         assert len(actcounts) > 0, "actcounts cannot be a of zero length."
+#         assert min(actcounts) >= 0., "Activity count cannot be negative."
         
-        return  1.0 * np.array(np.array(actcounts) >= threshold)
+#         return  1.0 * np.array(np.array(actcounts) >= threshold)
     
-    @staticmethod
-    def from_activity_counts2(actcounts: np.array,
-                              threshold0: float,
-                              threshold1: float) -> np.array:
-        """A hysteresis based based algorithm for computing UL use
-        from activity counts.
-        Note: Since this method requires information about the past value of
-        UL use, you must ensure that the activtiy counts input is from a
-        continuous time segment.  
-
-        Args:
-            actcounts (np.array): 1D numpy array containing the activity counts
-            time series.
-            threshold0 (float): Threshold below which UL use signal is 0.
-            threshold1 (float): Threshold above which UL use signal is 1.
-
-        Returns:
-            np.array: 1D numpy array of the UL use signal, which is a binary
-            signal indicating the presence or absence of a "functional"
-            movement any time instant.
-        """
-        assert len(actcounts) > 0, "actcounts cannot be a of zero length."
-        assert min(actcounts) >= 0., "Activity count cannot be negative."
-        assert threshold0 <= threshold1, "threshold0 must be smaller than threshold1."
+#     @staticmethod
+#     def from_activity_counts2(actcounts: np.array,
+#                               threshold0: float,
+#                               threshold1: float) -> np.array:
+#         """A hysteresis based based algorithm for computing UL use
+#         from activity counts.
+#         Note: Since this method requires information about the past value of
+#         UL use, you must ensure that the activtiy counts input is from a
+#         continuous time segment.  
+
+#         Args:
+#             actcounts (np.array): 1D numpy array containing the activity counts
+#             time series.
+#             threshold0 (float): Threshold below which UL use signal is 0.
+#             threshold1 (float): Threshold above which UL use signal is 1.
+
+#         Returns:
+#             np.array: 1D numpy array of the UL use signal, which is a binary
+#             signal indicating the presence or absence of a "functional"
+#             movement any time instant.
+#         """
+#         assert len(actcounts) > 0, "actcounts cannot be a of zero length."
+#         assert min(actcounts) >= 0., "Activity count cannot be negative."
+#         assert threshold0 <= threshold1, "threshold0 must be smaller than threshold1."
         
-        if threshold0 == threshold1:
-            print("Both thresholds are the same. Using from_activity_counts1 function to compute UL use.")
-            return ULUse.from_activity_counts1(actcounts, threshold0)
+#         if threshold0 == threshold1:
+#             print("Both thresholds are the same. Using from_activity_counts1 function to compute UL use.")
+#             return ULUse.from_activity_counts1(actcounts, threshold0)
 
-        _uluse = np.zeros(len(actcounts))
-        _uluse[actcounts >= threshold1] = 1
+#         _uluse = np.zeros(len(actcounts))
+#         _uluse[actcounts >= threshold1] = 1
         
-        # Indices in the intermediate region where the activity count is
-        # less than threshold1 but greater than threshold0.
-        _temp = np.where((actcounts >= threshold0)
-                         * (actcounts < threshold1))[0]
-        # Check if the very first point is in the intermediate region.
-        for i in _temp:
-            _uluse[i] = _uluse[i-1] if i > 0  else 0
+#         # Indices in the intermediate region where the activity count is
+#         # less than threshold1 but greater than threshold0.
+#         _temp = np.where((actcounts >= threshold0)
+#                          * (actcounts < threshold1))[0]
+#         # Check if the very first point is in the intermediate region.
+#         for i in _temp:
+#             _uluse[i] = _uluse[i-1] if i > 0  else 0
         
-        return _uluse
-
+#         return _uluse
 
 # def average_uluse(uluse: np.array, dur: float, sample_t: float) -> np.array:
 #     """Computes the average upper-limb use from the given UL use signal. The
 #     current version only supports causal averaging.
 
 #     Args:
 #         uluse (np.array): 1D numpy array of the UL use (binary) signal whose
@@ -157,15 +157,15 @@
     n_win = int(windur / sample_t)
     n_shift = int(windur / sample_t)
     ulact = signal.lfilter(b=np.ones(n_win), a=np.array([n_win]), x=intsig) 
     return (np.arange(0, len(intsig), n_shift), ulact[::n_shift])
 
 
 def Hq(aua: np.array, q: float) -> float:
-    """Computes the over  upper-limb activity using the average upper-limb
+    """Computes the overall upper-limb activity using the average upper-limb
     activity time series.
 
     Args:
         aua (np.array): 1D numpy array of the average upper-limb activity.
         q (float): Percentile to be used for computing the overall upper-limb
         activity. This value must be between 0 and 100.
```

### Comparing `monalysa-0.0.6/monalysa/ulfunc/ulint.py` & `monalysa-0.0.7/monalysa/ulfunc/ulint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
-ulint.py is a module containing different class, and functions for quanitfying
-the UL intensity construct.
+``ulint.py`` is a module containing different classes, and functions for quanitfying the UL intensity construct.
 
-Author: Sivakumar Balasubramanian
-Date: 17 Oct 2022
-Email: siva82kb@gmail.com 
+The current version of the module contains the following instantaneous UL intensity algorithms:
+
+1. Vector magnitude from the `ActiGraph <https://theactigraph.com/>`_ sensor.
+
+----
 """
 
 import numpy as np
 from scipy import signal
 from datetime import datetime as dt
 
 from .. import misc
@@ -59,15 +60,17 @@
         Time gap between two consecutive window locations.
     sample_t : float
         Sampling time of the intsig and usesig signal.
 
     Returns
     -------
     tuple[np.array, np.array]
-        A tuple of 1D numpy arrays. The first 1D  array is the list of time indices of the computed avarge UL intensity of use signal. The second ID array is the average UL intensity of use signal.
+        A tuple of 1D numpy arrays. The first 1D  array is the list of time
+        indices of the computed avarge UL intensity of use signal. The second
+        ID array is the average UL intensity of use signal.
     """
     
     assert np.shape(intsig) == np.shape(usesig), "intsig and usesig must have the same shape."
     assert np.nanmin(intsig) >= 0., "intsig signal cannot be negative."
     assert windur > 0, "windur (avaraging window duration) must be a positive number."
     assert winshift > 0, "winshift (time shift between consecutive windows) must be a positive number."
     assert sample_t > 0, "sample_t (sampling time) must be a positive number."
```

### Comparing `monalysa-0.0.6/monalysa/ulfunc/uluse.py` & `monalysa-0.0.7/monalysa/ulfunc/uluse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
-uluse.py is a module containing different class, and functions for quanitfying
-the UL use construct.
+``uluse.py`` is a module containing different classes, and functions for quanitfying
+the UL use construct - instantaneous and average use. 
 
-Author: Sivakumar Balasubramanian
-Date: 17 Oct 2022
-Email: siva82kb@gmail.com 
+The current version of the module contains the following instantaneous UL use algorithms:
+
+1. Vector magnitude from the Actigraph sensor (with and without hysterisis)
+2. GMAC (Gross Movement + Activity Countys)
+
+----
 """
 
 import numpy as np
 from scipy import signal
 from datetime import datetime as dt
 from scipy import signal
 
@@ -81,17 +84,20 @@
             _uluse[i] = 0
         else:
             _uluse[i] = _uluse[i - 1] if i > 0 else 0
 
     return (np.arange(len(_uluse)), _uluse)
 
 
-def from_gmac(acc_forearm, acc_ortho1, acc_ortho2, sampfreq, pitch_threshold=30, counts_threshold=0):
+def from_gmac(acc_forearm: np.array, acc_ortho1: np.array, acc_ortho2: np.array,
+              sampfreq: int, pitch_threshold: int=30,
+              counts_threshold: int=0) -> tuple[np.array, np.array]:
     """
     Computes UL use using the GMAC algorithm with pitch and counts estimated only from acceleration.
+    
     Args:
         acc_forearm (np.array):  1D numpy array containing acceleration along the length of the forearm.
         acc_ortho1 (np.array): 1D numpy array containing acceleration along one of the orthogonal axis to the forearm.
         acc_ortho2 (np.array): 1D numpy array containing acceleration along the other orthogonal axis to the forearm.
         sampfreq (int): Sampling frequency of acceleration data.
         pitch_threshold (int): Pitch between +/- pitch_threshold are considered functional, default=30 (Leuenberger et al. 2017).
         counts_threshold (int): Counts greater than counts_threshold are considered functional, default=0 (optimized for youden index).
```

### Comparing `monalysa-0.0.6/pyproject.toml` & `monalysa-0.0.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "monalysa"
-version = "0.0.6"
+version = "0.0.7"
 description = "A unified library for carrying out quantitative movement analysis."
 authors = ["Sivakumar Balasubramanian (Siva) <siva82kb@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/siva82kb/monalysa"
 repository = "https://github.com/siva82kb/monalysa"
 keywords = ["movement analysis", "biomechanics", "neurorehabilitation", "sport science"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry`.api"
```

### Comparing `monalysa-0.0.6/setup.py` & `monalysa-0.0.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 ['monalysa',
  'monalysa.preprocess',
  'monalysa.quality',
  'monalysa.tests',
  'monalysa.ulfunc']
 
 package_data = \
-{'': ['*'], 'monalysa': ['.idea/*', '.idea/inspectionProfiles/*']}
+{'': ['*'],
+ 'monalysa': ['.idea/*',
+              '.idea/inspectionProfiles/*',
+              '.pytest_cache/*',
+              '.pytest_cache/v/cache/*']}
 
 setup_kwargs = {
     'name': 'monalysa',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'A unified library for carrying out quantitative movement analysis.',
-    'long_description': '# <span style="color:#555"><span style="color:#A62B17">**Mo**</span>vement  A<span style="color:#A62B17">**nalys**</span>is Libr<span style="color:#A62B17">**a**</span>ry (Monalysa)</span>\n\nMonalysa, _aka_ <u>**Mo**</u>ovement a<u>**nalys**</u>is libr<u>**a**</u>y, is a unified python library for the quantitative analysis of sensorimotor behavior. Monalysa provides a set of data structures, functions, and classes for representing, analyzing, and visualizing movement-related data from different technologies (motion capture, inertial measurement units, robots, force/torque sensors, force plates, etc.).\n\n## Purpose of the library\nIn the spirit of open science, the monalysa library provides open-source code for a set of commonly used methods, measures, and tools for analyzing movement data. Such a library would be a step towards the standardization of procedures used for movement analysis.\n\n## Who is this library for?\nThis library is aimed at students, researchers, clinicians and industry professionals working with movement data.\n',
+    'long_description': '# <span style="color:#555"><span style="color:#A62B17">**Mo**</span>vement  A<span style="color:#A62B17">**nalys**</span>is Libr<span style="color:#A62B17">**a**</span>ry (Monalysa)</span>\n\nMonalysa, _aka_ <u>**Mo**</u>ovement a<u>**nalys**</u>is libr<u>**a**</u>y, is a unified python library for the quantitative analysis of sensorimotor behavior. Monalysa provides a set of data structures, functions, and classes for representing, analyzing, and visualizing movement-related data from different technologies (motion capture, inertial measurement units, robots, force/torque sensors, force plates, etc.).\n\n## Purpose of the library\nIn the spirit of open science, the monalysa library provides open-source code for a set of commonly used methods, measures, and tools for analyzing movement data. Such a library can be a step towards the standardization of procedures used for movement analysis.\n\n## Who is this library for?\nThis library is aimed at students, researchers, clinicians and industry professionals working with movement data.\n',
     'author': 'Sivakumar Balasubramanian (Siva)',
     'author_email': 'siva82kb@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/siva82kb/monalysa',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `monalysa-0.0.6/PKG-INFO` & `monalysa-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monalysa
-Version: 0.0.6
+Version: 0.0.7
 Summary: A unified library for carrying out quantitative movement analysis.
 Home-page: https://github.com/siva82kb/monalysa
 License: MIT
 Keywords: movement analysis,biomechanics,neurorehabilitation,sport science
 Author: Sivakumar Balasubramanian (Siva)
 Author-email: siva82kb@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -17,12 +17,12 @@
 Description-Content-Type: text/markdown
 
 # <span style="color:#555"><span style="color:#A62B17">**Mo**</span>vement  A<span style="color:#A62B17">**nalys**</span>is Libr<span style="color:#A62B17">**a**</span>ry (Monalysa)</span>
 
 Monalysa, _aka_ <u>**Mo**</u>ovement a<u>**nalys**</u>is libr<u>**a**</u>y, is a unified python library for the quantitative analysis of sensorimotor behavior. Monalysa provides a set of data structures, functions, and classes for representing, analyzing, and visualizing movement-related data from different technologies (motion capture, inertial measurement units, robots, force/torque sensors, force plates, etc.).
 
 ## Purpose of the library
-In the spirit of open science, the monalysa library provides open-source code for a set of commonly used methods, measures, and tools for analyzing movement data. Such a library would be a step towards the standardization of procedures used for movement analysis.
+In the spirit of open science, the monalysa library provides open-source code for a set of commonly used methods, measures, and tools for analyzing movement data. Such a library can be a step towards the standardization of procedures used for movement analysis.
 
 ## Who is this library for?
 This library is aimed at students, researchers, clinicians and industry professionals working with movement data.
```

