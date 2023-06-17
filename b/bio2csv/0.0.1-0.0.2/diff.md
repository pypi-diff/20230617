# Comparing `tmp/bio2csv-0.0.1.tar.gz` & `tmp/bio2csv-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio2csv-0.0.1.tar", last modified: Sat Jun 17 10:34:51 2023, max compression
+gzip compressed data, was "bio2csv-0.0.2.tar", last modified: Sat Jun 17 11:26:17 2023, max compression
```

## Comparing `bio2csv-0.0.1.tar` & `bio2csv-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 10:34:51.031059 bio2csv-0.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-06-17 10:28:42.000000 bio2csv-0.0.1/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2065 2023-06-17 10:34:51.031059 bio2csv-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1620 2023-06-17 10:34:46.000000 bio2csv-0.0.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 10:34:51.027059 bio2csv-0.0.1/bio2csv/
--rw-r--r--   0 runner    (1000) runner    (1000)     3114 2023-06-17 10:32:59.000000 bio2csv-0.0.1/bio2csv/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 10:34:51.031059 bio2csv-0.0.1/bio2csv.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2065 2023-06-17 10:34:50.000000 bio2csv-0.0.1/bio2csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      185 2023-06-17 10:34:50.000000 bio2csv-0.0.1/bio2csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-17 10:34:50.000000 bio2csv-0.0.1/bio2csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-17 10:34:50.000000 bio2csv-0.0.1/bio2csv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 bio2csv-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-17 10:34:51.031059 bio2csv-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      700 2023-06-17 10:31:20.000000 bio2csv-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 11:26:17.432229 bio2csv-0.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-06-17 10:28:42.000000 bio2csv-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     5767 2023-06-17 11:26:17.432229 bio2csv-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     5328 2023-06-17 11:25:13.000000 bio2csv-0.0.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 11:26:17.432229 bio2csv-0.0.2/bio2csv/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3336 2023-06-17 11:16:17.000000 bio2csv-0.0.2/bio2csv/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 11:26:17.432229 bio2csv-0.0.2/bio2csv.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5767 2023-06-17 11:26:17.000000 bio2csv-0.0.2/bio2csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      185 2023-06-17 11:26:17.000000 bio2csv-0.0.2/bio2csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-17 11:26:17.000000 bio2csv-0.0.2/bio2csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-17 11:26:17.000000 bio2csv-0.0.2/bio2csv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 bio2csv-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-17 11:26:17.432229 bio2csv-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      694 2023-06-17 11:25:52.000000 bio2csv-0.0.2/setup.py
```

### Comparing `bio2csv-0.0.1/LICENSE` & `bio2csv-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bio2csv-0.0.1/setup.py` & `bio2csv-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="bio2csv",
-    version="0.0.1",
+    version="0.0.2",
     author="Andrew Gao",
     author_email="gaodrew@stanford.edu",
-    description="the easiest way to download many articles from biorxiv",
+    description="the easiest way to scrape preprints from biorxiv",
     long_description=long_description, # don't touch this, this is your README.md
     long_description_content_type="text/markdown",
     url="https://github.com/andrewgcodes",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

