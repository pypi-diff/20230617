# Comparing `tmp/braintrust-0.0.4.tar.gz` & `tmp/braintrust-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust-0.0.4.tar", last modified: Sat Jun 10 17:46:57 2023, max compression
+gzip compressed data, was "braintrust-0.0.5.tar", last modified: Sat Jun 17 20:20:38 2023, max compression
```

## Comparing `braintrust-0.0.4.tar` & `braintrust-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-10 17:46:57.559114 braintrust-0.0.4/
--rw-r--r--   0 ankur      (501) staff       (20)      463 2023-06-10 17:46:57.558983 braintrust-0.0.4/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.4/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-10 17:46:57.559152 braintrust-0.0.4/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1582 2023-06-06 15:10:19.000000 braintrust-0.0.4/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-10 17:46:57.557287 braintrust-0.0.4/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-10 17:46:57.558103 braintrust-0.0.4/src/braintrust/
--rw-r--r--   0 ankur      (501) staff       (20)    16049 2023-06-10 17:46:14.000000 braintrust-0.0.4/src/braintrust/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)      123 2023-05-14 19:33:59.000000 braintrust-0.0.4/src/braintrust/cache.py
--rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.4/src/braintrust/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-10 17:46:14.000000 braintrust-0.0.4/src/braintrust/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-10 17:46:57.558813 braintrust-0.0.4/src/braintrust.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      463 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      347 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/entry_points.txt
--rw-r--r--   0 ankur      (501) staff       (20)      251 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-10 17:46:57.000000 braintrust-0.0.4/src/braintrust.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.555220 braintrust-0.0.5/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-17 20:20:38.555093 braintrust-0.0.5/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.5/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-17 20:20:38.555256 braintrust-0.0.5/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1623 2023-06-17 20:17:20.000000 braintrust-0.0.5/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.552139 braintrust-0.0.5/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.553587 braintrust-0.0.5/src/braintrust/
+-rw-r--r--   0 ankur      (501) staff       (20)    17955 2023-06-17 20:19:20.000000 braintrust-0.0.5/src/braintrust/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)      123 2023-05-14 19:33:59.000000 braintrust-0.0.5/src/braintrust/cache.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.554586 braintrust-0.0.5/src/braintrust/cli/
+-rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1406 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/__main__.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.554935 braintrust-0.0.5/src/braintrust/cli/install/
+-rw-r--r--   0 ankur      (501) staff       (20)      472 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/install/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     8239 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/install/api.py
+-rw-r--r--   0 ankur      (501) staff       (20)     7240 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/install/redshift.py
+-rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.5/src/braintrust/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-12 19:52:09.000000 braintrust-0.0.5/src/braintrust/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.554378 braintrust-0.0.5/src/braintrust.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      521 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/entry_points.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      302 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/top_level.txt
```

### Comparing `braintrust-0.0.4/setup.py` & `braintrust-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 with open(os.path.join(dir_name, "README.md"), "r", encoding="utf-8") as f:
     long_description = f.read()
 
 install_requires = ["openai", "GitPython", "requests"]
 
 extras_require = {
+    "cli": ["boto3", "psycopg2-binary"],
     "dev": [
         "black",
         "build",
         "flake8",
         "flake8-isort",
         "IPython",
         "isort==5.10.1",
```

### Comparing `braintrust-0.0.4/src/braintrust/__init__.py` & `braintrust-0.0.5/src/braintrust/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 """
 import atexit
 import datetime
 import json
 import logging
 import os
 import queue
+import textwrap
 import threading
 import traceback
 import urllib.parse
 import uuid
 from functools import cache as _cache
 from getpass import getpass
 from typing import Any
@@ -62,14 +63,15 @@
 
 
 _state = BrainTrustState()
 _logger = logging.getLogger("braintrust")
 
 API_URL = None
 ORG_ID = None
+ORG_NAME = None
 LOG_URL = None
 
 
 class HTTPConnection:
     def __init__(self, base_url=API_URL):
         self.session = requests.Session()
         self.base_url = base_url
@@ -123,24 +125,23 @@
     return api_get("ping")
 
 
 class Project(ModelWrapper):
     _ENDPOINT = "projects"
 
     def __init__(self, name):
-        unique_key, insert_args = {"name": name}, {"org_id": _user_info()["organizations"][0]["id"]}
+        unique_key = {"name": name, "org_id": ORG_ID}
 
         # Can we have an upsert (or insert if not exists) method instead?
         existing = []
         if unique_key:
             existing = api_get(self._ENDPOINT, unique_key)
 
         if not existing:
-            insert_args.update(unique_key)
-            existing = api_insert(self._ENDPOINT, insert_args)
+            existing = api_insert(self._ENDPOINT, unique_key)
 
         if existing:
             self.data = existing[0]
         else:
             assert False, "Unable to find record in " + self._ENDPOINT
 
 
@@ -280,15 +281,16 @@
         while True:
             while len(items) < batch_size:
                 try:
                     items.append(self.queue.get_nowait())
                 except queue.Empty:
                     break
 
-            api_insert("logs", items)
+            if len(items) > 0:
+                api_insert("logs", items)
 
             if len(items) < batch_size:
                 break
 
             items.clear()
 
 
@@ -320,14 +322,32 @@
             args["description"] = description
 
         self.data = api_insert("register-experiment", args)[0]
         self.logger = _LogThread(name=name)
 
     def log(self, inputs, output, expected, scores, metadata=None):
         user_id = _user_info()["id"]
+
+        if not isinstance(scores, dict):
+            raise ValueError("scores must be a dictionary of names with scores")
+        for name, score in scores.items():
+            if not isinstance(name, str):
+                raise ValueError("score names must be strings")
+            if not isinstance(score, (int, float)):
+                raise ValueError("score values must be numbers")
+            if score < 0 or score > 1:
+                raise ValueError("score values must be between 0 and 1")
+
+        if metadata:
+            if not isinstance(metadata, dict):
+                raise ValueError("metadata must be a dictionary")
+            for key in metadata.keys():
+                if not isinstance(key, str):
+                    raise ValueError("metadata keys must be strings")
+
         args = {
             "id": str(uuid.uuid4()),
             "inputs": inputs,
             "output": output,
             "expected": expected,
             "scores": scores,
             "project_id": self.project.id,
@@ -340,34 +360,37 @@
             args["metadata"] = metadata
 
         self.logger.log(args)
         return args["id"]
 
     def summarize(self):
         # TODO: Show results so far here as well
-        org_name = _user_info()["organizations"][0]["name"]
-
-        project_url = f"{API_URL}/app/{urllib.parse.quote(org_name)}/p/{urllib.parse.quote(self.project.name)}"
+        project_url = f"{API_URL}/app/{urllib.parse.quote(ORG_NAME)}/p/{urllib.parse.quote(self.project.name)}"
         experiment_url = f"{project_url}/{urllib.parse.quote(self.name)}"
 
-        print(f"See results for all experiments in {self.project.name} at {project_url}")
-        print(f"See results for {self.name} at {experiment_url}")
+        return textwrap.dedent(
+            f"""
+        See results for all experiments in {self.project.name} at {project_url}
+        See results for {self.name} at {experiment_url}"""
+        )
 
 
-def init(project, experiment=None, description=None, api_url=None):
+def init(project, experiment=None, description=None, api_url=None, org_name=None, disable_cache=False):
     """
     Initialize a new experiment in a specified project. If the project does not exist, it will be created.
 
     :param project: The name of the project to create the experiment in.
     :param experiment: The name of the experiment to create. If not specified, a name will be generated automatically.
     :param description: An optional description of the experiment.
     :param api_url: The URL of the BrainTrust API to use. If not specified, the default will be used.
+    :param org_name: (Optional) The name of a specific organization to connect to. This is useful if you belong to multiple.
+    :param disable_cache: Do not use cached login information.
     :returns: The experiment object.
     """
-    kwargs = {}
+    kwargs = {"org_name": org_name, "disable_cache": disable_cache}
     if api_url:
         kwargs["api_url"] = api_url
     login(**kwargs)
 
     _state.current_project = Project(project)
     _state.current_experiment = Experiment(_state.current_project, name=experiment, description=description)
     return _state.current_experiment
@@ -391,50 +414,56 @@
     navigate your experiments while digging into analyses. However, we may later use these values to re-score outputs or
     fine-tune your models.
     :param scores: A dictionary of numeric values (between 0 and 1) to log. The scores should give you a variety of signals
     that help you determine how accurate the outputs are compared to what you expect and diagnose failures. For example, a
     summarization app might have one score that tells you how accurate the summary is, and another that measures the word similarity
     between the generated and grouth truth summary. The word similarity score could help you determine whether the summarization was
     covering similar concepts or not. You can use these scores to help you sort, filter, and compare experiments.
-    :param metadata: (Optional) a JSON-serializable object with additional data about the test example, model outputs, or just
+    :param metadata: (Optional) a dictionary with additional data about the test example, model outputs, or just
     about anything else that's relevant, that you can use to help find and analyze examples later. For example, you could log the
-    `prompt`, example's `id`, or anything else that would be useful to slice/dice later.
+    `prompt`, example's `id`, or anything else that would be useful to slice/dice later. The values in `metadata` can be any
+    JSON-serializable type, but its keys must be strings.
     :returns: The `id` of the logged event.
     """
 
     if not _state.current_experiment:
         raise Exception("Not initialized. Please call init() or login() first")
 
     return _state.current_experiment.log(
         inputs=inputs, output=output, expected=expected, scores=scores, metadata=metadata
     )
 
 
-def login(api_url=os.environ.get("BRAINTRUST_API_URL", "https://www.braintrustdata.com")):
+def login(
+    api_url=os.environ.get("BRAINTRUST_API_URL", "https://www.braintrustdata.com"), org_name=None, disable_cache=False
+):
     """
     Login to BrainTrust. This will prompt you for your API token, which you can find at
     https://www.braintrustdata.com/app/token. This method is called automatically by `init()`.
 
     :param api_url: The URL of the BrainTrust API. Defaults to https://www.braintrustdata.com.
+    :param org_name: (Optional) The name of a specific organization to connect to. This is useful if you belong to multiple.
+    :param disable_cache: Do not use cached login information.
     """
 
-    global API_URL, ORG_ID, LOG_URL
+    global API_URL, ORG_ID, ORG_NAME, LOG_URL
 
     API_URL = api_url
 
     os.makedirs(CACHE_PATH, exist_ok=True)
 
     api_info = None
     ping_ok = False
-    if os.path.exists(API_INFO_PATH):
+    if os.path.exists(API_INFO_PATH) and not disable_cache:
         with open(API_INFO_PATH) as f:
             api_info = json.load(f)
 
         LOG_URL = api_info.get("log_url")
         ORG_ID = api_info.get("org_id")
+        ORG_NAME = api_info.get("org_name")
         conn = api_conn()
 
         token = api_info.get("token")
         if token is not None:
             conn.set_token(token)
 
         ping_resp = conn.get("ping")
@@ -444,34 +473,48 @@
         resp = requests.post(
             _urljoin(API_URL, "/api/token/refresh"), json={"refresh_token": api_info.get("refresh_token")}
         )
         if resp.ok:
             resp_data = resp.json()
             token = resp_data["id_token"]
             refresh_token = resp_data.get("refresh_token")
-            _save_api_info({**api_info, "token": token, "refresh_token": refresh_token})
+
+            if not disable_cache:
+                _save_api_info({**api_info, "token": token, "refresh_token": refresh_token})
 
             conn.set_token(token)
             ping_resp = conn.get("ping")
             ping_ok = ping_resp.ok
         else:
             _logger.warning(f"Failed to refresh token: [{resp.status_code}] {resp.text}")
 
-    if not ping_ok:
+    if not ping_ok or (ORG_ID is None or ORG_NAME is None or LOG_URL is None):
         print(f"Please copy your API token from {API_URL}/app/token")
         temp_token = getpass("Token: ")
 
         resp = requests.post(_urljoin(API_URL, "/api/id-token"), json={"token": temp_token})
         assert resp.ok, f"Failed to acquire token: {resp.text}"
         info = resp.json()
-        token, ORG_ID, LOG_URL = info["token"], info["org_info"][0]["id"], info["org_info"][0]["api_url"]
+        token = info["token"]
+        for orgs in info["org_info"]:
+            if org_name is None or orgs["name"] == org_name:
+                ORG_ID = orgs["id"]
+                ORG_NAME = orgs["name"]
+                LOG_URL = orgs["api_url"]
+                break
 
-        _save_api_info(
-            {"token": token, "org_id": ORG_ID, "log_url": LOG_URL, "refresh_token": info.get("refresh_token")}
-        )
+        if ORG_ID is None:
+            raise ValueError(
+                f"Organization {org_name} not found. Must be one of {', '.join([x['name'] for x in info['org_info']])}"
+            )
+
+        if not disable_cache:
+            _save_api_info(
+                {"token": token, "org_id": ORG_ID, "log_url": LOG_URL, "refresh_token": info.get("refresh_token")}
+            )
 
         conn = api_conn()
         conn.set_token(token)
 
     assert conn, "Conn should be set at this point (a bug)"
     resp = conn.get("ping")
     assert resp.ok, "Invalid token: " + resp.text
```

### Comparing `braintrust-0.0.4/src/braintrust/oai.py` & `braintrust-0.0.5/src/braintrust/oai.py`

 * *Files identical despite different names*

