# Comparing `tmp/kedro_ibis_dataset-0.0.5.tar.gz` & `tmp/kedro_ibis_dataset-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_ibis_dataset-0.0.5.tar", last modified: Sat Jun 17 00:24:25 2023, max compression
+gzip compressed data, was "kedro_ibis_dataset-0.0.6a0.tar", last modified: Sat Jun 17 00:27:02 2023, max compression
```

## Comparing `kedro_ibis_dataset-0.0.5.tar` & `kedro_ibis_dataset-0.0.6a0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.5/README.md
--rw-r--r--   0        0        0      597 2023-06-17 00:24:25.068268 kedro_ibis_dataset-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 23:01:44.746383 kedro_ibis_dataset-0.0.5/src/kedro_ibis_dataset/__init__.py
--rw-r--r--   0        0        0     2448 2023-06-16 23:07:41.966063 kedro_ibis_dataset-0.0.5/src/kedro_ibis_dataset/kedro_ibis_dataset.py
--rw-r--r--   0        0        0      363 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-06-16 19:34:49.301187 kedro_ibis_dataset-0.0.6a0/README.md
+-rw-r--r--   0        0        0      615 2023-06-17 00:27:02.049713 kedro_ibis_dataset-0.0.6a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 23:01:44.746383 kedro_ibis_dataset-0.0.6a0/src/kedro_ibis_dataset/__init__.py
+-rw-r--r--   0        0        0     2448 2023-06-16 23:07:41.966063 kedro_ibis_dataset-0.0.6a0/src/kedro_ibis_dataset/kedro_ibis_dataset.py
+-rw-r--r--   0        0        0      441 1970-01-01 00:00:00.000000 kedro_ibis_dataset-0.0.6a0/PKG-INFO
```

### Comparing `kedro_ibis_dataset-0.0.5/pyproject.toml` & `kedro_ibis_dataset-0.0.6a0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [project]
 name = "kedro-ibis-dataset"
-version = "0.0.5"
+version = "0.0.6a0"
 description = "Ibis connector for kedro catalog"
-repository = "https://github.com/inigohidalgo/kedro-ibis-dataset"
 authors = [
     { name = "Iñigo Hidalgo Rey", email = "inigohrey@gmail.com" },
 ]
 dependencies = [
     "kedro>=0.17.1",
     "ibis-framework>=5.1.0",
 ]
 requires-python = ">=3.8,<3.11"
 readme = "README.md"
 
+[project.urls]
+repository = "https://github.com/inigohidalgo/kedro-ibis-dataset"
+
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `kedro_ibis_dataset-0.0.5/src/kedro_ibis_dataset/kedro_ibis_dataset.py` & `kedro_ibis_dataset-0.0.6a0/src/kedro_ibis_dataset/kedro_ibis_dataset.py`

 * *Files identical despite different names*

