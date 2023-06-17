# Comparing `tmp/datasieve-0.1.4.tar.gz` & `tmp/datasieve-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.1.4.tar", max compression
+gzip compressed data, was "datasieve-0.1.5.tar", max compression
```

## Comparing `datasieve-0.1.4.tar` & `datasieve-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1059 2023-06-07 17:23:26.771074 datasieve-0.1.4/LICENSE
--rw-r--r--   0        0        0    11780 2023-06-07 17:23:26.771074 datasieve-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/__init__.py
--rw-r--r--   0        0        0     8427 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/pipeline.py
--rw-r--r--   0        0        0      567 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     3228 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/base_transform.py
--rw-r--r--   0        0        0     5683 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     2748 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1357 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/noise.py
--rw-r--r--   0        0        0     1432 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1191 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/sklearn_wrapper.py
--rw-r--r--   0        0        0     1621 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1453 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3275 2023-06-07 17:23:26.771074 datasieve-0.1.4/datasieve/utils.py
--rw-r--r--   0        0        0      544 2023-06-07 17:23:26.771074 datasieve-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    12406 1970-01-01 00:00:00.000000 datasieve-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-17 14:14:28.752287 datasieve-0.1.5/LICENSE
+-rw-r--r--   0        0        0    11780 2023-06-17 14:14:28.752287 datasieve-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/__init__.py
+-rw-r--r--   0        0        0     8644 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/pipeline.py
+-rw-r--r--   0        0        0      567 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     3228 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/base_transform.py
+-rw-r--r--   0        0        0     5683 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     2748 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1357 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/noise.py
+-rw-r--r--   0        0        0     1334 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1491 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/sklearn_wrapper.py
+-rw-r--r--   0        0        0     1589 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1585 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3275 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/utils.py
+-rw-r--r--   0        0        0      544 2023-06-17 14:14:28.752287 datasieve-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    12406 1970-01-01 00:00:00.000000 datasieve-0.1.5/PKG-INFO
```

### Comparing `datasieve-0.1.4/LICENSE` & `datasieve-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.4/README.md` & `datasieve-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.4/datasieve/pipeline.py` & `datasieve-0.1.5/datasieve/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,21 @@
         for _, (step_name, step) in enumerate(self.steps):
             if step_name == name:
                 return step
 
         logger.warning(f"Could not find step {name} in pipeline, returning None")
         return None
 
+    def __contains__(self, name: str):
+        for _, (step_name, _) in enumerate(self.steps):
+            if step_name == name:
+                return True
+
+        return False
+
     def append(self, step: Tuple[str, object], fitparams: dict = {}):
         """
         Append a step to the pipeline
         :param step: tuple of (str, transform())
         :param fitparams: dictionary of parameters to pass to fit
         """
         if step[0] in self.step_strings:
@@ -141,29 +148,30 @@
         return X, y, sample_weight
 
     # flake8: noqa: C901
     def _validate_arguments(self, X, y, sample_weight, fit=False, outlier_check=False):
         if isinstance(X, pd.DataFrame) and fit:
             self.pandas_types = True
             self.feature_list = X.columns
+            self.features_in = X.columns
             if y is not None:
                 self.label_list = y.columns
         elif fit:
             self.pandas_types = False
-            self.feature_list = list(np.arange(0, X.shape[1]))
+            self.features_in = list(np.arange(0, X.shape[1]))
             if y is not None:
                 if len(y.shape) > 1:
                     self.label_list = list(np.arange(0, y.shape[1]))
                 else:
                     self.label_list = [0]
         elif isinstance(X, pd.DataFrame) and not fit:
-            if list(X.columns) != list(self.feature_list):
-                raise Exception(f"Pipeline expected {self.feature_list} but got {X.columns}.")
+            if list(X.columns) != list(self.features_in):
+                raise Exception(f"Pipeline expected {self.features_in} but got {X.columns}.")
         elif not isinstance(X, pd.DataFrame) and not fit and self.pandas_types:
-            X = pd.DataFrame(X, columns=self.feature_list)
+            X = pd.DataFrame(X, columns=self.features_in)
 
         if self.pandas_types:
             try:
                 X = X.to_numpy()
                 if y is not None:
                     y = y.to_numpy()
             except AttributeError:
```

### Comparing `datasieve-0.1.4/datasieve/transforms/__init__.py` & `datasieve-0.1.5/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.4/datasieve/transforms/base_transform.py` & `datasieve-0.1.5/datasieve/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.4/datasieve/transforms/dbscan.py` & `datasieve-0.1.5/datasieve/transforms/dbscan.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.4/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.1.5/datasieve/transforms/dissimilarity_index.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.4/datasieve/transforms/noise.py` & `datasieve-0.1.5/datasieve/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.4/datasieve/transforms/pca.py` & `datasieve-0.1.5/datasieve/transforms/pca.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import numpy as np
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
 class PCA(BaseTransform):
     """
-    A subclass of the SKLearn PCA that ensures fit, transform, fit_transform and
-    inverse_transform all take the full set of params X, y, sample_weight (even if they
-    are unused) to follow the FlowdaptPipeline API.
+    A PCA that ensures the feature names are properly transformed and follow
+    along with the X throughout the pipeline.
     """
 
     def __init__(self, **kwargs):
         self._skl: decomposition.PCA = decomposition.PCA(**kwargs)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         n_components = X.shape[1]
```

### Comparing `datasieve-0.1.4/datasieve/transforms/sklearn_wrapper.py` & `datasieve-0.1.5/datasieve/transforms/svm_outlier_extractor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,43 @@
+from sklearn.linear_model import SGDOneClassSVM
 from datasieve.transforms.base_transform import BaseTransform
-from sklearn.base import BaseEstimator
-from joblib import parallel_backend
+from datasieve.utils import remove_outliers
+import logging
+import numpy as np
 
+logger = logging.getLogger('datasieve.pipeline')
 
-class SKLearnWrapper(BaseTransform):
+
+class SVMOutlierExtractor(BaseTransform):
     """
-    Wrapper that takes *most* SKLearn transforms and allows them to
-    work wiith the datasieve pipeline
+    A transform that uses SGDOneClassSVM to detect and remove outlier datapoints
+    from X, and follows through to remove the same points from y and sample_weights
     """
-    def __init__(self, sklearninstance: BaseEstimator, n_jobs=-1, backend="loky", **kwargs):
-        self.backend = backend
-        self.n_jobs = n_jobs
-        self._skl = sklearninstance
+
+    def __init__(self, **kwargs):
+        self._skl = SGDOneClassSVM(**kwargs)
+
+    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+        self.fit(X, y, sample_weight=sample_weight)
+        return self.transform(X, y, sample_weight, feature_list)
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        with parallel_backend(self.backend, n_jobs=self.n_jobs):
-            self._skl = self._skl.fit(X, y=y)
+        self._skl.fit(X, y=y, sample_weight=sample_weight)
         return X, y, sample_weight, feature_list
 
     def transform(self, X, y=None, sample_weight=None,
                   feature_list=None, outlier_check=False, **kwargs):
-        with parallel_backend(self.backend, n_jobs=self.n_jobs):
-            X = self._skl.transform(X)
-        return X, y, sample_weight, feature_list
+        y_pred = self._skl.predict(X)
+        y_pred = np.where(y_pred == -1, 0, y_pred)
+        if not outlier_check:
+            X, y, sample_weight = remove_outliers(X, y, sample_weight, y_pred)
+            num_tossed = len(y_pred) - len(X)
+            if num_tossed > 0:
+                logger.info(
+                    f"SVM detected {num_tossed} data points "
+                    "as outliers."
+                )
+        else:
+            y += y_pred
+            y -= 1
 
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        X = self._skl.inverse_transform(X)
         return X, y, sample_weight, feature_list
```

### Comparing `datasieve-0.1.4/datasieve/transforms/variance_threshold.py` & `datasieve-0.1.5/datasieve/transforms/variance_threshold.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,19 @@
         self.mask = None
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         self._skl.fit(X)
         self.mask = self._skl.get_support()
         if feature_list is not None:
             self.feature_list = np.array(feature_list)[self.mask]
-            logger.info("Variance will remove features "
-                        f"{len(feature_list) - len(self.feature_list)} "
-                        f"on transform. {np.array(feature_list)[~self.mask]}")
+            if len(feature_list) - len(self.feature_list) > 0:
+                logger.info("VarianceThreshold will remove "
+                            f"{len(feature_list) - len(self.feature_list)} "
+                            "features from the dataset."
+                            f"on transform. {np.array(feature_list)[~self.mask]}")
         else:
             self.feature_list = None
 
         return X, y, sample_weight, self.feature_list
 
     def transform(self, X, y=None, sample_weight=None,
                   feature_list=None, outlier_check=False, **kwargs):
```

### Comparing `datasieve-0.1.4/datasieve/utils.py` & `datasieve-0.1.5/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.4/pyproject.toml` & `datasieve-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.1.4"
+version = "0.1.5"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `datasieve-0.1.4/PKG-INFO` & `datasieve-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.1.4
+Version: 0.1.5
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

