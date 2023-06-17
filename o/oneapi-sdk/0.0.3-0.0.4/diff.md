# Comparing `tmp/oneapi_sdk-0.0.3.tar.gz` & `tmp/oneapi_sdk-0.0.4.tar.gz`

## Comparing `oneapi_sdk-0.0.3.tar` & `oneapi_sdk-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/design.md
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/pull_request_template.md
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/requirements.txt
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/.github/workflows/build-and-publish.yaml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/__init__.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/api_requestor.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/api_resources/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/api_resources/movie.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/api_resources/quote.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/api_resources/utils.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/api_resources/abstract/api_resource.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/api_resources/abstract/retrievable_api_resource.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/tests/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/tests/mocks.py
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/tests/test_api.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/oneapi/tests/test_utils.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/LICENSE
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/README.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/design.md
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/pull_request_template.md
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/.github/workflows/build-and-publish.yaml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/__init__.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/api_requestor.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/api_resources/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/api_resources/movie.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/api_resources/quote.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/api_resources/utils.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/api_resources/abstract/api_resource.py
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/api_resources/abstract/retrievable_api_resource.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/tests/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/tests/mocks.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/tests/test_api.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/oneapi/tests/test_utils.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/README.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 oneapi_sdk-0.0.4/PKG-INFO
```

### Comparing `oneapi_sdk-0.0.3/design.md` & `oneapi_sdk-0.0.4/design.md`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/pull_request_template.md` & `oneapi_sdk-0.0.4/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/.github/workflows/build-and-publish.yaml` & `oneapi_sdk-0.0.4/.github/workflows/build-and-publish.yaml`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/oneapi/api_requestor.py` & `oneapi_sdk-0.0.4/oneapi/api_requestor.py`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/oneapi/api_resources/movie.py` & `oneapi_sdk-0.0.4/oneapi/api_resources/movie.py`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/oneapi/api_resources/quote.py` & `oneapi_sdk-0.0.4/oneapi/api_resources/quote.py`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/oneapi/api_resources/utils.py` & `oneapi_sdk-0.0.4/oneapi/api_resources/utils.py`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/oneapi/api_resources/abstract/listable_api_resource.py` & `oneapi_sdk-0.0.4/oneapi/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/oneapi/tests/mocks.py` & `oneapi_sdk-0.0.4/oneapi/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/oneapi/tests/test_api.py` & `oneapi_sdk-0.0.4/oneapi/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/oneapi/tests/test_utils.py` & `oneapi_sdk-0.0.4/oneapi/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/LICENSE` & `oneapi_sdk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/README.md` & `oneapi_sdk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `oneapi_sdk-0.0.3/pyproject.toml` & `oneapi_sdk-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 # Exclude tests from the distribution
 [build]
 exclude = ["oneapi/tests/"]
 
 [project]
 name = "oneapi-sdk"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Eduardo Felipe Weber", email="eduardo-felipe-weber@hotmail.com" },
 ]
 description = "A Python SDK for The One API"
 readme = "README.md"
 requires-python = ">=3.9.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
-]
+]
+dynamic = ["dependencies"]
+
+[tool.hatch.metadata.hooks.requirements_txt]
+files = ["requirements.txt"]
```

