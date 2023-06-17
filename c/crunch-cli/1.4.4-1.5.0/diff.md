# Comparing `tmp/crunch-cli-1.4.4.tar.gz` & `tmp/crunch-cli-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crunch-cli-1.4.4.tar", last modified: Wed May 24 15:16:45 2023, max compression
+gzip compressed data, was "crunch-cli-1.5.0.tar", last modified: Sat Jun 17 13:17:52 2023, max compression
```

## Comparing `crunch-cli-1.4.4.tar` & `crunch-cli-1.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.948294 crunch-cli-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 15:16:45.948294 crunch-cli-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.940294 crunch-cli-1.4.4/crunch/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.944294 crunch-cli-1.4.4/crunch/command/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/command/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.944294 crunch-cli-1.4.4/crunch/demo-project/
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/demo-project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/demo-project/files.json
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/demo-project/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/demo-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/ensure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/crunch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:45.948294 crunch-cli-1.4.4/crunch_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 15:16:45.000000 crunch-cli-1.4.4/crunch_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 15:16:45.948294 crunch-cli-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-24 15:16:40.000000 crunch-cli-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/crunch/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/crunch/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/command/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/crunch/demo-project/
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/demo-project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/demo-project/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/demo-project/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/demo-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/ensure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/crunch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/crunch_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 13:17:52.000000 crunch-cli-1.5.0/crunch_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 13:17:52.053924 crunch-cli-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-17 13:17:43.000000 crunch-cli-1.5.0/setup.py
```

### Comparing `crunch-cli-1.4.4/crunch/command/convert.py` & `crunch-cli-1.5.0/crunch/command/convert.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/command/download.py` & `crunch-cli-1.5.0/crunch/command/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 ) -> typing.Tuple[typing.Dict[str, str], str, str, str]:
     current_crunch = session.get("/v1/crunches/@current").json()
     data_release = session.get(f"/v1/crunches/{current_crunch['number']}/data-release", params={
         "pushToken": push_token
     }).json()
 
     embargo = data_release["embargo"]
-    moon_column_name = data_release["moonColumnName"]
+    moon_column_name = data_release["moon"]["columnName"]
     data_files = data_release["dataFiles"]
 
     def get_file(key: str, file_name: str) -> DataFile:
         data_file = data_files[key]
 
         url = data_file["url"]
         path = os.path.join(
```

### Comparing `crunch-cli-1.4.4/crunch/command/push.py` & `crunch-cli-1.5.0/crunch/command/push.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/command/setup.py` & `crunch-cli-1.5.0/crunch/command/setup.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/command/test.py` & `crunch-cli-1.5.0/crunch/command/test.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/constants.py` & `crunch-cli-1.5.0/crunch/constants.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/demo-project/.gitignore` & `crunch-cli-1.5.0/crunch/demo-project/.gitignore`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/demo-project/main.py` & `crunch-cli-1.5.0/crunch/demo-project/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/ensure.py` & `crunch-cli-1.5.0/crunch/ensure.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/inline.py` & `crunch-cli-1.5.0/crunch/inline.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/library.py` & `crunch-cli-1.5.0/crunch/library.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/main.py` & `crunch-cli-1.5.0/crunch/main.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/tester.py` & `crunch-cli-1.5.0/crunch/tester.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch/utils.py` & `crunch-cli-1.5.0/crunch/utils.py`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/crunch_cli.egg-info/SOURCES.txt` & `crunch-cli-1.5.0/crunch_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crunch-cli-1.4.4/setup.py` & `crunch-cli-1.5.0/setup.py`

 * *Files identical despite different names*

