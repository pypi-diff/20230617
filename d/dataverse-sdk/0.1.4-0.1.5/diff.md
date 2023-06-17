# Comparing `tmp/dataverse-sdk-0.1.4.tar.gz` & `tmp/dataverse-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse-sdk-0.1.4.tar", last modified: Tue Jun 13 10:18:31 2023, max compression
+gzip compressed data, was "dataverse-sdk-0.1.5.tar", last modified: Sat Jun 17 06:47:36 2023, max compression
```

## Comparing `dataverse-sdk-0.1.4.tar` & `dataverse-sdk-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.396193 dataverse-sdk-0.1.4/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5983 2023-06-13 10:18:31.396077 dataverse-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5743 2023-05-24 06:41:33.000000 dataverse-sdk-0.1.4/README.md
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.393017 dataverse-sdk-0.1.4/dataverse_sdk/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/__init__.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.394163 dataverse-sdk-0.1.4/dataverse_sdk/apis/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/apis/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    10144 2023-06-13 10:15:56.000000 dataverse-sdk-0.1.4/dataverse_sdk/apis/backend.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    20188 2023-06-13 10:15:56.000000 dataverse-sdk-0.1.4/dataverse_sdk/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1550 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/connections.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      587 2023-06-09 02:47:03.000000 dataverse-sdk-0.1.4/dataverse_sdk/constants.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.394389 dataverse-sdk-0.1.4/dataverse_sdk/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/exceptions/client.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.395465 dataverse-sdk-0.1.4/dataverse_sdk/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     3036 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.4/dataverse_sdk/schemas/api.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     9954 2023-06-13 10:15:56.000000 dataverse-sdk-0.1.4/dataverse_sdk/schemas/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1164 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/schemas/common.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.395857 dataverse-sdk-0.1.4/dataverse_sdk/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      371 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.4/dataverse_sdk/utils/utils.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-13 10:18:31.393952 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     5983 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       18 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2023-06-13 10:18:31.000000 dataverse-sdk-0.1.4/dataverse_sdk.egg-info/top_level.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-06-13 10:18:31.396228 dataverse-sdk-0.1.4/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      613 2023-06-13 10:15:56.000000 dataverse-sdk-0.1.4/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.760347 dataverse-sdk-0.1.5/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     6110 2023-06-17 06:47:36.760228 dataverse-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     5870 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/README.md
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.757609 dataverse-sdk-0.1.5/dataverse_sdk/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/__init__.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.758539 dataverse-sdk-0.1.5/dataverse_sdk/apis/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/apis/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    10397 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/apis/backend.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    21842 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1550 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/connections.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      587 2023-06-09 02:47:03.000000 dataverse-sdk-0.1.5/dataverse_sdk/constants.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.758802 dataverse-sdk-0.1.5/dataverse_sdk/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       49 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/exceptions/client.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.759668 dataverse-sdk-0.1.5/dataverse_sdk/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     3036 2023-05-17 07:09:24.000000 dataverse-sdk-0.1.5/dataverse_sdk/schemas/api.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    10179 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/schemas/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1164 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/schemas/common.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.760024 dataverse-sdk-0.1.5/dataverse_sdk/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-05-12 08:24:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      657 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/dataverse_sdk/utils/utils.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2023-06-17 06:47:36.758339 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     6110 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       18 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2023-06-17 06:47:36.000000 dataverse-sdk-0.1.5/dataverse_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2023-06-17 06:47:36.760382 dataverse-sdk-0.1.5/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      613 2023-06-17 03:34:04.000000 dataverse-sdk-0.1.5/setup.py
```

### Comparing `dataverse-sdk-0.1.4/PKG-INFO` & `dataverse-sdk-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
@@ -181,16 +181,16 @@
 
 ```Python
 model = client.get_model(model_id=30)
 model = project.get_model(model_id=30)
 ```
 From the given model, we could get the label file and the triton model file by the commands below.
 ```Python
-model.get_label_file()
-model.get_triton_model_file()
+status, label_file_path = model.get_label_file(save_path="./labels.txt", timeout=6000)
+status, label_file_path = model.get_triton_model_file(save_path="./model.zip", timeout=6000)
 
 ```
 
 
 ## Troubleshooting
```

### Comparing `dataverse-sdk-0.1.4/README.md` & `dataverse-sdk-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -171,16 +171,16 @@
 
 ```Python
 model = client.get_model(model_id=30)
 model = project.get_model(model_id=30)
 ```
 From the given model, we could get the label file and the triton model file by the commands below.
 ```Python
-model.get_label_file()
-model.get_triton_model_file()
+status, label_file_path = model.get_label_file(save_path="./labels.txt", timeout=6000)
+status, label_file_path = model.get_triton_model_file(save_path="./model.zip", timeout=6000)
 
 ```
 
 
 ## Troubleshooting
```

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk/__init__.py` & `dataverse-sdk-0.1.5/dataverse_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk/apis/backend.py` & `dataverse-sdk-0.1.5/dataverse_sdk/apis/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import inspect
 import json
 import logging
-from io import BytesIO
 from typing import Optional, Union
 from urllib.parse import urlencode
 
 import requests
 from requests import sessions
 from requests.adapters import HTTPAdapter, Retry
 
@@ -44,14 +43,15 @@
     def send_request(
         self,
         url: str,
         method: str,
         attempts: int = 1,
         max_attempts: int = 5,
         data: Optional[Union[str, dict]] = None,
+        timeout: int = 3000,
         **kwargs,
     ):
         if attempts > max_attempts:
             msg = "Exceeds max attempts."
             logger.error(msg)
             raise Exception(msg)
 
@@ -62,15 +62,17 @@
             data = json.dumps(data)
 
         parent_func = inspect.stack()[2][3]
         try:
             with sessions.Session() as session:
                 session.mount("http://", self.adapter)
                 session.mount("https://", self.adapter)
-                resp = session.request(method=method, url=url, data=data, **kwargs)
+                resp = session.request(
+                    method=method, url=url, data=data, timeout=timeout, **kwargs
+                )
         except requests.exceptions.Timeout:
             logger.warning(f"Request timeout: {method} {url}")
             raise
         except requests.exceptions.HTTPError as e:
             logger.error(f"Invalid http: {repr(e)}")
             raise
         except requests.exceptions.ConnectionError as e:
@@ -201,27 +203,35 @@
         resp = self.send_request(
             url=f"{self.host}/api/ml_models/{model_id}/",
             method="get",
             headers=self.headers,
         )
         return resp.json()
 
-    def get_ml_model_labels(self, model_id: int) -> Optional[BytesIO]:
+    def get_ml_model_labels(
+        self, model_id: int, timeout: int = 3000
+    ) -> requests.models.Response:
         resp = self.send_request(
             url=f"{self.host}/api/ml_models/{model_id}/labels/",
             method="get",
             headers=self.headers,
+            stream=True,
+            timeout=timeout,
         )
         return resp
 
-    def get_ml_model_file(self, model_id: int) -> Optional[BytesIO]:
+    def get_ml_model_file(
+        self, model_id: int, timeout: int = 3000
+    ) -> requests.models.Response:
         resp = self.send_request(
             url=f"{self.host}/api/ml_models/{model_id}/model/",
             method="get",
             headers=self.headers,
+            stream=True,
+            timeout=timeout,
         )
         return resp
 
     def create_dataset(
         self,
         name: str,
         data_source: str,
```

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk/client.py` & `dataverse-sdk-0.1.5/dataverse_sdk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from io import BytesIO
+import logging
 from os.path import isfile
 from typing import Optional
 
 from pydantic import ValidationError
 
 from .apis.backend import BackendAPI
 from .connections import add_connection, get_connection
@@ -21,15 +21,15 @@
     MLModel,
     Ontology,
     Project,
     ProjectTag,
     Sensor,
 )
 from .schemas.common import AnnotationFormat, DatasetType, OntologyImageType, SensorType
-from .utils.utils import get_filepaths
+from .utils.utils import download_file_from_response, get_filepaths
 
 
 class DataverseClient:
     def __init__(
         self,
         host: DataverseHost,
         email: Optional[str] = None,
@@ -339,39 +339,83 @@
         if project is None:
             project = client.get_project(project_id=model_data["project"]["id"])
         model_data.update({"id": model_id, "project": project})
         return MLModel.create(model_data)
 
     @staticmethod
     def get_label_file(
-        model_id: int, client: Optional["DataverseClient"] = None
-    ) -> Optional[BytesIO]:
+        model_id: int,
+        save_path: str = "./labels.txt",
+        timeout: int = 3000,
+        client: Optional["DataverseClient"] = None,
+    ) -> tuple[bool, str]:
+        """Download the model label file (which is a string txt file)
+
+        Parameters
+        ----------
+        model_id : int
+        save_path : str, optional
+            local path for saving the label_file, by default './labels.txt'
+        timeout : int, optional
+            maximum timeout of the request, by default 3000
+        client : Optional[&quot;DataverseClient&quot;], optional
+            client class, by default None
+
+        Returns
+        -------
+        (status, save_path): tuple[bool, str]
+            the first item means whether the download success or not
+            the second item shows the save_path
+        """
         if client is None:
             client = DataverseClient.get_client()
         api = client._api_client
         try:
-            labels: BytesIO = api.get_ml_model_labels(model_id=model_id)
+            resp = api.get_ml_model_labels(model_id=model_id, timeout=timeout)
+            download_file_from_response(response=resp, save_path=save_path)
+            return True, save_path
         except Exception as e:
-            raise ClientConnectionError(f"Failed to get model labels: {e}")
-        if labels:
-            return labels
+            logging.exception("Fail to get model label file", e)
+            return False, save_path
 
     @staticmethod
     def get_triton_model_file(
-        model_id: int, client: Optional["DataverseClient"] = None
-    ) -> Optional[BytesIO]:
+        model_id: int,
+        save_path: str = "./model.zip",
+        timeout: int = 3000,
+        client: Optional["DataverseClient"] = None,
+    ) -> tuple[bool, str]:
+        """Download the triton model file (which is a zip file)
+
+        Parameters
+        ----------
+        model_id : int
+        save_path : str, optional
+            local path for saving the triton model file, by default './model.zip'
+        timeout : int, optional
+            maximum timeout of the request, by default 3000
+        client : Optional[&quot;DataverseClient&quot;], optional
+            client class, by default None
+
+        Returns
+        -------
+        (status, save_path): tuple[bool, str]
+            the first item means whether the download success or not
+            the second item shows the save_path
+        """
         if client is None:
             client = DataverseClient.get_client()
         api = client._api_client
         try:
-            model_file: BytesIO = api.get_ml_model_file(model_id=model_id)
+            resp = api.get_ml_model_file(model_id=model_id, timeout=timeout)
+            download_file_from_response(response=resp, save_path=save_path)
+            return True, save_path
         except Exception as e:
-            raise ClientConnectionError(f"Failed to get triton model file: {e}")
-        if model_file:
-            return model_file
+            logging.exception("Failed to get triton model file", e)
+            return False, save_path
 
     def get_dataset(self, dataset_id: int):
         """Get dataset detail and status by id
 
         Parameters
         ----------
         dataset_id : int
```

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk/connections.py` & `dataverse-sdk-0.1.5/dataverse_sdk/connections.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk/constants.py` & `dataverse-sdk-0.1.5/dataverse_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk/schemas/api.py` & `dataverse-sdk-0.1.5/dataverse_sdk/schemas/api.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk/schemas/client.py` & `dataverse-sdk-0.1.5/dataverse_sdk/schemas/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,18 +327,24 @@
             name=model_data["name"],
             project=project,
             classes=classes,
             updated_at=model_data["updated_at"],
             triton_model_name=model_data["triton_model_name"],
         )
 
-    def get_label_file(self) -> dict:
+    def get_label_file(
+        self, save_path: str = "./labels.txt", timeout: int = 3000
+    ) -> tuple[bool, str]:
         from ..client import DataverseClient
 
-        labels: dict = DataverseClient.get_label_file(model_id=self.id)
-        return labels
+        return DataverseClient.get_label_file(
+            model_id=self.id, save_path=save_path, timeout=timeout
+        )
 
-    def get_triton_model_file(self):
+    def get_triton_model_file(
+        self, save_path: str = "./model.zip", timeout: int = 3000
+    ) -> tuple[bool, str]:
         from ..client import DataverseClient
 
-        model_file = DataverseClient.get_triton_model_file(model_id=self.id)
-        return model_file
+        return DataverseClient.get_triton_model_file(
+            model_id=self.id, save_path=save_path, timeout=timeout
+        )
```

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk/schemas/common.py` & `dataverse-sdk-0.1.5/dataverse_sdk/schemas/common.py`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk.egg-info/PKG-INFO` & `dataverse-sdk-0.1.5/dataverse_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 0.1.4
+Version: 0.1.5
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
 
@@ -181,16 +181,16 @@
 
 ```Python
 model = client.get_model(model_id=30)
 model = project.get_model(model_id=30)
 ```
 From the given model, we could get the label file and the triton model file by the commands below.
 ```Python
-model.get_label_file()
-model.get_triton_model_file()
+status, label_file_path = model.get_label_file(save_path="./labels.txt", timeout=6000)
+status, label_file_path = model.get_triton_model_file(save_path="./model.zip", timeout=6000)
 
 ```
 
 
 ## Troubleshooting
```

### Comparing `dataverse-sdk-0.1.4/dataverse_sdk.egg-info/SOURCES.txt` & `dataverse-sdk-0.1.5/dataverse_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse-sdk-0.1.4/setup.py` & `dataverse-sdk-0.1.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "dataverse-sdk"
-PACKAGE_VERSION = "0.1.4"
+PACKAGE_VERSION = "0.1.5"
 DESC = "Dataverse SDK For Python"
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
```

