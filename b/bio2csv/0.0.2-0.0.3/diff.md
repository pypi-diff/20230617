# Comparing `tmp/bio2csv-0.0.2.tar.gz` & `tmp/bio2csv-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio2csv-0.0.2.tar", last modified: Sat Jun 17 11:26:17 2023, max compression
+gzip compressed data, was "bio2csv-0.0.3.tar", last modified: Sat Jun 17 11:39:27 2023, max compression
```

## Comparing `bio2csv-0.0.2.tar` & `bio2csv-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 11:26:17.432229 bio2csv-0.0.2/
--rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-06-17 10:28:42.000000 bio2csv-0.0.2/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     5767 2023-06-17 11:26:17.432229 bio2csv-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     5328 2023-06-17 11:25:13.000000 bio2csv-0.0.2/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 11:26:17.432229 bio2csv-0.0.2/bio2csv/
--rw-r--r--   0 runner    (1000) runner    (1000)     3336 2023-06-17 11:16:17.000000 bio2csv-0.0.2/bio2csv/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 11:26:17.432229 bio2csv-0.0.2/bio2csv.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     5767 2023-06-17 11:26:17.000000 bio2csv-0.0.2/bio2csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      185 2023-06-17 11:26:17.000000 bio2csv-0.0.2/bio2csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-17 11:26:17.000000 bio2csv-0.0.2/bio2csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-17 11:26:17.000000 bio2csv-0.0.2/bio2csv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 bio2csv-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-17 11:26:17.432229 bio2csv-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      694 2023-06-17 11:25:52.000000 bio2csv-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 11:39:27.199505 bio2csv-0.0.3/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1069 2023-06-17 10:28:42.000000 bio2csv-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     5978 2023-06-17 11:39:27.195505 bio2csv-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     5539 2023-06-17 11:38:42.000000 bio2csv-0.0.3/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 11:39:27.195505 bio2csv-0.0.3/bio2csv/
+-rw-r--r--   0 runner    (1000) runner    (1000)     3336 2023-06-17 11:16:17.000000 bio2csv-0.0.3/bio2csv/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-17 11:39:27.195505 bio2csv-0.0.3/bio2csv.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     5978 2023-06-17 11:39:27.000000 bio2csv-0.0.3/bio2csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      185 2023-06-17 11:39:27.000000 bio2csv-0.0.3/bio2csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-17 11:39:27.000000 bio2csv-0.0.3/bio2csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-06-17 11:39:27.000000 bio2csv-0.0.3/bio2csv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      473 2023-01-20 17:56:39.000000 bio2csv-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-17 11:39:27.199505 bio2csv-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      694 2023-06-17 11:39:19.000000 bio2csv-0.0.3/setup.py
```

### Comparing `bio2csv-0.0.2/LICENSE` & `bio2csv-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bio2csv-0.0.2/PKG-INFO` & `bio2csv-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio2csv
-Version: 0.0.2
+Version: 0.0.3
 Summary: the easiest way to scrape preprints from biorxiv
 Home-page: https://github.com/andrewgcodes
 Author: Andrew Gao
 Author-email: gaodrew@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,18 @@
 License-File: LICENSE
 
 # bio2csv 🐧
 
 `bio2csv` is a Python package that allows you to easily scrape all research papers that match a search query (such as [penguins](https://www.biorxiv.org/search/penguin)) on BioRxiv. It retrieves metadata (title, authors, link to each paper), and it can also fetch the abstract and the full text if specified.
 You can also scrape all research papers that fall under a specific Biorxiv subject area, such as Genetics or Paleontology. To encourage responsible use of biorxiv, short random delays are implemented into the code to prevent overload/spam.
 
+<a target="_blank" href="https://colab.research.google.com/github/andrewgcodes/bio2csv/blob/main/bio2csv.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.png" alt="Open In Colab"/>
+</a>
+
 ##  Easy Installation
 
 You can install the `bio2csv` [package](https://pypi.org/project/bio2csv/) with pip:
 
 ```bash
 pip install bio2csv
 ```
```

### Comparing `bio2csv-0.0.2/README.md` & `bio2csv-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # bio2csv 🐧
 
 `bio2csv` is a Python package that allows you to easily scrape all research papers that match a search query (such as [penguins](https://www.biorxiv.org/search/penguin)) on BioRxiv. It retrieves metadata (title, authors, link to each paper), and it can also fetch the abstract and the full text if specified.
 You can also scrape all research papers that fall under a specific Biorxiv subject area, such as Genetics or Paleontology. To encourage responsible use of biorxiv, short random delays are implemented into the code to prevent overload/spam.
 
+<a target="_blank" href="https://colab.research.google.com/github/andrewgcodes/bio2csv/blob/main/bio2csv.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.png" alt="Open In Colab"/>
+</a>
+
 ##  Easy Installation
 
 You can install the `bio2csv` [package](https://pypi.org/project/bio2csv/) with pip:
 
 ```bash
 pip install bio2csv
 ```
```

### Comparing `bio2csv-0.0.2/bio2csv/__init__.py` & `bio2csv-0.0.3/bio2csv/__init__.py`

 * *Files identical despite different names*

### Comparing `bio2csv-0.0.2/bio2csv.egg-info/PKG-INFO` & `bio2csv-0.0.3/bio2csv.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio2csv
-Version: 0.0.2
+Version: 0.0.3
 Summary: the easiest way to scrape preprints from biorxiv
 Home-page: https://github.com/andrewgcodes
 Author: Andrew Gao
 Author-email: gaodrew@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,18 @@
 License-File: LICENSE
 
 # bio2csv 🐧
 
 `bio2csv` is a Python package that allows you to easily scrape all research papers that match a search query (such as [penguins](https://www.biorxiv.org/search/penguin)) on BioRxiv. It retrieves metadata (title, authors, link to each paper), and it can also fetch the abstract and the full text if specified.
 You can also scrape all research papers that fall under a specific Biorxiv subject area, such as Genetics or Paleontology. To encourage responsible use of biorxiv, short random delays are implemented into the code to prevent overload/spam.
 
+<a target="_blank" href="https://colab.research.google.com/github/andrewgcodes/bio2csv/blob/main/bio2csv.ipynb">
+  <img src="https://colab.research.google.com/assets/colab-badge.png" alt="Open In Colab"/>
+</a>
+
 ##  Easy Installation
 
 You can install the `bio2csv` [package](https://pypi.org/project/bio2csv/) with pip:
 
 ```bash
 pip install bio2csv
 ```
```

### Comparing `bio2csv-0.0.2/setup.py` & `bio2csv-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="bio2csv",
-    version="0.0.2",
+    version="0.0.3",
     author="Andrew Gao",
     author_email="gaodrew@stanford.edu",
     description="the easiest way to scrape preprints from biorxiv",
     long_description=long_description, # don't touch this, this is your README.md
     long_description_content_type="text/markdown",
     url="https://github.com/andrewgcodes",
     packages=setuptools.find_packages(),
```

