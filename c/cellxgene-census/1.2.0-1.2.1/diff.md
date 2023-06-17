# Comparing `tmp/cellxgene_census-1.2.0.tar.gz` & `tmp/cellxgene_census-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene_census-1.2.0.tar", last modified: Wed Jun  7 03:41:02 2023, max compression
+gzip compressed data, was "cellxgene_census-1.2.1.tar", last modified: Sat Jun 17 00:54:46 2023, max compression
```

## Comparing `cellxgene_census-1.2.0.tar` & `cellxgene_census-1.2.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/release_process.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.882763 cellxgene_census-1.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/scripts/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.882763 cellxgene_census-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census/
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_open.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_presence_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_release_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18895 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/ml/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/_eager_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/_online.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 03:41:02.000000 cellxgene_census-1.2.0/src/cellxgene_census.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.886763 cellxgene_census-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25438 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/tests/experimental/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/ml/test_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 03:41:02.890763 cellxgene_census-1.2.0/tests/experimental/pp/
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/pp/test_hvg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/experimental/pp/test_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_get_anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_get_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_open.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-07 03:40:49.000000 cellxgene_census-1.2.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/release_process.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/scripts/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.233991 cellxgene_census-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/src/cellxgene_census/
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_presence_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_release_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/src/cellxgene_census/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/src/cellxgene_census/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/ml/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_eager_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_online.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.237991 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-17 00:54:46.000000 cellxgene_census-1.2.1/src/cellxgene_census.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    25438 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/tests/experimental/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/ml/test_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:54:46.241991 cellxgene_census-1.2.1/tests/experimental/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/pp/test_hvg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/experimental/pp/test_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_get_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_get_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_open.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-17 00:54:31.000000 cellxgene_census-1.2.1/tests/test_util.py
```

### Comparing `cellxgene_census-1.2.0/LICENSE` & `cellxgene_census-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/PKG-INFO` & `cellxgene_census-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene_census
-Version: 1.2.0
+Version: 1.2.1
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: experimental
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
 The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/).
```

### Comparing `cellxgene_census-1.2.0/README.md` & `cellxgene_census-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/pyproject.toml` & `cellxgene_census-1.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,37 +7,38 @@
 dynamic = ["version"]
 description = "API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/"
 authors = [
     { name = "Chan Zuckerberg Initiative", email = "soma@chanzuckerberg.com" }
 ]
 license = { text = "MIT" }
 readme = "README.md"
-requires-python = ">= 3.7, < 3.11"  # Python 3.11 is pending numba support
+requires-python = ">= 3.7, < 3.12"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 dependencies= [
     # NOTE: the tiledbsoma version must be >= to the version used in the Census builder, to
     # ensure that the assets are readable (tiledbsoma supports backward compatible reading).
     # Make sure this version does not fall behind the builder's tiledbsoma version.
     "tiledbsoma==1.2.5",
     "anndata",
-    "numpy>=1.21,<1.24",  # numpy is constrained by numba and the old pip solver
+    "numpy>=1.21,<1.25",  # numpy is constrained by numba and the old pip solver
     "requests",
     "typing_extensions",
     "s3fs",
     "scipy",
     # Temporary fix for Mac OSX, to be removed by https://github.com/chanzuckerberg/cellxgene-census/issues/415
     "certifi",
 ]
```

### Comparing `cellxgene_census-1.2.0/release_process.md` & `cellxgene_census-1.2.1/release_process.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/__init__.py` & `cellxgene_census-1.2.1/src/cellxgene_census/__init__.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/_experiment.py` & `cellxgene_census-1.2.1/src/cellxgene_census/_experiment.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/_get_anndata.py` & `cellxgene_census-1.2.1/src/cellxgene_census/_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/_open.py` & `cellxgene_census-1.2.1/src/cellxgene_census/_open.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/_presence_matrix.py` & `cellxgene_census-1.2.1/src/cellxgene_census/_presence_matrix.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/_release_directory.py` & `cellxgene_census-1.2.1/src/cellxgene_census/_release_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/experimental/ml/pytorch.py` & `cellxgene_census-1.2.1/src/cellxgene_census/experimental/ml/pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         pytorch_logger.debug(f"Retrieved batch: shape={self.X_batch.shape}, cum_stats: {self.stats}")
         return self.obs_batch_
 
 
 class ExperimentDataPipe(pipes.IterDataPipe[Dataset[ObsDatum]]):  # type: ignore
     """
     An iterable-style PyTorch ``DataPipe`` that reads obs and X data from a SOMA Experiment, and returns an iterator of
-    tuples of PyTorch ``Tensor``s:
+    tuples of PyTorch ``Tensor`` objects.
 
     >>> (tensor([0., 0., 0., 0., 0., 1., 0., 0., 0.]),  # X data
         tensor([2415,    0,    0], dtype=torch.int32)) # obs data, encoded
 
     Supports batching via `batch_size` param:
 
     >>> DataLoader(..., batch_size=3, ...):
@@ -455,39 +455,61 @@
 # TODO: Move into somacore.ExperimentAxisQuery
 def experiment_dataloader(
     datapipe: pipes.IterDataPipe,
     num_workers: int = 0,
     **dataloader_kwargs: Any,
 ) -> DataLoader:
     """
-    Factory method for PyTorch ``DataLoader``. Provides a safer, more convenient interface for instantiating a
-    ``DataLoader`` that works with the ``ExperimentDataPipe``, since not all of ``DataLoader``'s params can be
-    used (``batch_size``, ``sampler``, ``batch_sampler``, ``collate_fn``).
+    Factory method for PyTorch ``DataLoader``. This method can be used to safely instantiate a
+    ``DataLoader`` that works with the ``ExperimentDataPipe``, since not all of the ``DataLoader`` constructor params
+    can be used (``batch_size``, ``sampler``, ``batch_sampler``, ``collate_fn``).
 
     Returns:
         PyTorch ``DataLoader``.
 
     Lifecycle:
         experimental
     """
 
     unsupported_dataloader_args = ["batch_size", "sampler", "batch_sampler", "collate_fn"]
     if set(unsupported_dataloader_args).intersection(dataloader_kwargs.keys()):
         raise ValueError(f"The {','.join(unsupported_dataloader_args)} DataLoader params are not supported")
 
+    if num_workers > 0:
+        _init_multiprocessing()
+
     return DataLoader(
         datapipe,
         batch_size=None,  # batching is handled by our ExperimentDataPipe
         num_workers=num_workers,
         # avoid use of default collator, which adds an extra (3rd) dimension to the tensor batches
         collate_fn=_collate_noop,
         **dataloader_kwargs,
     )
 
 
+def _init_multiprocessing() -> None:
+    """Ensures use of "spawn" for starting child processes with multiprocessing.
+    Forked processes are known to be problematic:
+      https://pytorch.org/docs/stable/notes/multiprocessing.html#avoiding-and-fighting-deadlocks
+    Also, CUDA does not support forked child processes:
+      https://pytorch.org/docs/stable/notes/multiprocessing.html#cuda-in-multiprocessing
+
+    """
+    torch.multiprocessing.set_start_method("fork", force=True)
+    orig_start_method = torch.multiprocessing.get_start_method()
+    if orig_start_method != "spawn":
+        if orig_start_method:
+            pytorch_logger.warning(
+                "switching torch multiprocessing start method from "
+                f'"{torch.multiprocessing.get_start_method()}" to "spawn"'
+            )
+        torch.multiprocessing.set_start_method("spawn", force=True)
+
+
 # For testing only
 if __name__ == "__main__":
     import tiledbsoma as soma
 
     (
         census_uri_arg,
         organism_arg,
```

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/_eager_iter.py` & `cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_eager_iter.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/_highly_variable_genes.py` & `cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_highly_variable_genes.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census/experimental/pp/_online.py` & `cellxgene_census-1.2.1/src/cellxgene_census/experimental/pp/_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census.egg-info/PKG-INFO` & `cellxgene_census-1.2.1/src/cellxgene_census.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-census
-Version: 1.2.0
+Version: 1.2.1
 Summary: API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit https://github.com/chanzuckerberg/cellxgene-census/
 Author-email: Chan Zuckerberg Initiative <soma@chanzuckerberg.com>
 License: MIT
 Project-URL: homepage, https://github.com/chanzuckerberg/cellxgene-census
 Project-URL: repository, https://github.com/chanzuckerberg/cellxgene-census
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,16 @@
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: <3.12,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: experimental
 License-File: LICENSE
 
 # CZ CELLxGENE Discover Census
 
 The `cellxgene_census` package provides an API to facilitate the use of the CZ CELLxGENE Discover Census. For more information about the API and the project visit the [chanzuckerberg/cellxgene-census GitHub repo](https://github.com/chanzuckerberg/cellxgene-census/).
```

### Comparing `cellxgene_census-1.2.0/src/cellxgene_census.egg-info/SOURCES.txt` & `cellxgene_census-1.2.1/src/cellxgene_census.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/tests/README.md` & `cellxgene_census-1.2.1/tests/README.md`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/tests/conftest.py` & `cellxgene_census-1.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/tests/experimental/ml/test_pytorch.py` & `cellxgene_census-1.2.1/tests/experimental/ml/test_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+import sys
 from typing import Callable, List, Optional, Sequence, Tuple
 
 import numpy as np
 import pyarrow as pa
 import pytest
 import tiledbsoma as soma
 from scipy import sparse
@@ -258,17 +259,20 @@
 
     labels_encoded = batch[1][:, 1]
     labels_decoded = exp_data_pipe.obs_encoders()["label"].inverse_transform(labels_encoded)
     assert labels_decoded.tolist() == ["0", "1", "2"]
 
 
 @pytest.mark.experimental
+@pytest.mark.skipif(
+    (sys.version_info.major, sys.version_info.minor) == (3, 9), reason="fails intermittently with OOM error for 3.9"
+)
 # noinspection PyTestParametrized
 @pytest.mark.parametrize("n_obs,n_vars,X_layer_names,X_value_gen", [(6, 3, ("raw",), pytorch_x_value_gen)])
-def test__multiprocessing__returns_full_result(soma_experiment: Experiment) -> None:
+def test_multiprocessing__returns_full_result(soma_experiment: Experiment) -> None:
     dp = ExperimentDataPipe(
         soma_experiment,
         measurement_name="RNA",
         X_name="raw",
         obs_column_names=["label"],
     )
     dl = experiment_dataloader(dp, num_workers=2)
@@ -359,15 +363,15 @@
 
     dp = ExperimentDataPipe(
         soma_experiment,
         measurement_name="RNA",
         X_name="raw",
         obs_column_names=["label"],
     )
-    dl = experiment_dataloader(dp, num_workers=2)
+    dl = experiment_dataloader(dp, num_workers=1)  # multiprocessing used when num_workers > 0
     dp.obs_encoders()  # trigger query building
     row = next(iter(dl))  # trigger multiprocessing
 
     assert row is not None
 
 
 @pytest.mark.experimental
```

### Comparing `cellxgene_census-1.2.0/tests/experimental/pp/test_hvg.py` & `cellxgene_census-1.2.1/tests/experimental/pp/test_hvg.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/tests/experimental/pp/test_online.py` & `cellxgene_census-1.2.1/tests/experimental/pp/test_online.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/tests/test_acceptance.py` & `cellxgene_census-1.2.1/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/tests/test_directory.py` & `cellxgene_census-1.2.1/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/tests/test_get_anndata.py` & `cellxgene_census-1.2.1/tests/test_get_anndata.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/tests/test_get_helpers.py` & `cellxgene_census-1.2.1/tests/test_get_helpers.py`

 * *Files identical despite different names*

### Comparing `cellxgene_census-1.2.0/tests/test_open.py` & `cellxgene_census-1.2.1/tests/test_open.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 from unittest.mock import patch
 
 import anndata
 import numpy as np
 import pytest
 import requests_mock as rm
+import tiledb
 import tiledbsoma as soma
 
 import cellxgene_census
 from cellxgene_census._open import DEFAULT_TILEDB_CONFIGURATION
 from cellxgene_census._release_directory import CELL_CENSUS_RELEASE_DIRECTORY_URL
 
 
@@ -192,15 +193,15 @@
 
 
 @pytest.mark.live_corpus
 def test_opening_census_without_anon_access_fails_with_bogus_creds() -> None:
     os.environ["AWS_ACCESS_KEY_ID"] = "fake_id"
     os.environ["AWS_SECRET_ACCESS_KEY"] = "fake_key"
     # Passing an empty context
-    with pytest.raises(Exception):
+    with pytest.raises(tiledb.TileDBError, match=r"The AWS Access Key Id you provided does not exist in our records"):
         cellxgene_census.open_soma(census_version="latest", context=soma.SOMATileDBContext())
 
 
 @pytest.mark.live_corpus
 def test_can_open_with_anonymous_access() -> None:
     """
     With anonymous access, `open_soma` must be able to access the census even with bogus credentials
```

### Comparing `cellxgene_census-1.2.0/tests/test_util.py` & `cellxgene_census-1.2.1/tests/test_util.py`

 * *Files identical despite different names*

