# Comparing `tmp/heaserver-activity-1.0.0a8.tar.gz` & `tmp/heaserver-activity-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-activity-1.0.0a8.tar", last modified: Wed Feb 22 21:55:30 2023, max compression
+gzip compressed data, was "heaserver-activity-1.0.0a9.tar", last modified: Mon Jun 12 20:29:12 2023, max compression
```

## Comparing `heaserver-activity-1.0.0a8.tar` & `heaserver-activity-1.0.0a9.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-22 21:55:30.577951 heaserver-activity-1.0.0a8/
--rw-rw-rw-   0        0        0    11625 2022-05-16 17:21:14.000000 heaserver-activity-1.0.0a8/LICENSE
--rw-rw-rw-   0        0        0       39 2022-05-16 17:21:14.000000 heaserver-activity-1.0.0a8/MANIFEST.in
--rw-rw-rw-   0        0        0     4493 2023-02-22 21:55:30.577951 heaserver-activity-1.0.0a8/PKG-INFO
--rw-rw-rw-   0        0        0     3224 2022-07-01 00:54:20.000000 heaserver-activity-1.0.0a8/README.md
--rw-rw-rw-   0        0        0       42 2023-02-22 21:55:30.577951 heaserver-activity-1.0.0a8/setup.cfg
--rw-rw-rw-   0        0        0     1782 2023-02-22 21:55:00.000000 heaserver-activity-1.0.0a8/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-22 21:55:30.535830 heaserver-activity-1.0.0a8/src/
-drwxrwxrwx   0        0        0        0 2023-02-22 21:55:30.535830 heaserver-activity-1.0.0a8/src/heaserver/
-drwxrwxrwx   0        0        0        0 2023-02-22 21:55:30.551472 heaserver-activity-1.0.0a8/src/heaserver/activity/
--rw-rw-rw-   0        0        0        0 2022-05-16 17:21:14.000000 heaserver-activity-1.0.0a8/src/heaserver/activity/__init__.py
--rw-rw-rw-   0        0        0    13388 2023-01-24 00:59:59.000000 heaserver-activity-1.0.0a8/src/heaserver/activity/service.py
-drwxrwxrwx   0        0        0        0 2023-02-22 21:55:30.551472 heaserver-activity-1.0.0a8/src/heaserver/activity/wstl/
--rw-rw-rw-   0        0        0     6788 2023-01-23 20:31:56.000000 heaserver-activity-1.0.0a8/src/heaserver/activity/wstl/all.json
-drwxrwxrwx   0        0        0        0 2023-02-22 21:55:30.562313 heaserver-activity-1.0.0a8/src/heaserver_activity.egg-info/
--rw-rw-rw-   0        0        0     4493 2023-02-22 21:55:30.000000 heaserver-activity-1.0.0a8/src/heaserver_activity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      659 2023-02-22 21:55:30.000000 heaserver-activity-1.0.0a8/src/heaserver_activity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-22 21:55:30.000000 heaserver-activity-1.0.0a8/src/heaserver_activity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-02-22 21:55:30.000000 heaserver-activity-1.0.0a8/src/heaserver_activity.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-02-22 21:55:30.000000 heaserver-activity-1.0.0a8/src/heaserver_activity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-22 21:55:30.000000 heaserver-activity-1.0.0a8/src/heaserver_activity.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-22 21:55:30.535830 heaserver-activity-1.0.0a8/tests/
-drwxrwxrwx   0        0        0        0 2023-02-22 21:55:30.535830 heaserver-activity-1.0.0a8/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2023-02-22 21:55:30.577951 heaserver-activity-1.0.0a8/tests/heaserver/activitytest/
--rw-rw-rw-   0        0        0        0 2022-05-16 17:21:14.000000 heaserver-activity-1.0.0a8/tests/heaserver/activitytest/__init__.py
--rw-rw-rw-   0        0        0     4026 2022-10-26 18:06:35.000000 heaserver-activity-1.0.0a8/tests/heaserver/activitytest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2022-08-18 21:02:02.000000 heaserver-activity-1.0.0a8/tests/heaserver/activitytest/test_all.py
--rw-rw-rw-   0        0        0      688 2022-08-18 21:02:02.000000 heaserver-activity-1.0.0a8/tests/heaserver/activitytest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     4640 2023-01-23 20:31:56.000000 heaserver-activity-1.0.0a8/tests/heaserver/activitytest/testcase.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.071572 heaserver-activity-1.0.0a9/
+-rw-rw-rw-   0        0        0    11625 2022-05-16 17:21:14.000000 heaserver-activity-1.0.0a9/LICENSE
+-rw-rw-rw-   0        0        0       39 2022-05-16 17:21:14.000000 heaserver-activity-1.0.0a9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4452 2023-06-12 20:29:12.071572 heaserver-activity-1.0.0a9/PKG-INFO
+-rw-rw-rw-   0        0        0     3224 2022-07-01 00:54:20.000000 heaserver-activity-1.0.0a9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-12 20:29:12.071572 heaserver-activity-1.0.0a9/setup.cfg
+-rw-rw-rw-   0        0        0     1782 2023-06-12 20:28:53.000000 heaserver-activity-1.0.0a9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.006679 heaserver-activity-1.0.0a9/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.006679 heaserver-activity-1.0.0a9/src/heaserver/
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.034532 heaserver-activity-1.0.0a9/src/heaserver/activity/
+-rw-rw-rw-   0        0        0        0 2022-05-16 17:21:14.000000 heaserver-activity-1.0.0a9/src/heaserver/activity/__init__.py
+-rw-rw-rw-   0        0        0     4901 2023-06-12 16:26:25.000000 heaserver-activity-1.0.0a9/src/heaserver/activity/service.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.035533 heaserver-activity-1.0.0a9/src/heaserver/activity/wstl/
+-rw-rw-rw-   0        0        0     7416 2023-06-12 16:15:13.000000 heaserver-activity-1.0.0a9/src/heaserver/activity/wstl/all.json
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.064561 heaserver-activity-1.0.0a9/src/heaserver_activity.egg-info/
+-rw-rw-rw-   0        0        0     4452 2023-06-12 20:29:11.000000 heaserver-activity-1.0.0a9/src/heaserver_activity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      871 2023-06-12 20:29:12.000000 heaserver-activity-1.0.0a9/src/heaserver_activity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 20:29:11.000000 heaserver-activity-1.0.0a9/src/heaserver_activity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-12 20:29:11.000000 heaserver-activity-1.0.0a9/src/heaserver_activity.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-06-12 20:29:11.000000 heaserver-activity-1.0.0a9/src/heaserver_activity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-12 20:29:12.000000 heaserver-activity-1.0.0a9/src/heaserver_activity.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.006679 heaserver-activity-1.0.0a9/tests/
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.006679 heaserver-activity-1.0.0a9/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.070533 heaserver-activity-1.0.0a9/tests/heaserver/activitytest/
+-rw-rw-rw-   0        0        0        0 2022-05-16 17:21:14.000000 heaserver-activity-1.0.0a9/tests/heaserver/activitytest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-12 20:29:12.071572 heaserver-activity-1.0.0a9/tests/heaserver/activitytest/__pycache__/
+-rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver-activity-1.0.0a9/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.20088
+-rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver-activity-1.0.0a9/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.38284
+-rw-rw-rw-   0        0        0     2916 2023-06-12 16:23:12.000000 heaserver-activity-1.0.0a9/tests/heaserver/activitytest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      212 2023-06-12 04:38:18.000000 heaserver-activity-1.0.0a9/tests/heaserver/activitytest/test_all.py
+-rw-rw-rw-   0        0        0      338 2023-06-12 04:38:07.000000 heaserver-activity-1.0.0a9/tests/heaserver/activitytest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     4905 2023-06-12 17:23:42.000000 heaserver-activity-1.0.0a9/tests/heaserver/activitytest/testcase.py
```

### Comparing `heaserver-activity-1.0.0a8/LICENSE` & `heaserver-activity-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.0.0a8/PKG-INFO` & `heaserver-activity-1.0.0a9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: heaserver-activity
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: A service for tracking activity in hea
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
-License: UNKNOWN
 Keywords: heaserver-activity,microservice,healthcare,cancer,research,informatics
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: AsyncIO
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: English
@@ -83,9 +81,7 @@
 In MacOS or Linux, the equivalent command is:
 ```
 curl -X GET http://localhost:8080/activity/ -H 'accept: application/json'
 ```
 
 ### Packaging and releasing this project
 See the [RELEASING.md](RELEASING.md) file for details.
-
-
```

### Comparing `heaserver-activity-1.0.0a8/README.md` & `heaserver-activity-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.0.0a8/setup.py` & `heaserver-activity-1.0.0a9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-activity',
-    version='1.0.0a8',
+    version='1.0.0a9',
     description="A service for tracking activity in hea",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.activity'],
     package_data={'heaserver.activity': ['wstl/*.json']},
-    install_requires=['heaserver>=1.0.0a104, <1.0.0a105'],
+    install_requires=['heaserver>=1.0.0a131, <1.0.0a132'],
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-activity-1.0.0a8/src/heaserver/activity/wstl/all.json` & `heaserver-activity-1.0.0a9/src/heaserver/activity/wstl/all.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9470782352292769%*

 * *Differences: {"'wstl'": "{'actions': {0: {'name': 'heaserver-activity-desktopobjectaction-open'}, 1: {'name': "*

 * *           "'heaserver-activity-desktopobjectaction-get-self', 'description': 'View this desktop "*

 * *           "object action'}, 2: {'name': "*

 * *           "'heaserver-activity-desktopobjectaction-get-old-object-uri', 'prompt': 'Get old "*

 * *           "object', delete: ['description']}, 3: {'name': "*

 * *           "'heaserver-activity-desktopobjectaction-get-new-object-uri', 'type': 'safe', 'target': "*

 * *           "'it […]*

```diff
@@ -1,67 +1,140 @@
 {
     "wstl": {
         "actions": [
             {
-                "name": "heaserver-activity-activity-duplicate",
-                "prompt": "Duplicate",
+                "name": "heaserver-activity-desktopobjectaction-open",
+                "prompt": "Open",
                 "target": "item",
                 "type": "safe"
             },
             {
-                "name": "heaserver-activity-activity-open",
-                "prompt": "Open",
-                "target": "item",
+                "action": "read",
+                "description": "View this desktop object action",
+                "name": "heaserver-activity-desktopobjectaction-get-self",
+                "prompt": "View",
+                "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "read",
-                "description": "View this activity",
-                "name": "heaserver-activity-activity-get-self",
-                "prompt": "View",
+                "name": "heaserver-activity-desktopobjectaction-get-old-object-uri",
+                "prompt": "Get old object",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "read",
-                "description": "View the person who initiated this activity",
-                "name": "heaserver-activity-activity-get-person",
-                "prompt": "View",
+                "name": "heaserver-activity-desktopobjectaction-get-new-object-uri",
+                "prompt": "Get new object",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "update",
-                "description": "View and edit this Activity's properties",
+                "description": "View and edit this desktop object action's properties",
                 "inputs": [
                     {
+                        "hea": {
+                            "display": false
+                        },
                         "name": "id",
                         "prompt": "Id",
                         "readOnly": true
                     },
                     {
                         "name": "display_name",
                         "prompt": "Name",
+                        "readOnly": true,
                         "required": true
                     },
                     {
                         "name": "description",
                         "prompt": "Description",
+                        "readOnly": true,
                         "type": "textarea"
                     },
                     {
                         "hea": {
                             "optionsFromUrl": {
                                 "path": "/people/",
                                 "text": "display_name",
                                 "value": "id"
                             }
                         },
+                        "name": "user_id",
+                        "prompt": "User",
+                        "readOnly": true,
+                        "required": true,
+                        "type": "select"
+                    },
+                    {
+                        "hea": {
+                            "type": "datetime"
+                        },
+                        "name": "began",
+                        "prompt": "Began",
+                        "readOnly": true
+                    },
+                    {
+                        "hea": {
+                            "type": "datetime"
+                        },
+                        "name": "ended",
+                        "prompt": "Ended",
+                        "readOnly": true
+                    },
+                    {
+                        "hea": {
+                            "type": "datetime"
+                        },
+                        "name": "duration",
+                        "prompt": "Duration in seconds",
+                        "readOnly": true
+                    },
+                    {
+                        "name": "human_readable_duration",
+                        "prompt": "Duration",
+                        "readOnly": true
+                    },
+                    {
+                        "name": "status",
+                        "prompt": "Status",
+                        "readOnly": true,
+                        "suggest": [
+                            {
+                                "text": "Not started",
+                                "value": "NOT_STARTED"
+                            },
+                            {
+                                "text": "In progress",
+                                "value": "IN_PROGRESS"
+                            },
+                            {
+                                "text": "Completed",
+                                "value": "COMPLETED"
+                            },
+                            {
+                                "text": "Failed",
+                                "value": "FAILED"
+                            }
+                        ],
+                        "type": "select"
+                    },
+                    {
+                        "hea": {
+                            "optionsFromUrl": {
+                                "path": "/people/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
                         "name": "owner",
                         "prompt": "Owner",
+                        "readOnly": true,
                         "required": true,
                         "type": "select"
                     },
                     {
                         "hea": {
                             "type": "datetime"
                         },
@@ -75,38 +148,41 @@
                         },
                         "name": "modified",
                         "prompt": "Modified",
                         "readOnly": true
                     },
                     {
                         "name": "source",
-                        "prompt": "Source"
+                        "prompt": "Source",
+                        "readOnly": true
                     },
                     {
                         "hea": {
                             "optionsFromUrl": {
                                 "path": "/people/",
                                 "text": "display_name",
                                 "value": "id"
                             },
                             "section": "shares",
                             "sectionPrompt": "Shares"
                         },
                         "name": "user",
                         "prompt": "User",
+                        "readOnly": true,
                         "required": true,
                         "type": "select"
                     },
                     {
                         "hea": {
                             "cardinality": "multiple",
                             "section": "shares"
                         },
                         "name": "permissions",
                         "prompt": "Permissions",
+                        "readOnly": true,
                         "suggest": [
                             {
                                 "text": "Co-owner",
                                 "value": "COOWNER"
                             },
                             {
                                 "text": "Creator",
@@ -128,75 +204,16 @@
                                 "text": "Viewer",
                                 "value": "VIEWER"
                             }
                         ],
                         "type": "select"
                     }
                 ],
-                "name": "heaserver-activity-activity-get-properties",
+                "name": "heaserver-activity-desktopobjectaction-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
                 "type": "unsafe"
-            },
-            {
-                "action": "update",
-                "description": "Duplicate this activity",
-                "inputs": [
-                    {
-                        "name": "display_name",
-                        "prompt": "Name",
-                        "required": true
-                    },
-                    {
-                        "hea": {
-                            "display": false
-                        },
-                        "name": "description"
-                    },
-                    {
-                        "hea": {
-                            "display": false
-                        },
-                        "name": "owner"
-                    },
-                    {
-                        "hea": {
-                            "display": false
-                        },
-                        "name": "created"
-                    },
-                    {
-                        "hea": {
-                            "display": false
-                        },
-                        "name": "modified"
-                    },
-                    {
-                        "hea": {
-                            "display": false
-                        },
-                        "name": "source"
-                    },
-                    {
-                        "hea": {
-                            "display": false,
-                            "section": "shares"
-                        },
-                        "name": "user"
-                    },
-                    {
-                        "hea": {
-                            "display": false,
-                            "section": "shares"
-                        },
-                        "name": "permissions"
-                    }
-                ],
-                "name": "heaserver-activity-activity-duplicate-form",
-                "prompt": "Duplicate",
-                "target": "item cj-template",
-                "type": "unsafe"
             }
         ],
         "title": "HEA Server Activity Microservice"
     }
 }
```

### Comparing `heaserver-activity-1.0.0a8/src/heaserver_activity.egg-info/PKG-INFO` & `heaserver-activity-1.0.0a9/src/heaserver_activity.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: heaserver-activity
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: A service for tracking activity in hea
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
-License: UNKNOWN
 Keywords: heaserver-activity,microservice,healthcare,cancer,research,informatics
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Framework :: AsyncIO
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: English
@@ -83,9 +81,7 @@
 In MacOS or Linux, the equivalent command is:
 ```
 curl -X GET http://localhost:8080/activity/ -H 'accept: application/json'
 ```
 
 ### Packaging and releasing this project
 See the [RELEASING.md](RELEASING.md) file for details.
-
-
```

### Comparing `heaserver-activity-1.0.0a8/tests/heaserver/activitytest/permissionstestcase.py` & `heaserver-activity-1.0.0a9/tests/heaserver/activitytest/testcase.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 """
 Creates a test case class for use with the unittest library that is built into Python.
 """
-from typing import Optional
 
 from heaobject.activity import Status
 from heaserver.service.testcase.microservicetestcase import get_test_case_cls_default
 from heaserver.service.testcase.mockmongo import MockMongoManager
 from heaserver.activity import service
-from heaobject.user import NONE_USER, TEST_USER
-from heaobject.root import Permission
+from heaobject.user import NONE_USER
 from heaserver.service.testcase.expectedvalues import Action
 
+
 db_store = {
-    service.MONGODB_ACTIVITY_COLLECTION: [{
+    service.MONGODB_DESKTOP_OBJECT_ACTION_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'Reximus',
         'invites': [],
         'modified': None,
         'name': 'reximus',
         'owner': NONE_USER,
         'shares': [],
         'action': 'GET',
-        'status': Status.COMPLETE.name,
+        'status': Status.COMPLETED.name,
         'arn': 'a:1323444',
         'user_id': 'user-a',
         'source': None,
-        'type': 'heaobject.activity.AWSActivity',
-        'version': None
+        'type': 'heaobject.activity.DesktopObjectAction',
+        'old_object_uri': None,
+        'new_object_uri': None
     },
-        {
-            'id': '0123456789ab0123456789ab',
-            'created': None,
-            'derived_by': None,
-            'derived_from': [],
-            'description': None,
-            'display_name': 'Luximus',
-            'invites': [],
-            'modified': None,
-            'name': 'luximus',
-            'owner': NONE_USER,
-            'shares': [{
-                'type': 'heaobject.root.ShareImpl',
-                'invite': None,
-                'user': TEST_USER,
-                'permissions': [Permission.VIEWER.name]
-            }],
-            'action': 'GET',
-            'status': Status.IN_PROGRESS.name,
-            'arn': 'a:1323444',
-            'user_id': 'user-a',
-            'source': None,
-            'type': 'heaobject.activity.AWSActivity',
-            'version': None
-        }]}
+    {
+        'id': '0123456789ab0123456789ab',
+        'created': None,
+        'derived_by': None,
+        'derived_from': [],
+        'description': None,
+        'display_name': 'Luximus',
+        'invites': [],
+        'modified': None,
+        'name': 'luximus',
+        'owner': NONE_USER,
+        'action': 'GET',
+        'status': Status.IN_PROGRESS.name,
+        'arn': 'a:1323444',
+        'user_id': 'user-a',
+        'source': None,
+        'type': 'heaobject.activity.DesktopObjectAction',
+        'old_object_uri': None,
+        'new_object_uri': None
+    }]}
 
 
-PermissionsTestCase = \
-    get_test_case_cls_default(coll=service.MONGODB_ACTIVITY_COLLECTION,
-                              wstl_package=service.__package__,
-                              href='http://localhost:8080/activity/',
-                              fixtures=db_store,
-                              db_manager_cls=MockMongoManager,
-                              get_actions=[Action(name='heaserver-activity-activity-get-properties',
-                                                  rel=['properties']),
-                                           Action(name='heaserver-activity-activity-open',
-                                                  url='http://localhost:8080/activity/{id}/opener',
-                                                  rel=['opener']),
-                                           Action(name='heaserver-activity-activity-duplicate',
-                                                  url='http://localhost:8080/activity/{id}/duplicator',
-                                                  rel=['duplicator'])
-                                           ],
-                              get_all_actions=[Action(name='heaserver-activity-activity-get-properties',
-                                                      rel=['properties']),
-                                               Action(name='heaserver-activity-activity-open',
-                                                      url='http://localhost:8080/activity/{id}/opener',
-                                                      rel=['opener']),
-                                               Action(name='heaserver-activity-activity-duplicate',
-                                                      url='http://localhost:8080/activity/{id}/duplicator',
-                                                      rel=['duplicator'])],
-                              duplicate_action_name='heaserver-activity-activity-duplicate-form',
-                              put_content_status=404,
-                              sub=TEST_USER)
+TestCase = get_test_case_cls_default(coll=service.MONGODB_DESKTOP_OBJECT_ACTION_COLLECTION,
+                                     wstl_package=service.__package__,
+                                     href='http://localhost:8080/desktopobjectactions/',
+                                     fixtures=db_store,
+                                     db_manager_cls=MockMongoManager,
+                                     get_actions=[Action(name='heaserver-activity-desktopobjectaction-get-properties',
+                                                         rel=['hea-properties']),
+                                                  Action(name='heaserver-activity-desktopobjectaction-get-self',
+                                                         url='http://localhost:8080/desktopobjectactions/{id}',
+                                                         rel=['self']),
+                                                  Action(name='heaserver-activity-desktopobjectaction-get-old-object-uri',
+                                                         url='http://localhost:8080{+old_object_uri}',
+                                                         rel=['hea-desktop-object'],
+                                                         itemif='old_object_uri is not None and new_object_uri is None'),
+                                                  Action(name='heaserver-activity-desktopobjectaction-get-new-object-uri',
+                                                         url='http://localhost:8080{+new_object_uri}',
+                                                         rel=['hea-desktop-object'],
+                                                         itemif='new_object_uri is not None')
+                                                  ],
+                                     get_all_actions=[Action(name='heaserver-activity-desktopobjectaction-get-properties',
+                                                             rel=['hea-properties']),
+                                                      Action(name='heaserver-activity-desktopobjectaction-get-self',
+                                                             url='http://localhost:8080/desktopobjectactions/{id}',
+                                                             rel=['self']),
+                                                      Action(name='heaserver-activity-desktopobjectaction-get-old-object-uri',
+                                                             url='http://localhost:8080{+old_object_uri}',
+                                                             rel=['hea-desktop-object'],
+                                                             itemif='old_object_uri is not None and new_object_uri is None'),
+                                                      Action(name='heaserver-activity-desktopobjectaction-get-new-object-uri',
+                                                             url='http://localhost:8080{+new_object_uri}',
+                                                             rel=['hea-desktop-object'],
+                                                             itemif='new_object_uri is not None')])
```

