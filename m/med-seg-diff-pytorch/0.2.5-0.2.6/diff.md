# Comparing `tmp/med-seg-diff-pytorch-0.2.5.tar.gz` & `tmp/med-seg-diff-pytorch-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "med-seg-diff-pytorch-0.2.5.tar", last modified: Sun Mar 26 18:06:19 2023, max compression
+gzip compressed data, was "med-seg-diff-pytorch-0.2.6.tar", last modified: Sat Jun 17 16:47:59 2023, max compression
```

## Comparing `med-seg-diff-pytorch-0.2.5.tar` & `med-seg-diff-pytorch-0.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 18:06:19.872286 med-seg-diff-pytorch-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-26 18:06:05.000000 med-seg-diff-pytorch-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-26 18:06:19.872286 med-seg-diff-pytorch-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-26 18:06:05.000000 med-seg-diff-pytorch-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 18:06:19.868286 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-26 18:06:05.000000 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-03-26 18:06:05.000000 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-03-26 18:06:05.000000 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch/med_seg_diff_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 18:06:19.872286 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-26 18:06:19.000000 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-26 18:06:19.000000 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 18:06:19.000000 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-26 18:06:19.000000 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-26 18:06:19.000000 med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 18:06:19.872286 med-seg-diff-pytorch-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-26 18:06:05.000000 med-seg-diff-pytorch-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:47:59.172020 med-seg-diff-pytorch-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-17 16:47:42.000000 med-seg-diff-pytorch-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-17 16:47:59.172020 med-seg-diff-pytorch-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-17 16:47:42.000000 med-seg-diff-pytorch-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:47:59.168020 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-17 16:47:42.000000 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-17 16:47:42.000000 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26379 2023-06-17 16:47:42.000000 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch/med_seg_diff_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:47:59.172020 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-17 16:47:59.000000 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-17 16:47:59.000000 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:47:59.000000 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 16:47:59.000000 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-17 16:47:59.000000 med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 16:47:59.172020 med-seg-diff-pytorch-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-17 16:47:42.000000 med-seg-diff-pytorch-0.2.6/setup.py
```

### Comparing `med-seg-diff-pytorch-0.2.5/LICENSE` & `med-seg-diff-pytorch-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `med-seg-diff-pytorch-0.2.5/PKG-INFO` & `med-seg-diff-pytorch-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: med-seg-diff-pytorch
-Version: 0.2.5
+Version: 0.2.6
 Summary: MedSegDiff - SOTA medical image segmentation - Pytorch
 Home-page: https://github.com/lucidrains/med-seg-diff-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,denoising diffusion,medical segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `med-seg-diff-pytorch-0.2.5/README.md` & `med-seg-diff-pytorch-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch/dataset.py` & `med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch/med_seg_diff_pytorch.py` & `med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch/med_seg_diff_pytorch.py`

 * *Files identical despite different names*

### Comparing `med-seg-diff-pytorch-0.2.5/med_seg_diff_pytorch.egg-info/PKG-INFO` & `med-seg-diff-pytorch-0.2.6/med_seg_diff_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: med-seg-diff-pytorch
-Version: 0.2.5
+Version: 0.2.6
 Summary: MedSegDiff - SOTA medical image segmentation - Pytorch
 Home-page: https://github.com/lucidrains/med-seg-diff-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,denoising diffusion,medical segmentation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `med-seg-diff-pytorch-0.2.5/setup.py` & `med-seg-diff-pytorch-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'med-seg-diff-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.5',
+  version = '0.2.6',
   license='MIT',
   description = 'MedSegDiff - SOTA medical image segmentation - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/med-seg-diff-pytorch',
   keywords = [
```

