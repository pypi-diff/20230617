# Comparing `tmp/Algorithm-Selection-0.0.5.tar.gz` & `tmp/Algorithm-Selection-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Algorithm-Selection-0.0.5.tar", last modified: Tue Jun  6 16:24:06 2023, max compression
+gzip compressed data, was "Algorithm-Selection-0.0.7.tar", last modified: Fri Jun 16 23:18:25 2023, max compression
```

## Comparing `Algorithm-Selection-0.0.5.tar` & `Algorithm-Selection-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:24:06.053069 Algorithm-Selection-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-06-06 16:24:06.037094 Algorithm-Selection-0.0.5/Algorithm-Selection/
-drwxrwxrwx   0        0        0        0 2023-06-06 16:24:06.037094 Algorithm-Selection-0.0.5/Algorithm-Selection/metadata/
--rw-rw-rw-   0        0        0   370596 2023-06-01 13:56:52.000000 Algorithm-Selection-0.0.5/Algorithm-Selection/metadata/distance.csv
--rw-rw-rw-   0        0        0    12750 2023-06-03 11:45:32.000000 Algorithm-Selection-0.0.5/Algorithm-Selection/metadata_derivation.py
--rw-rw-rw-   0        0        0     5224 2023-06-06 13:54:45.000000 Algorithm-Selection-0.0.5/Algorithm-Selection/metalearning.py
--rw-rw-rw-   0        0        0    10119 2023-05-22 18:52:33.000000 Algorithm-Selection-0.0.5/Algorithm-Selection/preprocessing.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:24:06.049069 Algorithm-Selection-0.0.5/Algorithm_Selection.egg-info/
--rw-rw-rw-   0        0        0     3434 2023-06-06 16:24:05.000000 Algorithm-Selection-0.0.5/Algorithm_Selection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-06-06 16:24:05.000000 Algorithm-Selection-0.0.5/Algorithm_Selection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:24:05.000000 Algorithm-Selection-0.0.5/Algorithm_Selection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-06-06 16:24:05.000000 Algorithm-Selection-0.0.5/Algorithm_Selection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-06 16:24:05.000000 Algorithm-Selection-0.0.5/Algorithm_Selection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-03-27 19:48:42.000000 Algorithm-Selection-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      157 2023-05-21 19:44:03.000000 Algorithm-Selection-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3434 2023-06-06 16:24:06.049069 Algorithm-Selection-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2769 2023-03-27 19:48:42.000000 Algorithm-Selection-0.0.5/README.md
--rw-rw-rw-   0        0        0      608 2023-06-06 16:23:44.000000 Algorithm-Selection-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 16:24:06.053069 Algorithm-Selection-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      615 2023-06-06 16:20:04.000000 Algorithm-Selection-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:18:25.608399 Algorithm-Selection-0.0.7/
+drwxrwxrwx   0        0        0        0 2023-06-16 23:18:25.592667 Algorithm-Selection-0.0.7/Algorithm-Selection/
+-rw-rw-rw-   0        0        0        0 2023-06-16 23:14:17.000000 Algorithm-Selection-0.0.7/Algorithm-Selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:18:25.592667 Algorithm-Selection-0.0.7/Algorithm-Selection/metadata/
+-rw-rw-rw-   0        0        0   370596 2023-06-01 13:56:52.000000 Algorithm-Selection-0.0.7/Algorithm-Selection/metadata/distance.csv
+-rw-rw-rw-   0        0        0    12750 2023-06-03 11:45:32.000000 Algorithm-Selection-0.0.7/Algorithm-Selection/metadata_derivation.py
+-rw-rw-rw-   0        0        0     5224 2023-06-06 13:54:45.000000 Algorithm-Selection-0.0.7/Algorithm-Selection/metalearning.py
+-rw-rw-rw-   0        0        0    10119 2023-05-22 18:52:33.000000 Algorithm-Selection-0.0.7/Algorithm-Selection/preprocessing.py
+drwxrwxrwx   0        0        0        0 2023-06-16 23:18:25.608399 Algorithm-Selection-0.0.7/Algorithm_Selection.egg-info/
+-rw-rw-rw-   0        0        0      374 2023-06-16 23:18:25.000000 Algorithm-Selection-0.0.7/Algorithm_Selection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-06-16 23:18:25.000000 Algorithm-Selection-0.0.7/Algorithm_Selection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 23:18:25.000000 Algorithm-Selection-0.0.7/Algorithm_Selection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-06-16 23:18:25.000000 Algorithm-Selection-0.0.7/Algorithm_Selection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-16 23:18:25.000000 Algorithm-Selection-0.0.7/Algorithm_Selection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-03-27 19:48:42.000000 Algorithm-Selection-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      157 2023-05-21 19:44:03.000000 Algorithm-Selection-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      374 2023-06-16 23:18:25.608399 Algorithm-Selection-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2769 2023-03-27 19:48:42.000000 Algorithm-Selection-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-16 23:18:25.608399 Algorithm-Selection-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      615 2023-06-16 23:04:41.000000 Algorithm-Selection-0.0.7/setup.py
```

### Comparing `Algorithm-Selection-0.0.5/Algorithm-Selection/metadata/distance.csv` & `Algorithm-Selection-0.0.7/Algorithm-Selection/metadata/distance.csv`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.5/Algorithm-Selection/metadata_derivation.py` & `Algorithm-Selection-0.0.7/Algorithm-Selection/metadata_derivation.py`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.5/Algorithm-Selection/metalearning.py` & `Algorithm-Selection-0.0.7/Algorithm-Selection/metalearning.py`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.5/Algorithm-Selection/preprocessing.py` & `Algorithm-Selection-0.0.7/Algorithm-Selection/preprocessing.py`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.5/Algorithm_Selection.egg-info/PKG-INFO` & `Algorithm-Selection-0.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,30 @@
-Metadata-Version: 2.1
-Name: Algorithm-Selection
-Version: 0.0.5
-Summary: Functions dedicated to The Algoritm Selection problem with a focus on a metalearning approach
-Home-page: https://github.com/Junior-Prado/Algorithm-Selection
-Author: valfridojr
-Author-email: Valfrido da Ponte Prado Junior <juniorprado@alu.ufc.br>
-License: MIT License
-Project-URL: Homepage, https://github.com/Junior-Prado/Algorithm-Selection
-Keywords: metalearning
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ASP
-Functions dedicated to The Algoritm Selection problem with a focus on a metalearning approach
-
-
-On the preprocessing file there are three functions dedicated to prepare datasets to be used in later functions. Being then:
-
-load_database_aff: that as made to load OpenML datasets.
-load_database: that loads a batch of csv files into a list of pandas dataframes.
-preprocess_database: that modify a list of datasets into a format susceptible to extract metafeatures
-
-On the trainingdata file there is a class and two function, dedicated to extracting metafeatures and rankings of datasets. Being then:
-
-Feature_Extractor: function that takes metafeatures based on distance and correlation described in [inset reference]
-Clustering Evaluation: class that compares and rank the results of clustering performed in a dataset according to seven clustering algorithms of sklearn. It's useful on its own independent of other function on this repository
-rank_database: apply the other functions on this file to all datasets in a database and return prediction data that can be used to predict the ranking of unknown datasets. It is very slow but needsto be only used once
-
-Note1: rank database is useful if you have your own database and plans to expand it in the futures. The more coherent a database is the better the results of the predictions will be. For example: if your database is made of health data to predict if a person is susceptible to a hearth attack, the resulting data will be good at prediction exactly that for new datasets. but if you try to use that data to predict the ranking of a car crash dataset, your predictions will be of mark.
-
-Note2: test_data.csv is a precomputed prediction data made with a mix of real datasets that can be used to make your predictions and skip this whole process.
-
-On the metalearnig file there are four function, dedicated to making prediction based on metadata. Being then:
-
-split_test_data: auxiliary function that can split a prediction data into training and testing data.
-NN_weigth: auxiliary function that will use nearest neighbours to compare and metafeatures data of known data sets with a unkown one and make a weight vector based on it
-predicting_rank: will use NN_weigth and prediction data 'X' to predict the ranking of an dataset with metafeatures 'y'
-get_all_predictions: is a function that will split the prediction data n times and make predictions on the ranking of each instance and calculate correlation of each one with its true ranking
-
-Note3: get_all_predictions is useful to test how well your own prediction database is performing and find a good value of the number of neighbours that works for many datasets.
-Note4: all_scores.csv is the result of applying get_all_predictions to test_data.csv
-
+# ASP
+Functions dedicated to The Algoritm Selection problem with a focus on a metalearning approach
+
+
+On the preprocessing file there are three functions dedicated to prepare datasets to be used in later functions. Being then:
+
+load_database_aff: that as made to load OpenML datasets.
+load_database: that loads a batch of csv files into a list of pandas dataframes.
+preprocess_database: that modify a list of datasets into a format susceptible to extract metafeatures
+
+On the trainingdata file there is a class and two function, dedicated to extracting metafeatures and rankings of datasets. Being then:
+
+Feature_Extractor: function that takes metafeatures based on distance and correlation described in [inset reference]
+Clustering Evaluation: class that compares and rank the results of clustering performed in a dataset according to seven clustering algorithms of sklearn. It's useful on its own independent of other function on this repository
+rank_database: apply the other functions on this file to all datasets in a database and return prediction data that can be used to predict the ranking of unknown datasets. It is very slow but needsto be only used once
+
+Note1: rank database is useful if you have your own database and plans to expand it in the futures. The more coherent a database is the better the results of the predictions will be. For example: if your database is made of health data to predict if a person is susceptible to a hearth attack, the resulting data will be good at prediction exactly that for new datasets. but if you try to use that data to predict the ranking of a car crash dataset, your predictions will be of mark.
+
+Note2: test_data.csv is a precomputed prediction data made with a mix of real datasets that can be used to make your predictions and skip this whole process.
+
+On the metalearnig file there are four function, dedicated to making prediction based on metadata. Being then:
+
+split_test_data: auxiliary function that can split a prediction data into training and testing data.
+NN_weigth: auxiliary function that will use nearest neighbours to compare and metafeatures data of known data sets with a unkown one and make a weight vector based on it
+predicting_rank: will use NN_weigth and prediction data 'X' to predict the ranking of an dataset with metafeatures 'y'
+get_all_predictions: is a function that will split the prediction data n times and make predictions on the ranking of each instance and calculate correlation of each one with its true ranking
+
+Note3: get_all_predictions is useful to test how well your own prediction database is performing and find a good value of the number of neighbours that works for many datasets.
+Note4: all_scores.csv is the result of applying get_all_predictions to test_data.csv
+
```

### Comparing `Algorithm-Selection-0.0.5/LICENSE` & `Algorithm-Selection-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Algorithm-Selection-0.0.5/setup.py` & `Algorithm-Selection-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='Algorithm-Selection',
-    version='0.0.5',
+    version='0.0.7',
     license='MIT License',
     author='valfridojr',
     long_description='readme.MD',
     author_email='juniorprado@alu.ufc.br',
     keywords='metalearning',
     description=u'Functions dedicated to The Algoritm Selection problem with a focus on a metalearning approach',
     packages=['Algorithm-Selection'],
```

