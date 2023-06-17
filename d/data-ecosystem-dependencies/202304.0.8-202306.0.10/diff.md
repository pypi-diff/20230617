# Comparing `tmp/data_ecosystem_dependencies-202304.0.8.tar.gz` & `tmp/data_ecosystem_dependencies-202306.0.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_dependencies-202304.0.8.tar", max compression
+gzip compressed data, was "data_ecosystem_dependencies-202306.0.10.tar", max compression
```

## Comparing `data_ecosystem_dependencies-202304.0.8.tar` & `data_ecosystem_dependencies-202306.0.10.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      842 2023-04-10 23:23:29.903207 data_ecosystem_dependencies-202304.0.8/data_ecosystem_dependencies/__init__.py
--rw-r--r--   0        0        0    11357 2023-04-10 23:23:29.903207 data_ecosystem_dependencies-202304.0.8/license.md
--rw-r--r--   0        0        0     2541 2023-04-10 23:28:20.246324 data_ecosystem_dependencies-202304.0.8/pyproject.toml
--rw-r--r--   0        0        0      341 2023-04-10 23:23:29.903207 data_ecosystem_dependencies-202304.0.8/readme.md
--rw-r--r--   0        0        0      160 2023-04-10 23:23:29.903207 data_ecosystem_dependencies-202304.0.8/setup.cfg
--rw-r--r--   0        0        0     3050 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202304.0.8/PKG-INFO
+-rw-r--r--   0        0        0      842 2023-06-17 13:08:26.561973 data_ecosystem_dependencies-202306.0.10/data_ecosystem_dependencies/__init__.py
+-rw-r--r--   0        0        0    11357 2023-06-17 13:08:26.561973 data_ecosystem_dependencies-202306.0.10/license.md
+-rw-r--r--   0        0        0     2741 2023-06-17 13:14:42.374969 data_ecosystem_dependencies-202306.0.10/pyproject.toml
+-rw-r--r--   0        0        0      341 2023-06-17 13:08:26.561973 data_ecosystem_dependencies-202306.0.10/readme.md
+-rw-r--r--   0        0        0      160 2023-06-17 13:08:26.561973 data_ecosystem_dependencies-202306.0.10/setup.cfg
+-rw-r--r--   0        0        0     3261 1970-01-01 00:00:00.000000 data_ecosystem_dependencies-202306.0.10/PKG-INFO
```

### Comparing `data_ecosystem_dependencies-202304.0.8/data_ecosystem_dependencies/__init__.py` & `data_ecosystem_dependencies-202306.0.10/data_ecosystem_dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202304.0.8/license.md` & `data_ecosystem_dependencies-202306.0.10/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_dependencies-202304.0.8/pyproject.toml` & `data_ecosystem_dependencies-202306.0.10/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="data_ecosystem_dependencies"
-version="202304.0.8"
+version="202306.0.10"
 description="Data Ecosystem  Dependencies - Python (PADE)"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://github.com/cdcent/data_ecosystem_services"
 repository="https://github.com/cdcent/data_ecosystem_services"
 classifiers=[
@@ -32,15 +32,15 @@
 azure-identity = "^1.10.0"
 azure-storage-file-datalake = "^12.8.0"
 openpyxl = "^3.0.4"
 numpy = "^1.23.0"
 botocore = "1.24.18"
 boto3 = "1.21.18"
 setuptools = "65.6.3"
-requests = "^2.28.1"
+requests = "2.31.0"
 myst-parser = "^0.18.0"
 sphinx-markdown-tables = "^0.0.17"
 Sphinx = "^5.2.1"
 sphinx-markdown-builder = "^0.5.5"
 pathlib = "^1.0.1"
 opencensus-ext-azure = "^1.1.7"
 opencensus = "^0.11.0"
@@ -60,28 +60,34 @@
 pytest-cov = "^4.0.0"
 sphinx-rtd-theme = "^1.1.1"
 chardet = "^5.0.0"
 nbconvert = "^6.5.1"
 pip-system-certs = "^4.0"
 style = "^1.1.6"
 azure-keyvault = "^4.2.0"
+azure-mgmt-monitor = "^5.0.1"
+jinja2 = "^3.1.2"
+opentelemetry-sdk = "^1.17.0"
+azure-monitor-opentelemetry-exporter = {version = "^1.0.0b14", allow-prereleases = true}
+azure-storage-queue = "^12.6.0"
 
 [tool.poetry.dev-dependencies]
 pandas = "^1.4.2"
 wheel = "^0.38.1"
 check-wheel-contents = "^0.3.4"
 flake8 = "^4.0.1"
 flake8-bugbear = "^22.6.22"
 black = "^22.3.0"
 commitizen = "^2.28.0"
 pathlib = "^1.0.1"
 python-decouple = "^3.6"
 delta-spark = "2.1.0"
 findspark = "^2.0.1"
 
+
 [tool.pytest.ini_options]
 minversion="6.0"
 addopts="-ra -q --cov --cov-report html --cov-report term-missing --cov-fail-under 95"
 testpaths=[
     "tests"
 ]
```

### Comparing `data_ecosystem_dependencies-202304.0.8/PKG-INFO` & `data_ecosystem_dependencies-202306.0.10/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-dependencies
-Version: 202304.0.8
+Version: 202306.0.10
 Summary: Data Ecosystem  Dependencies - Python (PADE)
 Home-page: https://github.com/cdcent/data_ecosystem_services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -13,43 +13,47 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Sphinx (>=5.2.1,<6.0.0)
 Requires-Dist: adal (>=1.2.7,<2.0.0)
 Requires-Dist: azure-common (>=1.1.28,<2.0.0)
 Requires-Dist: azure-identity (>=1.10.0,<2.0.0)
 Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.5.0,<5.0.0)
+Requires-Dist: azure-mgmt-monitor (>=5.0.1,<6.0.0)
+Requires-Dist: azure-monitor-opentelemetry-exporter (>=1.0.0b14,<2.0.0)
 Requires-Dist: azure-storage-file-datalake (>=12.8.0,<13.0.0)
+Requires-Dist: azure-storage-queue (>=12.6.0,<13.0.0)
 Requires-Dist: boto3 (==1.21.18)
 Requires-Dist: botocore (==1.24.18)
 Requires-Dist: chardet (>=5.0.0,<6.0.0)
 Requires-Dist: docutils (==0.17.1)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: myst-parser (>=0.18.0,<0.19.0)
 Requires-Dist: nbconvert (>=6.5.1,<7.0.0)
 Requires-Dist: numpy (>=1.23.0,<2.0.0)
 Requires-Dist: opencensus (>=0.11.0,<0.12.0)
 Requires-Dist: opencensus-ext-azure (>=1.1.7,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.4,<4.0.0)
+Requires-Dist: opentelemetry-sdk (>=1.17.0,<2.0.0)
 Requires-Dist: pathlib (>=1.0.1,<2.0.0)
 Requires-Dist: pip-system-certs (>=4.0,<5.0)
 Requires-Dist: pyarrow (>=10.0.1,<11.0.0)
 Requires-Dist: pygments (>=2.13.0,<3.0.0)
 Requires-Dist: pyreadstat (>=1.1.9,<2.0.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests (==2.31.0)
 Requires-Dist: rsconnect-jupyter (>=1.6.0,<2.0.0)
 Requires-Dist: setuptools (==65.6.3)
 Requires-Dist: sphinx-autoapi (>=2.0.0,<3.0.0)
 Requires-Dist: sphinx-autodoc-typehints (>=1.19.5,<2.0.0)
 Requires-Dist: sphinx-markdown-builder (>=0.5.5,<0.6.0)
 Requires-Dist: sphinx-markdown-tables (>=0.0.17,<0.0.18)
 Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0)
```

