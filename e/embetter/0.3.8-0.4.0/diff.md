# Comparing `tmp/embetter-0.3.8.tar.gz` & `tmp/embetter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embetter-0.3.8.tar", last modified: Thu May  4 19:47:28 2023, max compression
+gzip compressed data, was "dist/embetter-0.4.0.tar", last modified: Sat Jun 17 12:49:36 2023, max compression
```

## Comparing `embetter-0.3.8.tar` & `embetter-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.895062 embetter-0.3.8/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5190 2023-05-04 19:47:28.895062 embetter-0.3.8/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4061 2023-05-04 19:18:34.000000 embetter-0.3.8/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.875062 embetter-0.3.8/embetter/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      185 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      326 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      742 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/error.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.879062 embetter-0.3.8/embetter/external/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      256 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/external/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2001 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/external/_cohere.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2356 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/external/_openai.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.883062 embetter-0.3.8/embetter/finetune/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      401 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/finetune/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5414 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/finetune/_contrastive.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2851 2023-05-04 19:30:13.000000 embetter-0.3.8/embetter/finetune/_forward.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2408 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/grab.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.883062 embetter-0.3.8/embetter/multi/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      185 2023-05-04 19:17:23.000000 embetter-0.3.8/embetter/multi/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1758 2023-05-04 19:30:13.000000 embetter-0.3.8/embetter/multi/_clip.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.887062 embetter-0.3.8/embetter/text/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      730 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3794 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/_bpemb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1579 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/_s2v.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3179 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/_sbert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2767 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/text/_spacy.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.891062 embetter-0.3.8/embetter/vision/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      361 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/vision/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1980 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/vision/_colorhist.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2205 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/vision/_loader.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2056 2023-05-04 19:11:56.000000 embetter-0.3.8/embetter/vision/_torchvis.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.879062 embetter-0.3.8/embetter.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5190 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      860 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1004 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2023-05-04 19:47:28.000000 embetter-0.3.8/embetter.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-04 19:47:28.895062 embetter-0.3.8/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2595 2023-05-04 19:32:08.000000 embetter-0.3.8/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:47:28.895062 embetter-0.3.8/tests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-04 19:12:23.000000 embetter-0.3.8/tests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      324 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       64 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_default.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      910 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_docs.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      452 2023-05-04 19:30:56.000000 embetter-0.3.8/tests/test_finetuners.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2521 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_text.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      871 2023-05-04 19:11:56.000000 embetter-0.3.8/tests/test_vision.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5227 2023-06-17 12:49:36.000000 embetter-0.4.0/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4061 2023-06-03 11:05:06.000000 embetter-0.4.0/README.md
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-05-01 13:07:12.000000 embetter-0.4.0/embetter/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      326 2022-09-17 15:40:35.000000 embetter-0.4.0/embetter/base.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      742 2022-07-16 12:25:08.000000 embetter-0.4.0/embetter/error.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/external/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      256 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/external/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2001 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/external/_cohere.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2356 2023-03-28 13:55:26.000000 embetter-0.4.0/embetter/external/_openai.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/finetune/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      401 2023-03-28 13:55:26.000000 embetter-0.4.0/embetter/finetune/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5414 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/finetune/_contrastive.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2851 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/finetune/_forward.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2408 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/grab.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/multi/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/multi/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1758 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/multi/_clip.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/text/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2023-03-28 13:55:26.000000 embetter-0.4.0/embetter/text/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3794 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/text/_bpemb.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1579 2023-03-28 13:55:22.000000 embetter-0.4.0/embetter/text/_s2v.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/text/_sbert.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2767 2023-03-28 13:55:22.000000 embetter-0.4.0/embetter/text/_spacy.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2437 2023-06-17 12:37:51.000000 embetter-0.4.0/embetter/utils.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/vision/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      361 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/vision/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1980 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/vision/_colorhist.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2205 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/vision/_loader.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2056 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/vision/_torchvis.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5227 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      878 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1209 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       15 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/top_level.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-06-17 12:49:36.000000 embetter-0.4.0/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2615 2023-06-17 12:26:56.000000 embetter-0.4.0/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/tests/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2021-10-31 16:15:20.000000 embetter-0.4.0/tests/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2022-12-05 09:29:24.000000 embetter-0.4.0/tests/test_base.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       64 2022-07-16 12:25:08.000000 embetter-0.4.0/tests/test_default.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      910 2023-02-09 16:06:49.000000 embetter-0.4.0/tests/test_docs.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      452 2023-06-03 11:05:04.000000 embetter-0.4.0/tests/test_finetuners.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3033 2023-06-17 12:37:00.000000 embetter-0.4.0/tests/test_text.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      871 2022-12-05 09:29:24.000000 embetter-0.4.0/tests/test_vision.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `embetter-0.3.8/PKG-INFO` & `embetter-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: embetter
-Version: 0.3.8
+Version: 0.4.0
 Summary: Just a bunch of useful embeddings to get started quickly.
 Home-page: https://koaning.github.io/embetter/
 Author: Vincent D. Warmerdam
+License: UNKNOWN
 Project-URL: Documentation, https://koaning.github.io/embetter/
 Project-URL: Source Code, https://github.com/koaning/embetter/
 Project-URL: Issue Tracker, https://github.com/koaning/embetter/issues
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -151,7 +153,9 @@
 
 All of the encoding tools you've seen here are also compatible
 with the [`partial_fit` mechanic](https://scikit-learn.org/0.15/modules/scaling_strategies.html#incremental-learning) 
 in scikit-learn. That means
 you can leverage [scikit-partial](https://github.com/koaning/scikit-partial)
 to build pipelines that can handle out-of-core datasets. 
 
+
+
```

### Comparing `embetter-0.3.8/README.md` & `embetter-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/error.py` & `embetter-0.4.0/embetter/error.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/external/_cohere.py` & `embetter-0.4.0/embetter/external/_cohere.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/external/_openai.py` & `embetter-0.4.0/embetter/external/_openai.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/finetune/_contrastive.py` & `embetter-0.4.0/embetter/finetune/_contrastive.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/finetune/_forward.py` & `embetter-0.4.0/embetter/finetune/_forward.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/grab.py` & `embetter-0.4.0/embetter/grab.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/multi/_clip.py` & `embetter-0.4.0/embetter/multi/_clip.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/text/__init__.py` & `embetter-0.4.0/embetter/text/__init__.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/text/_bpemb.py` & `embetter-0.4.0/embetter/text/_bpemb.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/text/_s2v.py` & `embetter-0.4.0/embetter/text/_s2v.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/text/_sbert.py` & `embetter-0.4.0/embetter/text/_sbert.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/text/_spacy.py` & `embetter-0.4.0/embetter/text/_spacy.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/vision/_colorhist.py` & `embetter-0.4.0/embetter/vision/_colorhist.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/vision/_loader.py` & `embetter-0.4.0/embetter/vision/_loader.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter/vision/_torchvis.py` & `embetter-0.4.0/embetter/vision/_torchvis.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/embetter.egg-info/PKG-INFO` & `embetter-0.4.0/embetter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: embetter
-Version: 0.3.8
+Version: 0.4.0
 Summary: Just a bunch of useful embeddings to get started quickly.
 Home-page: https://koaning.github.io/embetter/
 Author: Vincent D. Warmerdam
+License: UNKNOWN
 Project-URL: Documentation, https://koaning.github.io/embetter/
 Project-URL: Source Code, https://github.com/koaning/embetter/
 Project-URL: Issue Tracker, https://github.com/koaning/embetter/issues
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -151,7 +153,9 @@
 
 All of the encoding tools you've seen here are also compatible
 with the [`partial_fit` mechanic](https://scikit-learn.org/0.15/modules/scaling_strategies.html#incremental-learning) 
 in scikit-learn. That means
 you can leverage [scikit-partial](https://github.com/koaning/scikit-partial)
 to build pipelines that can handle out-of-core datasets. 
 
+
+
```

### Comparing `embetter-0.3.8/embetter.egg-info/SOURCES.txt` & `embetter-0.4.0/embetter.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 setup.py
 embetter/__init__.py
 embetter/base.py
 embetter/error.py
 embetter/grab.py
+embetter/utils.py
 embetter.egg-info/PKG-INFO
 embetter.egg-info/SOURCES.txt
 embetter.egg-info/dependency_links.txt
 embetter.egg-info/requires.txt
 embetter.egg-info/top_level.txt
 embetter/external/__init__.py
 embetter/external/_cohere.py
```

### Comparing `embetter-0.3.8/embetter.egg-info/requires.txt` & `embetter-0.4.0/embetter.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,85 @@
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 
 [all]
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 sentence-transformers>=2.2.2
 sense2vec==2.0.0
 bpemb>=0.3.3
 timm>=0.6.7
 openai>=0.25.0
 
 [bpemb]
 bpemb>=0.3.3
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 
 [dev]
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 sentence-transformers>=2.2.2
 sense2vec==2.0.0
 bpemb>=0.3.3
 timm>=0.6.7
 openai>=0.25.0
 mkdocs==1.1
 mkdocs-material==4.6.3
 mkdocstrings==0.8.0
 mktestdocs==0.1.2
 interrogate>=1.5.0
 flake8>=3.6.0
 pytest>=4.0.2
 black>=19.3b0
 pre-commit>=2.2.0
+mktestdocs==0.1.2
 datasets==2.8.0
 matplotlib==3.4.3
 
 [openai]
 openai>=0.25.0
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 
 [pytorch]
 torch>=1.12.0
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 
 [sense2vec]
 sense2vec==2.0.0
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 
 [sentence-tfm]
 sentence-transformers>=2.2.2
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 
 [spacy]
 spacy>=3.5.0
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 
 [text]
 sentence-transformers>=2.2.2
 sense2vec==2.0.0
 bpemb>=0.3.3
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
 
 [vision]
 timm>=0.6.7
 scikit-learn>=1.0.0
 pandas>=1.0.0
+diskcache>=5.6.1
```

### Comparing `embetter-0.3.8/setup.py` & `embetter-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pathlib
 from setuptools import setup, find_packages
 
 
-base_packages = ["scikit-learn>=1.0.0", "pandas>=1.0.0"]
+base_packages = ["scikit-learn>=1.0.0", "pandas>=1.0.0", "diskcache>=5.6.1"]
 
 sentence_encoder_pkgs = ["sentence-transformers>=2.2.2"]
 sense2vec_pkgs = ["sense2vec==2.0.0"]
 bpemb_packages = ["bpemb>=0.3.3"]
 spacy_packages = ["spacy>=3.5.0"]
 
 text_packages = sentence_encoder_pkgs + sense2vec_pkgs + bpemb_packages
@@ -38,15 +38,15 @@
 
 all_packages = base_packages + text_packages + vision_packages + openai_packages
 dev_packages = all_packages + docs_packages + test_packages
 
 
 setup(
     name="embetter",
-    version="0.3.8",
+    version="0.4.0",
     author="Vincent D. Warmerdam",
     packages=find_packages(exclude=["notebooks", "docs"]),
     description="Just a bunch of useful embeddings to get started quickly.",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     license_files=("LICENSE"),
     url="https://koaning.github.io/embetter/",
```

### Comparing `embetter-0.3.8/tests/test_docs.py` & `embetter-0.4.0/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `embetter-0.3.8/tests/test_text.py` & `embetter-0.4.0/tests/test_text.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pytest
 import numpy as np
 
 from spacy.vocab import Vocab
 from spacy.language import Language
 
 from embetter.text import SentenceEncoder, BytePairEncoder, spaCyEncoder
+from embetter.utils import cached
 
 
 test_sentences = [
     "This is a test sentence!",
     "And this is another one",
     "\rUnicode stuff: ♣️,♦️,❤️,♠️\n",
 ]
@@ -63,7 +64,22 @@
     # Embedding dim of underlying model
     output = encoder.fit_transform(test_sentences)
     assert isinstance(output, np.ndarray)
     assert output.shape == (len(test_sentences), 4 if setting == "both" else 2)
     # scikit-learn configures repr dynamically from defined attributes.
     # To test correct implementation we should test if calling repr breaks.
     assert repr(encoder)
+
+
+def test_basic_spacy_cached(nlp, tmpdir):
+    """Just an e2e test for the cache."""
+    encoder = spaCyEncoder(nlp)
+    output_before = encoder.transform(test_sentences)
+
+    # Now we cache it
+    encoder = cached(tmpdir, encoder)
+    output_during = encoder.transform(test_sentences)
+
+    encoder = cached(tmpdir, encoder)
+    output_after = encoder.transform(test_sentences)
+    assert (output_before == output_during).all()
+    assert (output_during == output_after).all()
```

### Comparing `embetter-0.3.8/tests/test_vision.py` & `embetter-0.4.0/tests/test_vision.py`

 * *Files identical despite different names*

