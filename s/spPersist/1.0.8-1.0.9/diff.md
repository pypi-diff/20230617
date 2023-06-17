# Comparing `tmp/spPersist-1.0.8.tar.gz` & `tmp/sppersist-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-1.0.8.tar", last modified: Thu Jun 15 13:35:37 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `spPersist-1.0.8.tar` & `sppersist-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:35:37.654169 spPersist-1.0.8/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-15 13:35:17.000000 spPersist-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 13:35:37.654169 spPersist-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-15 13:35:17.000000 spPersist-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 13:35:37.654169 spPersist-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8133 2023-06-15 13:35:17.000000 spPersist-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:35:37.650169 spPersist-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:35:37.652169 spPersist-1.0.8/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9595 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/ph.py
--rw-r--r--   0 root         (0) root         (0)     6742 2023-06-15 13:32:56.000000 spPersist-1.0.8/src/spPersist/pp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 13:35:37.654169 spPersist-1.0.8/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      389 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-15 13:35:37.000000 spPersist-1.0.8/src/spPersist.egg-info/top_level.txt
+-rw-r--r--   0        0        0    10798 2020-02-02 00:00:00.000000 sppersist-1.0.9/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 sppersist-1.0.9/src/spPersist/__init__.py
+-rw-r--r--   0        0        0     9595 2020-02-02 00:00:00.000000 sppersist-1.0.9/src/spPersist/dp.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 sppersist-1.0.9/src/spPersist/hc.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sppersist-1.0.9/src/spPersist/persistence_statistics.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 sppersist-1.0.9/src/spPersist/ph.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 sppersist-1.0.9/src/spPersist/pp.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 sppersist-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 sppersist-1.0.9/README.md
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 sppersist-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sppersist-1.0.9/PKG-INFO
```

### Comparing `spPersist-1.0.8/LICENSE` & `sppersist-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.8/PKG-INFO` & `sppersist-1.0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,24 @@
-Metadata-Version: 2.1
-Name: spPersist
-Version: 1.0.8
-Summary: Spatial transcriptomics with Persistent Homology
-Author: Lirong Yang
-Author-email: lirong.yang@outlook.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Spatial transcriptomics with Persistent Homology
-
-This is a package for classifying Spatial transcriptomics data according to its 
-spatial topology. The specific mathematical foundation for the classification is
-the theory of Persistent Homology and persistence diagram. The package 
-contains a data processing module, called dp, allowing users to load either the
-standard datasets from Visium and MERFISH, or published datasets into desired
-annotated data format for the analysis performed in this package. The format is
-compatible with the package Squidpy.
-
-The package also includes a pre-processing module, a 
-persistent homology module and a homological classification module, respectively
-named pp, ph and hc.
-
-The pre-processing module contains quality control metrics, deconvolution
-methods and cell type identifications.
-
-The persistent homology module contains functions for computing simplicial 
-complexes of point clouds (See data structures in the gudhi package.) and their
-topological measures. It also includes plotting features of the persistence 
-diagram.
-
-The homological classification module computes the number of holes and connected
-components as a dictionary.
+# Spatial transcriptomics with Persistent Homology
+
+This is a package for classifying Spatial transcriptomics data according to its 
+spatial topology. The specific mathematical foundation for the classification is
+the theory of Persistent Homology and persistence diagram. The package 
+contains a data processing module, called dp, allowing users to load either the
+standard datasets from Visium and MERFISH, or published datasets into desired
+annotated data format for the analysis performed in this package. The format is
+compatible with the package Squidpy.
+
+The package also includes a pre-processing module, a 
+persistent homology module and a homological classification module, respectively
+named pp, ph and hc.
+
+The pre-processing module contains quality control metrics, deconvolution
+methods and cell type identifications.
+
+The persistent homology module contains functions for computing simplicial 
+complexes of point clouds (See data structures in the gudhi package.) and their
+topological measures. It also includes plotting features of the persistence 
+diagram.
+
+The homological classification module computes the number of holes and connected
+components as a dictionary.
```

### Comparing `spPersist-1.0.8/src/spPersist/DTM_filtrations.py` & `sppersist-1.0.9/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.8/src/spPersist/dp.py` & `sppersist-1.0.9/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.8/src/spPersist/hc.py` & `sppersist-1.0.9/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.8/src/spPersist/persistence_statistics.py` & `sppersist-1.0.9/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.8/src/spPersist/ph.py` & `sppersist-1.0.9/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.8/src/spPersist/pp.py` & `sppersist-1.0.9/src/spPersist/pp.py`

 * *Files identical despite different names*

### Comparing `spPersist-1.0.8/src/spPersist.egg-info/PKG-INFO` & `sppersist-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 1.0.8
+Version: 1.0.9
 Summary: Spatial transcriptomics with Persistent Homology
-Author: Lirong Yang
-Author-email: lirong.yang@outlook.com
+Author-email: Lirong Yang <lirong.yang@outlook.com>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: cell2location
+Requires-Dist: gcsfs
+Requires-Dist: gudhi
+Requires-Dist: scanpy
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Spatial transcriptomics with Persistent Homology
 
 This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
 the theory of Persistent Homology and persistence diagram. The package 
 contains a data processing module, called dp, allowing users to load either the
@@ -27,8 +33,8 @@
 
 The persistent homology module contains functions for computing simplicial 
 complexes of point clouds (See data structures in the gudhi package.) and their
 topological measures. It also includes plotting features of the persistence 
 diagram.
 
 The homological classification module computes the number of holes and connected
-components as a dictionary.
+components as a dictionary.
```

