# Comparing `tmp/peopledatalabs-1.1.6.tar.gz` & `tmp/peopledatalabs-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peopledatalabs-1.1.6.tar", max compression
+gzip compressed data, was "peopledatalabs-1.1.8.tar", max compression
```

## Comparing `peopledatalabs-1.1.6.tar` & `peopledatalabs-1.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1073 2023-05-15 14:25:55.902452 peopledatalabs-1.1.6/LICENSE
--rw-r--r--   0        0        0    12222 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/README.md
--rw-r--r--   0        0        0     1638 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/__init__.py
--rw-r--r--   0        0        0     5592 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/endpoints/__init__.py
--rw-r--r--   0        0        0     1635 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/endpoints/company.py
--rw-r--r--   0        0        0      762 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/endpoints/location.py
--rw-r--r--   0        0        0     2812 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/endpoints/person.py
--rw-r--r--   0        0        0      744 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/endpoints/school.py
--rw-r--r--   0        0        0      314 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/errors.py
--rw-r--r--   0        0        0      984 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/logger.py
--rw-r--r--   0        0        0     5048 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/main.py
--rw-r--r--   0        0        0     2445 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/models/__init__.py
--rw-r--r--   0        0        0     2198 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/models/company.py
--rw-r--r--   0        0        0      215 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/models/location.py
--rw-r--r--   0        0        0     4349 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/models/person.py
--rw-r--r--   0        0        0      783 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/models/school.py
--rw-r--r--   0        0        0     2241 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/requests.py
--rw-r--r--   0        0        0     1139 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/settings.py
--rw-r--r--   0        0        0      460 2023-05-15 14:25:55.906452 peopledatalabs-1.1.6/src/peopledatalabs/utils.py
--rw-r--r--   0        0        0    13629 1970-01-01 00:00:00.000000 peopledatalabs-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/LICENSE
+-rw-r--r--   0        0        0    12222 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/README.md
+-rw-r--r--   0        0        0     1637 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/__init__.py
+-rw-r--r--   0        0        0     5754 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/__init__.py
+-rw-r--r--   0        0        0     1635 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/company.py
+-rw-r--r--   0        0        0      762 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/location.py
+-rw-r--r--   0        0        0     2812 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/person.py
+-rw-r--r--   0        0        0      744 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/endpoints/school.py
+-rw-r--r--   0        0        0      314 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/errors.py
+-rw-r--r--   0        0        0      984 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/logger.py
+-rw-r--r--   0        0        0     5048 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/main.py
+-rw-r--r--   0        0        0     2445 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/__init__.py
+-rw-r--r--   0        0        0     2198 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/company.py
+-rw-r--r--   0        0        0      215 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/location.py
+-rw-r--r--   0        0        0     4349 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/person.py
+-rw-r--r--   0        0        0      783 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/models/school.py
+-rw-r--r--   0        0        0     2241 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/requests.py
+-rw-r--r--   0        0        0     1139 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/settings.py
+-rw-r--r--   0        0        0      460 2023-06-17 00:46:17.373801 peopledatalabs-1.1.8/src/peopledatalabs/utils.py
+-rw-r--r--   0        0        0    13628 1970-01-01 00:00:00.000000 peopledatalabs-1.1.8/PKG-INFO
```

### Comparing `peopledatalabs-1.1.6/LICENSE` & `peopledatalabs-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/README.md` & `peopledatalabs-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/pyproject.toml` & `peopledatalabs-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peopledatalabs"
-version = "1.1.6"
+version = "1.1.8"
 description = "Official Python client for the People Data Labs API"
 homepage = "https://www.peopledatalabs.com"
 repository = "https://github.com/peopledatalabs/peopledatalabs-python"
 documentation = "https://docs.peopledatalabs.com"
 keywords = [
   "data enrichment",
   "people data labs",
@@ -25,27 +25,27 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/peopledatalabs/peopledatalabs-python/issues"
 "Source Code" = 'https://github.com/peopledatalabs/peopledatalabs-python'
 
 [tool.poetry.dependencies]
 python = "^3.7.2"
-email-validator = "^1.1"
-pydantic = ">=1.8,<1.10"
+email-validator = ">=1.1,<3.0"
+pydantic = "^1.8"
 python-dotenv = "^0"
 requests = "^2"
 
 [tool.poetry.dev-dependencies]
 autoflake = "^1.7"
 black = "^23.3.0"
-coverage = "^6.3.2"
+coverage = "^7.2.7"
 docformatter = "^1.7"
-flake8 = "^4.0.1"
+flake8 = "^5.0.4"
 pylint = "^2.17.4"
-pytest = "^7.1.1"
+pytest = "^7.3.2"
 pyupgrade = "^3.3.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
```

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/endpoints/__init__.py` & `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,18 @@
         return url
 
     def __getattr__(self, method_name):
         """
         Raises InvalidEndpointError when an undefined method is called.
         """
 
+        # disregard dunder methods
+        if method_name.startswith("__") and method_name.endswith("__"):
+            return self.__getattribute__(method_name)
+
         # pylint: disable=unused-argument
         def method(*args, **kwargs):
             cls_name = self.__class__.__name__
             raise InvalidEndpointError(
                 f"Invalid method {method_name} called for section {cls_name}."
             )
```

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/endpoints/company.py` & `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/endpoints/location.py` & `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/location.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/endpoints/person.py` & `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/endpoints/school.py` & `peopledatalabs-1.1.8/src/peopledatalabs/endpoints/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/logger.py` & `peopledatalabs-1.1.8/src/peopledatalabs/logger.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/main.py` & `peopledatalabs-1.1.8/src/peopledatalabs/main.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/models/__init__.py` & `peopledatalabs-1.1.8/src/peopledatalabs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/models/company.py` & `peopledatalabs-1.1.8/src/peopledatalabs/models/company.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/models/person.py` & `peopledatalabs-1.1.8/src/peopledatalabs/models/person.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/models/school.py` & `peopledatalabs-1.1.8/src/peopledatalabs/models/school.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/requests.py` & `peopledatalabs-1.1.8/src/peopledatalabs/requests.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/src/peopledatalabs/settings.py` & `peopledatalabs-1.1.8/src/peopledatalabs/settings.py`

 * *Files identical despite different names*

### Comparing `peopledatalabs-1.1.6/PKG-INFO` & `peopledatalabs-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peopledatalabs
-Version: 1.1.6
+Version: 1.1.8
 Summary: Official Python client for the People Data Labs API
 Home-page: https://www.peopledatalabs.com
 License: MIT
 Keywords: data enrichment,people data labs,person enrichment,company enrichment,search
 Author: People Data Labs
 Author-email: hello@peopledatalabs.com
 Requires-Python: >=3.7.2,<4.0.0
@@ -14,16 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: email-validator (>=1.1,<2.0)
-Requires-Dist: pydantic (>=1.8,<1.10)
+Requires-Dist: email-validator (>=1.1,<3.0)
+Requires-Dist: pydantic (>=1.8,<2.0)
 Requires-Dist: python-dotenv (>=0,<1)
 Requires-Dist: requests (>=2,<3)
 Project-URL: Bug Tracker, https://github.com/peopledatalabs/peopledatalabs-python/issues
 Project-URL: Documentation, https://docs.peopledatalabs.com
 Project-URL: Repository, https://github.com/peopledatalabs/peopledatalabs-python
 Project-URL: Source Code, https://github.com/peopledatalabs/peopledatalabs-python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: peopledatalabs Version: 1.1.6 Summary: Official
+Metadata-Version: 2.1 Name: peopledatalabs Version: 1.1.8 Summary: Official
 Python client for the People Data Labs API Home-page: https://
 www.peopledatalabs.com License: MIT Keywords: data enrichment,people data
 labs,person enrichment,company enrichment,search Author: People Data Labs
 Author-email: hello@peopledatalabs.com Requires-Python: >=3.7.2,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
 Implementation :: PyPy Classifier: Topic :: Software Development :: Libraries
-:: Python Modules Requires-Dist: email-validator (>=1.1,<2.0) Requires-Dist:
-pydantic (>=1.8,<1.10) Requires-Dist: python-dotenv (>=0,<1) Requires-Dist:
+:: Python Modules Requires-Dist: email-validator (>=1.1,<3.0) Requires-Dist:
+pydantic (>=1.8,<2.0) Requires-Dist: python-dotenv (>=0,<1) Requires-Dist:
 requests (>=2,<3) Project-URL: Bug Tracker, https://github.com/peopledatalabs/
 peopledatalabs-python/issues Project-URL: Documentation, https://
 docs.peopledatalabs.com Project-URL: Repository, https://github.com/
 peopledatalabs/peopledatalabs-python Project-URL: Source Code, https://
 github.com/peopledatalabs/peopledatalabs-python Description-Content-Type: text/
 markdown
                             [People Data Labs Logo]
```

