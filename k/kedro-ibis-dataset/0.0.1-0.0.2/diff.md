# Comparing `tmp/kedro_ibis_dataset-0.0.1.tar.gz` & `tmp/kedro_ibis_dataset-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_ibis_dataset-0.0.1.tar", last modified: Fri Jun 16 19:46:07 2023, max compression
+gzip compressed data, was "kedro_ibis_dataset-0.0.2.tar", last modified: Fri Jun 16 22:49:44 2023, max compression
```

## Comparing `kedro_ibis_dataset-0.0.1.tar` & `kedro_ibis_dataset-0.0.2.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.1/README.md
--rw-r--r--   0        0        0      430 2023-06-16 19:46:07.788220 kedro_ibis_dataset-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.2/README.md
+-rw-r--r--   0        0        0      429 2023-06-16 22:49:44.347651 kedro_ibis_dataset-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      363 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.2/PKG-INFO
```

