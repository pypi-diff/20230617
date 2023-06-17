# Comparing `tmp/botocore-a-la-carte-payment-cryptography-data-1.29.154.tar.gz` & `tmp/botocore-a-la-carte-payment-cryptography-data-1.29.155.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-payment-cryptography-data-1.29.154.tar", last modified: Fri Jun 16 01:26:17 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-payment-cryptography-data-1.29.155.tar", last modified: Sat Jun 17 01:21:37 2023, max compression
```

## Comparing `botocore-a-la-carte-payment-cryptography-data-1.29.154.tar` & `botocore-a-la-carte-payment-cryptography-data-1.29.155.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:26:17.626462 botocore-a-la-carte-payment-cryptography-data-1.29.154/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-16 01:26:17.000000 botocore-a-la-carte-payment-cryptography-data-1.29.154/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 01:26:17.626462 botocore-a-la-carte-payment-cryptography-data-1.29.154/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:26:17.626462 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:26:17.626462 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:26:17.626462 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore/data/payment-cryptography-data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:26:17.626462 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore/data/payment-cryptography-data/2022-02-03/
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-06-16 01:25:27.000000 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore/data/payment-cryptography-data/2022-02-03/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-16 01:25:27.000000 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore/data/payment-cryptography-data/2022-02-03/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   108331 2023-06-16 01:25:27.000000 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore/data/payment-cryptography-data/2022-02-03/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:26:17.626462 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore_a_la_carte_payment_cryptography_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-16 01:26:17.000000 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore_a_la_carte_payment_cryptography_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-16 01:26:17.000000 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore_a_la_carte_payment_cryptography_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:26:17.000000 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore_a_la_carte_payment_cryptography_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 01:26:17.000000 botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore_a_la_carte_payment_cryptography_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 01:26:17.626462 botocore-a-la-carte-payment-cryptography-data-1.29.154/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-16 01:26:17.000000 botocore-a-la-carte-payment-cryptography-data-1.29.154/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:37.596167 botocore-a-la-carte-payment-cryptography-data-1.29.155/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-17 01:21:37.000000 botocore-a-la-carte-payment-cryptography-data-1.29.155/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-17 01:21:37.596167 botocore-a-la-carte-payment-cryptography-data-1.29.155/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:37.592167 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:37.592167 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:37.592167 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore/data/payment-cryptography-data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:37.592167 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore/data/payment-cryptography-data/2022-02-03/
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-06-17 01:21:04.000000 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore/data/payment-cryptography-data/2022-02-03/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 01:21:04.000000 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore/data/payment-cryptography-data/2022-02-03/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   108331 2023-06-17 01:21:04.000000 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore/data/payment-cryptography-data/2022-02-03/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:37.596167 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore_a_la_carte_payment_cryptography_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-17 01:21:37.000000 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore_a_la_carte_payment_cryptography_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-17 01:21:37.000000 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore_a_la_carte_payment_cryptography_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:21:37.000000 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore_a_la_carte_payment_cryptography_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 01:21:37.000000 botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore_a_la_carte_payment_cryptography_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:21:37.596167 botocore-a-la-carte-payment-cryptography-data-1.29.155/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-17 01:21:37.000000 botocore-a-la-carte-payment-cryptography-data-1.29.155/setup.py
```

### Comparing `botocore-a-la-carte-payment-cryptography-data-1.29.154/LICENSE.txt` & `botocore-a-la-carte-payment-cryptography-data-1.29.155/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-payment-cryptography-data-1.29.154/PKG-INFO` & `botocore-a-la-carte-payment-cryptography-data-1.29.155/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-payment-cryptography-data
-Version: 1.29.154
+Version: 1.29.155
 Summary: payment-cryptography-data data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore/data/payment-cryptography-data/2022-02-03/endpoint-rule-set-1.json` & `botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore/data/payment-cryptography-data/2022-02-03/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore/data/payment-cryptography-data/2022-02-03/service-2.json` & `botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore/data/payment-cryptography-data/2022-02-03/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-payment-cryptography-data-1.29.154/botocore_a_la_carte_payment_cryptography_data.egg-info/PKG-INFO` & `botocore-a-la-carte-payment-cryptography-data-1.29.155/botocore_a_la_carte_payment_cryptography_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-payment-cryptography-data
-Version: 1.29.154
+Version: 1.29.155
 Summary: payment-cryptography-data data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-payment-cryptography-data-1.29.154/setup.py` & `botocore-a-la-carte-payment-cryptography-data-1.29.155/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-payment-cryptography-data',
-    version="1.29.154",
+    version="1.29.155",
     description='payment-cryptography-data data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/payment-cryptography-data/*/*.json'],
```

