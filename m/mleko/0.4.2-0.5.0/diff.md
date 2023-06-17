# Comparing `tmp/mleko-0.4.2.tar.gz` & `tmp/mleko-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.4.2.tar", max compression
+gzip compressed data, was "mleko-0.5.0.tar", max compression
```

## Comparing `mleko-0.4.2.tar` & `mleko-0.5.0.tar`

### file list

```diff
@@ -1,49 +1,57 @@
--rw-r--r--   0        0        0     1073 2023-06-11 08:22:08.292228 mleko-0.4.2/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-11 08:22:08.292228 mleko-0.4.2/README.md
--rw-r--r--   0        0        0     1323 2023-06-11 08:22:37.196064 mleko-0.4.2/mleko/__init__.py
--rw-r--r--   0        0        0      584 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/__init__.py
--rw-r--r--   0        0        0    11493 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0      805 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     2843 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1233 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0      398 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/format/__init__.py
--rw-r--r--   0        0        0     1933 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/format/vaex_cache_format_mixin.py
--rw-r--r--   0        0        0     5974 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      740 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      491 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1435 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    11572 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     1613 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0     5918 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     5267 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     4983 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5248 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7078 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5578 2023-06-11 08:22:08.292228 mleko-0.4.2/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      877 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     2211 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    18015 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0     9632 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      679 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     3815 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     5934 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0      644 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1420 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4496 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     3595 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      638 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     2359 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     2179 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2141 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     2248 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0        0 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/py.typed
--rw-r--r--   0        0        0      765 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4497 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3430 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1403 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     2836 2023-06-11 08:22:08.296228 mleko-0.4.2/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2839 2023-06-11 08:22:37.244064 mleko-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 mleko-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-17 16:53:35.711108 mleko-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-17 16:53:35.711108 mleko-0.5.0/README.md
+-rw-r--r--   0        0        0     1323 2023-06-17 16:54:05.835472 mleko-0.5.0/mleko/__init__.py
+-rw-r--r--   0        0        0      584 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    11493 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0      805 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     2843 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1233 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0      398 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/format/__init__.py
+-rw-r--r--   0        0        0     1938 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/format/vaex_cache_format_mixin.py
+-rw-r--r--   0        0        0     5974 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      740 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1435 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    11577 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     1613 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0     5884 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     5188 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     4990 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5255 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7080 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5585 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      877 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    18020 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0     9637 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      679 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     3815 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     5934 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0     1611 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/__init__.py
+-rw-r--r--   0        0        0     3073 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/base_transformer.py
+-rw-r--r--   0        0        0     4424 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/composite_transformer.py
+-rw-r--r--   0        0        0     4389 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/frequency_encoder_transformer.py
+-rw-r--r--   0        0        0     4021 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/label_encoder_transformer.py
+-rw-r--r--   0        0        0     3677 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/max_abs_scaler_transformer.py
+-rw-r--r--   0        0        0     4053 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/dataset/transform/min_max_scaler_transformer.py
+-rw-r--r--   0        0        0      644 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1420 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4496 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3595 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      697 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2359 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     2179 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2141 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     2248 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0     2088 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/pipeline/steps/transform_step.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/py.typed
+-rw-r--r--   0        0        0      765 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3430 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1413 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     2836 2023-06-17 16:53:35.715108 mleko-0.5.0/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2839 2023-06-17 16:54:05.887472 mleko-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 mleko-0.5.0/PKG-INFO
```

### Comparing `mleko-0.4.2/LICENSE` & `mleko-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/README.md` & `mleko-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/__init__.py` & `mleko-0.5.0/mleko/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
 from __future__ import annotations
 
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
```

### Comparing `mleko-0.4.2/mleko/cache/__init__.py` & `mleko-0.5.0/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/cache/cache_mixin.py` & `mleko-0.5.0/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/cache/fingerprinters/__init__.py` & `mleko-0.5.0/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-0.5.0/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-0.5.0/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-0.5.0/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/cache/format/vaex_cache_format_mixin.py` & `mleko-0.5.0/mleko/cache/format/vaex_cache_format_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The module containing the mixin class for `vaex` DataFrames to provide Arrow format caching capabilities."""
 from __future__ import annotations
 
 from pathlib import Path
 
 import vaex
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from mleko.utils.tqdm_helpers import set_tqdm_percent_wrapper
 
 
 class VaexCacheFormatMixin:
     """A mixin class for `vaex` DataFrames to provide Arrow format caching capabilities.
```

### Comparing `mleko-0.4.2/mleko/cache/lru_cache_mixin.py` & `mleko-0.5.0/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/dataset/__init__.py` & `mleko-0.5.0/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/dataset/convert/base_converter.py` & `mleko-0.5.0/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-0.5.0/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import multiprocessing
 from concurrent import futures
 from itertools import repeat
 from pathlib import Path
 
 import vaex
 from pyarrow import csv as arrow_csv
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from mleko.cache.fingerprinters import CSVFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.file_helpers import clear_directory
 
 from .base_converter import BaseConverter
```

### Comparing `mleko-0.4.2/mleko/dataset/feature_select/__init__.py` & `mleko-0.5.0/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-0.5.0/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         """Initializes the feature selector and ensures the destination directory exists.
 
         Note:
             The `features` and `ignore_features` arguments are mutually exclusive. If both are specified, a
             `ValueError` is raised.
 
         Args:
-            cache_directory: Directory where the selected features will be stored locally.
+            cache_directory: Directory where the resulting DataFrame will be stored locally.
             features: List of feature names to be used by the feature selector. If None, the default is all features
                 applicable to the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector. If None, the default is to
                 ignore no features.
             cache_size: The maximum number of cache entries.
 
         Raises:
@@ -62,25 +62,25 @@
             raise ValueError(error_msg)
 
         self._features: tuple[str, ...] | None = tuple(features) if features is not None else None
         self._ignore_features: tuple[str, ...] = tuple(ignore_features) if ignore_features is not None else tuple()
 
     @abstractmethod
     def select_features(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
-        """Selects features from the given DataFrame and returns a list of paths to the selected features.
+        """Selects features from the given DataFrame.
 
         Args:
             dataframe: DataFrame from which to select features.
             force_recompute: Whether to force the feature selector to recompute its output, even if it already exists.
 
         Raises:
             NotImplementedError: Must be implemented in the child class that inherits from `BaseFeatureSelector`.
 
         Returns:
-            A dataframe with the selected features.
+            A DataFrame with the selected features.
         """
         raise NotImplementedError
 
     @abstractmethod
     def _select_features(self, dataframe: vaex.DataFrame) -> vaex.DataFrame:
         """Selects features from the given DataFrame.
 
@@ -113,15 +113,15 @@
     @abstractmethod
     def _fingerprint(self) -> Hashable:
         """Returns a hashable object that uniquely identifies the feature selector.
 
         Note:
             Subclasses should call the parent method and include the result in the hashable object along with any other
             information that uniquely identifies the feature selector. All attributes that are used in the
-            that affect the output of the feature selector should be included in the hashable object.
+            feature selector that affect the output of the feature selector should be included in the hashable object.
 
         Returns:
             Hashable object that uniquely identifies the feature selector.
         """
         return self.__class__.__name__, self._features, self._ignore_features
 
     def _feature_set(self, dataframe: vaex.DataFrame) -> list[str]:
```

### Comparing `mleko-0.4.2/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-0.5.0/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,31 +24,30 @@
     multiple feature selectors need to be applied to a DataFrame and the cache needs to be shared between them.
     """
 
     @auto_repr
     def __init__(
         self,
         cache_directory: str | Path,
-        feature_selectors: list[BaseFeatureSelector] | tuple[BaseFeatureSelector, ...] | tuple[()] = (),
+        feature_selectors: list[BaseFeatureSelector] | tuple[BaseFeatureSelector, ...],
         cache_size: int = 1,
     ) -> None:
         """Initializes the composite feature selector.
 
         The composite feature selector will combine the feature selectors into a single feature selector. Each feature
         selector will be applied to the DataFrame in the order they are specified.
 
         Args:
-            cache_directory: Directory where the selected features will be stored locally.
+            cache_directory: Directory where the resulting DataFrame will be stored locally.
             feature_selectors: List of feature selectors to be combined.
             cache_size: The maximum number of entries to keep in the cache.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.feature_select import CompositeFeatureSelector, MissingRateFeatureSelector
-            >>> from mleko.utils.vaex_helpers import get_column
             >>> df = vaex.from_arrays(
             ...     a=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
             ...     b=[1, 2, 3, 4, None, None, None, None, None, None],
             ...     c=[1, 2, 3, 4, 5, 6, None, None, None, None],
             ... )
             >>> feature_selector = CompositeFeatureSelector(
             ...     cache_directory=".",
```

### Comparing `mleko-0.4.2/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-0.5.0/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module for the invariance feature selector."""
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Hashable
 
 import vaex
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.dataset.feature_select.base_feature_selector import BaseFeatureSelector
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_column, get_columns
 
@@ -38,15 +38,15 @@
             Only works with categorical and boolean features.
 
         Warning:
             Make sure to ignore any important features that need to be kept, such as the
             target feature or some identifier.
 
         Args:
-            cache_directory: Directory where the selected features will be stored locally.
+            cache_directory: Directory where the resulting DataFrame will be stored locally.
             features: List of feature names to be used by the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector.
             cache_size: The maximum number of entries to keep in the cache.
 
         Examples:
             >>> import vaex
             >>> from mleko.dataset.feature_select import InvarianceFeatureSelector
```

### Comparing `mleko-0.4.2/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-0.5.0/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module for the missing rate feature selector."""
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Hashable
 
 import vaex
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_column, get_columns
 
 from .base_feature_selector import BaseFeatureSelector
@@ -40,15 +40,15 @@
             Works with all types of features.
 
         Warning:
             Make sure to ignore any important features that need to be kept, such as the
             target feature or some identifier.
 
         Args:
-            cache_directory: Directory where the selected features will be stored locally.
+            cache_directory: Directory where the resulting DataFrame will be stored locally.
             missing_rate_threshold: The maximum missing rate allowed for a feature to be selected.
             features: List of feature names to be used by the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector.
             cache_size: The maximum number of entries to keep in the cache.
 
         Examples:
             >>> import vaex
```

### Comparing `mleko-0.4.2/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-0.5.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             Only works with numeric features.
 
         Warning:
             Make sure to ignore any important features that need to be kept, such as the
             target feature or some identifier.
 
         Args:
-            cache_directory: Directory where the selected features will be stored locally.
+            cache_directory: Directory where the resulting DataFrame will be stored locally.
             correlation_threshold: The maximum correlation allowed for a feature to be selected.
             features: List of feature names to be used by the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector.
             cache_size: The maximum number of entries to keep in the cache.
 
         Examples:
             >>> import vaex
```

### Comparing `mleko-0.4.2/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-0.5.0/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module for the variance feature selector."""
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Hashable
 
 import vaex
-from tqdm import tqdm
+from tqdm.auto import tqdm
 from vaex.ml import MaxAbsScaler
 
 from mleko.cache.fingerprinters.vaex_fingerprinter import VaexFingerprinter
 from mleko.dataset.feature_select.base_feature_selector import BaseFeatureSelector
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.vaex_helpers import get_column, get_columns
@@ -40,15 +40,15 @@
             Only works with numeric features.
 
         Warning:
             Make sure to ignore any important features that need to be kept, such as the
             target feature or some identifier.
 
         Args:
-            cache_directory: Directory where the selected features will be stored locally.
+            cache_directory: Directory where the resulting DataFrame will be stored locally.
             variance_threshold: The minimum variance allowed for a feature to be selected.
             features: List of feature names to be used by the feature selector.
             ignore_features: List of feature names to be ignored by the feature selector.
             cache_size: The maximum number of entries to keep in the cache.
 
         Examples:
             >>> import vaex
```

### Comparing `mleko-0.4.2/mleko/dataset/ingest/__init__.py` & `mleko-0.5.0/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/dataset/ingest/base_ingester.py` & `mleko-0.5.0/mleko/dataset/ingest/base_ingester.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,13 +43,15 @@
         Args:
             file_suffixes: List of file suffixes that should be returned from the destination directory,
                 such as `gz`, `zip`, and `csv`.
 
         Returns:
             A list of Path objects for all CSV, ZIP and GZ files in the destination directory.
         """
-        return [
-            Path(filepath)
-            for filepath in [
-                p for suffix in file_suffixes for p in glob.glob(f"{self._destination_directory}/*.{suffix}")
+        return sorted(
+            [
+                Path(filepath)
+                for filepath in [
+                    p for suffix in file_suffixes for p in glob.glob(f"{self._destination_directory}/*.{suffix}")
+                ]
             ]
-        ]
+        )
```

### Comparing `mleko-0.4.2/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-0.5.0/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from datetime import datetime
 from itertools import repeat
 from pathlib import Path
 from typing import NamedTuple
 
 import requests
 from requests.auth import HTTPBasicAuth
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.file_helpers import clear_directory
 
 from .base_ingester import BaseIngester
```

### Comparing `mleko-0.4.2/mleko/dataset/ingest/s3_ingester.py` & `mleko-0.5.0/mleko/dataset/ingest/s3_ingester.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from concurrent import futures
 from pathlib import Path
 from typing import Any
 
 import boto3
 from boto3.s3.transfer import TransferConfig as BotoTransferConfig
 from botocore.config import Config as BotoConfig
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from mleko.utils.custom_logger import CustomLogger
 from mleko.utils.decorators import auto_repr
 from mleko.utils.file_helpers import clear_directory
 
 from .base_ingester import BaseIngester
```

### Comparing `mleko-0.4.2/mleko/dataset/split/__init__.py` & `mleko-0.5.0/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/dataset/split/base_splitter.py` & `mleko-0.5.0/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/dataset/split/expression_splitter.py` & `mleko-0.5.0/mleko/dataset/split/expression_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/dataset/split/random_splitter.py` & `mleko-0.5.0/mleko/dataset/split/random_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/pipeline/__init__.py` & `mleko-0.5.0/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/pipeline/data_container.py` & `mleko-0.5.0/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/pipeline/pipeline.py` & `mleko-0.5.0/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/pipeline/pipeline_step.py` & `mleko-0.5.0/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/pipeline/steps/__init__.py` & `mleko-0.5.0/mleko/pipeline/steps/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,10 +6,11 @@
 """
 from __future__ import annotations
 
 from .convert_step import ConvertStep
 from .feature_select_step import FeatureSelectStep
 from .ingest_step import IngestStep
 from .split_step import SplitStep
+from .transform_step import TransformStep
 
 
-__all__ = ["IngestStep", "ConvertStep", "SplitStep", "FeatureSelectStep"]
+__all__ = ["IngestStep", "ConvertStep", "SplitStep", "FeatureSelectStep", "TransformStep"]
```

### Comparing `mleko-0.4.2/mleko/pipeline/steps/convert_step.py` & `mleko-0.5.0/mleko/pipeline/steps/convert_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/pipeline/steps/feature_select_step.py` & `mleko-0.5.0/mleko/pipeline/steps/feature_select_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/pipeline/steps/ingest_step.py` & `mleko-0.5.0/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/pipeline/steps/split_step.py` & `mleko-0.5.0/mleko/pipeline/steps/split_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/utils/__init__.py` & `mleko-0.5.0/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/utils/custom_logger.py` & `mleko-0.5.0/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/utils/decorators.py` & `mleko-0.5.0/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/utils/file_helpers.py` & `mleko-0.5.0/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/mleko/utils/tqdm_helpers.py` & `mleko-0.5.0/mleko/utils/tqdm_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """This module provides helper functions for `tqdm` progress bars."""
 from __future__ import annotations
 
 from typing import Callable
 
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 
 def set_tqdm_percent_wrapper(pbar: tqdm) -> Callable[[float], None]:
     """Return a function to set the percentage of a `tqdm` progress bar instead of incrementing it.
 
     This function returns a function that can be used to set the percentage of a `tqdm` progress bar instead of
     incrementing it. This is useful when the progress bar is used to track the progress of a task that is not
@@ -16,15 +16,15 @@
     Args:
         pbar: A `tqdm` progress bar instance.
 
     Returns:
         A function that sets the percentage based on the float value passed as a parameter.
 
     Example:
-        >>> from tqdm import tqdm
+        >>> from tqdm.auto import tqdm
         >>> from mleko.utils import set_tqdm_percent_wrapper
         >>> pbar = tqdm(total=100)
         >>> set_percent = set_tqdm_percent_wrapper(pbar)
         >>> set_percent(0.5)
         >>> pbar.n
         50
     """
```

### Comparing `mleko-0.4.2/mleko/utils/vaex_helpers.py` & `mleko-0.5.0/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.2/pyproject.toml` & `mleko-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "0.4.2"
+version = "0.5.0"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-0.4.2/PKG-INFO` & `mleko-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.4.2
+Version: 0.5.0
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 3 - Alpha
```

