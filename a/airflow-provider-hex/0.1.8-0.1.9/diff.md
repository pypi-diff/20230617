# Comparing `tmp/airflow-provider-hex-0.1.8.tar.gz` & `tmp/airflow-provider-hex-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow-provider-hex-0.1.8.tar", last modified: Mon Jan  9 05:01:00 2023, max compression
+gzip compressed data, was "airflow-provider-hex-0.1.9.tar", last modified: Sat Jun 17 03:35:17 2023, max compression
```

## Comparing `airflow-provider-hex-0.1.8.tar` & `airflow-provider-hex-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-09 05:01:00.294003 airflow-provider-hex-0.1.8/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3010 2023-01-09 05:01:00.294003 airflow-provider-hex-0.1.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2232 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/VERSION.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-09 05:01:00.294003 airflow-provider-hex-0.1.8/airflow_provider_hex/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/airflow_provider_hex/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-09 05:01:00.294003 airflow-provider-hex-0.1.8/airflow_provider_hex/hooks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/airflow_provider_hex/hooks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7088 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/airflow_provider_hex/hooks/hex.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-09 05:01:00.294003 airflow-provider-hex-0.1.8/airflow_provider_hex/operators/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/airflow_provider_hex/operators/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3404 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/airflow_provider_hex/operators/hex.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      488 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/airflow_provider_hex/types.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-01-09 05:01:00.294003 airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3010 2023-01-09 05:01:00.000000 airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      593 2023-01-09 05:01:00.000000 airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-01-09 05:01:00.000000 airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2023-01-09 05:01:00.000000 airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-01-09 05:00:22.000000 airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      183 2023-01-09 05:01:00.000000 airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2023-01-09 05:01:00.000000 airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1824 2023-01-09 05:01:00.294003 airflow-provider-hex-0.1.8/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       38 2023-01-09 05:00:19.000000 airflow-provider-hex-0.1.8/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-17 03:35:16.994929 airflow-provider-hex-0.1.9/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       20 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3422 2023-06-17 03:35:16.994929 airflow-provider-hex-0.1.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2644 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/VERSION.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-17 03:35:16.990929 airflow-provider-hex-0.1.9/airflow_provider_hex/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/airflow_provider_hex/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-17 03:35:16.990929 airflow-provider-hex-0.1.9/airflow_provider_hex/hooks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/airflow_provider_hex/hooks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7316 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/airflow_provider_hex/hooks/hex.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-17 03:35:16.994929 airflow-provider-hex-0.1.9/airflow_provider_hex/operators/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/airflow_provider_hex/operators/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3714 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/airflow_provider_hex/operators/hex.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1010 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/airflow_provider_hex/types.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-17 03:35:16.990929 airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3422 2023-06-17 03:35:16.000000 airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      593 2023-06-17 03:35:16.000000 airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-17 03:35:16.000000 airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2023-06-17 03:35:16.000000 airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-17 03:34:39.000000 airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      183 2023-06-17 03:35:16.000000 airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2023-06-17 03:35:16.000000 airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1824 2023-06-17 03:35:16.994929 airflow-provider-hex-0.1.9/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       38 2023-06-17 03:34:37.000000 airflow-provider-hex-0.1.9/setup.py
```

### Comparing `airflow-provider-hex-0.1.8/PKG-INFO` & `airflow-provider-hex-0.1.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: airflow-provider-hex
-Version: 0.1.8
-Summary: Apache Airflow Hex provider containing Hooks and Operators
-Home-page: https://github.com/hex-inc/airflow-provider-hex
-Author: Pedram Navid
-Author-email: pedram@pedramnavid.com
-License: Apache License 2.0
-Project-URL: Source Code, https://github.com/hex-inc/airflow-provider-hex
-Project-URL: Homepage, https://github.com/hex-inc/airflow-provider-hex
-Project-URL: Changelog, https://github.com/hex-inc/airflow-provider-hex/blob/main/CHANGELOG.md
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # Hex Airflow Provider
 
 Provides an Airflow Operator and Hook to trigger Hex project runs.
 
 This [Airflow Provider Package](https://airflow.apache.org/docs/apache-airflow-providers/)
 provides Hooks and Operators for interacting with the Hex API.
 
@@ -59,14 +40,17 @@
 
 In the asynchronous mode, the Operator will request that a Hex Project is run,
 but will not poll for completion. This can be useful for long-running projects.
 
 The operator accepts inputs in the form of a dictionary. These can be used to
 override existing input elements in your Hex project.
 
+You may also optionally include notifications for a particular run. See
+the [Hex API documentation](https://learn.hex.tech/docs/develop-logic/hex-api/api-reference#operation/RunProject) for details.
+
 ## Hooks
 
 The [`airflow_provider_hex.hooks.hex.HexHook`](/airflow_provider_hex/hooks/hex.py)
 provides a low-level interface to the Hex API.
 
 These can be useful for testing and development, as they provide both a generic
 `run` method which sends an authenticated request to the Hex API, as well as
@@ -77,16 +61,25 @@
 
 A simplified example DAG demonstrates how to use the [Airflow Operator](/example_dags/example_hex.py)
 
 ```python
 from airflow_provider_hex.operators.hex import HexRunProjectOperator
 
 PROJ_ID = 'abcdef-ghijkl-mnopq'
+notifications: list[NotificationDetails] = [
+    {
+        "type": "SUCCESS",
+        "includeSuccessScreenshot": True,
+        "slackChannelIds": ["HEX666SQG"],
+        "userIds": [],
+        "groupIds": [],
+    }
+]
 ...
 sync_run = HexRunProjectOperator(
     task_id="run",
     hex_conn_id="hex_default",
     project_id=PROJ_ID,
     dag=dag,
-    input_parameters={'myParam': 42}
+    notifications=notifications
 )
 ```
```

### Comparing `airflow-provider-hex-0.1.8/README.md` & `airflow-provider-hex-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: airflow-provider-hex
+Version: 0.1.9
+Summary: Apache Airflow Hex provider containing Hooks and Operators
+Home-page: https://github.com/hex-inc/airflow-provider-hex
+Author: Pedram Navid
+Author-email: pedram@pedramnavid.com
+License: Apache License 2.0
+Project-URL: Source Code, https://github.com/hex-inc/airflow-provider-hex
+Project-URL: Homepage, https://github.com/hex-inc/airflow-provider-hex
+Project-URL: Changelog, https://github.com/hex-inc/airflow-provider-hex/blob/main/CHANGELOG.md
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+
 # Hex Airflow Provider
 
 Provides an Airflow Operator and Hook to trigger Hex project runs.
 
 This [Airflow Provider Package](https://airflow.apache.org/docs/apache-airflow-providers/)
 provides Hooks and Operators for interacting with the Hex API.
 
@@ -40,14 +59,17 @@
 
 In the asynchronous mode, the Operator will request that a Hex Project is run,
 but will not poll for completion. This can be useful for long-running projects.
 
 The operator accepts inputs in the form of a dictionary. These can be used to
 override existing input elements in your Hex project.
 
+You may also optionally include notifications for a particular run. See
+the [Hex API documentation](https://learn.hex.tech/docs/develop-logic/hex-api/api-reference#operation/RunProject) for details.
+
 ## Hooks
 
 The [`airflow_provider_hex.hooks.hex.HexHook`](/airflow_provider_hex/hooks/hex.py)
 provides a low-level interface to the Hex API.
 
 These can be useful for testing and development, as they provide both a generic
 `run` method which sends an authenticated request to the Hex API, as well as
@@ -58,16 +80,25 @@
 
 A simplified example DAG demonstrates how to use the [Airflow Operator](/example_dags/example_hex.py)
 
 ```python
 from airflow_provider_hex.operators.hex import HexRunProjectOperator
 
 PROJ_ID = 'abcdef-ghijkl-mnopq'
+notifications: list[NotificationDetails] = [
+    {
+        "type": "SUCCESS",
+        "includeSuccessScreenshot": True,
+        "slackChannelIds": ["HEX666SQG"],
+        "userIds": [],
+        "groupIds": [],
+    }
+]
 ...
 sync_run = HexRunProjectOperator(
     task_id="run",
     hex_conn_id="hex_default",
     project_id=PROJ_ID,
     dag=dag,
-    input_parameters={'myParam': 42}
+    notifications=notifications
 )
 ```
```

### Comparing `airflow-provider-hex-0.1.8/airflow_provider_hex/__init__.py` & `airflow-provider-hex-0.1.9/airflow_provider_hex/__init__.py`

 * *Files identical despite different names*

### Comparing `airflow-provider-hex-0.1.8/airflow_provider_hex/hooks/hex.py` & `airflow-provider-hex-0.1.9/airflow_provider_hex/hooks/hex.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import datetime
 import time
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, List, Optional, cast
 from urllib.parse import urljoin
 
 import requests
 from airflow.exceptions import AirflowException
 from airflow.hooks.base import BaseHook
 from importlib_metadata import PackageNotFoundError, version
 
-from airflow_provider_hex.types import RunResponse, StatusResponse
+from airflow_provider_hex.types import NotificationDetails, RunResponse, StatusResponse
 
 PENDING = "PENDING"
 RUNNING = "RUNNING"
 KILLED = "KILLED"
 ERRORED = "ERRORED"
 COMPLETE = "COMPLETED"
 UNABLE_TO_ALLOCATE_KERNEL = "UNABLE_TO_ALLOCATE_KERNEL"
@@ -126,22 +126,26 @@
         return {"response": response.text}
 
     def run_project(
         self,
         project_id: str,
         inputs: Optional[Dict[str, Any]] = None,
         update_cache: bool = False,
+        notifications: List[NotificationDetails] = [],
     ) -> RunResponse:
         endpoint = f"/api/v1/project/{project_id}/run"
         method = "POST"
 
         data: Dict[str, Any] = {"updateCache": update_cache}
         if inputs:
             data["inputParams"] = inputs
 
+        if notifications:
+            data["notifications"] = notifications
+
         return cast(
             RunResponse,
             self.run(
                 method=method,
                 endpoint=endpoint,
                 data=data,
             ),
@@ -166,16 +170,17 @@
         self,
         project_id: str,
         inputs: Optional[dict],
         update_cache: bool = False,
         poll_interval: int = 3,
         poll_timeout: int = 600,
         kill_on_timeout: bool = True,
+        notifications: List[NotificationDetails] = [],
     ):
-        run_response = self.run_project(project_id, inputs, update_cache)
+        run_response = self.run_project(project_id, inputs, update_cache, notifications)
         run_id = run_response["runId"]
 
         poll_start = datetime.datetime.now()
         while True:
             run_status = self.run_status(project_id, run_id)
             project_status = run_status["status"]
 
@@ -195,15 +200,14 @@
                 )
 
             if (
                 poll_timeout
                 and datetime.datetime.now()
                 > poll_start + datetime.timedelta(seconds=poll_timeout)
             ):
-
                 self.log.error(
                     "Failed to complete project within %s seconds, cancelling run",
                     poll_timeout,
                 )
                 if kill_on_timeout:
                     self.cancel_run(project_id, run_id)
                 raise AirflowException(
```

### Comparing `airflow-provider-hex-0.1.8/airflow_provider_hex/operators/hex.py` & `airflow-provider-hex-0.1.9/airflow_provider_hex/operators/hex.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 from airflow.models import BaseOperator
 from airflow.models.dag import Context
 from airflow.utils.decorators import apply_defaults
 
 from airflow_provider_hex.hooks.hex import HexHook
+from airflow_provider_hex.types import NotificationDetails
 
 
 class HexRunProjectOperator(BaseOperator):
     """Runs a Hex Project, and optionally waits until completion.
 
     :param project_id: Hex Project ID
     :type project_id: str
@@ -47,41 +48,48 @@
         hex_conn_id: str = "hex_default",
         synchronous: bool = True,
         wait_seconds: int = 3,
         timeout: int = 3600,
         kill_on_timeout: bool = True,
         input_parameters: Optional[Dict[str, Any]] = None,
         update_cache: bool = False,
+        notifications: List[NotificationDetails] = [],
         **kwargs,
     ) -> None:
         super().__init__(**kwargs)
         self.project_id = project_id
         self.hex_conn_id = hex_conn_id
         self.synchronous = synchronous
         self.wait_seconds = wait_seconds
         self.timeout = timeout
         self.kill_on_timeout = kill_on_timeout
         self.input_parameters = input_parameters
         self.update_cache = update_cache
+        self.notifications = notifications
 
     def execute(self, context: Context) -> Any:
         hook = HexHook(self.hex_conn_id)
 
         if self.synchronous:
             self.log.info("Starting Hex Project")
             resp = hook.run_and_poll(
                 self.project_id,
                 inputs=self.input_parameters,
                 update_cache=self.update_cache,
                 poll_interval=self.wait_seconds,
                 poll_timeout=self.timeout,
                 kill_on_timeout=self.kill_on_timeout,
+                notifications=self.notifications,
             )
             self.log.info("Hex Project completed successfully")
 
         else:
             self.log.info("Starting Hex Project asynchronously")
-            resp = hook.run_project(self.project_id, inputs=self.input_parameters)
+            resp = hook.run_project(
+                self.project_id,
+                inputs=self.input_parameters,
+                notifications=self.notifications,
+            )
             self.log.info("Hex Project started successfully.")
 
         self.log.info(resp)
         return resp
```

### Comparing `airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/PKG-INFO` & `airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-provider-hex
-Version: 0.1.8
+Version: 0.1.9
 Summary: Apache Airflow Hex provider containing Hooks and Operators
 Home-page: https://github.com/hex-inc/airflow-provider-hex
 Author: Pedram Navid
 Author-email: pedram@pedramnavid.com
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/hex-inc/airflow-provider-hex
 Project-URL: Homepage, https://github.com/hex-inc/airflow-provider-hex
@@ -59,14 +59,17 @@
 
 In the asynchronous mode, the Operator will request that a Hex Project is run,
 but will not poll for completion. This can be useful for long-running projects.
 
 The operator accepts inputs in the form of a dictionary. These can be used to
 override existing input elements in your Hex project.
 
+You may also optionally include notifications for a particular run. See
+the [Hex API documentation](https://learn.hex.tech/docs/develop-logic/hex-api/api-reference#operation/RunProject) for details.
+
 ## Hooks
 
 The [`airflow_provider_hex.hooks.hex.HexHook`](/airflow_provider_hex/hooks/hex.py)
 provides a low-level interface to the Hex API.
 
 These can be useful for testing and development, as they provide both a generic
 `run` method which sends an authenticated request to the Hex API, as well as
@@ -77,16 +80,25 @@
 
 A simplified example DAG demonstrates how to use the [Airflow Operator](/example_dags/example_hex.py)
 
 ```python
 from airflow_provider_hex.operators.hex import HexRunProjectOperator
 
 PROJ_ID = 'abcdef-ghijkl-mnopq'
+notifications: list[NotificationDetails] = [
+    {
+        "type": "SUCCESS",
+        "includeSuccessScreenshot": True,
+        "slackChannelIds": ["HEX666SQG"],
+        "userIds": [],
+        "groupIds": [],
+    }
+]
 ...
 sync_run = HexRunProjectOperator(
     task_id="run",
     hex_conn_id="hex_default",
     project_id=PROJ_ID,
     dag=dag,
-    input_parameters={'myParam': 42}
+    notifications=notifications
 )
 ```
```

### Comparing `airflow-provider-hex-0.1.8/airflow_provider_hex.egg-info/SOURCES.txt` & `airflow-provider-hex-0.1.9/airflow_provider_hex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airflow-provider-hex-0.1.8/pyproject.toml` & `airflow-provider-hex-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `airflow-provider-hex-0.1.8/setup.cfg` & `airflow-provider-hex-0.1.9/setup.cfg`

 * *Files identical despite different names*

