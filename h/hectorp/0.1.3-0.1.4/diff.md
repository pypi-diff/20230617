# Comparing `tmp/hectorp-0.1.3.tar.gz` & `tmp/hectorp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hectorp-0.1.3.tar", last modified: Tue Jun 13 08:25:25 2023, max compression
+gzip compressed data, was "hectorp-0.1.4.tar", last modified: Sat Jun 17 17:30:24 2023, max compression
```

## Comparing `hectorp-0.1.3.tar` & `hectorp-0.1.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-13 08:25:25.717112 hectorp-0.1.3/
--rw-r--r--   0 msbos      (501) staff       (20)    35149 2021-12-30 10:00:17.000000 hectorp-0.1.3/LICENSE
--rw-r--r--   0 msbos      (501) staff       (20)     7673 2023-06-13 08:25:25.716523 hectorp-0.1.3/PKG-INFO
--rw-r--r--   0 msbos      (501) staff       (20)     7108 2022-08-19 15:58:12.000000 hectorp-0.1.3/README.md
--rw-r--r--   0 msbos      (501) staff       (20)      104 2021-12-30 10:00:17.000000 hectorp-0.1.3/pyproject.toml
--rw-r--r--   0 msbos      (501) staff       (20)       38 2023-06-13 08:25:25.717275 hectorp-0.1.3/setup.cfg
--rw-r--r--   0 msbos      (501) staff       (20)     1841 2023-06-13 08:24:37.000000 hectorp-0.1.3/setup.py
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-13 08:25:25.660943 hectorp-0.1.3/src/
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-13 08:25:25.709983 hectorp-0.1.3/src/hectorp/
--rw-r--r--   0 msbos      (501) staff       (20)        0 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/__init__.py
--rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/ammargrag.py
--rw-r--r--   0 msbos      (501) staff       (20)    10305 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/apply_WF.py
--rw-r--r--   0 msbos      (501) staff       (20)     4453 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/ar1.py
--rw-r--r--   0 msbos      (501) staff       (20)     3888 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/control.py
--rw-r--r--   0 msbos      (501) staff       (20)     2217 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/convert_rlrdata2mom.py
--rw-r--r--   0 msbos      (501) staff       (20)     7568 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/covariance.py
--rw-r--r--   0 msbos      (501) staff       (20)     3395 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/datasnooping.py
--rw-r--r--   0 msbos      (501) staff       (20)     1817 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/date2mjd.py
--rw-r--r--   0 msbos      (501) staff       (20)    14416 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/designmatrix.py
--rw-r--r--   0 msbos      (501) staff       (20)     8101 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/estimate_all_trends.py
--rw-r--r--   0 msbos      (501) staff       (20)    12518 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/estimatespectrum.py
--rw-r--r--   0 msbos      (501) staff       (20)     5701 2023-05-21 13:30:24.000000 hectorp-0.1.3/src/hectorp/estimatetrend.py
--rw-r--r--   0 msbos      (501) staff       (20)     8135 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/findoffsets.py
--rw-r--r--   0 msbos      (501) staff       (20)     3082 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/fullcov.py
--rw-r--r--   0 msbos      (501) staff       (20)     9744 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/ggm.py
--rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/levinson.py
--rw-r--r--   0 msbos      (501) staff       (20)     7625 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/matern.py
--rw-r--r--   0 msbos      (501) staff       (20)     1617 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/mjd2date.py
--rw-r--r--   0 msbos      (501) staff       (20)     9677 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/mle.py
--rw-r--r--   0 msbos      (501) staff       (20)     4204 2023-05-21 12:14:12.000000 hectorp-0.1.3/src/hectorp/msf.py
--rw-r--r--   0 msbos      (501) staff       (20)     3923 2023-05-20 07:28:42.000000 hectorp-0.1.3/src/hectorp/msfdump.py
--rw-r--r--   0 msbos      (501) staff       (20)     3527 2023-05-19 15:58:55.000000 hectorp-0.1.3/src/hectorp/msfgen.py
--rw-r--r--   0 msbos      (501) staff       (20)     3316 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/mycalendar.py
--rw-r--r--   0 msbos      (501) staff       (20)    16821 2023-05-21 14:07:16.000000 hectorp-0.1.3/src/hectorp/observations.py
--rw-r--r--   0 msbos      (501) staff       (20)     2574 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/ols.py
--rw-r--r--   0 msbos      (501) staff       (20)     4682 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/powerlaw.py
--rw-r--r--   0 msbos      (501) staff       (20)     8520 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/predicttrenderror.py
--rw-r--r--   0 msbos      (501) staff       (20)     1102 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/pyfftw_ex1.py
--rw-r--r--   0 msbos      (501) staff       (20)     4866 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/removeoutliers.py
--rw-r--r--   0 msbos      (501) staff       (20)       55 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/run_schur.py
--rw-r--r--   0 msbos      (501) staff       (20)     8995 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/schur.py
--rw-r--r--   0 msbos      (501) staff       (20)    11672 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/simulatenoise.py
--rw-r--r--   0 msbos      (501) staff       (20)     9805 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/test_Schur.py
--rw-r--r--   0 msbos      (501) staff       (20)     1050 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/test_opencl.py
--rw-r--r--   0 msbos      (501) staff       (20)     1852 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/test_reikna.py
--rw-r--r--   0 msbos      (501) staff       (20)     5265 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/varyingannual.py
--rw-r--r--   0 msbos      (501) staff       (20)     3067 2023-05-19 13:52:41.000000 hectorp-0.1.3/src/hectorp/white.py
-drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-13 08:25:25.715696 hectorp-0.1.3/src/hectorp.egg-info/
--rw-r--r--   0 msbos      (501) staff       (20)     7673 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/PKG-INFO
--rw-r--r--   0 msbos      (501) staff       (20)     1218 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/SOURCES.txt
--rw-r--r--   0 msbos      (501) staff       (20)        1 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/dependency_links.txt
--rw-r--r--   0 msbos      (501) staff       (20)      596 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/entry_points.txt
--rw-r--r--   0 msbos      (501) staff       (20)       37 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/requires.txt
--rw-r--r--   0 msbos      (501) staff       (20)        8 2023-06-13 08:25:25.000000 hectorp-0.1.3/src/hectorp.egg-info/top_level.txt
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-17 17:30:24.757862 hectorp-0.1.4/
+-rw-r--r--   0 msbos      (501) staff       (20)    35149 2021-12-30 10:00:17.000000 hectorp-0.1.4/LICENSE
+-rw-r--r--   0 msbos      (501) staff       (20)     7628 2023-06-17 17:30:24.757492 hectorp-0.1.4/PKG-INFO
+-rw-r--r--   0 msbos      (501) staff       (20)     7063 2023-06-17 17:28:12.000000 hectorp-0.1.4/README.md
+-rw-r--r--   0 msbos      (501) staff       (20)      104 2021-12-30 10:00:17.000000 hectorp-0.1.4/pyproject.toml
+-rw-r--r--   0 msbos      (501) staff       (20)       38 2023-06-17 17:30:24.757985 hectorp-0.1.4/setup.cfg
+-rw-r--r--   0 msbos      (501) staff       (20)     1841 2023-06-17 17:26:23.000000 hectorp-0.1.4/setup.py
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-17 17:30:24.734069 hectorp-0.1.4/src/
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-17 17:30:24.754075 hectorp-0.1.4/src/hectorp/
+-rw-r--r--   0 msbos      (501) staff       (20)        0 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/__init__.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7125 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/ammargrag.py
+-rw-r--r--   0 msbos      (501) staff       (20)    10305 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/apply_WF.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4453 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/ar1.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3888 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/control.py
+-rw-r--r--   0 msbos      (501) staff       (20)     2217 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/convert_rlrdata2mom.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7568 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/covariance.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3395 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/datasnooping.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1817 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/date2mjd.py
+-rw-r--r--   0 msbos      (501) staff       (20)    14416 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/designmatrix.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8101 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/estimate_all_trends.py
+-rw-r--r--   0 msbos      (501) staff       (20)    12518 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/estimatespectrum.py
+-rw-r--r--   0 msbos      (501) staff       (20)     5702 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/estimatetrend.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8135 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/findoffsets.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3082 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/fullcov.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9744 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/ggm.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7122 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/levinson.py
+-rw-r--r--   0 msbos      (501) staff       (20)     7625 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/matern.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1617 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/mjd2date.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9677 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/mle.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4205 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/msf.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3923 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/msfdump.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3527 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/msfgen.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3316 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/mycalendar.py
+-rw-r--r--   0 msbos      (501) staff       (20)    16821 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/observations.py
+-rw-r--r--   0 msbos      (501) staff       (20)     2574 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/ols.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4682 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/powerlaw.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8520 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/predicttrenderror.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1102 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/pyfftw_ex1.py
+-rw-r--r--   0 msbos      (501) staff       (20)     4866 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/removeoutliers.py
+-rw-r--r--   0 msbos      (501) staff       (20)       55 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/run_schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)     8995 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)    11672 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/simulatenoise.py
+-rw-r--r--   0 msbos      (501) staff       (20)     9805 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/test_Schur.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1050 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/test_opencl.py
+-rw-r--r--   0 msbos      (501) staff       (20)     1852 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/test_reikna.py
+-rw-r--r--   0 msbos      (501) staff       (20)     5265 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/varyingannual.py
+-rw-r--r--   0 msbos      (501) staff       (20)     3067 2023-06-17 17:28:34.000000 hectorp-0.1.4/src/hectorp/white.py
+drwxr-xr-x   0 msbos      (501) staff       (20)        0 2023-06-17 17:30:24.756999 hectorp-0.1.4/src/hectorp.egg-info/
+-rw-r--r--   0 msbos      (501) staff       (20)     7628 2023-06-17 17:30:24.000000 hectorp-0.1.4/src/hectorp.egg-info/PKG-INFO
+-rw-r--r--   0 msbos      (501) staff       (20)     1218 2023-06-17 17:30:24.000000 hectorp-0.1.4/src/hectorp.egg-info/SOURCES.txt
+-rw-r--r--   0 msbos      (501) staff       (20)        1 2023-06-17 17:30:24.000000 hectorp-0.1.4/src/hectorp.egg-info/dependency_links.txt
+-rw-r--r--   0 msbos      (501) staff       (20)      596 2023-06-17 17:30:24.000000 hectorp-0.1.4/src/hectorp.egg-info/entry_points.txt
+-rw-r--r--   0 msbos      (501) staff       (20)       37 2023-06-17 17:30:24.000000 hectorp-0.1.4/src/hectorp.egg-info/requires.txt
+-rw-r--r--   0 msbos      (501) staff       (20)        8 2023-06-17 17:30:24.000000 hectorp-0.1.4/src/hectorp.egg-info/top_level.txt
```

### Comparing `hectorp-0.1.3/LICENSE` & `hectorp-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/PKG-INFO` & `hectorp-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectorp
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of programs to analyse geodetic time series
 Home-page: https://gitlab.com/machielsimonbos/hectorp
 Author: Machiel Bos
 Author-email: machielbos@protonmail.com
 Project-URL: Bug Tracker, https://gitlab.com/machielsimonbos/hectorp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -112,9 +112,7 @@
 | 5000 10% |      16 |       63.8 |
 | 8000 10% |      33 |       81.0 |
 | 5000 20% |      26 |       70.0 |
 | 8000 20% |      60 |      140.0 |
 
 
 
-
-### 4. References <a name="references"></a>
```

### Comparing `hectorp-0.1.3/README.md` & `hectorp-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -97,9 +97,7 @@
 | 5000 10% |      16 |       63.8 |
 | 8000 10% |      33 |       81.0 |
 | 5000 20% |      26 |       70.0 |
 | 8000 20% |      60 |      140.0 |
 
 
 
-
-### 4. References <a name="references"></a>
```

### Comparing `hectorp-0.1.3/setup.py` & `hectorp-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hectorp",
-    version="0.1.3",
+    version="0.1.4",
     author="Machiel Bos",
     author_email="machielbos@protonmail.com",
     description="A collection of programs to analyse geodetic time series",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/machielsimonbos/hectorp",
     project_urls={
```

### Comparing `hectorp-0.1.3/src/hectorp/ammargrag.py` & `hectorp-0.1.4/src/hectorp/levinson.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # for Toeplitz Systems", By Michael K. Ng  (page 28-29)
 #
 # Equations are taken from Bos et al. (2013), "Fast error analysis of 
 # continuous GNSS observations with missing data", Journal of Geodesy,
 # DOI 10.1007/s00190-012-0605-0.
 #
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/apply_WF.py` & `hectorp-0.1.4/src/hectorp/apply_WF.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/src/hectorp/ar1.py` & `hectorp-0.1.4/src/hectorp/ar1.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/src/hectorp/control.py` & `hectorp-0.1.4/src/hectorp/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # control.py
 #
-# This file is part of HectorP 0.1.2
+# This file is part of HectorP 0.1.4
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/convert_rlrdata2mom.py` & `hectorp-0.1.4/src/hectorp/convert_rlrdata2mom.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/src/hectorp/covariance.py` & `hectorp-0.1.4/src/hectorp/covariance.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  1) power-law noise using Eq. (7) of Bos et al. (2008).
 #  2) white noise
 #
 # Bos, MS, Fernandes, RMS, Williams, SDP & Bastos, L (2008). "Fast error 
 # analysis of continuous GPS observations". Journal of Geodesy, 82(3), 157-166.
 #
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/datasnooping.py` & `hectorp-0.1.4/src/hectorp/datasnooping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # datasnooping.py
 #
 # Class which computes residuals and removes outliers
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/date2mjd.py` & `hectorp-0.1.4/src/hectorp/date2mjd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This small program computes the Modified Julian Date (MJD).
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
```

### Comparing `hectorp-0.1.3/src/hectorp/designmatrix.py` & `hectorp-0.1.4/src/hectorp/designmatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # designmatrix.py
 #
 # Create design matrix
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/estimate_all_trends.py` & `hectorp-0.1.4/src/hectorp/estimate_all_trends.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program find all files in ./obs_files and estimate all trends.
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -153,15 +153,15 @@
 #===============================================================================
 # Main program
 #===============================================================================
 
 def main():
 
     print("\n*******************************************")
-    print("    estimate_all_trends, version 0.1.2")
+    print("    estimate_all_trends, version 0.1.4")
     print("*******************************************\n")
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Estimate all trends')
 
     #--- List arguments that can be given 
     parser.add_argument('-n', dest='noisemodels', action='store',default='PLWN',
```

### Comparing `hectorp-0.1.3/src/hectorp/estimatespectrum.py` & `hectorp-0.1.4/src/hectorp/estimatespectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This program uses the Welch method of scipy to compute the power spectral 
 # density (one-sided).
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -185,15 +185,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    estimatespectrum, version 0.1.2")
+        print("    estimatespectrum, version 0.1.4")
         print("***************************************")
 
     #--- Get Classes
     observations = Observations()
 
     #--- Sampling frequency (change daily period into number of seconds)
     DeltaT = observations.sampling_period
```

### Comparing `hectorp-0.1.3/src/hectorp/estimatetrend.py` & `hectorp-0.1.4/src/hectorp/estimatetrend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program estimates a trend from the observations.
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -67,15 +67,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    estimatetrend, version 0.1.2")
+        print("    estimatetrend, version 0.1.4")
         print("***************************************")
 
    
     #--- Get basename of filename
     datafile = control.params['DataFile']
     unit = control.params['PhysicalUnit']
     try:
@@ -116,15 +116,15 @@
     #--- Get data
     if observations.ts_format=='mom':
         mjd = observations.data.index.to_numpy()
         t   = (mjd-51544)/365.25 + 2000
     else:
         t   = observations.data.index.to_numpy()
     x = observations.data['obs'].to_numpy()
-    print(x)
+    #print(x)
     if 'mod' in observations.data.columns:
         xhat = observations.data['mod'].to_numpy() 
 
     #--- Show graph?
     if graph==True or save_eps==True or save_png==True:
         fig = plt.figure(figsize=(6, 4), dpi=150)
         plt.plot(t, x, 'b-', label='observed')
```

### Comparing `hectorp-0.1.3/src/hectorp/findoffsets.py` & `hectorp-0.1.4/src/hectorp/findoffsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # Perform cycles of offset detection for a single station [optionally 3D]
 #  1) Compute noise and SLT model parameters
 #  2) Compute for each epoch the new log-likelihood when an offset is added
 #     but maintaining the noise parameters constant.
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -86,15 +86,15 @@
 #===============================================================================
 # Main program
 #===============================================================================
 
 def main():
 
     print("\n***************************************")
-    print("    findoffsets, version 0.1.2")
+    print("    findoffsets, version 0.1.4")
     print("***************************************")
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Find offsets in time series')
 
     #--- List arguments that can be given 
     parser.add_argument('-s', dest='station', action='store', required=True,
```

### Comparing `hectorp-0.1.3/src/hectorp/fullcov.py` & `hectorp-0.1.4/src/hectorp/fullcov.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # fullcov.py
 # 
 # Python3 implemenation of FullCov.cpp. 
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/ggm.py` & `hectorp-0.1.4/src/hectorp/ggm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ggm.py
 #
 # Create the first row of the covariance matrix for Generalised Gauss Markov
 # noise.
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/levinson.py` & `hectorp-0.1.4/src/hectorp/ammargrag.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # for Toeplitz Systems", By Michael K. Ng  (page 28-29)
 #
 # Equations are taken from Bos et al. (2013), "Fast error analysis of 
 # continuous GNSS observations with missing data", Journal of Geodesy,
 # DOI 10.1007/s00190-012-0605-0.
 #
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY 
@@ -109,15 +109,15 @@
             l2[1:m] = r[0:m-1]
 
             #-- Scale l1 & l2
             l1 *= 1.0/math.sqrt(delta)
             l2 *= 1.0/math.sqrt(delta)
 
             start1 = time.time()
-            print("step 1: {0:8.3f} s\n".format(float(time.time() - start0)))
+            #print("step 1: {0:8.3f} s\n".format(float(time.time() - start0)))
             #--- Perform FFT on l1 and l2
             self.Fl1 = np.fft.rfft(l1)
             self.Fl2 = np.fft.rfft(l2) 
 
             #--- Currently there might be NaN's in H and x. Make those zero
             xm = np.zeros(m)
             for i in range(0,m):
@@ -196,11 +196,11 @@
 
             #--- Compute sigma_eta
             t1 = self.y1 - A1.T @ theta
             t2 = self.y2 - A2.T @ theta
             sigma_eta = math.sqrt((np.dot(t1,t1) - np.dot(t2,t2))/m)
 
         #--- Total time in AmmarGrag
-        print("step 2: {0:8.3f} s\n".format(float(time.time() - start1)))
-        print("--- {0:8.3f} s ---\n".format(float(time.time() - start0)))
+        #print("step 2: {0:8.3f} s\n".format(float(time.time() - start1)))
+        #print("--- {0:8.3f} s ---\n".format(float(time.time() - start0)))
 
         return [theta,C_theta,self.ln_det_C,sigma_eta]
```

### Comparing `hectorp-0.1.3/src/hectorp/matern.py` & `hectorp-0.1.4/src/hectorp/matern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 #
 # This class implements the Matérn noise model. Eqs. are taken from
 # Lilly et al. (2017) "Fractional Brownian motion, the Matérn process, and 
 # stochastic modeling of turbulent dispersion", Nonlinear Processes in 
 # Geophysics, 24: 481-514 
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/mjd2date.py` & `hectorp-0.1.4/src/hectorp/mjd2date.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # Simple MJD to date converter.
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
```

### Comparing `hectorp-0.1.3/src/hectorp/mle.py` & `hectorp-0.1.4/src/hectorp/mle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # mle.py
 #
 # Class which computes the log-likelihood and searches for the maximum value.
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/msf.py` & `hectorp-0.1.4/src/hectorp/msf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 #
 # msf.py
 #
 # A simple class that helps to read and write msf-files
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY 
@@ -148,14 +148,14 @@
         Args:
             header (dictionary)
 
         Returns:
             True if passed
         """
 
-        print(header)
+        #print(header)
         assert 'sampling_period' in header.keys()
         assert 'mjd' in header.keys()
         assert 'column_names' in header.keys()
         assert 'offsets' in header.keys()
 
         return True
```

### Comparing `hectorp-0.1.3/src/hectorp/msfdump.py` & `hectorp-0.1.4/src/hectorp/msfdump.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Create text file from msf-json file
 #
 # Example:
 # --------
 # msfdump -i drone_flight1.msf -o data.txt
 #
-# This program is part of HectorP 0.1.2
+# This program is part of HectorP 0.1.4
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/msfgen.py` & `hectorp-0.1.4/src/hectorp/msfgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Create msf-json files
 #
 # Example:
 # --------
 # msfgen -ji meta.json -di imu.dat -o drone_flight1.msf
 #
-# This program is part of HectorP 0.1.2
+# This program is part of HectorP 0.1.4
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/mycalendar.py` & `hectorp-0.1.4/src/hectorp/mycalendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# This file is part of HectorP 0.1.2
+# This file is part of HectorP 0.1.4
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/observations.py` & `hectorp-0.1.4/src/hectorp/observations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # observations.py
 #
 # A simple interface that reads and writes mom-files and stores
 # them into a Python class 'observations'.
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/ols.py` & `hectorp-0.1.4/src/hectorp/ols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ols.py
 # 
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/powerlaw.py` & `hectorp-0.1.4/src/hectorp/powerlaw.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Create the first row of the covariance matrix for power-law noise models
 # using Eq. (7) of Bos et al. (2008).
 #
 # Bos, MS, Fernandes, RMS, Williams, SDP & Bastos, L (2008). "Fast error 
 # analysis of continuous GPS observations". Journal of Geodesy, 82(3), 157-166.
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/predicttrenderror.py` & `hectorp-0.1.4/src/hectorp/predicttrenderror.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This program uses the estimated noise models parameters to predict the 
 # trend error for given number of observations.
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -113,15 +113,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    predict error, version 0.1.2")
+        print("    predict error, version 0.1.4")
         print("***************************************")
 
     #--- Get Classes
     white = White()
     powerlaw = Powerlaw()
     ggm = GGM()
     varyingannual = VaryingAnnual()
```

### Comparing `hectorp-0.1.3/src/hectorp/pyfftw_ex1.py` & `hectorp-0.1.4/src/hectorp/pyfftw_ex1.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/src/hectorp/removeoutliers.py` & `hectorp-0.1.4/src/hectorp/removeoutliers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program removes outliers from the observations.
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -71,15 +71,15 @@
     try:
         verbose = control.params['Verbose']
     except:
         verbose = True
 
     if verbose==True:
         print("\n***************************************")
-        print("    removeoutliers, version 0.1.2")
+        print("    removeoutliers, version 0.1.4")
         print("***************************************")
 
     #--- Get Classes
     datasnooping = DataSnooping()
     observations = Observations()
 
     #--- Get data
```

### Comparing `hectorp-0.1.3/src/hectorp/schur.py` & `hectorp-0.1.4/src/hectorp/schur.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # the first column of the Toeplitz covariance matrix C.
 #
 # Equations are taken from Bos et al. (2013), "Fast error analysis of 
 # continuous GNSS observations with missing data", Journal of Geodesy,
 # DOI 10.1007/s00190-012-0605-0.
 #
 #
-# This file is part of HectorP 0.1.2.
+# This file is part of HectorP 0.1.4.
 #
 # HectorP is free software: you can redistribute it and/or modify it under the 
 # terms of the GNU General Public License as published by the Free Software 
 # Foundation, either version 3 of the License, or (at your option) any later 
 # version.
 #
 # HectorP is distributed in the hope that it will be useful, but WITHOUT ANY
```

### Comparing `hectorp-0.1.3/src/hectorp/simulatenoise.py` & `hectorp-0.1.4/src/hectorp/simulatenoise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 #
 # This program creates synthetic noise.
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
@@ -242,15 +242,15 @@
 #===============================================================================
 # Main program
 #===============================================================================
 
 def main():
 
     print("\n***************************************")
-    print("    simulatenoise, version 0.1.2")
+    print("    simulatenoise, version 0.1.4")
     print("***************************************")
 
     #--- Parse command line arguments in a bit more professional way
     parser = argparse.ArgumentParser(description= 'Simulate noise time series')
 
     #--- List arguments that can be given 
     parser.add_argument('-i', required=False, default='simulatenoise.ctl', \
```

### Comparing `hectorp-0.1.3/src/hectorp/test_Schur.py` & `hectorp-0.1.4/src/hectorp/test_Schur.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # This program tests the generalised Schur algorithm to find the 
 # Cholesky decomposition of the inverse covariance matrix.
 #
-#  This script is part of HectorP 0.1.2
+#  This script is part of HectorP 0.1.4
 #
 #  HectorP is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  HectorP is distributed in the hope that it will be useful,
```

### Comparing `hectorp-0.1.3/src/hectorp/test_opencl.py` & `hectorp-0.1.4/src/hectorp/test_opencl.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/src/hectorp/test_reikna.py` & `hectorp-0.1.4/src/hectorp/test_reikna.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/src/hectorp/varyingannual.py` & `hectorp-0.1.4/src/hectorp/varyingannual.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/src/hectorp/white.py` & `hectorp-0.1.4/src/hectorp/white.py`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/src/hectorp.egg-info/PKG-INFO` & `hectorp-0.1.4/src/hectorp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hectorp
-Version: 0.1.3
+Version: 0.1.4
 Summary: A collection of programs to analyse geodetic time series
 Home-page: https://gitlab.com/machielsimonbos/hectorp
 Author: Machiel Bos
 Author-email: machielbos@protonmail.com
 Project-URL: Bug Tracker, https://gitlab.com/machielsimonbos/hectorp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -112,9 +112,7 @@
 | 5000 10% |      16 |       63.8 |
 | 8000 10% |      33 |       81.0 |
 | 5000 20% |      26 |       70.0 |
 | 8000 20% |      60 |      140.0 |
 
 
 
-
-### 4. References <a name="references"></a>
```

### Comparing `hectorp-0.1.3/src/hectorp.egg-info/SOURCES.txt` & `hectorp-0.1.4/src/hectorp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hectorp-0.1.3/src/hectorp.egg-info/entry_points.txt` & `hectorp-0.1.4/src/hectorp.egg-info/entry_points.txt`

 * *Files identical despite different names*

