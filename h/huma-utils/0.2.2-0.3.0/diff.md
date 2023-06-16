# Comparing `tmp/huma_utils-0.2.2.tar.gz` & `tmp/huma_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_utils-0.2.2.tar", max compression
+gzip compressed data, was "huma_utils-0.3.0.tar", max compression
```

## Comparing `huma_utils-0.2.2.tar` & `huma_utils-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-06-16 21:20:36.784634 huma_utils-0.2.2/LICENSE
--rw-r--r--   0        0        0       35 2023-06-16 21:20:36.784634 huma_utils-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/__init__.py
--rw-r--r--   0        0        0      291 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/chain_utils.py
--rw-r--r--   0        0        0      330 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/datetime_utils.py
--rw-r--r--   0        0        0        0 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/py.typed
--rw-r--r--   0        0        0      428 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/pydantic_utils.py
--rw-r--r--   0        0        0      702 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/request_utils.py
--rw-r--r--   0        0        0     1113 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/string_utils.py
--rw-r--r--   0        0        0      543 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/test_helpers/address_helpers.py
--rw-r--r--   0        0        0      809 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/test_helpers/api_test_helpers.py
--rw-r--r--   0        0        0     2147 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/test_helpers/vcr_helpers.py
--rw-r--r--   0        0        0     1129 2023-06-16 21:20:36.784634 huma_utils-0.2.2/huma_utils/web3_utils.py
--rw-r--r--   0        0        0     2240 2023-06-16 21:20:36.784634 huma_utils-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 huma_utils-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-16 22:38:13.882538 huma_utils-0.3.0/LICENSE
+-rw-r--r--   0        0        0       35 2023-06-16 22:38:13.882538 huma_utils-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/__init__.py
+-rw-r--r--   0        0        0      291 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/chain_utils.py
+-rw-r--r--   0        0        0      330 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/datetime_utils.py
+-rw-r--r--   0        0        0        0 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/py.typed
+-rw-r--r--   0        0        0      428 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/pydantic_utils.py
+-rw-r--r--   0        0        0      702 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/request_utils.py
+-rw-r--r--   0        0        0     1113 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/string_utils.py
+-rw-r--r--   0        0        0      543 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/test_helpers/address_helpers.py
+-rw-r--r--   0        0        0      809 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/test_helpers/api_test_helpers.py
+-rw-r--r--   0        0        0     2042 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/test_helpers/vcr_helpers.py
+-rw-r--r--   0        0        0     1129 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/web3_utils.py
+-rw-r--r--   0        0        0     2240 2023-06-16 22:38:13.886538 huma_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 huma_utils-0.3.0/PKG-INFO
```

### Comparing `huma_utils-0.2.2/LICENSE` & `huma_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.2/huma_utils/request_utils.py` & `huma_utils-0.3.0/huma_utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.2/huma_utils/string_utils.py` & `huma_utils-0.3.0/huma_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.2/huma_utils/test_helpers/address_helpers.py` & `huma_utils-0.3.0/huma_utils/test_helpers/address_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.2/huma_utils/test_helpers/api_test_helpers.py` & `huma_utils-0.3.0/huma_utils/test_helpers/api_test_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.2/huma_utils/test_helpers/vcr_helpers.py` & `huma_utils-0.3.0/huma_utils/test_helpers/vcr_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 import vcr
 from vcr import cassette, request
 
 
 def _match_alchemy_url(
     incoming_req: vcr.request.Request, recorded_req: vcr.request.Request
 ) -> bool:
-    # It's an unfortunate fact that Alchemy puts the API key at the end of the URL directly as
-    # part of the path, so if whoever runs the test uses a different API key then request matching
-    # would fail. So let's not compare the last part of the URL when it's an Alchemy URL.
+    # It's an unfortunate fact that Alchemy embeds the chain and API key in the URL directly as
+    # part of the path, so if whoever runs the test uses a different chain or API key then request matching
+    # would fail. So let's not compare the entire URL when it's an Alchemy URL.
     if "alchemy.com" in incoming_req.host and "alchemy.com" in recorded_req.host:
-        filtered_r1_url = incoming_req.uri[: incoming_req.uri.rfind("/")]
-        return filtered_r1_url == recorded_req.uri
+        return True
 
     return incoming_req.uri == recorded_req.uri
 
 
 my_vcr = vcr.VCR()
 my_vcr.register_matcher(name="alchemy_url", matcher=_match_alchemy_url)
```

### Comparing `huma_utils-0.2.2/huma_utils/web3_utils.py` & `huma_utils-0.3.0/huma_utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.2.2/pyproject.toml` & `huma_utils-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huma-utils"
-version = "0.2.2"
+version = "0.3.0"
 description = ""
 authors = ["flowers-huang <flora221@stanford.edu>"]
 readme = "README.md"
 packages = [{include = "huma_utils"}]
 
 [tool.poetry.dependencies]
 python = "~3.10"
```

