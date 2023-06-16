# Comparing `tmp/Algorithm-Selection-0.0.8.tar.gz` & `tmp/Algorithm-Selection-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Algorithm-Selection-0.0.8.tar", last modified: Fri Jun 16 23:28:57 2023, max compression
+gzip compressed data, was "Algorithm-Selection-0.0.9.tar", last modified: Fri Jun 16 23:32:21 2023, max compression
```

## Comparing `Algorithm-Selection-0.0.8.tar` & `Algorithm-Selection-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:57.361279 Algorithm-Selection-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:57.351074 Algorithm-Selection-0.0.8/Algorithm-Selection/
--rw-rw-rw-   0        0        0        0 2023-06-16 23:14:17.000000 Algorithm-Selection-0.0.8/Algorithm-Selection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:57.351074 Algorithm-Selection-0.0.8/Algorithm-Selection/metadata/
--rw-rw-rw-   0        0        0   370596 2023-06-01 13:56:52.000000 Algorithm-Selection-0.0.8/Algorithm-Selection/metadata/distance.csv
--rw-rw-rw-   0        0        0    12750 2023-06-03 11:45:32.000000 Algorithm-Selection-0.0.8/Algorithm-Selection/metadata_derivation.py
--rw-rw-rw-   0        0        0     5224 2023-06-06 13:54:45.000000 Algorithm-Selection-0.0.8/Algorithm-Selection/metalearning.py
--rw-rw-rw-   0        0        0    10119 2023-05-22 18:52:33.000000 Algorithm-Selection-0.0.8/Algorithm-Selection/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:57.361279 Algorithm-Selection-0.0.8/Algorithm_Selection.egg-info/
--rw-rw-rw-   0        0        0      374 2023-06-16 23:28:57.000000 Algorithm-Selection-0.0.8/Algorithm_Selection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-06-16 23:28:57.000000 Algorithm-Selection-0.0.8/Algorithm_Selection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 23:28:57.000000 Algorithm-Selection-0.0.8/Algorithm_Selection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-16 23:28:57.000000 Algorithm-Selection-0.0.8/Algorithm_Selection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-16 23:28:57.000000 Algorithm-Selection-0.0.8/Algorithm_Selection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-03-27 19:48:42.000000 Algorithm-Selection-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      157 2023-05-21 19:44:03.000000 Algorithm-Selection-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      374 2023-06-16 23:28:57.361279 Algorithm-Selection-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2769 2023-03-27 19:48:42.000000 Algorithm-Selection-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-06-16 23:28:57.361279 Algorithm-Selection-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      615 2023-06-16 23:28:38.000000 Algorithm-Selection-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:32:21.814706 Algorithm-Selection-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-06-16 23:32:21.789919 Algorithm-Selection-0.0.9/Algorithm-Selection/
+-rw-rw-rw-   0        0        0        0 2023-06-16 23:14:17.000000 Algorithm-Selection-0.0.9/Algorithm-Selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:32:21.789919 Algorithm-Selection-0.0.9/Algorithm-Selection/metadata/
+-rw-rw-rw-   0        0        0   370596 2023-06-01 13:56:52.000000 Algorithm-Selection-0.0.9/Algorithm-Selection/metadata/distance.csv
+-rw-rw-rw-   0        0        0    12750 2023-06-03 11:45:32.000000 Algorithm-Selection-0.0.9/Algorithm-Selection/metadata_derivation.py
+-rw-rw-rw-   0        0        0     5224 2023-06-06 13:54:45.000000 Algorithm-Selection-0.0.9/Algorithm-Selection/metalearning.py
+-rw-rw-rw-   0        0        0    10119 2023-05-22 18:52:33.000000 Algorithm-Selection-0.0.9/Algorithm-Selection/preprocessing.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:32:21.805921 Algorithm-Selection-0.0.9/Algorithm_Selection.egg-info/
+-rw-rw-rw-   0        0        0      374 2023-06-16 23:32:21.000000 Algorithm-Selection-0.0.9/Algorithm_Selection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-06-16 23:32:21.000000 Algorithm-Selection-0.0.9/Algorithm_Selection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 23:32:21.000000 Algorithm-Selection-0.0.9/Algorithm_Selection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-16 23:32:21.000000 Algorithm-Selection-0.0.9/Algorithm_Selection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-16 23:32:21.000000 Algorithm-Selection-0.0.9/Algorithm_Selection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-03-27 19:48:42.000000 Algorithm-Selection-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      157 2023-05-21 19:44:03.000000 Algorithm-Selection-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      374 2023-06-16 23:32:21.814706 Algorithm-Selection-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2769 2023-03-27 19:48:42.000000 Algorithm-Selection-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 23:32:21.814706 Algorithm-Selection-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      620 2023-06-16 23:31:50.000000 Algorithm-Selection-0.0.9/setup.py
```

### Comparing `Algorithm-Selection-0.0.8/Algorithm-Selection/metadata/distance.csv` & `Algorithm-Selection-0.0.9/Algorithm-Selection/metadata/distance.csv`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.8/Algorithm-Selection/metadata_derivation.py` & `Algorithm-Selection-0.0.9/Algorithm-Selection/metadata_derivation.py`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.8/Algorithm-Selection/metalearning.py` & `Algorithm-Selection-0.0.9/Algorithm-Selection/metalearning.py`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.8/Algorithm-Selection/preprocessing.py` & `Algorithm-Selection-0.0.9/Algorithm-Selection/preprocessing.py`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.8/LICENSE` & `Algorithm-Selection-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.8/README.md` & `Algorithm-Selection-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.8/setup.py` & `Algorithm-Selection-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='Algorithm-Selection',
-    version='0.0.8',
+    version='0.0.9',
     license='MIT License',
     author='valfridojr',
     long_description='readme.MD',
     author_email='juniorprado@alu.ufc.br',
     keywords='metalearning',
     description=u'Functions dedicated to The Algoritm Selection problem with a focus on a metalearning approach',
     packages=['Algorithm-Selection'],
-    install_requires=['requests','numpy','pandas','sklearn','scipy', 'os'],
+    install_requires=['requests','numpy','pandas','scikit-learn','scipy', 'os'],
     url = 'https://github.com/Junior-Prado/Algorithm-Selection'
 )
```

