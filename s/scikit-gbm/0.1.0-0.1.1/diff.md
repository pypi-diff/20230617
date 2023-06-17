# Comparing `tmp/scikit-gbm-0.1.0.tar.gz` & `tmp/scikit-gbm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-gbm-0.1.0.tar", last modified: Sun Jun 11 19:44:06 2023, max compression
+gzip compressed data, was "scikit-gbm-0.1.1.tar", last modified: Sat Jun 17 20:01:29 2023, max compression
```

## Comparing `scikit-gbm-0.1.0.tar` & `scikit-gbm-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-11 19:44:06.880912 scikit-gbm-0.1.0/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1077 2023-04-15 14:39:04.000000 scikit-gbm-0.1.0/LICENSE
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2295 2023-06-11 19:44:06.880912 scikit-gbm-0.1.0/PKG-INFO
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1747 2023-06-10 20:23:41.000000 scikit-gbm-0.1.0/README.md
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      720 2023-06-11 19:42:50.000000 scikit-gbm-0.1.0/pyproject.toml
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       75 2023-06-10 23:00:01.000000 scikit-gbm-0.1.0/requirements.txt
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-11 19:44:06.852914 scikit-gbm-0.1.0/scikit_gbm.egg-info/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2295 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/PKG-INFO
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      387 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/SOURCES.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        1 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/dependency_links.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       75 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/requires.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        6 2023-06-11 19:44:06.000000 scikit-gbm-0.1.0/scikit_gbm.egg-info/top_level.txt
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       38 2023-06-11 19:44:06.880912 scikit-gbm-0.1.0/setup.cfg
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-11 19:44:06.864913 scikit-gbm-0.1.0/skgbm/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       48 2023-06-09 20:23:00.000000 scikit-gbm-0.1.0/skgbm/__init__.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     4073 2023-06-10 20:23:41.000000 scikit-gbm-0.1.0/skgbm/base.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1787 2023-06-09 20:23:00.000000 scikit-gbm-0.1.0/skgbm/preprocessing.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     3664 2023-06-10 19:49:26.000000 scikit-gbm-0.1.0/skgbm/tools.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     5348 2023-06-09 20:23:00.000000 scikit-gbm-0.1.0/skgbm/tree.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     7896 2023-06-10 23:04:56.000000 scikit-gbm-0.1.0/skgbm/trees_extraction.py
-drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-11 19:44:06.880912 scikit-gbm-0.1.0/tests/
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2587 2023-04-15 16:16:57.000000 scikit-gbm-0.1.0/tests/test_gbm_wrapper.py
--rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1574 2023-06-09 20:23:00.000000 scikit-gbm-0.1.0/tests/test_trees_to_dataframe.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.534784 scikit-gbm-0.1.1/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1077 2023-04-15 14:39:04.000000 scikit-gbm-0.1.1/LICENSE
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2141 2023-06-17 20:01:29.534784 scikit-gbm-0.1.1/PKG-INFO
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1594 2023-06-16 22:11:35.000000 scikit-gbm-0.1.1/README.md
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      720 2023-06-17 20:00:24.000000 scikit-gbm-0.1.1/pyproject.toml
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       97 2023-06-16 21:48:45.000000 scikit-gbm-0.1.1/requirements.txt
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.502785 scikit-gbm-0.1.1/scikit_gbm.egg-info/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2141 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/PKG-INFO
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      465 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/SOURCES.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        1 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/dependency_links.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       97 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/requires.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)        6 2023-06-17 20:01:29.000000 scikit-gbm-0.1.1/scikit_gbm.egg-info/top_level.txt
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       38 2023-06-17 20:01:29.534784 scikit-gbm-0.1.1/setup.cfg
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.502785 scikit-gbm-0.1.1/skgbm/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)       48 2023-06-09 20:23:00.000000 scikit-gbm-0.1.1/skgbm/__init__.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     4073 2023-06-10 20:23:41.000000 scikit-gbm-0.1.1/skgbm/base.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.502785 scikit-gbm-0.1.1/skgbm/preprocessing/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)      126 2023-06-16 21:48:45.000000 scikit-gbm-0.1.1/skgbm/preprocessing/__init__.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     8592 2023-06-17 18:31:13.000000 scikit-gbm-0.1.1/skgbm/preprocessing/discretizer.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     3693 2023-06-17 18:06:40.000000 scikit-gbm-0.1.1/skgbm/preprocessing/featurizer.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     3662 2023-06-16 21:48:45.000000 scikit-gbm-0.1.1/skgbm/tools.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     5348 2023-06-09 20:23:00.000000 scikit-gbm-0.1.1/skgbm/tree.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     8165 2023-06-16 21:48:45.000000 scikit-gbm-0.1.1/skgbm/trees_extraction.py
+drwxrwxr-x   0 krzysztof  (1000) krzysztof  (1000)        0 2023-06-17 20:01:29.518784 scikit-gbm-0.1.1/tests/
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     2587 2023-04-15 16:16:57.000000 scikit-gbm-0.1.1/tests/test_gbm_wrapper.py
+-rw-rw-r--   0 krzysztof  (1000) krzysztof  (1000)     1574 2023-06-09 20:23:00.000000 scikit-gbm-0.1.1/tests/test_trees_to_dataframe.py
```

### Comparing `scikit-gbm-0.1.0/LICENSE` & `scikit-gbm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.1.0/PKG-INFO` & `scikit-gbm-0.1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: scikit-gbm
-Version: 0.1.0
+Version: 0.1.1
 Summary: scikit-learn compatible tools to work with GBM models
 Author-email: Krzysztof Joachimiak <joachimiak.krzysztof@gmail.com>
 Project-URL: Homepage, https://github.com/krzjoa/scikit-gbm
 Project-URL: Bug Tracker, https://github.com/krzjoa/scikit-gbm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scikit-gbm
 
 [![Documentation Status](https://readthedocs.org/projects/scikit-gbm/badge/?version=latest)](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/scikit-gbm.svg)](https://badge.fury.io/py/scikit-gbm)
 
 scikit-learn compatible tools to work with GBM models
 
 ## Installation
 
 ```
 pip install scikit-gbm
@@ -26,59 +27,45 @@
 # or 
 
 pip install git+https://github.com/krzjoa/scikit-gbm.git
 ```
 
 ## Usage
 
-For the moment, the only available class is `GBMFeaturezier`. It's a wrapper around
-scikit-learn GBMs, XGBoost, LightGBM and CatBoost models. 
+Fo the moment, you can find the following tools in the library:
+
+* `GBMFeaturizer`
+* `GBMDiscretizer`
+* `trees_to_dataframe`
+
+Take a look at the [documentation](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest) to learn more.
+A simple example, how to use `GBMFeaturizer` in a classification task.
 
 ```python
 
 # Classification
 from sklearn.datasets import make_classification
+from sklearn.model_selection import train_test_split
 from sklearn.pipeline import Pipeline
 from sklearn.linear_model import LogisticRegression
 
 from skgbm.preprocessing import GBMFeaturizer
 from lightgbm import LGBMRegressor
 from xgboost import XGBClassifier
 
 X, y = make_classification()
-# train_test_split
+X_train, X_test, y_train, y_test = train_test_split(X, y)
 
 pipeline = \
     Pipeline([
         ('gbm_featurizer', GBMFeaturizer(XGBClassifier())),
         ('logistic_regression', LogisticRegression())
     ])
 
 # Try also:
 # ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
 
-
-# Regression
-X, y = load_breast_cancer(return_X_y=True)
-X_train, X_test, y_train, y_test = train_test_split(X, y)
-
-# Try also:
-# ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
-# ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
-# ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
-
-pipeline = \
-    Pipeline([
-        ('gbm_featurizer', GBMFeaturizer(XGBClassifier())),
-        ('logistic_regression', LogisticRegression())
-    ])
-
-# Training
-pipeline.fit(X_train, y_train)
-
 # Predictions for the test set
 pipeline_pred = pipeline.predict(X_test)
-
-
 ```
```

### Comparing `scikit-gbm-0.1.0/pyproject.toml` & `scikit-gbm-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scikit-gbm"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Krzysztof Joachimiak", email="joachimiak.krzysztof@gmail.com" },
 ]
 description = "scikit-learn compatible tools to work with GBM models"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scikit-gbm-0.1.0/scikit_gbm.egg-info/PKG-INFO` & `scikit-gbm-0.1.1/scikit_gbm.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: scikit-gbm
-Version: 0.1.0
+Version: 0.1.1
 Summary: scikit-learn compatible tools to work with GBM models
 Author-email: Krzysztof Joachimiak <joachimiak.krzysztof@gmail.com>
 Project-URL: Homepage, https://github.com/krzjoa/scikit-gbm
 Project-URL: Bug Tracker, https://github.com/krzjoa/scikit-gbm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scikit-gbm
 
 [![Documentation Status](https://readthedocs.org/projects/scikit-gbm/badge/?version=latest)](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest)
+[![PyPI version](https://badge.fury.io/py/scikit-gbm.svg)](https://badge.fury.io/py/scikit-gbm)
 
 scikit-learn compatible tools to work with GBM models
 
 ## Installation
 
 ```
 pip install scikit-gbm
@@ -26,59 +27,45 @@
 # or 
 
 pip install git+https://github.com/krzjoa/scikit-gbm.git
 ```
 
 ## Usage
 
-For the moment, the only available class is `GBMFeaturezier`. It's a wrapper around
-scikit-learn GBMs, XGBoost, LightGBM and CatBoost models. 
+Fo the moment, you can find the following tools in the library:
+
+* `GBMFeaturizer`
+* `GBMDiscretizer`
+* `trees_to_dataframe`
+
+Take a look at the [documentation](https://scikit-gbm.readthedocs.io/en/latest/?badge=latest) to learn more.
+A simple example, how to use `GBMFeaturizer` in a classification task.
 
 ```python
 
 # Classification
 from sklearn.datasets import make_classification
+from sklearn.model_selection import train_test_split
 from sklearn.pipeline import Pipeline
 from sklearn.linear_model import LogisticRegression
 
 from skgbm.preprocessing import GBMFeaturizer
 from lightgbm import LGBMRegressor
 from xgboost import XGBClassifier
 
 X, y = make_classification()
-# train_test_split
+X_train, X_test, y_train, y_test = train_test_split(X, y)
 
 pipeline = \
     Pipeline([
         ('gbm_featurizer', GBMFeaturizer(XGBClassifier())),
         ('logistic_regression', LogisticRegression())
     ])
 
 # Try also:
 # ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
 # ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
 
-
-# Regression
-X, y = load_breast_cancer(return_X_y=True)
-X_train, X_test, y_train, y_test = train_test_split(X, y)
-
-# Try also:
-# ('gbm_featurizer', GBMFeaturizer(GradientBoostingClassifier())),
-# ('gbm_featurizer', GBMFeaturizer(LGBMClassifier())),
-# ('gbm_featurizer', GBMFeaturizer(CatBoostClassifier())),
-
-pipeline = \
-    Pipeline([
-        ('gbm_featurizer', GBMFeaturizer(XGBClassifier())),
-        ('logistic_regression', LogisticRegression())
-    ])
-
-# Training
-pipeline.fit(X_train, y_train)
-
 # Predictions for the test set
 pipeline_pred = pipeline.predict(X_test)
-
-
 ```
```

### Comparing `scikit-gbm-0.1.0/skgbm/base.py` & `scikit-gbm-0.1.1/skgbm/base.py`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.1.0/skgbm/tools.py` & `scikit-gbm-0.1.1/skgbm/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,9 +62,8 @@
     >>> from skgbm.tools import trees_to_dataframe
     >>> from sklearn.datasets import make_regression
     >>> from sklearn.ensemble import GradientBoostingRegressor
     >>> X, y = make_regression()
     >>> gb_reg = GradientBoostingRegressor().fit(X, y)
     >>> gb_df = trees_to_dataframe(gb_reg)
     """
-    return GBMWrapper(obj).trees_to_dataframe()
-
+    return GBMWrapper(obj).trees_to_dataframe()
```

### Comparing `scikit-gbm-0.1.0/skgbm/tree.py` & `scikit-gbm-0.1.1/skgbm/tree.py`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.1.0/skgbm/trees_extraction.py` & `scikit-gbm-0.1.1/skgbm/trees_extraction.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,22 +165,33 @@
     # TODO: standarize node_index? (i.e. remove L and S)
     return _filter_cols(trees_df)
     
 # =============================================================================
 #                                  CATBOOST
 # =============================================================================
 
-def catboost_trees_to_dataframe(obj):
-    
+def _catboost_raw_trees(obj):
     # Saving temporary model dump and loading JSON file
     model_name = '_tmp.dump'
     obj.save_model('_tmp.dump', 'json')
     with open(model_name) as f:
         trees_json = json.load(f)
     os.remove(model_name)
+    return trees_json
+
+def _catboost_get_splits(trees_json):
+    return [split['border'] 
+            for tree in  trees_json['oblivious_trees']
+            for split in tree['splits']
+        ]
+
+
+def catboost_trees_to_dataframe(obj):
+    
+    trees_json = _catboost_raw_trees(obj)
     
     # Getting parts of the model
     oblivious_trees = trees_json['oblivious_trees']
     features_info   = trees_json['features_info']
     
     # Parsing model dump
     df = []
```

### Comparing `scikit-gbm-0.1.0/tests/test_gbm_wrapper.py` & `scikit-gbm-0.1.1/tests/test_gbm_wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit-gbm-0.1.0/tests/test_trees_to_dataframe.py` & `scikit-gbm-0.1.1/tests/test_trees_to_dataframe.py`

 * *Files identical despite different names*

