# Comparing `tmp/data_ecosystem_dependencies-202306.0.10.tar.gz` & `tmp/data_ecosystem_dependencies-202306.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_dependencies-202306.0.10.tar", max compression
+gzip compressed data, was "data_ecosystem_dependencies-202306.0.12.tar", max compression
```

## Comparing `data_ecosystem_dependencies-202306.0.10.tar` & `data_ecosystem_dependencies-202306.0.12.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      842 2023-06-17 13:08:26.561973 data_ecosystem_dependencies-202306.0.10/data_ecosystem_dependencies/__init__.py
--rw-r--r--   0        0        0    11357 2023-06-17 13:08:26.561973 data_ecosystem_dependencies-202306.0.10/license.md
--rw-r--r--   0        0        0     2741 2023-06-17 13:14:42.374969 data_ecosystem_dependencies-202306.0.10/pyproject.toml
--rw-r--r--   0        0        0      341 2023-06-17 13:08:26.561973 data_ecosystem_dependencies-202306.0.10/readme.md
--rw-r--r--   0        0        0      160 2023-06-17 13:08:26.561973 data_ecosystem_dependencies-202306.0.10/setup.cfg
--rw-r--r--   0        0        0     3261 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202306.0.10/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-06-17 14:07:49.619497 data_ecosystem_dependencies-202306.0.12/data_ecosystem_dependencies/__init__.py
+-rw-r--r--   0        0        0    11357 2023-06-17 14:07:49.619497 data_ecosystem_dependencies-202306.0.12/license.md
+-rw-r--r--   0        0        0     2740 2023-06-17 14:11:04.055944 data_ecosystem_dependencies-202306.0.12/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-06-17 14:07:49.619497 data_ecosystem_dependencies-202306.0.12/readme.md
+-rw-r--r--   0        0        0      160 2023-06-17 14:07:49.619497 data_ecosystem_dependencies-202306.0.12/setup.cfg
+-rw-r--r--   0        0        0     3259 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202306.0.12/PKG-INFO
```

### Comparing `data_ecosystem_dependencies-202306.0.10/data_ecosystem_dependencies/__init__.py` & `data_ecosystem_dependencies-202306.0.12/data_ecosystem_dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202306.0.10/license.md` & `data_ecosystem_dependencies-202306.0.12/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202306.0.10/pyproject.toml` & `data_ecosystem_dependencies-202306.0.12/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="data_ecosystem_dependencies"
-version="202306.0.10"
+version="202306.0.12"
 description="Data Ecosystem  Dependencies - Python (PADE)"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://github.com/cdcent/data_ecosystem_services"
 repository="https://github.com/cdcent/data_ecosystem_services"
 classifiers=[
@@ -21,15 +21,15 @@
             "setup.py",
             "pyproject.toml"]
 packages = [{include = "data_ecosystem_dependencies"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pytest = "^7.1.2"
-python-dotenv = "^0.20.0"
+python-dotenv = "^1.0.0"
 adal = "^1.2.7"
 azure-common = "^1.1.28"
 azure-keyvault-secrets = "^4.5.0"
 azure-identity = "^1.10.0"
 azure-storage-file-datalake = "^12.8.0"
 openpyxl = "^3.0.4"
 numpy = "^1.23.0"
```

### Comparing `data_ecosystem_dependencies-202306.0.10/PKG-INFO` & `data_ecosystem_dependencies-202306.0.12/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-dependencies
-Version: 202306.0.10
+Version: 202306.0.12
 Summary: Data Ecosystem  Dependencies - Python (PADE)
 Home-page: https://github.com/cdcent/data_ecosystem_services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -44,15 +44,15 @@
 Requires-Dist: pip-system-certs (>=4.0,<5.0)
 Requires-Dist: pyarrow (>=10.0.1,<11.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
 Requires-Dist: pyreadstat (>=1.1.9,<2.0.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rsconnect-jupyter (>=1.6.0,<2.0.0)
 Requires-Dist: setuptools (==65.6.3)
 Requires-Dist: sphinx-autoapi (>=2.0.0,<3.0.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.19.5,<2.0.0)
 Requires-Dist: sphinx-markdown-builder (>=0.5.5,<0.6.0)
 Requires-Dist: sphinx-markdown-tables (>=0.0.17,<0.0.18)
```

