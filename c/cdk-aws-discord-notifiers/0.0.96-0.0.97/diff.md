# Comparing `tmp/cdk-aws-discord-notifiers-0.0.96.tar.gz` & `tmp/cdk-aws-discord-notifiers-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-aws-discord-notifiers-0.0.96.tar", last modified: Fri Jun 16 00:09:07 2023, max compression
+gzip compressed data, was "cdk-aws-discord-notifiers-0.0.97.tar", last modified: Sat Jun 17 00:09:06 2023, max compression
```

## Comparing `cdk-aws-discord-notifiers-0.0.96.tar` & `cdk-aws-discord-notifiers-0.0.97.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:09:07.545879 cdk-aws-discord-notifiers-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-16 00:08:53.000000 cdk-aws-discord-notifiers-0.0.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 00:08:53.000000 cdk-aws-discord-notifiers-0.0.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-16 00:09:07.545879 cdk-aws-discord-notifiers-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-16 00:08:53.000000 cdk-aws-discord-notifiers-0.0.96/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-16 00:08:53.000000 cdk-aws-discord-notifiers-0.0.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 00:09:07.545879 cdk-aws-discord-notifiers-0.0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-16 00:08:53.000000 cdk-aws-discord-notifiers-0.0.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:09:07.537878 cdk-aws-discord-notifiers-0.0.96/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:09:07.541878 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws-discord-notifiers/
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-16 00:08:53.000000 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws-discord-notifiers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:09:07.541878 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws-discord-notifiers/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-16 00:08:53.000000 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws-discord-notifiers/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  2509666 2023-06-16 00:08:53.000000 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.96.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:08:53.000000 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws-discord-notifiers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 00:09:07.545879 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws_discord_notifiers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-16 00:09:07.000000 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-16 00:09:07.000000 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 00:09:07.000000 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws_discord_notifiers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-16 00:09:07.000000 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws_discord_notifiers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 00:09:07.000000 cdk-aws-discord-notifiers-0.0.96/src/cdk_aws_discord_notifiers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:09:06.756871 cdk-aws-discord-notifiers-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-17 00:08:51.000000 cdk-aws-discord-notifiers-0.0.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 00:08:51.000000 cdk-aws-discord-notifiers-0.0.97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-17 00:09:06.756871 cdk-aws-discord-notifiers-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-17 00:08:51.000000 cdk-aws-discord-notifiers-0.0.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-17 00:08:51.000000 cdk-aws-discord-notifiers-0.0.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 00:09:06.756871 cdk-aws-discord-notifiers-0.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-17 00:08:51.000000 cdk-aws-discord-notifiers-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:09:06.748871 cdk-aws-discord-notifiers-0.0.97/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:09:06.752871 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws-discord-notifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-17 00:08:51.000000 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws-discord-notifiers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:09:06.752871 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws-discord-notifiers/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-17 00:08:51.000000 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws-discord-notifiers/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2509687 2023-06-17 00:08:51.000000 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.97.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 00:08:51.000000 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws-discord-notifiers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 00:09:06.752871 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws_discord_notifiers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-17 00:09:06.000000 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-17 00:09:06.000000 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 00:09:06.000000 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws_discord_notifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-17 00:09:06.000000 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws_discord_notifiers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-17 00:09:06.000000 cdk-aws-discord-notifiers-0.0.97/src/cdk_aws_discord_notifiers.egg-info/top_level.txt
```

### Comparing `cdk-aws-discord-notifiers-0.0.96/LICENSE` & `cdk-aws-discord-notifiers-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-aws-discord-notifiers-0.0.96/PKG-INFO` & `cdk-aws-discord-notifiers-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-aws-discord-notifiers
-Version: 0.0.96
+Version: 0.0.97
 Summary: A package that vends constructs to notify about AWS resources via discord
 Home-page: https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-aws-discord-notifiers-0.0.96/README.md` & `cdk-aws-discord-notifiers-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `cdk-aws-discord-notifiers-0.0.96/setup.py` & `cdk-aws-discord-notifiers-0.0.97/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-aws-discord-notifiers",
-    "version": "0.0.96",
+    "version": "0.0.97",
     "description": "A package that vends constructs to notify about AWS resources via discord",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdk-aws-discord-notifiers.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_aws-discord-notifiers",
         "cdk_aws-discord-notifiers._jsii"
     ],
     "package_data": {
         "cdk_aws-discord-notifiers._jsii": [
-            "cdk-aws-discord-notifiers@0.0.96.jsii.tgz"
+            "cdk-aws-discord-notifiers@0.0.97.jsii.tgz"
         ],
         "cdk_aws-discord-notifiers": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-aws-discord-notifiers-0.0.96/src/cdk_aws-discord-notifiers/__init__.py` & `cdk-aws-discord-notifiers-0.0.97/src/cdk_aws-discord-notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-aws-discord-notifiers-0.0.96/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO` & `cdk-aws-discord-notifiers-0.0.97/src/cdk_aws_discord_notifiers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-aws-discord-notifiers
-Version: 0.0.96
+Version: 0.0.97
 Summary: A package that vends constructs to notify about AWS resources via discord
 Home-page: https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdk-aws-discord-notifiers.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-aws-discord-notifiers-0.0.96/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt` & `cdk-aws-discord-notifiers-0.0.97/src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 src/cdk_aws-discord-notifiers/__init__.py
 src/cdk_aws-discord-notifiers/py.typed
 src/cdk_aws-discord-notifiers/_jsii/__init__.py
-src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.96.jsii.tgz
+src/cdk_aws-discord-notifiers/_jsii/cdk-aws-discord-notifiers@0.0.97.jsii.tgz
 src/cdk_aws_discord_notifiers.egg-info/PKG-INFO
 src/cdk_aws_discord_notifiers.egg-info/SOURCES.txt
 src/cdk_aws_discord_notifiers.egg-info/dependency_links.txt
 src/cdk_aws_discord_notifiers.egg-info/requires.txt
 src/cdk_aws_discord_notifiers.egg-info/top_level.txt
```

