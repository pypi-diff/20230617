# Comparing `tmp/quantile-estimator-0.1.1.tar.gz` & `tmp/quantile-estimator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantile-estimator-0.1.1.tar", last modified: Fri Jun  9 14:28:02 2023, max compression
+gzip compressed data, was "quantile-estimator-0.1.2.tar", last modified: Sat Jun 17 10:58:51 2023, max compression
```

## Comparing `quantile-estimator-0.1.1.tar` & `quantile-estimator-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/quantile_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/quantile_estimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/quantile_estimator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/quantile_estimator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-09 14:28:02.000000 quantile-estimator-0.1.1/quantile_estimator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-09 14:28:02.000000 quantile-estimator-0.1.1/quantile_estimator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:28:02.000000 quantile-estimator-0.1.1/quantile_estimator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 14:28:02.000000 quantile-estimator-0.1.1/quantile_estimator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:58:51.024342 quantile-estimator-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-17 10:58:42.000000 quantile-estimator-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-17 10:58:51.020342 quantile-estimator-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-17 10:58:42.000000 quantile-estimator-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:58:51.020342 quantile-estimator-0.1.2/quantile_estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-06-17 10:58:42.000000 quantile-estimator-0.1.2/quantile_estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 10:58:42.000000 quantile-estimator-0.1.2/quantile_estimator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 10:58:51.020342 quantile-estimator-0.1.2/quantile_estimator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-17 10:58:50.000000 quantile-estimator-0.1.2/quantile_estimator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-17 10:58:50.000000 quantile-estimator-0.1.2/quantile_estimator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 10:58:50.000000 quantile-estimator-0.1.2/quantile_estimator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 10:58:50.000000 quantile-estimator-0.1.2/quantile_estimator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 10:58:51.024342 quantile-estimator-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-17 10:58:42.000000 quantile-estimator-0.1.2/setup.py
```

### Comparing `quantile-estimator-0.1.1/LICENSE` & `quantile-estimator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quantile-estimator-0.1.1/PKG-INFO` & `quantile-estimator-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantile-estimator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Implementation of Graham Cormode and S. Muthukrishnan's Effective Computation of Biased Quantiles over Data Streams in ICDE'05
 Home-page: https://github.com/RefaceAI/quantile-estimator
 Author: RefaceAI
 Author-email: github-support@reface.ai
 License: Apache License 2.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
@@ -18,9 +18,11 @@
 quantile-estimator
 ==========================
 
 Python Implementation of Graham Cormode and S. Muthukrishnan's Effective Computation of Biased Quantiles over Data Streams in ICDE’05
 
 ## Installation
 ```
-pip install quantile-estimator==0.1.1
+pip install quantile-estimator==0.1.2
 ```
+
+This package can be found on [PyPI](https://pypi.org/project/quantile-estimator/).
```

### Comparing `quantile-estimator-0.1.1/quantile_estimator/__init__.py` & `quantile-estimator-0.1.2/quantile_estimator/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,22 @@
         """
         self._flush()
 
         current = self._head
         if not current:
             return float("nan")
 
+        if rank == 0.0:
+            return current._value
+
+        if rank == 1.0:
+            while current._successor:
+                current = current._successor
+            return current._value
+
         mid_rank = math.floor(rank * self._observations)
         max_rank = mid_rank + math.floor(self._invariant(mid_rank, self._observations) / 2)
 
         rank = 0.0
         while current._successor:
             rank += current._rank
             if rank + current._successor._rank + current._successor._delta > max_rank:
@@ -170,16 +178,16 @@
             [0, 1] interval.
         inaccuracy: A floating point value for the allowed error for the
             estimate along the [0, 1] interval.
     """
     def __init__(self, quantile, inaccuracy):
         self._quantile = quantile
         self._inaccuracy = inaccuracy
-        self._coefficient_i = (2.0 * inaccuracy) / (1.0 - quantile)
-        self._coefficient_ii = 2.0 * inaccuracy / quantile
+        self._coefficient_i = (2.0 * inaccuracy) / (1.0 - quantile) if quantile != 1. else float("nan")
+        self._coefficient_ii = 2.0 * inaccuracy / quantile if quantile != .0 else float("nan")
 
     """Computes the delta for the observation."""
     def _delta(self, rank, n):
         if rank <= math.floor((self._quantile * n)):
             return self._coefficient_i * (n - rank)
 
         return self._coefficient_ii * rank
```

### Comparing `quantile-estimator-0.1.1/quantile_estimator.egg-info/PKG-INFO` & `quantile-estimator-0.1.2/quantile_estimator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantile-estimator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Implementation of Graham Cormode and S. Muthukrishnan's Effective Computation of Biased Quantiles over Data Streams in ICDE'05
 Home-page: https://github.com/RefaceAI/quantile-estimator
 Author: RefaceAI
 Author-email: github-support@reface.ai
 License: Apache License 2.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
@@ -18,9 +18,11 @@
 quantile-estimator
 ==========================
 
 Python Implementation of Graham Cormode and S. Muthukrishnan's Effective Computation of Biased Quantiles over Data Streams in ICDE’05
 
 ## Installation
 ```
-pip install quantile-estimator==0.1.1
+pip install quantile-estimator==0.1.2
 ```
+
+This package can be found on [PyPI](https://pypi.org/project/quantile-estimator/).
```

### Comparing `quantile-estimator-0.1.1/setup.py` & `quantile-estimator-0.1.2/setup.py`

 * *Files identical despite different names*

