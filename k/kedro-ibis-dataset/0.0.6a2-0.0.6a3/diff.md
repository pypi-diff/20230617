# Comparing `tmp/kedro_ibis_dataset-0.0.6a2.tar.gz` & `tmp/kedro_ibis_dataset-0.0.6a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_ibis_dataset-0.0.6a2.tar", last modified: Sat Jun 17 00:55:43 2023, max compression
+gzip compressed data, was "kedro_ibis_dataset-0.0.6a3.tar", last modified: Sat Jun 17 00:59:47 2023, max compression
```

## Comparing `kedro_ibis_dataset-0.0.6a2.tar` & `kedro_ibis_dataset-0.0.6a3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.6a2/README.md
--rw-r--r--   0        0        0      615 2023-06-17 00:55:42.997036 kedro_ibis_dataset-0.0.6a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 23:01:44.746383 kedro_ibis_dataset-0.0.6a2/src/kedro_ibis_dataset/__init__.py
--rw-r--r--   0        0        0     2448 2023-06-16 23:07:41.966063 kedro_ibis_dataset-0.0.6a2/src/kedro_ibis_dataset/kedro_ibis_dataset.py
--rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.6a2/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.6a3/README.md
+-rw-r--r--   0        0        0      683 2023-06-17 00:59:47.794857 kedro_ibis_dataset-0.0.6a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 23:01:44.746383 kedro_ibis_dataset-0.0.6a3/src/kedro_ibis_dataset/__init__.py
+-rw-r--r--   0        0        0     2448 2023-06-16 23:07:41.966063 kedro_ibis_dataset-0.0.6a3/src/kedro_ibis_dataset/kedro_ibis_dataset.py
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.6a3/PKG-INFO
```

### Comparing `kedro_ibis_dataset-0.0.6a2/src/kedro_ibis_dataset/kedro_ibis_dataset.py` & `kedro_ibis_dataset-0.0.6a3/src/kedro_ibis_dataset/kedro_ibis_dataset.py`

 * *Files identical despite different names*

