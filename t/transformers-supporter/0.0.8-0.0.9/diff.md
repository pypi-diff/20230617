# Comparing `tmp/transformers-supporter-0.0.8.tar.gz` & `tmp/transformers-supporter-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers-supporter-0.0.8.tar", last modified: Sun Apr 16 16:31:40 2023, max compression
+gzip compressed data, was "transformers-supporter-0.0.9.tar", last modified: Sun Apr 16 16:44:00 2023, max compression
```

## Comparing `transformers-supporter-0.0.8.tar` & `transformers-supporter-0.0.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.628436 transformers-supporter-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     2414 2023-04-16 16:31:40.628436 transformers-supporter-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2120 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 16:31:40.628436 transformers-supporter-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      618 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.621436 transformers-supporter-0.0.8/transformers_supporter/
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.622436 transformers-supporter-0.0.8/transformers_supporter/models/
--rw-r--r--   0 root         (0) root         (0)     1936 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.623436 transformers-supporter-0.0.8/transformers_supporter/models/ann/
--rw-r--r--   0 root         (0) root         (0)       96 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/ann/__init__.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/ann/configuration_ann.py
--rw-r--r--   0 root         (0) root         (0)     6060 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/ann/feature_extraction_ann.py
--rw-r--r--   0 root         (0) root         (0)     4462 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/ann/modeling_ann.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.623436 transformers-supporter-0.0.8/transformers_supporter/models/cnn/
--rw-r--r--   0 root         (0) root         (0)       94 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/cnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/cnn/configuration_cnn.py
--rw-r--r--   0 root         (0) root         (0)     4714 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/cnn/image_processing_cnn.py
--rw-r--r--   0 root         (0) root         (0)     3743 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/cnn/modeling_cnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.624436 transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/configuration_custom_bert.py
--rw-r--r--   0 root         (0) root         (0)     2949 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/modeling_custom_bert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.624436 transformers-supporter-0.0.8/transformers_supporter/models/custom_wav2vec2/
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_wav2vec2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2748 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_wav2vec2/feature_extraction_custom_wav2vec2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.625436 transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/
--rw-r--r--   0 root         (0) root         (0)       81 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/configuration_embedded_1dcnn.py
--rw-r--r--   0 root         (0) root         (0)     2292 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/modeling_embedded_1dcnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.625436 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1329 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/configuration_embedded_rnn.py
--rw-r--r--   0 root         (0) root         (0)     6524 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/modeling_embedded_rnn.py
--rw-r--r--   0 root         (0) root         (0)     5639 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/tokenization_embedded_rnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.626436 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/
--rw-r--r--   0 root         (0) root         (0)      118 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/configuration_faster_rcnn.py
--rw-r--r--   0 root         (0) root         (0)     3626 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/image_processing_faster_rcnn.py
--rw-r--r--   0 root         (0) root         (0)     4103 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/modeling_faster_rcnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.626436 transformers-supporter-0.0.8/transformers_supporter/models/rnn/
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/rnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/rnn/configuration_rnn.py
--rw-r--r--   0 root         (0) root         (0)     3432 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/rnn/modeling_rnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.627436 transformers-supporter-0.0.8/transformers_supporter/pipelines/
--rw-r--r--   0 root         (0) root         (0)      633 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1372 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/custom_image_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/fixed_length_translation_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_binary_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_regression_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.622436 transformers-supporter-0.0.8/transformers_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2414 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2407 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.980780 transformers-supporter-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-04-16 16:44:00.980780 transformers-supporter-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 16:44:00.980780 transformers-supporter-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.973780 transformers-supporter-0.0.9/transformers_supporter/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.975780 transformers-supporter-0.0.9/transformers_supporter/models/
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.975780 transformers-supporter-0.0.9/transformers_supporter/models/ann/
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/ann/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/ann/configuration_ann.py
+-rw-r--r--   0 root         (0) root         (0)     6060 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/ann/feature_extraction_ann.py
+-rw-r--r--   0 root         (0) root         (0)     4462 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/ann/modeling_ann.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.976780 transformers-supporter-0.0.9/transformers_supporter/models/cnn/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/cnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      783 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/cnn/configuration_cnn.py
+-rw-r--r--   0 root         (0) root         (0)     4714 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/cnn/image_processing_cnn.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/cnn/modeling_cnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.976780 transformers-supporter-0.0.9/transformers_supporter/models/custom_bert/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/custom_bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      815 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/custom_bert/configuration_custom_bert.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/custom_bert/modeling_custom_bert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.977780 transformers-supporter-0.0.9/transformers_supporter/models/custom_wav2vec2/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/custom_wav2vec2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/custom_wav2vec2/feature_extraction_custom_wav2vec2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.977780 transformers-supporter-0.0.9/transformers_supporter/models/embedded_1dcnn/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/embedded_1dcnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      830 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/embedded_1dcnn/configuration_embedded_1dcnn.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/embedded_1dcnn/modeling_embedded_1dcnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.978780 transformers-supporter-0.0.9/transformers_supporter/models/embedded_rnn/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/embedded_rnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/embedded_rnn/configuration_embedded_rnn.py
+-rw-r--r--   0 root         (0) root         (0)     6548 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/embedded_rnn/modeling_embedded_rnn.py
+-rw-r--r--   0 root         (0) root         (0)     5639 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/embedded_rnn/tokenization_embedded_rnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.978780 transformers-supporter-0.0.9/transformers_supporter/models/faster_rcnn/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/faster_rcnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/faster_rcnn/configuration_faster_rcnn.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/faster_rcnn/image_processing_faster_rcnn.py
+-rw-r--r--   0 root         (0) root         (0)     4103 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/faster_rcnn/modeling_faster_rcnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.979780 transformers-supporter-0.0.9/transformers_supporter/models/rnn/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/rnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/rnn/configuration_rnn.py
+-rw-r--r--   0 root         (0) root         (0)     3450 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/models/rnn/modeling_rnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.980780 transformers-supporter-0.0.9/transformers_supporter/pipelines/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/pipelines/custom_image_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/pipelines/fixed_length_translation_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/pipelines/tabular_binary_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/pipelines/tabular_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter/pipelines/tabular_regression_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:44:00.974780 transformers-supporter-0.0.9/transformers_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-16 16:44:00.000000 transformers-supporter-0.0.9/transformers_supporter.egg-info/top_level.txt
```

### Comparing `transformers-supporter-0.0.8/PKG-INFO` & `transformers-supporter-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-supporter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Transformers supporter
 Home-page: https://github.com/automatethem/transformers-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `transformers-supporter-0.0.8/README.md` & `transformers-supporter-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/setup.py` & `transformers-supporter-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='transformers-supporter',
-	version='0.0.8',
+	version='0.0.9',
 	description='Transformers supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/transformers-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/__init__.py` & `transformers-supporter-0.0.9/transformers_supporter/models/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/ann/configuration_ann.py` & `transformers-supporter-0.0.9/transformers_supporter/models/ann/configuration_ann.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/ann/feature_extraction_ann.py` & `transformers-supporter-0.0.9/transformers_supporter/models/ann/feature_extraction_ann.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/ann/modeling_ann.py` & `transformers-supporter-0.0.9/transformers_supporter/models/ann/modeling_ann.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/cnn/configuration_cnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/custom_bert/configuration_custom_bert.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
-from transformers import AutoModelForImageClassification
+from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 
-class CnnConfig(PretrainedConfig):
-    model_type = "cnn"
+class CustomBertConfig(PretrainedConfig):
+    model_type = "custom-bert"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
         #Keys are always strings in JSON so convert ids to int here.       
-        super().__init__(**kwargs) 
+        super().__init__(**kwargs)
 
 #오토 설정에 등록
-model_path = 'cnn'
-AutoConfig.register(model_path, CnnConfig)
+model_path = 'custom-bert'
+AutoConfig.register(model_path, CustomBertConfig)
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/cnn/image_processing_cnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/cnn/image_processing_cnn.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/cnn/modeling_cnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/cnn/modeling_cnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForImageClassification
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 from .configuration_cnn import CnnConfig
     
 class CnnForImageClassification(PreTrainedModel):
     config_class = CnnConfig
 
     def __init__(self, config):
@@ -21,15 +21,15 @@
             torch.nn.ReLU(),
             torch.nn.MaxPool2d(kernel_size=2, stride=2, padding=0),
             torch.nn.Conv2d(in_channels=32, out_channels=32, kernel_size=5, stride=1, padding=0),
             torch.nn.BatchNorm2d(num_features=32),
             torch.nn.ReLU(),
             torch.nn.MaxPool2d(kernel_size=2, stride=2, padding=0),
             torch.nn.Flatten(), #배치를 제외한 모든 차원을 평탄화
-            pytorch_helper.layers.LazilyInitializedLinear(out_features=config.num_labels)
+            pytorch_supporter.layers.LazilyInitializedLinear(out_features=config.num_labels)
         )
 
     def forward(self, pixel_values, labels=None):
         #print(pixel_values.shape) #
         logits = self.layer(pixel_values)
         #print(logits.shape) #torch.Size([16, 3])
         if labels == None:
@@ -43,15 +43,15 @@
 AutoModelForImageClassification.register(CnnConfig, CnnForImageClassification)
 
 ####################
 
 from transformers import PreTrainedModel
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 from .configuration_cnn import CnnConfig
 
 class CnnForKeyPointDetection(PreTrainedModel):
     config_class = CnnConfig
 
     def __init__(self, config):
@@ -63,15 +63,15 @@
             torch.nn.MaxPool2d(kernel_size=2, stride=2, padding=0),
             torch.nn.Conv2d(in_channels=32, out_channels=32, kernel_size=5, stride=1, padding=0),
             torch.nn.BatchNorm2d(num_features=32),
             torch.nn.ReLU(),
             torch.nn.MaxPool2d(kernel_size=2, stride=2, padding=0),
             torch.nn.Flatten(), #배치를 제외한 모든 차원을 평탄화
             torch.nn.Linear(in_features=14112, out_features=config.num_labels * 2)
-            #pytorch_helper.layers.LazilyInitializedLinear(out_features=30)
+            #pytorch_supporter.layers.LazilyInitializedLinear(out_features=30)
         )
 
     def forward(self, pixel_values, labels=None):
         #print(pixel_values.shape) #
         logits = self.layer(pixel_values)
         #print(logits.shape) #torch.Size([16, 3])
         if labels == None:
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/configuration_custom_bert.py` & `transformers-supporter-0.0.9/transformers_supporter/models/embedded_1dcnn/configuration_embedded_1dcnn.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 
-class CustomBertConfig(PretrainedConfig):
-    model_type = "custom-bert"
+class Embedded1dcnnConfig(PretrainedConfig):
+    model_type = "embedded-1dcnn"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
         #Keys are always strings in JSON so convert ids to int here.       
-        super().__init__(**kwargs)
+        super().__init__(**kwargs)   
 
 #오토 설정에 등록
-model_path = 'custom-bert'
-AutoConfig.register(model_path, CustomBertConfig)
+model_path = 'embedded-1dcnn'
+AutoConfig.register(model_path, Embedded1dcnnConfig)
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/modeling_custom_bert.py` & `transformers-supporter-0.0.9/transformers_supporter/models/custom_bert/modeling_custom_bert.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 from .configuration_custom_bert import CustomBertConfig
 
 '''
 class CustomBertForSequenceClassification(PreTrainedModel):
     config_class = CustomBertConfig
 
@@ -36,16 +36,16 @@
 #torch.nn.Sequential 버전
 class CustomBertForSequenceClassification(PreTrainedModel):
     config_class = CustomBertConfig
 
     def __init__(self, config):
         super().__init__(config)
         self.layer = torch.nn.Sequential(
-            pytorch_helper.layers.DictToParameters(AutoModel.from_pretrained(config.bert_model_path)),
-            pytorch_helper.layers.SelectFromArray(index=1), #x.pooler_output
+            pytorch_supporter.layers.DictToParameters(AutoModel.from_pretrained(config.bert_model_path)),
+            pytorch_supporter.layers.SelectFromArray(index=1), #x.pooler_output
             torch.nn.Linear(in_features=768, out_features=config.num_labels)
         )
 
     def forward(self, input_ids, attention_mask=None, token_type_ids=None, labels=None):
         logits = self.layer(dict(input_ids=input_ids, attention_mask=attention_mask, token_type_ids=token_type_ids))
         #print(pooler_output.shape) #torch.Size([1, 768])
         #print(logits.shape) #torch.Size([16, 3])
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/custom_wav2vec2/feature_extraction_custom_wav2vec2.py` & `transformers-supporter-0.0.9/transformers_supporter/models/custom_wav2vec2/feature_extraction_custom_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/configuration_embedded_1dcnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/cnn/configuration_cnn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
-from transformers import AutoModelForSequenceClassification
+from transformers import AutoModelForImageClassification
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 
-class Embedded1dcnnConfig(PretrainedConfig):
-    model_type = "embedded-1dcnn"
+class CnnConfig(PretrainedConfig):
+    model_type = "cnn"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
         #Keys are always strings in JSON so convert ids to int here.       
-        super().__init__(**kwargs)   
+        super().__init__(**kwargs) 
 
 #오토 설정에 등록
-model_path = 'embedded-1dcnn'
-AutoConfig.register(model_path, Embedded1dcnnConfig)
+model_path = 'cnn'
+AutoConfig.register(model_path, CnnConfig)
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/modeling_embedded_1dcnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/embedded_1dcnn/modeling_embedded_1dcnn.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,39 +2,39 @@
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 from .configuration_embedded_1dcnn import Embedded1dcnnConfig
 
 class Embedded1dcnnForSequenceClassification(PreTrainedModel):
     config_class = Embedded1dcnnConfig
 
     def __init__(self, config):
         super().__init__(config)
         self.layer = torch.nn.Sequential(
             torch.nn.Embedding(num_embeddings=config.vocab_size, embedding_dim=32), #
             #https://chriskhanhtran.github.io/posts/cnn-sentence-classification/
             #Permute `x_embed` to match input shape requirement of `nn.Conv1d`.
             #Output shape: (b, embed_dim, max_len)
-            pytorch_helper.layers.Permute((0, 2, 1)),
+            pytorch_supporter.layers.Permute((0, 2, 1)),
             torch.nn.Conv1d(in_channels=32, out_channels=32, kernel_size=5, stride=1, padding=0),
             torch.nn.BatchNorm1d(num_features=32),
             torch.nn.ReLU(),
             torch.nn.MaxPool1d(kernel_size=2, stride=2, padding=0),
             torch.nn.Conv1d(in_channels=32, out_channels=32, kernel_size=5, stride=1, padding=0),
             torch.nn.BatchNorm1d(num_features=32),
             torch.nn.ReLU(),
             torch.nn.MaxPool1d(kernel_size=2, stride=2, padding=0),
             torch.nn.Flatten(), #배치를 제외한 모든 차원을 평탄화
-            pytorch_helper.layers.LazilyInitializedLinear(out_features=config.num_labels)
+            pytorch_supporter.layers.LazilyInitializedLinear(out_features=config.num_labels)
         )
 
     def forward(self, input_ids, labels=None):
         logits = self.layer(input_ids)
         print(logits.shape) #torch.Size([16, 3])
         if labels == None:
             return transformers.file_utils.ModelOutput({'logits': logits})
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/configuration_embedded_rnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/embedded_rnn/configuration_embedded_rnn.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 
 class EmbeddedRnnConfig(PretrainedConfig):
     model_type = "embedded-rnn"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/modeling_embedded_rnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/embedded_rnn/modeling_embedded_rnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 from .configuration_embedded_rnn import EmbeddedRnnConfig
 
 class EmbeddedRnnForSequenceClassification(PreTrainedModel):
     config_class = EmbeddedRnnConfig
 
     def __init__(self, config):
         super().__init__(config)        
         self.layer = torch.nn.Sequential(
             torch.nn.Embedding(num_embeddings=config.vocab_size, embedding_dim=32),
-            pytorch_helper.layers.HiddenStateResetLSTM(input_size=32, hidden_size=32, batch_first=True),
-            pytorch_helper.layers.LSTMLastHiddenState(),
+            pytorch_supporter.layers.HiddenStateResetLSTM(input_size=32, hidden_size=32, batch_first=True),
+            pytorch_supporter.layers.LSTMLastHiddenState(),
             torch.nn.Linear(in_features=32, out_features=config.num_labels)
         )
 
     def forward(self, input_ids, labels=None):
         logits = self.layer(input_ids)
         #print(logits.shape) #torch.Size([16, 3])
         if labels == None:
@@ -39,27 +39,27 @@
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 import torch
 from torch.nn import functional as F
-import pytorch_helper
+import pytorch_supporter
 import transformers
 from .configuration_embedded_rnn import EmbeddedRnnConfig
 
 class EmbeddedRnnForFixedLengthTranslation(PreTrainedModel):
     config_class = EmbeddedRnnConfig
 
     def __init__(self, config):
         super().__init__(config)        
         self.layer = torch.nn.Sequential(
             torch.nn.Embedding(num_embeddings=config.vocab_size, embedding_dim=32),
-            pytorch_helper.layers.HiddenStateResetLSTM(input_size=32, hidden_size=32, batch_first=True),
-            pytorch_helper.layers.SelectFromArray(index=0), #lstm output, 모든 타임 스텝(토큰: 숫자, 문자, 단어)의 숨은 상태, torch.Size([8, 380, 32]) 
+            pytorch_supporter.layers.HiddenStateResetLSTM(input_size=32, hidden_size=32, batch_first=True),
+            pytorch_supporter.layers.SelectFromArray(index=0), #lstm output, 모든 타임 스텝(토큰: 숫자, 문자, 단어)의 숨은 상태, torch.Size([8, 380, 32]) 
             torch.nn.Linear(in_features=32, out_features=config.vocab_size)
         )
 
     def forward(self, input_ids, labels=None):
         logits = self.layer(input_ids)
         #print(logits.shape) #torch.Size([2, 3, 7])
         if labels == None:
@@ -95,16 +95,16 @@
 class PretrainedEmbeddedRnnForSequenceClassification(PreTrainedModel):
     config_class = PretrainedEmbeddedRnnConfig
 
     def __init__(self, config):
         super().__init__(config)  
         self.layer = torch.nn.Sequential(
             self.load_pretrained_embedding(num_embeddings=config.vocab_size, embedding_dim=300, id_to_token=config.id_to_token),
-            pytorch_helper.layers.HiddenStateResetLSTM(input_size=300, hidden_size=32, batch_first=True),
-            pytorch_helper.layers.LSTMLastHiddenState(),
+            pytorch_supporter.layers.HiddenStateResetLSTM(input_size=300, hidden_size=32, batch_first=True),
+            pytorch_supporter.layers.LSTMLastHiddenState(),
             torch.nn.Linear(in_features=32, out_features=config.num_labels)
         )
 
     def load_pretrained_embedding(self, num_embeddings, embedding_dim, id_to_token):
         #사이즈가 작은 파일들만 가져왔습니다. 다른 모델을 써보고 싶다면, 아래 링크를 참고해서 코드를 변경해서 사용하세요.
         #https://pytorch.org/text/stable/_modules/torchtext/vocab/vectors.html#Vectors
         '''
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/tokenization_embedded_rnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/embedded_rnn/tokenization_embedded_rnn.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/configuration_faster_rcnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/faster_rcnn/configuration_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/image_processing_faster_rcnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/faster_rcnn/image_processing_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/modeling_faster_rcnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/faster_rcnn/modeling_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/models/rnn/modeling_rnn.py` & `transformers-supporter-0.0.9/transformers_supporter/models/rnn/modeling_rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForAudioClassification
-import pytorch_helper
+import pytorch_supporter
 import torch
 from torch.nn import functional as F
 import transformers
 from .configuration_rnn import RnnConfig
 
 class RnnForAudioClassification(PreTrainedModel):
     config_class = RnnConfig
 
     def __init__(self, config):
         super().__init__(config)        
         self.layer = torch.nn.Sequential(
-            pytorch_helper.layers.HiddenStateResetLSTM(input_size=1, hidden_size=32, batch_first=True),
-            pytorch_helper.layers.LSTMLastHiddenState(),
+            pytorch_supporter.layers.HiddenStateResetLSTM(input_size=1, hidden_size=32, batch_first=True),
+            pytorch_supporter.layers.LSTMLastHiddenState(),
             torch.nn.Linear(in_features=32, out_features=config.num_labels)
         )
 
     def forward(self, input_values, labels=None):
         if len(input_values.shape) == 2:
             input_values = input_values.unsqueeze(-1)
         
@@ -42,28 +42,28 @@
 
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForAudioClassification
-import pytorch_helper
+import pytorch_supporter
 import torch
 from torch.nn import functional as F
 import transformers
 from .configuration_rnn import RnnConfig
 
 class RnnForTimeSeriesRegression(PreTrainedModel):
     config_class = RnnConfig
 
     def __init__(self, config):
         super().__init__(config)        
         self.layer = torch.nn.Sequential(
-            pytorch_helper.layers.HiddenStateResetLSTM(input_size=1, hidden_size=32, batch_first=True),
-            pytorch_helper.layers.LSTMLastHiddenState(),
+            pytorch_supporter.layers.HiddenStateResetLSTM(input_size=1, hidden_size=32, batch_first=True),
+            pytorch_supporter.layers.LSTMLastHiddenState(),
             torch.nn.Linear(in_features=32, out_features=32),
             #torch.nn.BatchNorm1d(num_features=32),
             torch.nn.ReLU(),
             torch.nn.Linear(in_features=32, out_features=1)   
         )
 
     def forward(self, input_values, labels=None):
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter/pipelines/__init__.py` & `transformers-supporter-0.0.9/transformers_supporter/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/pipelines/custom_image_classification_pipeline.py` & `transformers-supporter-0.0.9/transformers_supporter/pipelines/custom_image_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/pipelines/fixed_length_translation_pipeline.py` & `transformers-supporter-0.0.9/transformers_supporter/pipelines/fixed_length_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_binary_classification_pipeline.py` & `transformers-supporter-0.0.9/transformers_supporter/pipelines/tabular_binary_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_classification_pipeline.py` & `transformers-supporter-0.0.9/transformers_supporter/pipelines/tabular_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_regression_pipeline.py` & `transformers-supporter-0.0.9/transformers_supporter/pipelines/tabular_regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.8/transformers_supporter.egg-info/PKG-INFO` & `transformers-supporter-0.0.9/transformers_supporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers-supporter
-Version: 0.0.8
+Version: 0.0.9
 Summary: Transformers supporter
 Home-page: https://github.com/automatethem/transformers-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `transformers-supporter-0.0.8/transformers_supporter.egg-info/SOURCES.txt` & `transformers-supporter-0.0.9/transformers_supporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

