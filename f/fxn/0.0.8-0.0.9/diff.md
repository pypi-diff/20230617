# Comparing `tmp/fxn-0.0.8.tar.gz` & `tmp/fxn-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fxn-0.0.8.tar", last modified: Mon May 29 20:40:37 2023, max compression
+gzip compressed data, was "fxn-0.0.9.tar", last modified: Tue May 30 17:50:24 2023, max compression
```

## Comparing `fxn-0.0.8.tar` & `fxn-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.663996 fxn-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 20:40:20.000000 fxn-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 20:40:37.663996 fxn-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 20:40:20.000000 fxn-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.659996 fxn-0.0.8/fxn/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.659996 fxn-0.0.8/fxn/api/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/featureinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.663996 fxn-0.0.8/fxn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.659996 fxn-0.0.8/fxn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:40:37.663996 fxn-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 20:40:20.000000 fxn-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:24.241686 fxn-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-30 17:50:02.000000 fxn-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-30 17:50:24.241686 fxn-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 17:50:02.000000 fxn-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:24.237686 fxn-0.0.9/fxn/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:24.241686 fxn-0.0.9/fxn/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/featureinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:24.241686 fxn-0.0.9/fxn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/cli/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/cli/predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-30 17:50:02.000000 fxn-0.0.9/fxn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:50:24.237686 fxn-0.0.9/fxn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-30 17:50:24.000000 fxn-0.0.9/fxn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 17:50:24.000000 fxn-0.0.9/fxn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:50:24.000000 fxn-0.0.9/fxn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 17:50:24.000000 fxn-0.0.9/fxn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 17:50:24.000000 fxn-0.0.9/fxn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 17:50:24.000000 fxn-0.0.9/fxn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 17:50:24.241686 fxn-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-30 17:50:02.000000 fxn-0.0.9/setup.py
```

### Comparing `fxn-0.0.8/LICENSE` & `fxn-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/PKG-INFO` & `fxn-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.8/fxn/api/api.py` & `fxn-0.0.9/fxn/api/api.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/fxn/api/dtype.py` & `fxn-0.0.9/fxn/api/dtype.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/fxn/api/featureinput.py` & `fxn-0.0.9/fxn/api/featureinput.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/fxn/api/prediction.py` & `fxn-0.0.9/fxn/api/prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         )
         # Check
         prediction = response["createPrediction"]
         if not prediction:
             return None
         # Parse results
         if "results" in prediction and not raw_outputs:
-            prediction["results"] = [_parse_output_feature(feature) for feature in prediction["results"]]
+            prediction["results"] = [_parse_output_feature(feature) for feature in prediction["results"]] if prediction["results"] is not None else None
         # Create
         prediction = CloudPrediction(**prediction) if prediction["type"] == PredictorType.Cloud else EdgePrediction(**prediction)
         # Return
         return prediction
 
 @dataclass(frozen=True)
 class CloudPrediction (Prediction):
```

### Comparing `fxn-0.0.8/fxn/api/predictor.py` & `fxn-0.0.9/fxn/api/predictor.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/fxn/api/profile.py` & `fxn-0.0.9/fxn/api/profile.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/fxn/api/storage.py` & `fxn-0.0.9/fxn/api/storage.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/fxn/api/tag.py` & `fxn-0.0.9/fxn/api/tag.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/fxn/api/user.py` & `fxn-0.0.9/fxn/api/user.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/fxn/cli/auth.py` & `fxn-0.0.9/fxn/cli/auth.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.8/fxn/cli/misc.py` & `fxn-0.0.9/fxn/cli/misc.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,26 +6,22 @@
 from rich import print
 from typer import Exit, Option
 from typing import Callable
 from webbrowser import open as open_browser
 
 from ..version import __version__
 
-def create_learn_callback (url: str) -> Callable[[bool], None]:
-    # Define callback
-    def callback (value: bool):
-        if value:
-            open_browser(url)
-            raise Exit()
-    # Return
-    return callback
+def _learn_callback (value: bool):
+    if value:
+        open_browser("https://docs.fxn.ai")
+        raise Exit()
 
 def _version_callback (value: bool):
     if value:
         print(__version__)
         raise Exit()
 
 def cli_options (
-    learn: bool = Option(None, "--learn", callback=create_learn_callback("https://docs.fxn.ai"), help="Learn about Function."),
+    learn: bool = Option(None, "--learn", callback=_learn_callback, help="Learn about Function."),
     version: bool = Option(None, "--version", callback=_version_callback, help="Get the Function CLI version.")
 ):
     pass
```

### Comparing `fxn-0.0.8/fxn/cli/predict.py` & `fxn-0.0.9/fxn/cli/predict.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     prediction = Prediction.create(
         tag=tag,
         **inputs,
         raw_outputs=raw_outputs,
         access_key=get_access_key()
     )
     # Parse results
-    if hasattr(prediction, "results"):
+    images = []
+    if hasattr(prediction, "results") and prediction.results is not None:
         images = [feature for feature in prediction.results if isinstance(feature, Image.Image)]
         results = [_serialize_feature(feature) for feature in prediction.results]
         object.__setattr__(prediction, "results", results)
     # Print
     print_json(data=asdict(prediction))
     # Show images
     for image in images:
```

### Comparing `fxn-0.0.8/fxn/cli/predictors.py` & `fxn-0.0.9/fxn/cli/predictors.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,50 +2,44 @@
 #   Function
 #   Copyright © 2023 NatML Inc. All Rights Reserved.
 #
 
 from dataclasses import asdict
 from rich import print_json
 from pathlib import Path
-from typer import Argument, Option, Typer
+from typer import Argument, Option
 from typing import List
 
 from ..api import Acceleration, AccessMode, Predictor, PredictorType
 from .auth import get_access_key
-from .misc import create_learn_callback
 
-app = Typer(no_args_is_help=True)
-
-@app.command(name="retrieve", help="Retrieve a predictor.")
 def retrieve_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ):
     predictor = Predictor.retrieve(
         tag=tag,
         access_key=get_access_key()
     )
     predictor = asdict(predictor) if predictor else None
     print_json(data=predictor)
 
-@app.command(name="search", help="Search predictors.")
 def search_predictors (
     query: str=Argument(..., help="Search query."),
     offset: int=Option(None, help="Pagination offset."),
     count: int=Option(None, help="Pagination count.")
 ):
     predictors = Predictor.search(
         query=query,
         offset=offset,
         count=count,
         access_key=get_access_key()
     )
     predictors = [asdict(predictor) for predictor in predictors]
     print_json(data=predictors)
 
-@app.command(name="create", help="Create a predictor.")
 def create_predictor (
     tag: str=Argument(..., help="Predictor tag."),
     notebook: Path=Argument(..., help="Path to predictor notebook."),
     type: PredictorType=Option(None, case_sensitive=False, help="Predictor type. This defaults to `CLOUD`."),
     access: AccessMode=Option(None, case_sensitive=False, help="Predictor access mode. This defaults to `PUBLIC`."),
     description: str=Option(None, help="Predictor description. This supports Markdown."),
     media: Path=Option(None, help="Predictor image path."),
@@ -67,32 +61,24 @@
         license=license,
         overwrite=overwrite,
         access_key=get_access_key()
     )
     predictor = asdict(predictor)
     print_json(data=predictor)
 
-@app.command(name="delete", help="Delete a predictor.")
 def delete_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ):
     result = Predictor.delete(
         tag=tag,
         access_key=get_access_key()
     )
     print_json(data=result)
 
-@app.command(name="archive", help="Archive an active predictor.")
 def archive_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ):
     predictor = Predictor.archive(
         tag=tag,
         access_key=get_access_key()
     )
-    print_json(data=asdict(predictor))
-
-@app.callback()
-def predictor_options (
-    learn: bool = Option(None, "--learn", callback=create_learn_callback("https://docs.fxn.ai/predictors"), help="Learn about predictors in Function.")
-):
-    pass
+    print_json(data=asdict(predictor))
```

### Comparing `fxn-0.0.8/fxn.egg-info/PKG-INFO` & `fxn-0.0.9/fxn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.8
+Version: 0.0.9
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.8/fxn.egg-info/SOURCES.txt` & `fxn-0.0.9/fxn.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 LICENSE
 README.md
 setup.py
 fxn/__init__.py
+fxn/magic.py
 fxn/version.py
 fxn.egg-info/PKG-INFO
 fxn.egg-info/SOURCES.txt
 fxn.egg-info/dependency_links.txt
 fxn.egg-info/entry_points.txt
 fxn.egg-info/requires.txt
 fxn.egg-info/top_level.txt
 fxn/api/__init__.py
 fxn/api/api.py
 fxn/api/dtype.py
+fxn/api/environment.py
 fxn/api/feature.py
 fxn/api/featureinput.py
 fxn/api/prediction.py
 fxn/api/predictor.py
 fxn/api/profile.py
 fxn/api/storage.py
 fxn/api/tag.py
 fxn/api/user.py
 fxn/cli/__init__.py
 fxn/cli/auth.py
+fxn/cli/env.py
 fxn/cli/misc.py
 fxn/cli/predict.py
-fxn/cli/predictors.py
-fxn/cli/users.py
+fxn/cli/predictors.py
```

### Comparing `fxn-0.0.8/setup.py` & `fxn-0.0.9/setup.py`

 * *Files identical despite different names*

