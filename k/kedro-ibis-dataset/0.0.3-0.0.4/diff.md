# Comparing `tmp/kedro_ibis_dataset-0.0.3.tar.gz` & `tmp/kedro_ibis_dataset-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_ibis_dataset-0.0.3.tar", last modified: Fri Jun 16 23:02:04 2023, max compression
+gzip compressed data, was "kedro_ibis_dataset-0.0.4.tar", last modified: Fri Jun 16 23:53:58 2023, max compression
```

## Comparing `kedro_ibis_dataset-0.0.3.tar` & `kedro_ibis_dataset-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.3/README.md
--rw-r--r--   0        0        0      429 2023-06-16 23:02:04.743792 kedro_ibis_dataset-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 23:01:44.746383 kedro_ibis_dataset-0.0.3/src/kedro_ibis_dataset/__init__.py
--rw-r--r--   0        0        0     2423 2023-06-16 22:22:03.556747 kedro_ibis_dataset-0.0.3/src/kedro_ibis_dataset/kedro_ibis_dataset.py
--rw-r--r--   0        0        0      363 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.4/README.md
+-rw-r--r--   0        0        0      495 2023-06-16 23:53:58.224115 kedro_ibis_dataset-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 23:01:44.746383 kedro_ibis_dataset-0.0.4/src/kedro_ibis_dataset/__init__.py
+-rw-r--r--   0        0        0     2448 2023-06-16 23:07:41.966063 kedro_ibis_dataset-0.0.4/src/kedro_ibis_dataset/kedro_ibis_dataset.py
+-rw-r--r--   0        0        0      363 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.4/PKG-INFO
```

### Comparing `kedro_ibis_dataset-0.0.3/src/kedro_ibis_dataset/kedro_ibis_dataset.py` & `kedro_ibis_dataset-0.0.4/src/kedro_ibis_dataset/kedro_ibis_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing import Dict
+
 from kedro.io import AbstractDataSet, DataSetError
 import ibis
 
 
 class IbisDataSet(AbstractDataSet):
     """``IbisDataSet`` loads and `TODO` data to a table in an Ibis connection.
     When loading data, it returns an Ibis table which is a lazy connection to the data.
     """
-    connections: dict[str, ibis.BaseBackend] = {}
+    connections: Dict[str, ibis.BaseBackend] = {}
 
-    def __init__(self, table_name: str, credentials: dict[str, str]):
+    def __init__(self, table_name: str, credentials: Dict[str, str]):
         """Creates a new instance of ``IbisDataSet`` pointing to a table in an Ibis connection.
         The connection is created only once per connection string and shared across all instances.
 
         Args:
             table_name: The name of the table which will be returned when loading data.
             credentials: A dictionary containing the connection string under the key "con".
```

