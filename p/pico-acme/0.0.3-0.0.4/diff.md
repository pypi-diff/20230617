# Comparing `tmp/pico_acme-0.0.3.tar.gz` & `tmp/pico_acme-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pico_acme-0.0.3.tar", last modified: Sat Jun 17 03:59:36 2023, max compression
+gzip compressed data, was "pico_acme-0.0.4.tar", last modified: Sat Jun 17 04:03:49 2023, max compression
```

## Comparing `pico_acme-0.0.3.tar` & `pico_acme-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2023-06-17 03:59:36.026811 pico_acme-0.0.3/
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3161 2023-06-17 03:59:36.026811 pico_acme-0.0.3/PKG-INFO
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     2622 2023-06-17 03:48:11.000000 pico_acme-0.0.3/README.md
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)    11358 2023-06-17 03:47:23.000000 pico_acme-0.0.3/license.md
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      242 2023-06-17 03:55:38.000000 pico_acme-0.0.3/pyproject.toml
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       77 2023-06-17 03:59:36.026811 pico_acme-0.0.3/setup.cfg
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      961 2023-06-17 03:04:57.000000 pico_acme-0.0.3/setup.py
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2023-06-17 03:59:36.026811 pico_acme-0.0.3/src/
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2023-06-17 03:59:36.026811 pico_acme-0.0.3/src/pico_acme/
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      203 2023-06-17 03:04:25.000000 pico_acme-0.0.3/src/pico_acme/__init__.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3738 2023-06-17 03:04:25.000000 pico_acme-0.0.3/src/pico_acme/core.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     2075 2023-06-17 02:06:10.000000 pico_acme-0.0.3/src/pico_acme/route53.py
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        6 2023-06-17 03:55:48.000000 pico_acme-0.0.3/src/pico_acme/version
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      123 2023-06-17 02:13:45.000000 pico_acme-0.0.3/src/pico_acme/version.py
-drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2023-06-17 03:59:36.026811 pico_acme-0.0.3/src/pico_acme.egg-info/
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3161 2023-06-17 03:59:36.000000 pico_acme-0.0.3/src/pico_acme.egg-info/PKG-INFO
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      358 2023-06-17 03:59:36.000000 pico_acme-0.0.3/src/pico_acme.egg-info/SOURCES.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        1 2023-06-17 03:59:36.000000 pico_acme-0.0.3/src/pico_acme.egg-info/dependency_links.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       12 2023-06-17 03:59:36.000000 pico_acme-0.0.3/src/pico_acme.egg-info/requires.txt
--rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       10 2023-06-17 03:59:36.000000 pico_acme-0.0.3/src/pico_acme.egg-info/top_level.txt
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2023-06-17 04:03:49.314803 pico_acme-0.0.4/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3183 2023-06-17 04:03:49.314803 pico_acme-0.0.4/PKG-INFO
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     2644 2023-06-17 04:03:06.000000 pico_acme-0.0.4/README.md
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)    11358 2023-06-17 03:47:23.000000 pico_acme-0.0.4/license.md
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      242 2023-06-17 03:55:38.000000 pico_acme-0.0.4/pyproject.toml
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       77 2023-06-17 04:03:49.314803 pico_acme-0.0.4/setup.cfg
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      961 2023-06-17 03:04:57.000000 pico_acme-0.0.4/setup.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2023-06-17 04:03:49.314803 pico_acme-0.0.4/src/
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2023-06-17 04:03:49.314803 pico_acme-0.0.4/src/pico_acme/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      203 2023-06-17 03:04:25.000000 pico_acme-0.0.4/src/pico_acme/__init__.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3738 2023-06-17 03:04:25.000000 pico_acme-0.0.4/src/pico_acme/core.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     2075 2023-06-17 02:06:10.000000 pico_acme-0.0.4/src/pico_acme/route53.py
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        6 2023-06-17 04:03:25.000000 pico_acme-0.0.4/src/pico_acme/version
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      123 2023-06-17 02:13:45.000000 pico_acme-0.0.4/src/pico_acme/version.py
+drwxrwxr-x   0 aapeli    (1000) aapeli    (1000)        0 2023-06-17 04:03:49.314803 pico_acme-0.0.4/src/pico_acme.egg-info/
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)     3183 2023-06-17 04:03:49.000000 pico_acme-0.0.4/src/pico_acme.egg-info/PKG-INFO
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)      358 2023-06-17 04:03:49.000000 pico_acme-0.0.4/src/pico_acme.egg-info/SOURCES.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)        1 2023-06-17 04:03:49.000000 pico_acme-0.0.4/src/pico_acme.egg-info/dependency_links.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       12 2023-06-17 04:03:49.000000 pico_acme-0.0.4/src/pico_acme.egg-info/requires.txt
+-rw-rw-r--   0 aapeli    (1000) aapeli    (1000)       10 2023-06-17 04:03:49.000000 pico_acme-0.0.4/src/pico_acme.egg-info/top_level.txt
```

### Comparing `pico_acme-0.0.3/PKG-INFO` & `pico_acme-0.0.4/src/pico_acme.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pico_acme
-Version: 0.0.3
+Name: pico-acme
+Version: 0.0.4
 Summary: Pico ACME: tiny ACMEv2 client
 Home-page: https://github.com/aapeliv/pico-acme
 Author: Aapeli Vuorinen
 Project-URL: GitHub, https://github.com/aapeliv/pico-acme
 Project-URL: Bug Tracker, https://github.com/aapeliv/pico-acme/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,19 +19,23 @@
 
 Supports only single domains and DNS challenge. Currently implements AWS Route 53 but you can trivially implement your own provider.
 
 Licensed under Apache 2.0 as this reuses some code from certbot.
 
 ## quick start
 
-Note that you need to install `boto3` separately to use `route53`.
+Install from PyPI:
 
-Create the following files in a folder:
+```sh
+pip install pico-acme
+```
+
+(Note that you need to install `boto3` separately to use `route53`.)
 
-`new.py`:
+### `new.py`:
 
 ```py
 ROUTE53_HOSTED_ZONE_ID = "..."
 ACCOUNT_EMAIL = "domains@example.com"
 DOMAIN = "example.com"
 
 # create account, get cert, and save details
@@ -60,15 +64,15 @@
     f.write(key_pem)
 
 # save the cert for later
 with open("fullchain.pem", "w") as f:
     f.write(fullchain_pem)
 ```
 
-`renew.py`:
+### `renew.py`:
 
 ```py
 ROUTE53_HOSTED_ZONE_ID = "..."
 DOMAIN = "example.com"
 
 # later, load account, private key, and renew cert
 import pico_acme
```

### Comparing `pico_acme-0.0.3/README.md` & `pico_acme-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 Supports only single domains and DNS challenge. Currently implements AWS Route 53 but you can trivially implement your own provider.
 
 Licensed under Apache 2.0 as this reuses some code from certbot.
 
 ## quick start
 
-Note that you need to install `boto3` separately to use `route53`.
+Install from PyPI:
 
-Create the following files in a folder:
+```sh
+pip install pico-acme
+```
+
+(Note that you need to install `boto3` separately to use `route53`.)
 
-`new.py`:
+### `new.py`:
 
 ```py
 ROUTE53_HOSTED_ZONE_ID = "..."
 ACCOUNT_EMAIL = "domains@example.com"
 DOMAIN = "example.com"
 
 # create account, get cert, and save details
@@ -45,15 +49,15 @@
     f.write(key_pem)
 
 # save the cert for later
 with open("fullchain.pem", "w") as f:
     f.write(fullchain_pem)
 ```
 
-`renew.py`:
+### `renew.py`:
 
 ```py
 ROUTE53_HOSTED_ZONE_ID = "..."
 DOMAIN = "example.com"
 
 # later, load account, private key, and renew cert
 import pico_acme
```

### Comparing `pico_acme-0.0.3/license.md` & `pico_acme-0.0.4/license.md`

 * *Files identical despite different names*

### Comparing `pico_acme-0.0.3/setup.py` & `pico_acme-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `pico_acme-0.0.3/src/pico_acme/core.py` & `pico_acme-0.0.4/src/pico_acme/core.py`

 * *Files identical despite different names*

### Comparing `pico_acme-0.0.3/src/pico_acme/route53.py` & `pico_acme-0.0.4/src/pico_acme/route53.py`

 * *Files identical despite different names*

### Comparing `pico_acme-0.0.3/src/pico_acme.egg-info/PKG-INFO` & `pico_acme-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pico-acme
-Version: 0.0.3
+Name: pico_acme
+Version: 0.0.4
 Summary: Pico ACME: tiny ACMEv2 client
 Home-page: https://github.com/aapeliv/pico-acme
 Author: Aapeli Vuorinen
 Project-URL: GitHub, https://github.com/aapeliv/pico-acme
 Project-URL: Bug Tracker, https://github.com/aapeliv/pico-acme/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,19 +19,23 @@
 
 Supports only single domains and DNS challenge. Currently implements AWS Route 53 but you can trivially implement your own provider.
 
 Licensed under Apache 2.0 as this reuses some code from certbot.
 
 ## quick start
 
-Note that you need to install `boto3` separately to use `route53`.
+Install from PyPI:
 
-Create the following files in a folder:
+```sh
+pip install pico-acme
+```
+
+(Note that you need to install `boto3` separately to use `route53`.)
 
-`new.py`:
+### `new.py`:
 
 ```py
 ROUTE53_HOSTED_ZONE_ID = "..."
 ACCOUNT_EMAIL = "domains@example.com"
 DOMAIN = "example.com"
 
 # create account, get cert, and save details
@@ -60,15 +64,15 @@
     f.write(key_pem)
 
 # save the cert for later
 with open("fullchain.pem", "w") as f:
     f.write(fullchain_pem)
 ```
 
-`renew.py`:
+### `renew.py`:
 
 ```py
 ROUTE53_HOSTED_ZONE_ID = "..."
 DOMAIN = "example.com"
 
 # later, load account, private key, and renew cert
 import pico_acme
```

