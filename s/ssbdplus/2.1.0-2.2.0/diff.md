# Comparing `tmp/ssbdplus-2.1.0.tar.gz` & `tmp/ssbdplus-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssbdplus-2.1.0.tar", last modified: Sat Jun 17 06:18:08 2023, max compression
+gzip compressed data, was "ssbdplus-2.2.0.tar", last modified: Sat Jun 17 06:28:49 2023, max compression
```

## Comparing `ssbdplus-2.1.0.tar` & `ssbdplus-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:18:08.329325 ssbdplus-2.1.0/
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1092 2023-06-17 05:34:23.000000 ssbdplus-2.1.0/LICENSE
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1172 2023-06-17 06:18:08.329325 ssbdplus-2.1.0/PKG-INFO
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      528 2023-06-17 06:11:41.000000 ssbdplus-2.1.0/README.md
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      103 2023-06-17 05:59:22.000000 ssbdplus-2.1.0/pyproject.toml
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      769 2023-06-17 06:18:08.329325 ssbdplus-2.1.0/setup.cfg
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:18:08.325325 ssbdplus-2.1.0/src/
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:18:08.325325 ssbdplus-2.1.0/src/ssbdplus/
--rw-rw-r--   0 vijay     (1000) vijay     (1000)       80 2023-06-17 05:57:00.000000 ssbdplus-2.1.0/src/ssbdplus/__init__.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     3353 2023-06-17 05:34:23.000000 ssbdplus-2.1.0/src/ssbdplus/m1.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     5060 2023-06-17 05:34:23.000000 ssbdplus-2.1.0/src/ssbdplus/m2.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1448 2023-06-17 05:34:23.000000 ssbdplus-2.1.0/src/ssbdplus/pipeline.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     2055 2023-06-17 06:13:24.000000 ssbdplus-2.1.0/src/ssbdplus/prefetch.py
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:18:08.325325 ssbdplus-2.1.0/src/ssbdplus.egg-info/
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1172 2023-06-17 06:18:08.000000 ssbdplus-2.1.0/src/ssbdplus.egg-info/PKG-INFO
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      299 2023-06-17 06:18:08.000000 ssbdplus-2.1.0/src/ssbdplus.egg-info/SOURCES.txt
--rw-rw-r--   0 vijay     (1000) vijay     (1000)        1 2023-06-17 06:18:08.000000 ssbdplus-2.1.0/src/ssbdplus.egg-info/dependency_links.txt
--rw-rw-r--   0 vijay     (1000) vijay     (1000)        9 2023-06-17 06:18:08.000000 ssbdplus-2.1.0/src/ssbdplus.egg-info/top_level.txt
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:28:49.812673 ssbdplus-2.2.0/
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1092 2023-06-17 06:21:23.000000 ssbdplus-2.2.0/LICENSE
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1162 2023-06-17 06:28:49.812673 ssbdplus-2.2.0/PKG-INFO
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      529 2023-06-17 06:27:58.000000 ssbdplus-2.2.0/README.md
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      103 2023-06-17 05:59:22.000000 ssbdplus-2.2.0/pyproject.toml
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      758 2023-06-17 06:28:49.812673 ssbdplus-2.2.0/setup.cfg
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:28:49.808673 ssbdplus-2.2.0/src/
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:28:49.808673 ssbdplus-2.2.0/src/ssbdplus/
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)       80 2023-06-17 05:57:00.000000 ssbdplus-2.2.0/src/ssbdplus/__init__.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     3353 2023-06-17 05:34:23.000000 ssbdplus-2.2.0/src/ssbdplus/m1.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     5060 2023-06-17 05:34:23.000000 ssbdplus-2.2.0/src/ssbdplus/m2.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1448 2023-06-17 05:34:23.000000 ssbdplus-2.2.0/src/ssbdplus/pipeline.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     2055 2023-06-17 06:13:24.000000 ssbdplus-2.2.0/src/ssbdplus/prefetch.py
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:28:49.812673 ssbdplus-2.2.0/src/ssbdplus.egg-info/
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1162 2023-06-17 06:28:49.000000 ssbdplus-2.2.0/src/ssbdplus.egg-info/PKG-INFO
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      299 2023-06-17 06:28:49.000000 ssbdplus-2.2.0/src/ssbdplus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)        1 2023-06-17 06:28:49.000000 ssbdplus-2.2.0/src/ssbdplus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)        9 2023-06-17 06:28:49.000000 ssbdplus-2.2.0/src/ssbdplus.egg-info/top_level.txt
```

### Comparing `ssbdplus-2.1.0/LICENSE` & `ssbdplus-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssbdplus-2.1.0/PKG-INFO` & `ssbdplus-2.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ssbdplus
-Version: 2.1.0
-Summary: Models pertaining to the paper, Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
+Version: 2.2.0
+Summary: Models pertaining to the paper, Introducing SSBD+ Dataset with a Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
 Home-page: https://github.com/sarl-iiitb/ssbd-pipeline
 Author: SARL, IIITB
 Author-email: mr@iiitb.ac.in
 Project-URL: Bug Tracker, https://github.com/sarl-iiitb/ssbd-pipeline/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,14 @@
 
 --- 
 All relevant links can be found here:
 ###  Installation and Usage: [INSTALL.md](./docs/INSTALL.md)
 
 `pip install --upgrade ssbdplus`  
 
-###  Models and their description: [MODELS.md](./docs/MODELS.md) 
+###  Models and their descriptions: [MODELS.md](./docs/MODELS.md) 
 
 ```py
 from ssbdplus.pipeline import SSBDPipeline
 
 model = SSBDPipeline()
 ```
```

### Comparing `ssbdplus-2.1.0/README.md` & `ssbdplus-2.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
 --- 
 All relevant links can be found here:
 ###  Installation and Usage: [INSTALL.md](./docs/INSTALL.md)
 
 `pip install --upgrade ssbdplus`  
 
-###  Models and their description: [MODELS.md](./docs/MODELS.md) 
+###  Models and their descriptions: [MODELS.md](./docs/MODELS.md) 
 
 ```py
 from ssbdplus.pipeline import SSBDPipeline
 
 model = SSBDPipeline()
 ```
```

### Comparing `ssbdplus-2.1.0/setup.cfg` & `ssbdplus-2.2.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = ssbdplus
-version = 2.1.0
+version = 2.2.0
 author = SARL, IIITB
 author_email = mr@iiitb.ac.in
-description = Models pertaining to the paper, Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
+description = Models pertaining to the paper, Introducing SSBD+ Dataset with a Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sarl-iiitb/ssbd-pipeline
 project_urls = 
 	Bug Tracker = https://github.com/sarl-iiitb/ssbd-pipeline/issues
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `ssbdplus-2.1.0/src/ssbdplus/m1.py` & `ssbdplus-2.2.0/src/ssbdplus/m1.py`

 * *Files identical despite different names*

### Comparing `ssbdplus-2.1.0/src/ssbdplus/m2.py` & `ssbdplus-2.2.0/src/ssbdplus/m2.py`

 * *Files identical despite different names*

### Comparing `ssbdplus-2.1.0/src/ssbdplus/pipeline.py` & `ssbdplus-2.2.0/src/ssbdplus/pipeline.py`

 * *Files identical despite different names*

### Comparing `ssbdplus-2.1.0/src/ssbdplus/prefetch.py` & `ssbdplus-2.2.0/src/ssbdplus/prefetch.py`

 * *Files identical despite different names*

### Comparing `ssbdplus-2.1.0/src/ssbdplus.egg-info/PKG-INFO` & `ssbdplus-2.2.0/src/ssbdplus.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ssbdplus
-Version: 2.1.0
-Summary: Models pertaining to the paper, Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
+Version: 2.2.0
+Summary: Models pertaining to the paper, Introducing SSBD+ Dataset with a Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
 Home-page: https://github.com/sarl-iiitb/ssbd-pipeline
 Author: SARL, IIITB
 Author-email: mr@iiitb.ac.in
 Project-URL: Bug Tracker, https://github.com/sarl-iiitb/ssbd-pipeline/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,14 +23,14 @@
 
 --- 
 All relevant links can be found here:
 ###  Installation and Usage: [INSTALL.md](./docs/INSTALL.md)
 
 `pip install --upgrade ssbdplus`  
 
-###  Models and their description: [MODELS.md](./docs/MODELS.md) 
+###  Models and their descriptions: [MODELS.md](./docs/MODELS.md) 
 
 ```py
 from ssbdplus.pipeline import SSBDPipeline
 
 model = SSBDPipeline()
 ```
```

