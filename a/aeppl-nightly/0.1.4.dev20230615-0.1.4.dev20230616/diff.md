# Comparing `tmp/aeppl-nightly-0.1.4.dev20230615.tar.gz` & `tmp/aeppl-nightly-0.1.4.dev20230616.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl-nightly-0.1.4.dev20230615.tar", last modified: Thu Jun 15 00:35:05 2023, max compression
+gzip compressed data, was "aeppl-nightly-0.1.4.dev20230616.tar", last modified: Fri Jun 16 00:36:07 2023, max compression
```

## Comparing `aeppl-nightly-0.1.4.dev20230615.tar` & `aeppl-nightly-0.1.4.dev20230616.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:35:05.212946 aeppl-nightly-0.1.4.dev20230615/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 00:35:05.212946 aeppl-nightly-0.1.4.dev20230615/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:35:05.212946 aeppl-nightly-0.1.4.dev20230615/aeppl/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-15 00:35:05.212946 aeppl-nightly-0.1.4.dev20230615/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:35:05.208946 aeppl-nightly-0.1.4.dev20230615/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 00:35:05.000000 aeppl-nightly-0.1.4.dev20230615/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-15 00:35:05.000000 aeppl-nightly-0.1.4.dev20230615/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:35:05.000000 aeppl-nightly-0.1.4.dev20230615/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 00:35:04.000000 aeppl-nightly-0.1.4.dev20230615/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-15 00:35:05.000000 aeppl-nightly-0.1.4.dev20230615/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-15 00:35:05.000000 aeppl-nightly-0.1.4.dev20230615/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 00:35:05.212946 aeppl-nightly-0.1.4.dev20230615/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 00:35:05.212946 aeppl-nightly-0.1.4.dev20230615/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-15 00:34:52.000000 aeppl-nightly-0.1.4.dev20230615/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:36:07.667792 aeppl-nightly-0.1.4.dev20230616/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-16 00:36:07.667792 aeppl-nightly-0.1.4.dev20230616/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:36:07.667792 aeppl-nightly-0.1.4.dev20230616/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-16 00:36:07.667792 aeppl-nightly-0.1.4.dev20230616/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:36:07.663792 aeppl-nightly-0.1.4.dev20230616/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-16 00:36:07.000000 aeppl-nightly-0.1.4.dev20230616/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-16 00:36:07.000000 aeppl-nightly-0.1.4.dev20230616/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:36:07.000000 aeppl-nightly-0.1.4.dev20230616/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:36:07.000000 aeppl-nightly-0.1.4.dev20230616/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 00:36:07.000000 aeppl-nightly-0.1.4.dev20230616/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 00:36:07.000000 aeppl-nightly-0.1.4.dev20230616/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-16 00:36:07.667792 aeppl-nightly-0.1.4.dev20230616/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:36:07.667792 aeppl-nightly-0.1.4.dev20230616/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-16 00:35:55.000000 aeppl-nightly-0.1.4.dev20230616/versioneer.py
```

### Comparing `aeppl-nightly-0.1.4.dev20230615/LICENSE` & `aeppl-nightly-0.1.4.dev20230616/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/PKG-INFO` & `aeppl-nightly-0.1.4.dev20230616/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.4.dev20230615
+Version: 0.1.4.dev20230616
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.4.dev20230615/README.md` & `aeppl-nightly-0.1.4.dev20230616/README.md`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/abstract.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/censoring.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/convolutions.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/cumsum.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/dists.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/joint_logprob.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/logprob.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/mixture.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/printing.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/rewriting.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/scan.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/tensor.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/transforms.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl/utils.py` & `aeppl-nightly-0.1.4.dev20230616/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl_nightly.egg-info/PKG-INFO` & `aeppl-nightly-0.1.4.dev20230616/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.4.dev20230615
+Version: 0.1.4.dev20230616
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.4.dev20230615/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl-nightly-0.1.4.dev20230616/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/setup.cfg` & `aeppl-nightly-0.1.4.dev20230616/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/setup.py` & `aeppl-nightly-0.1.4.dev20230616/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_abstract.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_censoring.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_composite_logprob.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_composite_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_convolutions.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_cumsum.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_dist.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_joint_logprob.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_logprob.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_mixture.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_printing.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_rewriting.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_scan.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_tensor.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_transforms.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/tests/test_utils.py` & `aeppl-nightly-0.1.4.dev20230616/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230615/versioneer.py` & `aeppl-nightly-0.1.4.dev20230616/versioneer.py`

 * *Files identical despite different names*

