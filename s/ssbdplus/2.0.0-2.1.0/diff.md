# Comparing `tmp/ssbdplus-2.0.0.tar.gz` & `tmp/ssbdplus-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssbdplus-2.0.0.tar", last modified: Sat Jun 17 06:01:01 2023, max compression
+gzip compressed data, was "ssbdplus-2.1.0.tar", last modified: Sat Jun 17 06:18:08 2023, max compression
```

## Comparing `ssbdplus-2.0.0.tar` & `ssbdplus-2.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:01:01.554729 ssbdplus-2.0.0/
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1092 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/LICENSE
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1183 2023-06-17 06:01:01.554729 ssbdplus-2.0.0/PKG-INFO
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      539 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/README.md
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      103 2023-06-17 05:59:22.000000 ssbdplus-2.0.0/pyproject.toml
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      769 2023-06-17 06:01:01.558730 ssbdplus-2.0.0/setup.cfg
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:01:01.426728 ssbdplus-2.0.0/src/
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:01:01.554729 ssbdplus-2.0.0/src/ssbdplus/
--rw-rw-r--   0 vijay     (1000) vijay     (1000)       80 2023-06-17 05:57:00.000000 ssbdplus-2.0.0/src/ssbdplus/__init__.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     3353 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/src/ssbdplus/m1.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     5060 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/src/ssbdplus/m2.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1448 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/src/ssbdplus/pipeline.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1962 2023-06-17 05:58:11.000000 ssbdplus-2.0.0/src/ssbdplus/prefetch.py
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:01:01.554729 ssbdplus-2.0.0/src/ssbdplus.egg-info/
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1183 2023-06-17 06:01:01.000000 ssbdplus-2.0.0/src/ssbdplus.egg-info/PKG-INFO
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      299 2023-06-17 06:01:01.000000 ssbdplus-2.0.0/src/ssbdplus.egg-info/SOURCES.txt
--rw-rw-r--   0 vijay     (1000) vijay     (1000)        1 2023-06-17 06:01:01.000000 ssbdplus-2.0.0/src/ssbdplus.egg-info/dependency_links.txt
--rw-rw-r--   0 vijay     (1000) vijay     (1000)        9 2023-06-17 06:01:01.000000 ssbdplus-2.0.0/src/ssbdplus.egg-info/top_level.txt
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:18:08.329325 ssbdplus-2.1.0/
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1092 2023-06-17 05:34:23.000000 ssbdplus-2.1.0/LICENSE
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1172 2023-06-17 06:18:08.329325 ssbdplus-2.1.0/PKG-INFO
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      528 2023-06-17 06:11:41.000000 ssbdplus-2.1.0/README.md
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      103 2023-06-17 05:59:22.000000 ssbdplus-2.1.0/pyproject.toml
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      769 2023-06-17 06:18:08.329325 ssbdplus-2.1.0/setup.cfg
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:18:08.325325 ssbdplus-2.1.0/src/
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:18:08.325325 ssbdplus-2.1.0/src/ssbdplus/
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)       80 2023-06-17 05:57:00.000000 ssbdplus-2.1.0/src/ssbdplus/__init__.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     3353 2023-06-17 05:34:23.000000 ssbdplus-2.1.0/src/ssbdplus/m1.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     5060 2023-06-17 05:34:23.000000 ssbdplus-2.1.0/src/ssbdplus/m2.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1448 2023-06-17 05:34:23.000000 ssbdplus-2.1.0/src/ssbdplus/pipeline.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     2055 2023-06-17 06:13:24.000000 ssbdplus-2.1.0/src/ssbdplus/prefetch.py
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:18:08.325325 ssbdplus-2.1.0/src/ssbdplus.egg-info/
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1172 2023-06-17 06:18:08.000000 ssbdplus-2.1.0/src/ssbdplus.egg-info/PKG-INFO
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      299 2023-06-17 06:18:08.000000 ssbdplus-2.1.0/src/ssbdplus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)        1 2023-06-17 06:18:08.000000 ssbdplus-2.1.0/src/ssbdplus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)        9 2023-06-17 06:18:08.000000 ssbdplus-2.1.0/src/ssbdplus.egg-info/top_level.txt
```

### Comparing `ssbdplus-2.0.0/LICENSE` & `ssbdplus-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssbdplus-2.0.0/PKG-INFO` & `ssbdplus-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ssbdplus
-Version: 2.0.0
+Version: 2.1.0
 Summary: Models pertaining to the paper, Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
 Home-page: https://github.com/sarl-iiitb/ssbd-pipeline
 Author: SARL, IIITB
 Author-email: mr@iiitb.ac.in
 Project-URL: Bug Tracker, https://github.com/sarl-iiitb/ssbd-pipeline/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SSBD+
-Code and material relevant to the paper, "Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos"  
+Code and material relevant to the paper, "Introducing SSBD+ Dataset with a Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos"  
 
 
 ![Pipelined Architecture](./docs/images/SSBDPipeline.png)
 
 
 
 ---
```

### Comparing `ssbdplus-2.0.0/README.md` & `ssbdplus-2.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SSBD+
-Code and material relevant to the paper, "Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos"  
+Code and material relevant to the paper, "Introducing SSBD+ Dataset with a Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos"  
 
 
 ![Pipelined Architecture](./docs/images/SSBDPipeline.png)
 
 
 
 ---
```

### Comparing `ssbdplus-2.0.0/setup.cfg` & `ssbdplus-2.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ssbdplus
-version = 2.0.0
+version = 2.1.0
 author = SARL, IIITB
 author_email = mr@iiitb.ac.in
 description = Models pertaining to the paper, Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sarl-iiitb/ssbd-pipeline
 project_urls =
```

### Comparing `ssbdplus-2.0.0/src/ssbdplus/m1.py` & `ssbdplus-2.1.0/src/ssbdplus/m1.py`

 * *Files identical despite different names*

### Comparing `ssbdplus-2.0.0/src/ssbdplus/m2.py` & `ssbdplus-2.1.0/src/ssbdplus/m2.py`

 * *Files identical despite different names*

### Comparing `ssbdplus-2.0.0/src/ssbdplus/pipeline.py` & `ssbdplus-2.1.0/src/ssbdplus/pipeline.py`

 * *Files identical despite different names*

### Comparing `ssbdplus-2.0.0/src/ssbdplus/prefetch.py` & `ssbdplus-2.1.0/src/ssbdplus/prefetch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import torch.nn as nn
 import torch
 import torchvision.models as models
 import torch.nn.functional as F
 
 """
-    @class Prefetch used to classify YOLO bounding boxes as adults or children
-           This model was used as a part of preprocessing.
+    @class Prefetch
+        Used to classify YOLO bounding boxes as adults or children
+        This model was used as a part of preprocessing.
+        @component VGG-19 base CNN model
+        @component Fully-connected NN
+        
         @param dropout_rate: The dropout rate used by the model
             @default 0.40
         @param dim_fc_layer_1: The dimension of the first hidden layer
             @default 256
         @param dim_fc_layer_2: The dimension of the second hidden layer
             @default 64
 """
```

### Comparing `ssbdplus-2.0.0/src/ssbdplus.egg-info/PKG-INFO` & `ssbdplus-2.1.0/src/ssbdplus.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ssbdplus
-Version: 2.0.0
+Version: 2.1.0
 Summary: Models pertaining to the paper, Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
 Home-page: https://github.com/sarl-iiitb/ssbd-pipeline
 Author: SARL, IIITB
 Author-email: mr@iiitb.ac.in
 Project-URL: Bug Tracker, https://github.com/sarl-iiitb/ssbd-pipeline/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SSBD+
-Code and material relevant to the paper, "Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos"  
+Code and material relevant to the paper, "Introducing SSBD+ Dataset with a Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos"  
 
 
 ![Pipelined Architecture](./docs/images/SSBDPipeline.png)
 
 
 
 ---
```

