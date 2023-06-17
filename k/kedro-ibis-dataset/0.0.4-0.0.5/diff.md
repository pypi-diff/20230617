# Comparing `tmp/kedro_ibis_dataset-0.0.4.tar.gz` & `tmp/kedro_ibis_dataset-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_ibis_dataset-0.0.4.tar", last modified: Fri Jun 16 23:53:58 2023, max compression
+gzip compressed data, was "kedro_ibis_dataset-0.0.5.tar", last modified: Sat Jun 17 00:24:25 2023, max compression
```

## Comparing `kedro_ibis_dataset-0.0.4.tar` & `kedro_ibis_dataset-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.4/README.md
--rw-r--r--   0        0        0      495 2023-06-16 23:53:58.224115 kedro_ibis_dataset-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 23:01:44.746383 kedro_ibis_dataset-0.0.4/src/kedro_ibis_dataset/__init__.py
--rw-r--r--   0        0        0     2448 2023-06-16 23:07:41.966063 kedro_ibis_dataset-0.0.4/src/kedro_ibis_dataset/kedro_ibis_dataset.py
--rw-r--r--   0        0        0      363 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.5/README.md
+-rw-r--r--   0        0        0      597 2023-06-17 00:24:25.068268 kedro_ibis_dataset-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 23:01:44.746383 kedro_ibis_dataset-0.0.5/src/kedro_ibis_dataset/__init__.py
+-rw-r--r--   0        0        0     2448 2023-06-16 23:07:41.966063 kedro_ibis_dataset-0.0.5/src/kedro_ibis_dataset/kedro_ibis_dataset.py
+-rw-r--r--   0        0        0      363 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.5/PKG-INFO
```

### Comparing `kedro_ibis_dataset-0.0.4/src/kedro_ibis_dataset/kedro_ibis_dataset.py` & `kedro_ibis_dataset-0.0.5/src/kedro_ibis_dataset/kedro_ibis_dataset.py`

 * *Files identical despite different names*

