# Comparing `tmp/caafe-0.1.5.tar.gz` & `tmp/caafe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caafe-0.1.5.tar", last modified: Thu May 25 18:31:13 2023, max compression
+gzip compressed data, was "caafe-0.1.6.tar", last modified: Sat Jun 17 19:56:29 2023, max compression
```

## Comparing `caafe-0.1.5.tar` & `caafe-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:31:13.511086 caafe-0.1.5/
--rw-r--r--   0 root         (0) root         (0)      381 2023-05-25 18:30:36.000000 caafe-0.1.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     6846 2023-05-25 18:31:13.511086 caafe-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6002 2023-05-25 18:30:36.000000 caafe-0.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:31:13.510086 caafe-0.1.5/caafe/
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11664 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/caafe.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/caafe_evaluate.py
--rw-r--r--   0 root         (0) root         (0)    11101 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/data.py
--rw-r--r--   0 root         (0) root         (0)     4399 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/evaluate.py
--rw-r--r--   0 root         (0) root         (0)     3605 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/feature_extension_baselines.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/metrics.py
--rw-r--r--   0 root         (0) root         (0)     4439 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/plotting.py
--rw-r--r--   0 root         (0) root         (0)     4467 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/preprocessing.py
--rw-r--r--   0 root         (0) root         (0)     7895 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/run_llm_code.py
--rw-r--r--   0 root         (0) root         (0)     7065 2023-05-25 18:30:36.000000 caafe-0.1.5/caafe/sklearn_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:31:13.510086 caafe-0.1.5/caafe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6846 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-25 18:31:13.000000 caafe-0.1.5/caafe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 18:31:13.511086 caafe-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1182 2023-05-25 18:31:10.000000 caafe-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:31:13.511086 caafe-0.1.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-25 18:30:36.000000 caafe-0.1.5/tests/test_sklearn_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 19:56:29.716981 caafe-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-17 19:55:22.000000 caafe-0.1.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     6846 2023-06-17 19:56:29.716981 caafe-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6002 2023-06-17 19:55:22.000000 caafe-0.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 19:56:29.714981 caafe-0.1.6/caafe/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11664 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/caafe.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/caafe_evaluate.py
+-rw-r--r--   0 root         (0) root         (0)    11101 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/data.py
+-rw-r--r--   0 root         (0) root         (0)     4399 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/evaluate.py
+-rw-r--r--   0 root         (0) root         (0)     3605 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/feature_extension_baselines.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     4439 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/plotting.py
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/preprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     7895 2023-06-17 19:55:22.000000 caafe-0.1.6/caafe/run_llm_code.py
+-rw-r--r--   0 root         (0) root         (0)     7069 2023-06-17 19:56:24.000000 caafe-0.1.6/caafe/sklearn_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 19:56:29.715981 caafe-0.1.6/caafe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6846 2023-06-17 19:56:29.000000 caafe-0.1.6/caafe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      435 2023-06-17 19:56:29.000000 caafe-0.1.6/caafe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 19:56:29.000000 caafe-0.1.6/caafe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-17 19:56:29.000000 caafe-0.1.6/caafe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-17 19:56:29.000000 caafe-0.1.6/caafe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 19:56:29.716981 caafe-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-06-17 19:56:10.000000 caafe-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 19:56:29.716981 caafe-0.1.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 19:55:22.000000 caafe-0.1.6/tests/test_sklearn_wrapper.py
```

### Comparing `caafe-0.1.5/PKG-INFO` & `caafe-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caafe
-Version: 0.1.5
+Version: 0.1.6
 Summary: Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.
 Home-page: https://github.com/automl/CAAFE
 Author: Noah Hollmann, Samuel Müller, Frank Hutter
 Author-email: noah.homa@gmail.com
 License: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Free for non-commercial use
```

### Comparing `caafe-0.1.5/README.md` & `caafe-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/caafe.py` & `caafe-0.1.6/caafe/caafe.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/caafe_evaluate.py` & `caafe-0.1.6/caafe/caafe_evaluate.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/data.py` & `caafe-0.1.6/caafe/data.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/evaluate.py` & `caafe-0.1.6/caafe/evaluate.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/feature_extension_baselines.py` & `caafe-0.1.6/caafe/feature_extension_baselines.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/metrics.py` & `caafe-0.1.6/caafe/metrics.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/plotting.py` & `caafe-0.1.6/caafe/plotting.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/preprocessing.py` & `caafe-0.1.6/caafe/preprocessing.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/run_llm_code.py` & `caafe-0.1.6/caafe/run_llm_code.py`

 * *Files identical despite different names*

### Comparing `caafe-0.1.5/caafe/sklearn_wrapper.py` & `caafe-0.1.6/caafe/sklearn_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             df_train, df_test=None, target_column=target_name, return_mappings=True
         )
 
         df_train, y = split_target_column(df_train, target_name)
 
         X, y = df_train.values, y.values.astype(int)
         # Check that X and y have correct shape
-        X, y = check_X_y(X, y)
+        # X, y = check_X_y(X, y)
 
         # Store the classes seen during fit
         self.classes_ = unique_labels(y)
 
         self.base_classifier.fit(X, y)
 
         # Return the classifier
@@ -187,15 +187,15 @@
         )
 
         X = make_dataset_numeric(X, mappings=self.mappings)
 
         X = X.values
 
         # Input validation
-        X = check_array(X)
+        # X = check_array(X)
 
         return X
 
     def predict_proba(self, X):
         X = self.predict_preprocess(X)
         return self.base_classifier.predict_proba(X)
```

### Comparing `caafe-0.1.5/caafe.egg-info/PKG-INFO` & `caafe-0.1.6/caafe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caafe
-Version: 0.1.5
+Version: 0.1.6
 Summary: Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.
 Home-page: https://github.com/automl/CAAFE
 Author: Noah Hollmann, Samuel Müller, Frank Hutter
 Author-email: noah.homa@gmail.com
 License: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Free for non-commercial use
```

### Comparing `caafe-0.1.5/setup.py` & `caafe-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="caafe",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     description="Context-Aware Automated Feature Engineering (CAAFE) is an automated machine learning tool that uses large language models for feature engineering in tabular datasets. It generates Python code for new features along with explanations for their utility, enhancing interpretability.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Noah Hollmann, Samuel Müller, Frank Hutter",
     author_email="noah.homa@gmail.com",
     url="https://github.com/automl/CAAFE",
```

