# Comparing `tmp/transitfit-3.0.7.tar.gz` & `tmp/transitfit-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transitfit-3.0.7.tar", last modified: Fri Jun 16 13:33:56 2023, max compression
+gzip compressed data, was "transitfit-3.0.8.tar", last modified: Sat Jun 17 14:26:10 2023, max compression
```

## Comparing `transitfit-3.0.7.tar` & `transitfit-3.0.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-16 13:33:56.470275 transitfit-3.0.7/
--rw-rw-r--   0 a         (1000) a         (1000)    35129 2023-05-18 21:20:57.000000 transitfit-3.0.7/LICENSE
--rw-rw-r--   0 a         (1000) a         (1000)     3944 2023-06-16 13:33:56.470275 transitfit-3.0.7/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)     3303 2023-05-18 21:20:57.000000 transitfit-3.0.7/README.md
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-16 13:33:56.470275 transitfit-3.0.7/filters/
--rw-rw-r--   0 a         (1000) a         (1000)      542 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/CousinsI.csv
--rw-rw-r--   0 a         (1000) a         (1000)      674 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/CousinsR.csv
--rw-rw-r--   0 a         (1000) a         (1000)      231 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/JohnsonB.csv
--rw-rw-r--   0 a         (1000) a         (1000)      341 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/JohnsonI.csv
--rw-rw-r--   0 a         (1000) a         (1000)      296 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/JohnsonR.csv
--rw-rw-r--   0 a         (1000) a         (1000)      176 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/JohnsonU.csv
--rw-rw-r--   0 a         (1000) a         (1000)      200 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/JohnsonV.csv
--rw-rw-r--   0 a         (1000) a         (1000)     8960 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/Kepler.csv
--rw-rw-r--   0 a         (1000) a         (1000)     1259 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_g.csv
--rw-rw-r--   0 a         (1000) a         (1000)    35084 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_gprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)     1255 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_i.csv
--rw-rw-r--   0 a         (1000) a         (1000)    36720 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_iprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)     1064 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_r.csv
--rw-rw-r--   0 a         (1000) a         (1000)    31574 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_rprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)      672 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_u.csv
--rw-rw-r--   0 a         (1000) a         (1000)    15446 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_uprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)     2030 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_z.csv
--rw-rw-r--   0 a         (1000) a         (1000)    92169 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/SLOAN_zprime.csv
--rw-rw-r--   0 a         (1000) a         (1000)     6743 2023-05-18 21:20:57.000000 transitfit-3.0.7/filters/TESS.csv
--rw-rw-r--   0 a         (1000) a         (1000)      104 2023-05-18 21:20:57.000000 transitfit-3.0.7/pyproject.toml
--rw-rw-r--   0 a         (1000) a         (1000)      897 2023-06-16 13:33:56.470275 transitfit-3.0.7/setup.cfg
--rw-rw-r--   0 a         (1000) a         (1000)     1559 2023-05-18 21:25:42.000000 transitfit-3.0.7/setup.py
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-16 13:33:56.466275 transitfit-3.0.7/transitfit/
--rw-rw-r--   0 a         (1000) a         (1000)      440 2023-06-16 13:04:43.000000 transitfit-3.0.7/transitfit/__init__.py
--rw-rw-r--   0 a         (1000) a         (1000)     7634 2023-05-18 21:20:57.000000 transitfit-3.0.7/transitfit/_ldtk_handler.py
--rw-rw-r--   0 a         (1000) a         (1000)     7687 2023-05-18 21:20:57.000000 transitfit-3.0.7/transitfit/_likelihood.py
--rw-rw-r--   0 a         (1000) a         (1000)    11790 2023-05-18 21:20:57.000000 transitfit-3.0.7/transitfit/_limb_darkening_handler.py
--rw-rw-r--   0 a         (1000) a         (1000)     8547 2023-05-18 21:25:01.000000 transitfit-3.0.7/transitfit/_paramarray.py
--rw-rw-r--   0 a         (1000) a         (1000)     2547 2023-05-18 21:25:01.000000 transitfit-3.0.7/transitfit/_params.py
--rw-rw-r--   0 a         (1000) a         (1000)    16682 2023-05-18 21:25:01.000000 transitfit-3.0.7/transitfit/_pipeline.py
--rw-rw-r--   0 a         (1000) a         (1000)     9903 2023-05-18 21:20:57.000000 transitfit-3.0.7/transitfit/_utils.py
--rw-rw-r--   0 a         (1000) a         (1000)     1644 2023-05-18 21:20:57.000000 transitfit-3.0.7/transitfit/detrender.py
--rw-rw-r--   0 a         (1000) a         (1000)     2354 2023-05-18 21:20:57.000000 transitfit-3.0.7/transitfit/detrending_funcs.py
--rw-rw-r--   0 a         (1000) a         (1000)    15800 2023-05-24 08:55:11.000000 transitfit-3.0.7/transitfit/error_analysis.py
--rw-rw-r--   0 a         (1000) a         (1000)    32649 2023-05-18 21:20:57.000000 transitfit-3.0.7/transitfit/io.py
--rw-rw-r--   0 a         (1000) a         (1000)    22728 2023-05-18 21:25:01.000000 transitfit-3.0.7/transitfit/lightcurve.py
--rw-rw-r--   0 a         (1000) a         (1000)    52943 2023-05-18 21:25:01.000000 transitfit-3.0.7/transitfit/output_handler.py
--rw-rw-r--   0 a         (1000) a         (1000)    14804 2023-05-18 21:25:01.000000 transitfit-3.0.7/transitfit/plotting.py
--rw-rw-r--   0 a         (1000) a         (1000)    25606 2023-06-13 12:31:25.000000 transitfit-3.0.7/transitfit/priorinfo.py
--rw-rw-r--   0 a         (1000) a         (1000)    72989 2023-05-18 21:25:01.000000 transitfit-3.0.7/transitfit/retriever.py
--rw-rw-r--   0 a         (1000) a         (1000)     1878 2023-05-18 21:20:57.000000 transitfit-3.0.7/transitfit/time_conversions.py
-drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-16 13:33:56.466275 transitfit-3.0.7/transitfit.egg-info/
--rw-rw-r--   0 a         (1000) a         (1000)     3944 2023-06-16 13:33:56.000000 transitfit-3.0.7/transitfit.egg-info/PKG-INFO
--rw-rw-r--   0 a         (1000) a         (1000)     1392 2023-06-16 13:33:56.000000 transitfit-3.0.7/transitfit.egg-info/SOURCES.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-16 13:33:56.000000 transitfit-3.0.7/transitfit.egg-info/dependency_links.txt
--rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-18 21:21:16.000000 transitfit-3.0.7/transitfit.egg-info/not-zip-safe
--rw-rw-r--   0 a         (1000) a         (1000)      101 2023-06-16 13:33:56.000000 transitfit-3.0.7/transitfit.egg-info/requires.txt
--rw-rw-r--   0 a         (1000) a         (1000)       11 2023-06-16 13:33:56.000000 transitfit-3.0.7/transitfit.egg-info/top_level.txt
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-17 14:26:10.259761 transitfit-3.0.8/
+-rw-rw-r--   0 a         (1000) a         (1000)    35129 2023-05-18 21:20:57.000000 transitfit-3.0.8/LICENSE
+-rw-rw-r--   0 a         (1000) a         (1000)     3944 2023-06-17 14:26:10.259761 transitfit-3.0.8/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)     3303 2023-05-18 21:20:57.000000 transitfit-3.0.8/README.md
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-17 14:26:10.259761 transitfit-3.0.8/filters/
+-rw-rw-r--   0 a         (1000) a         (1000)      542 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/CousinsI.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      674 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/CousinsR.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      231 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonB.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      341 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonI.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      296 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonR.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      176 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonU.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      200 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/JohnsonV.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     8960 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/Kepler.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     1259 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_g.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    35084 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_gprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     1255 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_i.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    36720 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_iprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     1064 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_r.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    31574 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_rprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      672 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_u.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    15446 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_uprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     2030 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_z.csv
+-rw-rw-r--   0 a         (1000) a         (1000)    92169 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/SLOAN_zprime.csv
+-rw-rw-r--   0 a         (1000) a         (1000)     6743 2023-05-18 21:20:57.000000 transitfit-3.0.8/filters/TESS.csv
+-rw-rw-r--   0 a         (1000) a         (1000)      104 2023-05-18 21:20:57.000000 transitfit-3.0.8/pyproject.toml
+-rw-rw-r--   0 a         (1000) a         (1000)      897 2023-06-17 14:26:10.259761 transitfit-3.0.8/setup.cfg
+-rw-rw-r--   0 a         (1000) a         (1000)     1559 2023-05-18 21:25:42.000000 transitfit-3.0.8/setup.py
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-17 14:26:10.247760 transitfit-3.0.8/transitfit/
+-rw-rw-r--   0 a         (1000) a         (1000)      440 2023-06-17 14:19:14.000000 transitfit-3.0.8/transitfit/__init__.py
+-rw-rw-r--   0 a         (1000) a         (1000)     7634 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/_ldtk_handler.py
+-rw-rw-r--   0 a         (1000) a         (1000)     7687 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/_likelihood.py
+-rw-rw-r--   0 a         (1000) a         (1000)    11790 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/_limb_darkening_handler.py
+-rw-rw-r--   0 a         (1000) a         (1000)     8547 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/_paramarray.py
+-rw-rw-r--   0 a         (1000) a         (1000)     2547 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/_params.py
+-rw-rw-r--   0 a         (1000) a         (1000)    16682 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/_pipeline.py
+-rw-rw-r--   0 a         (1000) a         (1000)     9903 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/_utils.py
+-rw-rw-r--   0 a         (1000) a         (1000)     1644 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/detrender.py
+-rw-rw-r--   0 a         (1000) a         (1000)     2354 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/detrending_funcs.py
+-rw-rw-r--   0 a         (1000) a         (1000)    16505 2023-06-17 14:25:48.000000 transitfit-3.0.8/transitfit/error_analysis.py
+-rw-rw-r--   0 a         (1000) a         (1000)    32649 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/io.py
+-rw-rw-r--   0 a         (1000) a         (1000)    22728 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/lightcurve.py
+-rw-rw-r--   0 a         (1000) a         (1000)    52943 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/output_handler.py
+-rw-rw-r--   0 a         (1000) a         (1000)    14804 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/plotting.py
+-rw-rw-r--   0 a         (1000) a         (1000)    25606 2023-06-13 12:31:25.000000 transitfit-3.0.8/transitfit/priorinfo.py
+-rw-rw-r--   0 a         (1000) a         (1000)    72989 2023-05-18 21:25:01.000000 transitfit-3.0.8/transitfit/retriever.py
+-rw-rw-r--   0 a         (1000) a         (1000)     1878 2023-05-18 21:20:57.000000 transitfit-3.0.8/transitfit/time_conversions.py
+drwxrwxr-x   0 a         (1000) a         (1000)        0 2023-06-17 14:26:10.247760 transitfit-3.0.8/transitfit.egg-info/
+-rw-rw-r--   0 a         (1000) a         (1000)     3944 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/PKG-INFO
+-rw-rw-r--   0 a         (1000) a         (1000)     1392 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/SOURCES.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/dependency_links.txt
+-rw-rw-r--   0 a         (1000) a         (1000)        1 2023-05-18 21:21:16.000000 transitfit-3.0.8/transitfit.egg-info/not-zip-safe
+-rw-rw-r--   0 a         (1000) a         (1000)      101 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/requires.txt
+-rw-rw-r--   0 a         (1000) a         (1000)       11 2023-06-17 14:26:10.000000 transitfit-3.0.8/transitfit.egg-info/top_level.txt
```

### Comparing `transitfit-3.0.7/LICENSE` & `transitfit-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/PKG-INFO` & `transitfit-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transitfit
-Version: 3.0.7
+Version: 3.0.8
 Summary: A package to fit exoplanet transit light curves
 Home-page: https://github.com/SPEARNET/TransitFit
 Author: Joshua Hayes and collaborators
 Author-email: Eamonn.Kerins@manchester.ac.uk
 Project-URL: Documentation, https://transitfit.readthedocs.io/en/latest/index.html
 Keywords: exoplanets,transits,fitting
 Classifier: Programming Language :: Python :: 3
```

### Comparing `transitfit-3.0.7/README.md` & `transitfit-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/CousinsI.csv` & `transitfit-3.0.8/filters/CousinsI.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/CousinsR.csv` & `transitfit-3.0.8/filters/CousinsR.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/Kepler.csv` & `transitfit-3.0.8/filters/Kepler.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_g.csv` & `transitfit-3.0.8/filters/SLOAN_g.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_gprime.csv` & `transitfit-3.0.8/filters/SLOAN_gprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_i.csv` & `transitfit-3.0.8/filters/SLOAN_i.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_iprime.csv` & `transitfit-3.0.8/filters/SLOAN_iprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_r.csv` & `transitfit-3.0.8/filters/SLOAN_r.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_rprime.csv` & `transitfit-3.0.8/filters/SLOAN_rprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_u.csv` & `transitfit-3.0.8/filters/SLOAN_u.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_uprime.csv` & `transitfit-3.0.8/filters/SLOAN_uprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_z.csv` & `transitfit-3.0.8/filters/SLOAN_z.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/SLOAN_zprime.csv` & `transitfit-3.0.8/filters/SLOAN_zprime.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/filters/TESS.csv` & `transitfit-3.0.8/filters/TESS.csv`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/setup.cfg` & `transitfit-3.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/setup.py` & `transitfit-3.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/_ldtk_handler.py` & `transitfit-3.0.8/transitfit/_ldtk_handler.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/_likelihood.py` & `transitfit-3.0.8/transitfit/_likelihood.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/_limb_darkening_handler.py` & `transitfit-3.0.8/transitfit/_limb_darkening_handler.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/_paramarray.py` & `transitfit-3.0.8/transitfit/_paramarray.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/_params.py` & `transitfit-3.0.8/transitfit/_params.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/_pipeline.py` & `transitfit-3.0.8/transitfit/_pipeline.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/_utils.py` & `transitfit-3.0.8/transitfit/_utils.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/detrender.py` & `transitfit-3.0.8/transitfit/detrender.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/detrending_funcs.py` & `transitfit-3.0.8/transitfit/detrending_funcs.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/error_analysis.py` & `transitfit-3.0.8/transitfit/error_analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,45 +73,64 @@
     if key in val_dict:
         val_dict[key] = np.ndarray.flatten(np.append(val_dict[key], vals))
     else:
         val_dict[key] = np.ndarray.flatten(vals)
 
 
 def q_to_u_err(q, q_err):
+    """Converts error in q to errors in u parameters for quadratic limb-darkening
+
+    Args:
+        q (list): values of q0, q1
+        q_err (list): errors on q0, q1
+
+    Returns:
+        list: errors on u0, u1
+    """
 
     u_err = []
     u_err.append(np.sqrt(((q[1] * q_err[0])**2)/q[0] + 4 * q[0] * q_err[1]**2))
     u_err.append(np.sqrt(
         (((1 - 2 * q[1]) * q_err[0])**2)/(0.25 * q[0]) + 4 * q[0] * q_err[1] ** 2))
 
     return u_err
 
 
 def q_to_u(q, q_err_l, q_err_u):
+    """Converts q (Kipping parameters) to limb darkening parameters u.
+    Handles only quadratic limb darkening currently.
+
+    Args:
+        q (list): values of q0, q1
+        q_err_l (list): lower bound of errors on q0, q1
+        q_err_u (list): upper bound of errors on q0, q1
+
+    Returns:
+        tuple: the values of u, lower bound on values, upper bound on values.
+    """
 
     u = [2 * np.sqrt(q[0]) * q[1], np.sqrt(q[0]) * (1 - 2 * q[1])]
 
     u_err_l = q_to_u_err(q, q_err_l)
     u_err_u = q_to_u_err(q, q_err_u)
 
     return u, u_err_l, u_err_u
 
 
 class ErrorLimits:
     """
     Initializes the error limit analysis.
+
+    Args:
+        output_parmeters (str): path of the output_parameters folder
+                                generated by TransitFit
     """
 
     def __init__(self, output_parmeters):
-        """
-
-        Args:
-            output_parmeters (str): path of the output_parameters folder
-                                    generated by TransitFit
-        """
+        
         # The path to the output_parameters folder from the TransitFit output.
         self.OUTPUT_PARAMETERS_FOLDER = output_parmeters
 
         # This will be the name of the output file
         self.MODIFIED_SUMMARY_OUTPUT = 'modifed_output.csv'
 
         # Summary_output file
@@ -164,14 +183,16 @@
             self.folded_params = []
 
         # The list of required parameters to analyze
         self.required_params = ['P', 't0', 'a/r*', 'inc', 'rp/r*']
         self.values = {}
 
     def handle_ttv(self):
+        """ Handles the case of TTV analysis.
+        """
         all_epochs = np.empty(0)
         for i, fmpk in enumerate(self.folded_mode_priors_pkl):
             with open(fmpk, 'rb') as handle:
                 priors = pickle.load(handle)
 
             fitting_params = priors.fitting_params  # [name, tidx,fidx, eidx]
             # filters = fitting_params[:,2]
@@ -247,14 +268,16 @@
 
         print(
             f"Saved results in {self.OUTPUT_PARAMETERS_FOLDER+'/'+self.MODIFIED_SUMMARY_OUTPUT}")
 
         return
 
     def get_errors(self):
+        """ Gets the upper and lower error bound on values.
+        """
 
         # Initalising values dictionary and filters list.
         # selvalues = {}
         filters = []
 
         if self.allow_ttv:
             self.handle_ttv()
```

### Comparing `transitfit-3.0.7/transitfit/io.py` & `transitfit-3.0.8/transitfit/io.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/lightcurve.py` & `transitfit-3.0.8/transitfit/lightcurve.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/output_handler.py` & `transitfit-3.0.8/transitfit/output_handler.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/plotting.py` & `transitfit-3.0.8/transitfit/plotting.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/priorinfo.py` & `transitfit-3.0.8/transitfit/priorinfo.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/retriever.py` & `transitfit-3.0.8/transitfit/retriever.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit/time_conversions.py` & `transitfit-3.0.8/transitfit/time_conversions.py`

 * *Files identical despite different names*

### Comparing `transitfit-3.0.7/transitfit.egg-info/PKG-INFO` & `transitfit-3.0.8/transitfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transitfit
-Version: 3.0.7
+Version: 3.0.8
 Summary: A package to fit exoplanet transit light curves
 Home-page: https://github.com/SPEARNET/TransitFit
 Author: Joshua Hayes and collaborators
 Author-email: Eamonn.Kerins@manchester.ac.uk
 Project-URL: Documentation, https://transitfit.readthedocs.io/en/latest/index.html
 Keywords: exoplanets,transits,fitting
 Classifier: Programming Language :: Python :: 3
```

### Comparing `transitfit-3.0.7/transitfit.egg-info/SOURCES.txt` & `transitfit-3.0.8/transitfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

