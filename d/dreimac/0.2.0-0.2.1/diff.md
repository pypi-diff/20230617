# Comparing `tmp/dreimac-0.2.0.tar.gz` & `tmp/dreimac-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreimac-0.2.0.tar", last modified: Mon May  8 16:30:17 2023, max compression
+gzip compressed data, was "dreimac-0.2.1.tar", last modified: Sat Jun 17 17:33:16 2023, max compression
```

## Comparing `dreimac-0.2.0.tar` & `dreimac-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-05-08 16:28:38.000000 dreimac-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-08 16:30:17.384883 dreimac-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-05-08 16:28:38.000000 dreimac-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/dreimac/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/circularcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/combinatorial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/emcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/plotting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/projectivecoords.py
--rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/toroidalcoords.py
--rw-r--r--   0 runner    (1001) docker     (123)    36173 2023-05-08 16:28:38.000000 dreimac-0.2.0/dreimac/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/dreimac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 16:30:17.000000 dreimac-0.2.0/dreimac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:30:17.384883 dreimac-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-08 16:28:38.000000 dreimac-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:30:17.384883 dreimac-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_circular.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_combinatorial_number_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-08 16:28:38.000000 dreimac-0.2.0/test/test_projective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:33:16.720614 dreimac-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11376 2023-06-17 17:31:40.000000 dreimac-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-17 17:33:16.720614 dreimac-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-17 17:31:40.000000 dreimac-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:33:16.720614 dreimac-0.2.1/dreimac/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-17 17:31:40.000000 dreimac-0.2.1/dreimac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 17:31:40.000000 dreimac-0.2.1/dreimac/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-17 17:31:40.000000 dreimac-0.2.1/dreimac/circularcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-17 17:31:40.000000 dreimac-0.2.1/dreimac/combinatorial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-06-17 17:31:40.000000 dreimac-0.2.1/dreimac/emcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-06-17 17:31:40.000000 dreimac-0.2.1/dreimac/plotting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-17 17:31:40.000000 dreimac-0.2.1/dreimac/projectivecoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14987 2023-06-17 17:31:40.000000 dreimac-0.2.1/dreimac/toroidalcoords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36173 2023-06-17 17:31:40.000000 dreimac-0.2.1/dreimac/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:33:16.720614 dreimac-0.2.1/dreimac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-06-17 17:33:16.000000 dreimac-0.2.1/dreimac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-17 17:33:16.000000 dreimac-0.2.1/dreimac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:33:16.000000 dreimac-0.2.1/dreimac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-17 17:33:16.000000 dreimac-0.2.1/dreimac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-17 17:33:16.000000 dreimac-0.2.1/dreimac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 17:33:16.720614 dreimac-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-17 17:31:40.000000 dreimac-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:33:16.720614 dreimac-0.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-17 17:31:40.000000 dreimac-0.2.1/test/test_circular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-17 17:31:40.000000 dreimac-0.2.1/test/test_combinatorial_number_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-17 17:31:40.000000 dreimac-0.2.1/test/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-17 17:31:40.000000 dreimac-0.2.1/test/test_projective.py
```

### Comparing `dreimac-0.2.0/LICENSE` & `dreimac-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/PKG-INFO` & `dreimac-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreimac
-Version: 0.2.0
+Version: 0.2.1
 Summary: DREiMac: Dimension reduction with Eilenberg-MacLane coordinates
 Home-page: UNKNOWN
 Author: Jose A. Perea, Luis Scoccola, Chris Tralie
 Author-email: ctralie@alumni.princeton.edu
 License: Apache2
 Description: [![PyPI version](https://badge.fury.io/py/dreimac.svg)](https://badge.fury.io/py/dreimac)
         [![Downloads](https://static.pepy.tech/badge/dreimac)](https://pepy.tech/project/dreimac)
@@ -15,14 +15,16 @@
         
         DREiMac is a library for topological data coordinatization, visualization, and dimensionality reduction.
         Currently, DREiMac is able to find topology-preserving representations of point clouds taking values in the circle, in higher dimensional tori, and in the real projective space.
         
         In a few words, DREiMac takes as input a point cloud together with a topological feature of the point cloud (in the form of a persistent cohomology class), and returns a map from the point cloud to a well-understood topological space (a circle, a product of circles, or a projective space), which preserves the given topological feature in a precise sense.
         For more information, please check the theory and examples in the [documentation](https://scikit-tda.org/DREiMac/index.html).
         
+        For an implementation of the complex projective coordinates algorithm and the lens coordinates algorithm, check out the [experimental branch](https://github.com/scikit-tda/DREiMac/tree/experimental)!
+        
         ## Basic usage
         
         Here is a simple example; please check the Jupyter notebooks in the `notebooks` directory for further examples.
         
         ```python
         # basic imports
         from dreimac import CircularCoords
```

### Comparing `dreimac-0.2.0/README.md` & `dreimac-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 DREiMac is a library for topological data coordinatization, visualization, and dimensionality reduction.
 Currently, DREiMac is able to find topology-preserving representations of point clouds taking values in the circle, in higher dimensional tori, and in the real projective space.
 
 In a few words, DREiMac takes as input a point cloud together with a topological feature of the point cloud (in the form of a persistent cohomology class), and returns a map from the point cloud to a well-understood topological space (a circle, a product of circles, or a projective space), which preserves the given topological feature in a precise sense.
 For more information, please check the theory and examples in the [documentation](https://scikit-tda.org/DREiMac/index.html).
 
+For an implementation of the complex projective coordinates algorithm and the lens coordinates algorithm, check out the [experimental branch](https://github.com/scikit-tda/DREiMac/tree/experimental)!
+
 ## Basic usage
 
 Here is a simple example; please check the Jupyter notebooks in the `notebooks` directory for further examples.
 
 ```python
 # basic imports
 from dreimac import CircularCoords
```

### Comparing `dreimac-0.2.0/dreimac/circularcoords.py` & `dreimac-0.2.1/dreimac/circularcoords.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/dreimac/combinatorial.py` & `dreimac-0.2.1/dreimac/combinatorial.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/dreimac/emcoords.py` & `dreimac-0.2.1/dreimac/emcoords.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/dreimac/plotting_utils.py` & `dreimac-0.2.1/dreimac/plotting_utils.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/dreimac/projectivecoords.py` & `dreimac-0.2.1/dreimac/projectivecoords.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/dreimac/toroidalcoords.py` & `dreimac-0.2.1/dreimac/toroidalcoords.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/dreimac/utils.py` & `dreimac-0.2.1/dreimac/utils.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/dreimac.egg-info/PKG-INFO` & `dreimac-0.2.1/dreimac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreimac
-Version: 0.2.0
+Version: 0.2.1
 Summary: DREiMac: Dimension reduction with Eilenberg-MacLane coordinates
 Home-page: UNKNOWN
 Author: Jose A. Perea, Luis Scoccola, Chris Tralie
 Author-email: ctralie@alumni.princeton.edu
 License: Apache2
 Description: [![PyPI version](https://badge.fury.io/py/dreimac.svg)](https://badge.fury.io/py/dreimac)
         [![Downloads](https://static.pepy.tech/badge/dreimac)](https://pepy.tech/project/dreimac)
@@ -15,14 +15,16 @@
         
         DREiMac is a library for topological data coordinatization, visualization, and dimensionality reduction.
         Currently, DREiMac is able to find topology-preserving representations of point clouds taking values in the circle, in higher dimensional tori, and in the real projective space.
         
         In a few words, DREiMac takes as input a point cloud together with a topological feature of the point cloud (in the form of a persistent cohomology class), and returns a map from the point cloud to a well-understood topological space (a circle, a product of circles, or a projective space), which preserves the given topological feature in a precise sense.
         For more information, please check the theory and examples in the [documentation](https://scikit-tda.org/DREiMac/index.html).
         
+        For an implementation of the complex projective coordinates algorithm and the lens coordinates algorithm, check out the [experimental branch](https://github.com/scikit-tda/DREiMac/tree/experimental)!
+        
         ## Basic usage
         
         Here is a simple example; please check the Jupyter notebooks in the `notebooks` directory for further examples.
         
         ```python
         # basic imports
         from dreimac import CircularCoords
```

### Comparing `dreimac-0.2.0/setup.py` & `dreimac-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/test/test_circular.py` & `dreimac-0.2.1/test/test_circular.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/test/test_combinatorial_number_system.py` & `dreimac-0.2.1/test/test_combinatorial_number_system.py`

 * *Files identical despite different names*

### Comparing `dreimac-0.2.0/test/test_projective.py` & `dreimac-0.2.1/test/test_projective.py`

 * *Files identical despite different names*

