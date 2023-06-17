# Comparing `tmp/ssbdplus-1.0.0.tar.gz` & `tmp/ssbdplus-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssbdplus-1.0.0.tar", last modified: Thu Feb  9 05:30:24 2023, max compression
+gzip compressed data, was "ssbdplus-2.0.0.tar", last modified: Sat Jun 17 06:01:01 2023, max compression
```

## Comparing `ssbdplus-1.0.0.tar` & `ssbdplus-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-02-09 05:30:24.204589 ssbdplus-1.0.0/
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1092 2023-02-08 09:18:19.000000 ssbdplus-1.0.0/LICENSE
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1066 2023-02-09 05:30:24.204589 ssbdplus-1.0.0/PKG-INFO
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      421 2023-02-09 05:27:04.000000 ssbdplus-1.0.0/README.md
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      103 2023-02-09 04:43:28.000000 ssbdplus-1.0.0/pyproject.toml
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      769 2023-02-09 05:30:24.208589 ssbdplus-1.0.0/setup.cfg
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-02-09 05:30:24.204589 ssbdplus-1.0.0/src/
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-02-09 05:30:24.204589 ssbdplus-1.0.0/src/ssbdplus/
--rw-rw-r--   0 vijay     (1000) vijay     (1000)       56 2023-02-09 05:28:30.000000 ssbdplus-1.0.0/src/ssbdplus/__init__.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     3353 2023-02-09 05:29:01.000000 ssbdplus-1.0.0/src/ssbdplus/m1.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     5060 2023-02-09 05:29:01.000000 ssbdplus-1.0.0/src/ssbdplus/m2.py
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1448 2023-02-09 05:29:01.000000 ssbdplus-1.0.0/src/ssbdplus/pipeline.py
-drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-02-09 05:30:24.204589 ssbdplus-1.0.0/src/ssbdplus.egg-info/
--rw-rw-r--   0 vijay     (1000) vijay     (1000)     1066 2023-02-09 05:30:24.000000 ssbdplus-1.0.0/src/ssbdplus.egg-info/PKG-INFO
--rw-rw-r--   0 vijay     (1000) vijay     (1000)      274 2023-02-09 05:30:24.000000 ssbdplus-1.0.0/src/ssbdplus.egg-info/SOURCES.txt
--rw-rw-r--   0 vijay     (1000) vijay     (1000)        1 2023-02-09 05:30:24.000000 ssbdplus-1.0.0/src/ssbdplus.egg-info/dependency_links.txt
--rw-rw-r--   0 vijay     (1000) vijay     (1000)        9 2023-02-09 05:30:24.000000 ssbdplus-1.0.0/src/ssbdplus.egg-info/top_level.txt
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:01:01.554729 ssbdplus-2.0.0/
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1092 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/LICENSE
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1183 2023-06-17 06:01:01.554729 ssbdplus-2.0.0/PKG-INFO
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      539 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/README.md
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      103 2023-06-17 05:59:22.000000 ssbdplus-2.0.0/pyproject.toml
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      769 2023-06-17 06:01:01.558730 ssbdplus-2.0.0/setup.cfg
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:01:01.426728 ssbdplus-2.0.0/src/
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:01:01.554729 ssbdplus-2.0.0/src/ssbdplus/
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)       80 2023-06-17 05:57:00.000000 ssbdplus-2.0.0/src/ssbdplus/__init__.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     3353 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/src/ssbdplus/m1.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     5060 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/src/ssbdplus/m2.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1448 2023-06-17 05:34:23.000000 ssbdplus-2.0.0/src/ssbdplus/pipeline.py
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1962 2023-06-17 05:58:11.000000 ssbdplus-2.0.0/src/ssbdplus/prefetch.py
+drwxrwxr-x   0 vijay     (1000) vijay     (1000)        0 2023-06-17 06:01:01.554729 ssbdplus-2.0.0/src/ssbdplus.egg-info/
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)     1183 2023-06-17 06:01:01.000000 ssbdplus-2.0.0/src/ssbdplus.egg-info/PKG-INFO
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)      299 2023-06-17 06:01:01.000000 ssbdplus-2.0.0/src/ssbdplus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)        1 2023-06-17 06:01:01.000000 ssbdplus-2.0.0/src/ssbdplus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vijay     (1000) vijay     (1000)        9 2023-06-17 06:01:01.000000 ssbdplus-2.0.0/src/ssbdplus.egg-info/top_level.txt
```

### Comparing `ssbdplus-1.0.0/LICENSE` & `ssbdplus-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssbdplus-1.0.0/setup.cfg` & `ssbdplus-2.0.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ssbdplus
-version = 1.0.0
+version = 2.0.0
 author = SARL, IIITB
 author_email = mr@iiitb.ac.in
 description = Models pertaining to the paper, Introducing SSBD+ Dataset with an Attentive Convolutional Pipeline for detecting Self-Stimulatory Behaviours in Children using raw videos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sarl-iiitb/ssbd-pipeline
 project_urls =
```

### Comparing `ssbdplus-1.0.0/src/ssbdplus/m1.py` & `ssbdplus-2.0.0/src/ssbdplus/m1.py`

 * *Files identical despite different names*

### Comparing `ssbdplus-1.0.0/src/ssbdplus/m2.py` & `ssbdplus-2.0.0/src/ssbdplus/m2.py`

 * *Files identical despite different names*

### Comparing `ssbdplus-1.0.0/src/ssbdplus/pipeline.py` & `ssbdplus-2.0.0/src/ssbdplus/pipeline.py`

 * *Files identical despite different names*

