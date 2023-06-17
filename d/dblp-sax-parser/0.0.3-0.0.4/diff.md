# Comparing `tmp/dblp_sax_parser-0.0.3.tar.gz` & `tmp/dblp_sax_parser-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblp_sax_parser-0.0.3.tar", last modified: Wed Jun 14 06:43:08 2023, max compression
+gzip compressed data, was "dblp_sax_parser-0.0.4.tar", last modified: Sat Jun 17 11:49:30 2023, max compression
```

## Comparing `dblp_sax_parser-0.0.3.tar` & `dblp_sax_parser-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 leonsun    (501) staff       (20)        0 2023-06-14 06:43:08.158032 dblp_sax_parser-0.0.3/
--rw-r--r--   0 leonsun    (501) staff       (20)     1061 2023-06-06 13:10:43.000000 dblp_sax_parser-0.0.3/LICENSE
--rw-r--r--   0 leonsun    (501) staff       (20)     1684 2023-06-14 06:43:08.157883 dblp_sax_parser-0.0.3/PKG-INFO
--rw-r--r--   0 leonsun    (501) staff       (20)     1136 2023-06-14 04:40:00.000000 dblp_sax_parser-0.0.3/README.md
--rw-r--r--   0 leonsun    (501) staff       (20)      659 2023-06-14 06:41:32.000000 dblp_sax_parser-0.0.3/pyproject.toml
--rw-r--r--   0 leonsun    (501) staff       (20)       38 2023-06-14 06:43:08.158093 dblp_sax_parser-0.0.3/setup.cfg
-drwxr-xr-x   0 leonsun    (501) staff       (20)        0 2023-06-14 06:43:08.156376 dblp_sax_parser-0.0.3/src/
--rw-r--r--   0 leonsun    (501) staff       (20)        0 2023-06-06 11:32:43.000000 dblp_sax_parser-0.0.3/src/__init__.py
--rw-r--r--   0 leonsun    (501) staff       (20)    14802 2023-06-14 06:40:50.000000 dblp_sax_parser-0.0.3/src/dblp_parser.py
-drwxr-xr-x   0 leonsun    (501) staff       (20)        0 2023-06-14 06:43:08.157306 dblp_sax_parser-0.0.3/src/dblp_sax_parser.egg-info/
--rw-r--r--   0 leonsun    (501) staff       (20)     1684 2023-06-14 06:43:08.000000 dblp_sax_parser-0.0.3/src/dblp_sax_parser.egg-info/PKG-INFO
--rw-r--r--   0 leonsun    (501) staff       (20)      264 2023-06-14 06:43:08.000000 dblp_sax_parser-0.0.3/src/dblp_sax_parser.egg-info/SOURCES.txt
--rw-r--r--   0 leonsun    (501) staff       (20)        1 2023-06-14 06:43:08.000000 dblp_sax_parser-0.0.3/src/dblp_sax_parser.egg-info/dependency_links.txt
--rw-r--r--   0 leonsun    (501) staff       (20)       21 2023-06-14 06:43:08.000000 dblp_sax_parser-0.0.3/src/dblp_sax_parser.egg-info/top_level.txt
-drwxr-xr-x   0 leonsun    (501) staff       (20)        0 2023-06-14 06:43:08.157509 dblp_sax_parser-0.0.3/test/
--rw-r--r--   0 leonsun    (501) staff       (20)     2504 2023-06-14 06:39:50.000000 dblp_sax_parser-0.0.3/test/test_dblp_parser.py
+drwxr-xr-x   0 leonsun    (501) staff       (20)        0 2023-06-17 11:49:30.917585 dblp_sax_parser-0.0.4/
+-rw-r--r--   0 leonsun    (501) staff       (20)     1061 2023-06-06 13:10:43.000000 dblp_sax_parser-0.0.4/LICENSE
+-rw-r--r--   0 leonsun    (501) staff       (20)     4823 2023-06-17 11:49:30.917447 dblp_sax_parser-0.0.4/PKG-INFO
+-rw-r--r--   0 leonsun    (501) staff       (20)     4275 2023-06-17 10:39:08.000000 dblp_sax_parser-0.0.4/README.md
+-rw-r--r--   0 leonsun    (501) staff       (20)      714 2023-06-17 11:49:22.000000 dblp_sax_parser-0.0.4/pyproject.toml
+-rw-r--r--   0 leonsun    (501) staff       (20)       38 2023-06-17 11:49:30.917644 dblp_sax_parser-0.0.4/setup.cfg
+drwxr-xr-x   0 leonsun    (501) staff       (20)        0 2023-06-17 11:49:30.916097 dblp_sax_parser-0.0.4/src/
+-rw-r--r--   0 leonsun    (501) staff       (20)        0 2023-06-06 11:32:43.000000 dblp_sax_parser-0.0.4/src/__init__.py
+-rw-r--r--   0 leonsun    (501) staff       (20)    14802 2023-06-14 06:40:50.000000 dblp_sax_parser-0.0.4/src/dblp_parser.py
+drwxr-xr-x   0 leonsun    (501) staff       (20)        0 2023-06-17 11:49:30.916912 dblp_sax_parser-0.0.4/src/dblp_sax_parser.egg-info/
+-rw-r--r--   0 leonsun    (501) staff       (20)     4823 2023-06-17 11:49:30.000000 dblp_sax_parser-0.0.4/src/dblp_sax_parser.egg-info/PKG-INFO
+-rw-r--r--   0 leonsun    (501) staff       (20)      306 2023-06-17 11:49:30.000000 dblp_sax_parser-0.0.4/src/dblp_sax_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 leonsun    (501) staff       (20)        1 2023-06-17 11:49:30.000000 dblp_sax_parser-0.0.4/src/dblp_sax_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 leonsun    (501) staff       (20)       44 2023-06-17 11:49:30.000000 dblp_sax_parser-0.0.4/src/dblp_sax_parser.egg-info/requires.txt
+-rw-r--r--   0 leonsun    (501) staff       (20)       21 2023-06-17 11:49:30.000000 dblp_sax_parser-0.0.4/src/dblp_sax_parser.egg-info/top_level.txt
+drwxr-xr-x   0 leonsun    (501) staff       (20)        0 2023-06-17 11:49:30.917070 dblp_sax_parser-0.0.4/test/
+-rw-r--r--   0 leonsun    (501) staff       (20)     2504 2023-06-14 06:39:50.000000 dblp_sax_parser-0.0.4/test/test_dblp_parser.py
```

### Comparing `dblp_sax_parser-0.0.3/LICENSE` & `dblp_sax_parser-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dblp_sax_parser-0.0.3/pyproject.toml` & `dblp_sax_parser-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 [build-system]
-requires = ["setuptools>=65.3","pandas>=2.0.2","hurry.filesize>=0.9"]
+requires = [
+  "setuptools>=65.3"
+  ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dblp_sax_parser"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Leon", email="leonsunwl@gmail.com" },
 ]
 description = "A parsing package for dblp using the Simple API for XML (SAX)"
 readme = "README.md"
 requires-python = ">=3.11.3"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "requests",
+    "pandas >= 2.0.2",
+    "hurry.filesize >= 0.09"
+]
 
 [project.urls]
 "Homepage" = "https://github.com/leonswl/dblp-sax-parser"
 "Bug Tracker" = "https://github.com/leonswl/dblp-sax-parser/issues"
```

### Comparing `dblp_sax_parser-0.0.3/src/dblp_parser.py` & `dblp_sax_parser-0.0.4/src/dblp_parser.py`

 * *Files identical despite different names*

### Comparing `dblp_sax_parser-0.0.3/test/test_dblp_parser.py` & `dblp_sax_parser-0.0.4/test/test_dblp_parser.py`

 * *Files identical despite different names*

