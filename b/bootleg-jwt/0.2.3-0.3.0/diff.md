# Comparing `tmp/bootleg-jwt-0.2.3.tar.gz` & `tmp/bootleg-jwt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootleg-jwt-0.2.3.tar", last modified: Wed Mar  1 10:32:21 2023, max compression
+gzip compressed data, was "bootleg-jwt-0.3.0.tar", last modified: Sat Jun 17 01:43:53 2023, max compression
```

## Comparing `bootleg-jwt-0.2.3.tar` & `bootleg-jwt-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rae       (1000) rae       (1000)        0 2023-03-01 10:32:21.205643 bootleg-jwt-0.2.3/
--rw-r--r--   0 rae       (1000) rae       (1000)     1073 2023-02-11 06:51:15.000000 bootleg-jwt-0.2.3/LICENSE
--rw-r--r--   0 rae       (1000) rae       (1000)    12183 2023-03-01 10:32:21.205643 bootleg-jwt-0.2.3/PKG-INFO
--rw-r--r--   0 rae       (1000) rae       (1000)    11193 2023-02-26 03:54:21.000000 bootleg-jwt-0.2.3/README.md
-drwxr-xr-x   0 rae       (1000) rae       (1000)        0 2023-03-01 10:32:21.201643 bootleg-jwt-0.2.3/bootleg_jwt.egg-info/
--rw-r--r--   0 rae       (1000) rae       (1000)    12183 2023-03-01 10:32:21.000000 bootleg-jwt-0.2.3/bootleg_jwt.egg-info/PKG-INFO
--rw-r--r--   0 rae       (1000) rae       (1000)      346 2023-03-01 10:32:21.000000 bootleg-jwt-0.2.3/bootleg_jwt.egg-info/SOURCES.txt
--rw-r--r--   0 rae       (1000) rae       (1000)        1 2023-03-01 10:32:21.000000 bootleg-jwt-0.2.3/bootleg_jwt.egg-info/dependency_links.txt
--rw-r--r--   0 rae       (1000) rae       (1000)       38 2023-03-01 10:32:21.000000 bootleg-jwt-0.2.3/bootleg_jwt.egg-info/requires.txt
--rw-r--r--   0 rae       (1000) rae       (1000)       12 2023-03-01 10:32:21.000000 bootleg-jwt-0.2.3/bootleg_jwt.egg-info/top_level.txt
--rw-r--r--   0 rae       (1000) rae       (1000)       99 2023-02-24 00:01:14.000000 bootleg-jwt-0.2.3/pyproject.toml
--rw-r--r--   0 rae       (1000) rae       (1000)       38 2023-03-01 10:32:21.205643 bootleg-jwt-0.2.3/setup.cfg
--rw-r--r--   0 rae       (1000) rae       (1000)     1678 2023-02-26 03:54:21.000000 bootleg-jwt-0.2.3/setup.py
-drwxr-xr-x   0 rae       (1000) rae       (1000)        0 2023-03-01 10:32:21.201643 bootleg-jwt-0.2.3/src/
-drwxr-xr-x   0 rae       (1000) rae       (1000)        0 2023-03-01 10:32:21.205643 bootleg-jwt-0.2.3/src/bootleg_jwt/
--rw-r--r--   0 rae       (1000) rae       (1000)       88 2023-02-26 03:54:21.000000 bootleg-jwt-0.2.3/src/bootleg_jwt/__init__.py
--rw-r--r--   0 rae       (1000) rae       (1000)     2275 2023-03-01 10:31:48.000000 bootleg-jwt-0.2.3/src/bootleg_jwt/funcs.py
--rw-r--r--   0 rae       (1000) rae       (1000)     1757 2023-02-26 03:54:21.000000 bootleg-jwt-0.2.3/src/bootleg_jwt/main.py
--rw-r--r--   0 rae       (1000) rae       (1000)      142 2023-02-26 03:54:21.000000 bootleg-jwt-0.2.3/src/bootleg_jwt/messages.py
--rw-r--r--   0 rae       (1000) rae       (1000)      836 2023-02-26 03:54:21.000000 bootleg-jwt-0.2.3/src/bootleg_jwt/schema.py
+drwxr-xr-x   0 freyja    (1000) freyja    (1000)        0 2023-06-17 01:43:53.284002 bootleg-jwt-0.3.0/
+-rw-r--r--   0 freyja    (1000) freyja    (1000)     1073 2023-05-12 13:39:03.000000 bootleg-jwt-0.3.0/LICENSE
+-rw-r--r--   0 freyja    (1000) freyja    (1000)    13263 2023-06-17 01:43:53.284002 bootleg-jwt-0.3.0/PKG-INFO
+-rw-r--r--   0 freyja    (1000) freyja    (1000)    12273 2023-06-17 01:08:52.000000 bootleg-jwt-0.3.0/README.md
+drwxr-xr-x   0 freyja    (1000) freyja    (1000)        0 2023-06-17 01:43:53.284002 bootleg-jwt-0.3.0/bootleg_jwt.egg-info/
+-rw-r--r--   0 freyja    (1000) freyja    (1000)    13263 2023-06-17 01:43:53.000000 bootleg-jwt-0.3.0/bootleg_jwt.egg-info/PKG-INFO
+-rw-r--r--   0 freyja    (1000) freyja    (1000)      346 2023-06-17 01:43:53.000000 bootleg-jwt-0.3.0/bootleg_jwt.egg-info/SOURCES.txt
+-rw-r--r--   0 freyja    (1000) freyja    (1000)        1 2023-06-17 01:43:53.000000 bootleg-jwt-0.3.0/bootleg_jwt.egg-info/dependency_links.txt
+-rw-r--r--   0 freyja    (1000) freyja    (1000)       38 2023-06-17 01:43:53.000000 bootleg-jwt-0.3.0/bootleg_jwt.egg-info/requires.txt
+-rw-r--r--   0 freyja    (1000) freyja    (1000)       12 2023-06-17 01:43:53.000000 bootleg-jwt-0.3.0/bootleg_jwt.egg-info/top_level.txt
+-rw-r--r--   0 freyja    (1000) freyja    (1000)       99 2023-05-12 13:39:02.000000 bootleg-jwt-0.3.0/pyproject.toml
+-rw-r--r--   0 freyja    (1000) freyja    (1000)       38 2023-06-17 01:43:53.284002 bootleg-jwt-0.3.0/setup.cfg
+-rw-r--r--   0 freyja    (1000) freyja    (1000)     1678 2023-05-12 13:39:03.000000 bootleg-jwt-0.3.0/setup.py
+drwxr-xr-x   0 freyja    (1000) freyja    (1000)        0 2023-06-17 01:43:53.284002 bootleg-jwt-0.3.0/src/
+drwxr-xr-x   0 freyja    (1000) freyja    (1000)        0 2023-06-17 01:43:53.284002 bootleg-jwt-0.3.0/src/bootleg_jwt/
+-rw-r--r--   0 freyja    (1000) freyja    (1000)       95 2023-06-16 23:36:30.000000 bootleg-jwt-0.3.0/src/bootleg_jwt/__init__.py
+-rw-r--r--   0 freyja    (1000) freyja    (1000)     4911 2023-06-17 00:04:02.000000 bootleg-jwt-0.3.0/src/bootleg_jwt/funcs.py
+-rw-r--r--   0 freyja    (1000) freyja    (1000)     5107 2023-06-17 00:44:32.000000 bootleg-jwt-0.3.0/src/bootleg_jwt/main.py
+-rw-r--r--   0 freyja    (1000) freyja    (1000)      142 2023-05-17 09:16:45.000000 bootleg-jwt-0.3.0/src/bootleg_jwt/messages.py
+-rw-r--r--   0 freyja    (1000) freyja    (1000)      813 2023-06-16 23:37:19.000000 bootleg-jwt-0.3.0/src/bootleg_jwt/schema.py
```

### Comparing `bootleg-jwt-0.2.3/LICENSE` & `bootleg-jwt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bootleg-jwt-0.2.3/PKG-INFO` & `bootleg-jwt-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootleg-jwt
-Version: 0.2.3
+Version: 0.3.0
 Summary: Sign tokens with blake2b, then verify them.
 Home-page: https://github.com/freyjagp/bootleg-jwt
 Author: Freyja Odinthrir
 Project-URL: Bug Reports, https://github.com/freyjagp/bootleg-jwt/issues
 Project-URL: Source, https://github.com/freyjagp/bootleg-jwt/
 Keywords: cryptography,tokens,hashing
 Classifier: Development Status :: 4 - Beta
@@ -22,20 +22,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bootleg-jwt <!-- omit in toc -->
 
 `bootleg-jwt` aims to mimic JSON Web Tokens in a simple, `pydantic` way.
 
-This module provides two main functions:
+___
+
+## New for v0.3.0 <!-- omit in toc -->
+
+Version 0.3.0 extends v0.2.x with backwards compatible addition of the `_salt` and `_person` arguments. When these arguments are passed alongside a token, the token's hash is generated using them. Note: the `_salt` and `_person` arguments may not be longer than 16 bytes. This is a limitation of the blake2b hashing algorithm. If a string is supplied, it will be encoded to utf-8 and truncated automatically. Otherwise, any bytestring longer than 16 bytes will fail validation. This is by design.
+
+`_salt` and `_person` allow the token to be namespaced and salted. This provides an extra layer of validation, allowing implementations of `BootlegJWT` to perform more checks on tokens, other than what is baked in. This would allow, for example, invalidating all tokens with a particular salt or namespace.
+
+___
+
+## Table of Contents <!-- omit in toc -->
 
 - [Generate a token](#generate-a-token)
 - [Validate a token](#validate-a-token)
-
-These are designed to be very simple to use. See below:
+- [Renew a token](#renew-a-token)
 
 ## Generate a token
 
 ```python
 from bootleg_jwt import BootlegJWT, Payload, header, body
 from pydantic import BaseModel
 from os import environ              # An environment variable is required.
@@ -327,7 +336,11 @@
     }
 }
 ------------------------------
  True
 
 
 ```
+
+## Renew a token
+
+Using `BootlegJWT.renew(token)`, you may pass a token to BootlegJWT in bytestring form. This function will return an instance of `BootlegJWT` with a new token and expiration date, retaining all of the input token's properties.
```

### Comparing `bootleg-jwt-0.2.3/README.md` & `bootleg-jwt-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 # bootleg-jwt <!-- omit in toc -->
 
 `bootleg-jwt` aims to mimic JSON Web Tokens in a simple, `pydantic` way.
 
-This module provides two main functions:
+___
+
+## New for v0.3.0 <!-- omit in toc -->
+
+Version 0.3.0 extends v0.2.x with backwards compatible addition of the `_salt` and `_person` arguments. When these arguments are passed alongside a token, the token's hash is generated using them. Note: the `_salt` and `_person` arguments may not be longer than 16 bytes. This is a limitation of the blake2b hashing algorithm. If a string is supplied, it will be encoded to utf-8 and truncated automatically. Otherwise, any bytestring longer than 16 bytes will fail validation. This is by design.
+
+`_salt` and `_person` allow the token to be namespaced and salted. This provides an extra layer of validation, allowing implementations of `BootlegJWT` to perform more checks on tokens, other than what is baked in. This would allow, for example, invalidating all tokens with a particular salt or namespace.
+
+___
+
+## Table of Contents <!-- omit in toc -->
 
 - [Generate a token](#generate-a-token)
 - [Validate a token](#validate-a-token)
-
-These are designed to be very simple to use. See below:
+- [Renew a token](#renew-a-token)
 
 ## Generate a token
 
 ```python
 from bootleg_jwt import BootlegJWT, Payload, header, body
 from pydantic import BaseModel
 from os import environ              # An environment variable is required.
@@ -303,7 +312,11 @@
     }
 }
 ------------------------------
  True
 
 
 ```
+
+## Renew a token
+
+Using `BootlegJWT.renew(token)`, you may pass a token to BootlegJWT in bytestring form. This function will return an instance of `BootlegJWT` with a new token and expiration date, retaining all of the input token's properties.
```

### Comparing `bootleg-jwt-0.2.3/bootleg_jwt.egg-info/PKG-INFO` & `bootleg-jwt-0.3.0/bootleg_jwt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootleg-jwt
-Version: 0.2.3
+Version: 0.3.0
 Summary: Sign tokens with blake2b, then verify them.
 Home-page: https://github.com/freyjagp/bootleg-jwt
 Author: Freyja Odinthrir
 Project-URL: Bug Reports, https://github.com/freyjagp/bootleg-jwt/issues
 Project-URL: Source, https://github.com/freyjagp/bootleg-jwt/
 Keywords: cryptography,tokens,hashing
 Classifier: Development Status :: 4 - Beta
@@ -22,20 +22,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bootleg-jwt <!-- omit in toc -->
 
 `bootleg-jwt` aims to mimic JSON Web Tokens in a simple, `pydantic` way.
 
-This module provides two main functions:
+___
+
+## New for v0.3.0 <!-- omit in toc -->
+
+Version 0.3.0 extends v0.2.x with backwards compatible addition of the `_salt` and `_person` arguments. When these arguments are passed alongside a token, the token's hash is generated using them. Note: the `_salt` and `_person` arguments may not be longer than 16 bytes. This is a limitation of the blake2b hashing algorithm. If a string is supplied, it will be encoded to utf-8 and truncated automatically. Otherwise, any bytestring longer than 16 bytes will fail validation. This is by design.
+
+`_salt` and `_person` allow the token to be namespaced and salted. This provides an extra layer of validation, allowing implementations of `BootlegJWT` to perform more checks on tokens, other than what is baked in. This would allow, for example, invalidating all tokens with a particular salt or namespace.
+
+___
+
+## Table of Contents <!-- omit in toc -->
 
 - [Generate a token](#generate-a-token)
 - [Validate a token](#validate-a-token)
-
-These are designed to be very simple to use. See below:
+- [Renew a token](#renew-a-token)
 
 ## Generate a token
 
 ```python
 from bootleg_jwt import BootlegJWT, Payload, header, body
 from pydantic import BaseModel
 from os import environ              # An environment variable is required.
@@ -327,7 +336,11 @@
     }
 }
 ------------------------------
  True
 
 
 ```
+
+## Renew a token
+
+Using `BootlegJWT.renew(token)`, you may pass a token to BootlegJWT in bytestring form. This function will return an instance of `BootlegJWT` with a new token and expiration date, retaining all of the input token's properties.
```

### Comparing `bootleg-jwt-0.2.3/setup.py` & `bootleg-jwt-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `bootleg-jwt-0.2.3/src/bootleg_jwt/schema.py` & `bootleg-jwt-0.3.0/src/bootleg_jwt/schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class Duration(BaseModel):
     unit: Unit = Unit()
     value: int = 60
 
 class Header(BaseModel):
-    type: str = "Default Token Type"
+    type: str
     duration: Duration
     created: Timestamp
     expires: Timestamp
 
 
 class Body(BaseModel):
     user: Any = "USER"
```

