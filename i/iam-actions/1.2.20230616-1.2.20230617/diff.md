# Comparing `tmp/iam_actions-1.2.20230616.tar.gz` & `tmp/iam_actions-1.2.20230617.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230616.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230617.tar", max compression
```

## Comparing `iam_actions-1.2.20230616.tar` & `iam_actions-1.2.20230617.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/LICENSE
--rw-r--r--   0        0        0     2302 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/README.md
--rw-r--r--   0        0        0      228 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/iam_actions/__init__.py
--rw-r--r--   0        0        0  4319760 2023-06-16 02:37:32.308753 iam_actions-1.2.20230616/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-06-16 02:35:59.403902 iam_actions-1.2.20230616/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-06-16 02:35:59.407902 iam_actions-1.2.20230616/iam_actions/generate/services.py
--rw-r--r--   0        0        0   555328 2023-06-16 02:37:32.308753 iam_actions-1.2.20230616/iam_actions/policies.json
--rw-r--r--   0        0        0   196366 2023-06-16 02:37:32.308753 iam_actions-1.2.20230616/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   538626 2023-06-16 02:37:32.308753 iam_actions-1.2.20230616/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-06-16 02:37:33.096760 iam_actions-1.2.20230616/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230616/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230616/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/LICENSE
+-rw-r--r--   0        0        0     2302 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/README.md
+-rw-r--r--   0        0        0      228 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4326719 2023-06-17 02:32:44.581665 iam_actions-1.2.20230617/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-06-17 02:31:19.037263 iam_actions-1.2.20230617/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   556740 2023-06-17 02:32:44.581665 iam_actions-1.2.20230617/iam_actions/policies.json
+-rw-r--r--   0        0        0   196395 2023-06-17 02:32:44.581665 iam_actions-1.2.20230617/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   540016 2023-06-17 02:32:44.581665 iam_actions-1.2.20230617/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-06-17 02:32:45.585669 iam_actions-1.2.20230617/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230617/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230617/PKG-INFO
```

### Comparing `iam_actions-1.2.20230616/LICENSE` & `iam_actions-1.2.20230617/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230616/README.md` & `iam_actions-1.2.20230617/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230616/iam_actions/actions.json` & `iam_actions-1.2.20230617/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997214628780033%*

 * *Differences: {"'datasync'": "{'UpdateDiscoveryJob': {'access_level': 'Write', 'description': 'Grants permission "*

 * *               "to update a discovery job', 'resources': ['discoveryjob']}}",*

 * * "'events'": "{'StartReplay': {'resources': {insert: [(1, 'event-bus'), (2, 'replay')]}}}",*

 * * "'frauddetector'": "{'ListTagsForResource': {'resources': {insert: [(8, 'list')]}}, "*

 * *                    "'TagResource': {'resources': {insert: [(8, 'list')]}}, 'UntagResource': "*

 * *                    "{'resources': {insert: [(8, 'list')]}} […]*

```diff
@@ -34671,20 +34671,22 @@
             "description": "Grants permission to update the name of an agent",
             "orphan": false,
             "resources": [
                 "agent"
             ]
         },
         "UpdateDiscoveryJob": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateDiscoveryJob",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to update a discovery job",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "discoveryjob"
+            ]
         },
         "UpdateLocationHdfs": {
             "access_level": "Write",
             "action": "UpdateLocationHdfs",
             "condition_keys": [],
             "description": "Grants permission to update an HDFS sync Location",
             "orphan": false,
@@ -59730,15 +59732,17 @@
         "StartReplay": {
             "access_level": "Write",
             "action": "StartReplay",
             "condition_keys": [],
             "description": "Grants permission to start a replay of an archive",
             "orphan": false,
             "resources": [
-                "archive"
+                "archive",
+                "event-bus",
+                "replay"
             ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
@@ -62842,14 +62846,15 @@
                 "batch-prediction",
                 "detector",
                 "detector-version",
                 "entity-type",
                 "event-type",
                 "external-model",
                 "label",
+                "list",
                 "model",
                 "model-version",
                 "outcome",
                 "rule",
                 "variable"
             ]
         },
@@ -62968,14 +62973,15 @@
                 "batch-prediction",
                 "detector",
                 "detector-version",
                 "entity-type",
                 "event-type",
                 "external-model",
                 "label",
+                "list",
                 "model",
                 "model-version",
                 "outcome",
                 "rule",
                 "variable"
             ]
         },
@@ -62993,14 +62999,15 @@
                 "batch-prediction",
                 "detector",
                 "detector-version",
                 "entity-type",
                 "event-type",
                 "external-model",
                 "label",
+                "list",
                 "model",
                 "model-version",
                 "outcome",
                 "rule",
                 "variable"
             ]
         },
@@ -106562,14 +106569,264 @@
             "description": "Grants permission to modify basic settings for an AWS Panorama Appliance",
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
+    "payment-cryptography": {
+        "CreateAlias": {
+            "access_level": "Undocumented",
+            "action": "CreateAlias",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateKey": {
+            "access_level": "Undocumented",
+            "action": "CreateKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DecryptData": {
+            "access_level": "Undocumented",
+            "action": "DecryptData",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteAlias": {
+            "access_level": "Undocumented",
+            "action": "DeleteAlias",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteKey": {
+            "access_level": "Undocumented",
+            "action": "DeleteKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "EncryptData": {
+            "access_level": "Undocumented",
+            "action": "EncryptData",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ExportKey": {
+            "access_level": "Undocumented",
+            "action": "ExportKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GenerateCardValidationData": {
+            "access_level": "Undocumented",
+            "action": "GenerateCardValidationData",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GenerateMac": {
+            "access_level": "Undocumented",
+            "action": "GenerateMac",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GeneratePinData": {
+            "access_level": "Undocumented",
+            "action": "GeneratePinData",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetAlias": {
+            "access_level": "Undocumented",
+            "action": "GetAlias",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetKey": {
+            "access_level": "Undocumented",
+            "action": "GetKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetParametersForExport": {
+            "access_level": "Undocumented",
+            "action": "GetParametersForExport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetParametersForImport": {
+            "access_level": "Undocumented",
+            "action": "GetParametersForImport",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetPublicKeyCertificate": {
+            "access_level": "Undocumented",
+            "action": "GetPublicKeyCertificate",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ImportKey": {
+            "access_level": "Undocumented",
+            "action": "ImportKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListAliases": {
+            "access_level": "Undocumented",
+            "action": "ListAliases",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListKeys": {
+            "access_level": "Undocumented",
+            "action": "ListKeys",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ReEncryptData": {
+            "access_level": "Undocumented",
+            "action": "ReEncryptData",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "RestoreKey": {
+            "access_level": "Undocumented",
+            "action": "RestoreKey",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StartKeyUsage": {
+            "access_level": "Undocumented",
+            "action": "StartKeyUsage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "StopKeyUsage": {
+            "access_level": "Undocumented",
+            "action": "StopKeyUsage",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TranslatePinData": {
+            "access_level": "Undocumented",
+            "action": "TranslatePinData",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateAlias": {
+            "access_level": "Undocumented",
+            "action": "UpdateAlias",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "VerifyAuthRequestCryptogram": {
+            "access_level": "Undocumented",
+            "action": "VerifyAuthRequestCryptogram",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "VerifyCardValidationData": {
+            "access_level": "Undocumented",
+            "action": "VerifyCardValidationData",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "VerifyMac": {
+            "access_level": "Undocumented",
+            "action": "VerifyMac",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "VerifyPinData": {
+            "access_level": "Undocumented",
+            "action": "VerifyPinData",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "payments": {
         "CreatePaymentInstrument": {
             "access_level": "Undocumented",
             "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
@@ -111137,18 +111394,18 @@
             "action": "ListCustomPermissions",
             "condition_keys": [],
             "description": "Grants permission to list custom permissions resources in QuickSight account",
             "orphan": false,
             "resources": []
         },
         "ListCustomerManagedKeys": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListCustomerManagedKeys",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all registered customer managed keys",
             "orphan": false,
             "resources": []
         },
         "ListDashboardVersions": {
             "access_level": "List",
             "action": "ListDashboardVersions",
             "condition_keys": [],
@@ -111258,18 +111515,18 @@
                 "aws:TagKeys"
             ],
             "description": "Grants permission to list all SPICE ingestions on a dataset",
             "orphan": false,
             "resources": []
         },
         "ListKMSKeysForUser": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListKMSKeysForUser",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list a user's KMS keys",
             "orphan": false,
             "resources": []
         },
         "ListNamespaces": {
             "access_level": "List",
             "action": "ListNamespaces",
             "condition_keys": [],
@@ -111443,18 +111700,18 @@
             "description": "Grants permission to put dataset refresh properties for a dataset",
             "orphan": false,
             "resources": [
                 "dataset"
             ]
         },
         "RegisterCustomerManagedKey": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RegisterCustomerManagedKey",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to register a customer managed key",
             "orphan": false,
             "resources": []
         },
         "RegisterUser": {
             "access_level": "Write",
             "action": "RegisterUser",
             "condition_keys": [
@@ -111464,18 +111721,18 @@
             "description": "Grants permission to create a QuickSight user, whose identity is associated with the IAM identity/role specified in the request",
             "orphan": false,
             "resources": [
                 "user"
             ]
         },
         "RemoveCustomerManagedKey": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RemoveCustomerManagedKey",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to remove a customer managed key",
             "orphan": false,
             "resources": []
         },
         "RestoreAnalysis": {
             "access_level": "Write",
             "action": "RestoreAnalysis",
             "condition_keys": [],
@@ -116351,20 +116608,22 @@
             "resources": [
                 "route"
             ]
         }
     },
     "rekognition": {
         "AssociateFaces": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "AssociateFaces",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to associate multiple individual faces with a single user",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "collection"
+            ]
         },
         "CompareFaces": {
             "access_level": "Read",
             "action": "CompareFaces",
             "condition_keys": [],
             "description": "Grants permission to compare faces in the source input image with each face detected in the target input image",
             "orphan": false,
@@ -116446,20 +116705,22 @@
             "description": "Grants permission to create an Amazon Rekognition stream processor",
             "orphan": false,
             "resources": [
                 "collection"
             ]
         },
         "CreateUser": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateUser",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a new user in a collection using a unique user ID you provide",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "collection"
+            ]
         },
         "DeleteCollection": {
             "access_level": "Write",
             "action": "DeleteCollection",
             "condition_keys": [],
             "description": "Grants permission to delete the specified collection",
             "orphan": false,
@@ -116524,20 +116785,22 @@
             "description": "Grants permission to delete the specified stream processor",
             "orphan": false,
             "resources": [
                 "streamprocessor"
             ]
         },
         "DeleteUser": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteUser",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a user from a collection based on the provided user ID",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "collection"
+            ]
         },
         "DescribeCollection": {
             "access_level": "Read",
             "action": "DescribeCollection",
             "condition_keys": [],
             "description": "Grants permission to read details about a collection",
             "orphan": false,
@@ -116630,20 +116893,22 @@
             "action": "DetectText",
             "condition_keys": [],
             "description": "Grants permission to detect text in the input image and convert it into machine-readable text",
             "orphan": false,
             "resources": []
         },
         "DisassociateFaces": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DisassociateFaces",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to remove the association between a user ID and a face ID",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "collection"
+            ]
         },
         "DistributeDatasetEntries": {
             "access_level": "Write",
             "action": "DistributeDatasetEntries",
             "condition_keys": [],
             "description": "Grants permission to distribute the entries in a training dataset across the training dataset and the test dataset for a project",
             "orphan": false,
@@ -116808,20 +117073,22 @@
             "description": "Grants permission to return a list of tags associated with a resource",
             "orphan": false,
             "resources": [
                 "projectversion"
             ]
         },
         "ListUsers": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "ListUsers",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list UserIds and the UserStatus",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "collection"
+            ]
         },
         "PutProjectPolicy": {
             "access_level": "Write",
             "action": "PutProjectPolicy",
             "condition_keys": [],
             "description": "Grants permission to attach a resource policy to a project",
             "orphan": false,
@@ -116854,28 +117121,32 @@
             "description": "Grants permission to search the specificed collection for the largest face in the input image",
             "orphan": false,
             "resources": [
                 "collection"
             ]
         },
         "SearchUsers": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "SearchUsers",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to search the specificed collection for user match result with given either face ID or user ID",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "collection"
+            ]
         },
         "SearchUsersByImage": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "SearchUsersByImage",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to search the specificed collection for user match result by using the largest face in the input image",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "collection"
+            ]
         },
         "StartCelebrityRecognition": {
             "access_level": "Write",
             "action": "StartCelebrityRecognition",
             "condition_keys": [],
             "description": "Grants permission to start the asynchronous recognition of celebrities in a stored video",
             "orphan": false,
```

### Comparing `iam_actions-1.2.20230616/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230617/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230616/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230617/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230616/iam_actions/generate/generate.py` & `iam_actions-1.2.20230617/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230616/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230617/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230616/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230617/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230616/iam_actions/generate/services.py` & `iam_actions-1.2.20230617/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230616/iam_actions/policies.json` & `iam_actions-1.2.20230617/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997361477572559%*

 * *Differences: {"'serviceMap'": "{'AWS Payment Cryptography': OrderedDict([('StringPrefix', "*

 * *                 "'payment-cryptography'), ('Actions', ['CreateAlias', 'CreateKey', 'DecryptData', "*

 * *                 "'DeleteAlias', 'DeleteKey', 'EncryptData', 'ExportKey', "*

 * *                 "'GenerateCardValidationData', 'GenerateMac', 'GeneratePinData', 'GetAlias', "*

 * *                 "'GetKey', 'GetParametersForExport', 'GetParametersForImport', "*

 * *                 "'GetPublicKeyCertificate', 'ImportKey', 'ListAliases', 'List […]*

```diff
@@ -7204,14 +7204,66 @@
             "StringPrefix": "panorama",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ]
         },
+        "AWS Payment Cryptography": {
+            "ARNFormat": "arn:aws:payment-cryptography:${Region}:${Account}:${ResourceType}/${Id}",
+            "ARNRegex": "^arn:aws:payment-cryptography:.+",
+            "Actions": [
+                "CreateAlias",
+                "CreateKey",
+                "DecryptData",
+                "DeleteAlias",
+                "DeleteKey",
+                "EncryptData",
+                "ExportKey",
+                "GenerateCardValidationData",
+                "GenerateMac",
+                "GeneratePinData",
+                "GetAlias",
+                "GetKey",
+                "GetParametersForExport",
+                "GetParametersForImport",
+                "GetPublicKeyCertificate",
+                "ImportKey",
+                "ListAliases",
+                "ListKeys",
+                "ListTagsForResource",
+                "ReEncryptData",
+                "RestoreKey",
+                "StartKeyUsage",
+                "StopKeyUsage",
+                "TagResource",
+                "TranslatePinData",
+                "UntagResource",
+                "UpdateAlias",
+                "VerifyAuthRequestCryptogram",
+                "VerifyCardValidationData",
+                "VerifyMac",
+                "VerifyPinData"
+            ],
+            "HasResource": true,
+            "StringPrefix": "payment-cryptography",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys",
+                "payment-cryptography:CertificateAuthorityPublicKeyIdentifier",
+                "payment-cryptography:ImportKeyMaterial",
+                "payment-cryptography:KeyAlgorithm",
+                "payment-cryptography:KeyClass",
+                "payment-cryptography:KeyUsage",
+                "payment-cryptography:RequestAlias",
+                "payment-cryptography:ResourceAliases",
+                "payment-cryptography:WrappingKeyIdentifier"
+            ]
+        },
         "AWS Payments": {
             "Actions": [
                 "CreatePaymentInstrument",
                 "DeletePaymentInstrument",
                 "GetPaymentInstrument",
                 "GetPaymentStatus",
                 "ListPaymentPreferences",
```

### Comparing `iam_actions-1.2.20230616/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230617/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972375690607734%*

 * *Differences: {"'payment-cryptography'": 'OrderedDict()'}*

```diff
@@ -4697,14 +4697,15 @@
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "package": {
             "arn_pattern": "arn:*:panorama:*:*:package/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
+    "payment-cryptography": {},
     "payments": {},
     "personalize": {
         "algorithm": {
             "arn_pattern": "arn:*:personalize:*:*:algorithm/*",
             "condition_keys": null
         },
         "batchInferenceJob": {
```

### Comparing `iam_actions-1.2.20230616/iam_actions/services.json` & `iam_actions-1.2.20230617/iam_actions/services.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972375690607734%*

 * *Differences: {"'payment-cryptography'": "OrderedDict([('Actions', ['CreateAlias', 'CreateKey', 'DecryptData', "*

 * *                           "'DeleteAlias', 'DeleteKey', 'EncryptData', 'ExportKey', "*

 * *                           "'GenerateCardValidationData', 'GenerateMac', 'GeneratePinData', "*

 * *                           "'GetAlias', 'GetKey', 'GetParametersForExport', "*

 * *                           "'GetParametersForImport', 'GetPublicKeyCertificate', 'ImportKey', "*

 * *                           "'ListAliases', 'ListKeys', 'Lis […]*

```diff
@@ -14947,14 +14947,72 @@
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
             "AWS Panorama"
         ]
     },
+    "payment-cryptography": {
+        "ARNFormats": [
+            "arn:aws:payment-cryptography:${Region}:${Account}:${ResourceType}/${Id}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:payment-cryptography:.+"
+        ],
+        "Actions": [
+            "CreateAlias",
+            "CreateKey",
+            "DecryptData",
+            "DeleteAlias",
+            "DeleteKey",
+            "EncryptData",
+            "ExportKey",
+            "GenerateCardValidationData",
+            "GenerateMac",
+            "GeneratePinData",
+            "GetAlias",
+            "GetKey",
+            "GetParametersForExport",
+            "GetParametersForImport",
+            "GetPublicKeyCertificate",
+            "ImportKey",
+            "ListAliases",
+            "ListKeys",
+            "ListTagsForResource",
+            "ReEncryptData",
+            "RestoreKey",
+            "StartKeyUsage",
+            "StopKeyUsage",
+            "TagResource",
+            "TranslatePinData",
+            "UntagResource",
+            "UpdateAlias",
+            "VerifyAuthRequestCryptogram",
+            "VerifyCardValidationData",
+            "VerifyMac",
+            "VerifyPinData"
+        ],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys",
+            "payment-cryptography:CertificateAuthorityPublicKeyIdentifier",
+            "payment-cryptography:ImportKeyMaterial",
+            "payment-cryptography:KeyAlgorithm",
+            "payment-cryptography:KeyClass",
+            "payment-cryptography:KeyUsage",
+            "payment-cryptography:RequestAlias",
+            "payment-cryptography:ResourceAliases",
+            "payment-cryptography:WrappingKeyIdentifier"
+        ],
+        "HasResource": true,
+        "ServiceNames": [
+            "AWS Payment Cryptography"
+        ]
+    },
     "payments": {
         "ARNFormats": [],
         "ARNRegexes": [],
         "Actions": [
             "CreatePaymentInstrument",
             "DeletePaymentInstrument",
             "GetPaymentInstrument",
```

### Comparing `iam_actions-1.2.20230616/pyproject.toml` & `iam_actions-1.2.20230617/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230616"
+version = "1.2.20230617"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230616/setup.py` & `iam_actions-1.2.20230617/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230616',
+    'version': '1.2.20230617',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230616/PKG-INFO` & `iam_actions-1.2.20230617/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230616
+Version: 1.2.20230617
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

