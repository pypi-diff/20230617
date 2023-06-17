# Comparing `tmp/python-benedict-0.8.0.tar.gz` & `tmp/python-benedict-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-benedict-0.8.0.tar", last modified: Fri Sep 20 14:25:18 2019, max compression
+gzip compressed data, was "dist/python-benedict-0.9.0.tar", last modified: Mon Sep 23 12:14:48 2019, max compression
```

## Comparing `python-benedict-0.8.0.tar` & `python-benedict-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-20 14:25:18.000000 python-benedict-0.8.0/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-20 14:25:18.000000 python-benedict-0.8.0/benedict/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      184 2019-07-05 15:16:17.000000 python-benedict-0.8.0/benedict/__init__.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-20 14:25:18.000000 python-benedict-0.8.0/benedict/dicts/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3262 2019-09-17 08:25:27.000000 python-benedict-0.8.0/benedict/dicts/__init__.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     4132 2019-09-20 13:07:29.000000 python-benedict-0.8.0/benedict/dicts/io.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     5787 2019-08-30 11:53:52.000000 python-benedict-0.8.0/benedict/dicts/keypath.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     8579 2019-07-05 15:27:55.000000 python-benedict-0.8.0/benedict/dicts/parse.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1315 2019-09-12 14:24:27.000000 python-benedict-0.8.0/benedict/dicts/utility.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      293 2019-09-20 13:41:36.000000 python-benedict-0.8.0/benedict/metadata.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-20 14:25:18.000000 python-benedict-0.8.0/benedict/utils/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        0 2019-06-05 09:45:03.000000 python-benedict-0.8.0/benedict/utils/__init__.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3390 2019-09-17 09:15:52.000000 python-benedict-0.8.0/benedict/utils/io_util.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1103 2019-07-09 11:08:33.000000 python-benedict-0.8.0/benedict/utils/keypath_util.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     4409 2019-09-11 13:59:29.000000 python-benedict-0.8.0/benedict/utils/parse_util.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1591 2019-09-12 14:51:43.000000 python-benedict-0.8.0/benedict/utils/utility_util.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1069 2019-05-15 14:04:33.000000 python-benedict-0.8.0/LICENSE.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      115 2019-05-14 08:51:58.000000 python-benedict-0.8.0/MANIFEST.in
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    17782 2019-09-20 14:25:18.000000 python-benedict-0.8.0/PKG-INFO
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-20 14:25:18.000000 python-benedict-0.8.0/python_benedict.egg-info/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        1 2019-09-20 14:25:18.000000 python-benedict-0.8.0/python_benedict.egg-info/dependency_links.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    17782 2019-09-20 14:25:18.000000 python-benedict-0.8.0/python_benedict.egg-info/PKG-INFO
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      162 2019-09-20 14:25:18.000000 python-benedict-0.8.0/python_benedict.egg-info/requires.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      556 2019-09-20 14:25:18.000000 python-benedict-0.8.0/python_benedict.egg-info/SOURCES.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        9 2019-09-20 14:25:18.000000 python-benedict-0.8.0/python_benedict.egg-info/top_level.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    13110 2019-09-20 14:15:51.000000 python-benedict-0.8.0/README.md
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       79 2019-09-20 14:25:18.000000 python-benedict-0.8.0/setup.cfg
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2289 2019-07-18 14:46:08.000000 python-benedict-0.8.0/setup.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-23 12:14:48.000000 python-benedict-0.9.0/
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-23 12:14:48.000000 python-benedict-0.9.0/benedict/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      184 2019-07-05 15:16:17.000000 python-benedict-0.9.0/benedict/__init__.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-23 12:14:48.000000 python-benedict-0.9.0/benedict/dicts/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3262 2019-09-17 08:25:27.000000 python-benedict-0.9.0/benedict/dicts/__init__.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     4391 2019-09-23 10:33:37.000000 python-benedict-0.9.0/benedict/dicts/io.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     5787 2019-08-30 11:53:52.000000 python-benedict-0.9.0/benedict/dicts/keypath.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     8579 2019-07-05 15:27:55.000000 python-benedict-0.9.0/benedict/dicts/parse.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1315 2019-09-12 14:24:27.000000 python-benedict-0.9.0/benedict/dicts/utility.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      293 2019-09-23 10:59:34.000000 python-benedict-0.9.0/benedict/metadata.py
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-23 12:14:48.000000 python-benedict-0.9.0/benedict/utils/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        0 2019-06-05 09:45:03.000000 python-benedict-0.9.0/benedict/utils/__init__.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     3810 2019-09-23 10:45:31.000000 python-benedict-0.9.0/benedict/utils/io_util.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1103 2019-07-09 11:08:33.000000 python-benedict-0.9.0/benedict/utils/keypath_util.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     4409 2019-09-11 13:59:29.000000 python-benedict-0.9.0/benedict/utils/parse_util.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1591 2019-09-12 14:51:43.000000 python-benedict-0.9.0/benedict/utils/utility_util.py
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1069 2019-05-15 14:04:33.000000 python-benedict-0.9.0/LICENSE.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      115 2019-05-14 08:51:58.000000 python-benedict-0.9.0/MANIFEST.in
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    18526 2019-09-23 12:14:48.000000 python-benedict-0.9.0/PKG-INFO
+drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2019-09-23 12:14:48.000000 python-benedict-0.9.0/python_benedict.egg-info/
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        1 2019-09-23 12:14:48.000000 python-benedict-0.9.0/python_benedict.egg-info/dependency_links.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    18526 2019-09-23 12:14:48.000000 python-benedict-0.9.0/python_benedict.egg-info/PKG-INFO
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      162 2019-09-23 12:14:48.000000 python-benedict-0.9.0/python_benedict.egg-info/requires.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)      556 2019-09-23 12:14:48.000000 python-benedict-0.9.0/python_benedict.egg-info/SOURCES.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)        9 2019-09-23 12:14:48.000000 python-benedict-0.9.0/python_benedict.egg-info/top_level.txt
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)    13694 2019-09-23 11:07:37.000000 python-benedict-0.9.0/README.md
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)       79 2019-09-23 12:14:48.000000 python-benedict-0.9.0/setup.cfg
+-rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2289 2019-07-18 14:46:08.000000 python-benedict-0.9.0/setup.py
```

### Comparing `python-benedict-0.8.0/benedict/dicts/__init__.py` & `python-benedict-0.9.0/benedict/dicts/__init__.py`

 * *Files identical despite different names*

### Comparing `python-benedict-0.8.0/benedict/dicts/io.py` & `python-benedict-0.9.0/benedict/dicts/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,25 +60,33 @@
         try:
             d = IODict.from_json(s, **kwargs)
         except ValueError:
             try:
                 d = IODict.from_toml(s, **kwargs)
             except ValueError:
                 try:
-                    d = IODict.from_yaml(s, **kwargs)
+                    d = IODict.from_xml(s, **kwargs)
                 except ValueError:
-                    d = None
+                    try:
+                        d = IODict.from_yaml(s, **kwargs)
+                    except ValueError:
+                        d = None
         return d
 
     # @staticmethod
     # def from_base64(s, **kwargs):
     #     return IODict._load_and_decode(s,
     #         io_util.decode_base64, **kwargs)
 
     @staticmethod
+    def from_csv(s, **kwargs):
+        return IODict._load_and_decode(s,
+            io_util.decode_csv, **kwargs)
+
+    @staticmethod
     def from_json(s, **kwargs):
         return IODict._load_and_decode(s,
             io_util.decode_json, **kwargs)
 
     # @staticmethod
     # def from_query_string(s, **kwargs):
     #     return IODict._load_and_decode(s,
```

### Comparing `python-benedict-0.8.0/benedict/dicts/keypath.py` & `python-benedict-0.9.0/benedict/dicts/keypath.py`

 * *Files identical despite different names*

### Comparing `python-benedict-0.8.0/benedict/dicts/parse.py` & `python-benedict-0.9.0/benedict/dicts/parse.py`

 * *Files identical despite different names*

### Comparing `python-benedict-0.8.0/benedict/dicts/utility.py` & `python-benedict-0.9.0/benedict/dicts/utility.py`

 * *Files identical despite different names*

### Comparing `python-benedict-0.8.0/benedict/utils/io_util.py` & `python-benedict-0.9.0/benedict/utils/io_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # -*- coding: utf-8 -*-
 
-# import base64
+from six import StringIO
+
+import base64
+import csv
 import errno
 import json
 import os
 import requests
 import xmltodict
 import toml
 import yaml
@@ -25,14 +28,22 @@
 #     # from urlparse import parse_qs, urlparse
 
 # def decode_base64(s, **kwargs):
 #     j = base64.b64decode(s, **kwargs)
 #     return decode_json(j, **kwargs)
 
 
+def decode_csv(s, **kwargs):
+    kwargs.setdefault('delimiter', ';')
+    kwargs.setdefault('quoting', csv.QUOTE_ALL)
+    f = StringIO(s)
+    data = csv.DictReader(f, **kwargs)
+    return data
+
+
 def decode_json(s, **kwargs):
     data = json.loads(s, **kwargs)
     return data
 
 
 # def decode_query_string(s, **kwargs):
 #     if s.startswith('https://') or s.startswith('http://'):
@@ -58,14 +69,15 @@
 #     #     key = kv[0]
 #     #     val = url_unquote(kv[1])
 #     #     d[key] = val
 #     # return d
 
 
 def decode_xml(s, **kwargs):
+    kwargs.setdefault('dict_constructor', dict)
     data = xmltodict.parse(s, **kwargs)
     return data
 
 
 def decode_toml(s, **kwargs):
     data = toml.loads(s, **kwargs)
     return data
@@ -78,14 +90,20 @@
 
 
 # def encode_base64(d, **kwargs):
 #     j = encode_json(d, **kwargs)
 #     return base64.b64encode(j, **kwargs)
 
 
+# def encode_csv(d, **kwargs):
+#     kwargs.setdefault('delimiter', ';')
+#     kwargs.setdefault('quoting', csv.QUOTE_ALL)
+#     return data
+
+
 def encode_json(d, **kwargs):
     data = json.dumps(d, **kwargs)
     return data
 
 
 # def encode_query_string(d, **kwargs):
 #     return ''#url_quote(d)
```

### Comparing `python-benedict-0.8.0/benedict/utils/keypath_util.py` & `python-benedict-0.9.0/benedict/utils/keypath_util.py`

 * *Files identical despite different names*

### Comparing `python-benedict-0.8.0/benedict/utils/parse_util.py` & `python-benedict-0.9.0/benedict/utils/parse_util.py`

 * *Files identical despite different names*

### Comparing `python-benedict-0.8.0/benedict/utils/utility_util.py` & `python-benedict-0.9.0/benedict/utils/utility_util.py`

 * *Files identical despite different names*

### Comparing `python-benedict-0.8.0/LICENSE.txt` & `python-benedict-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python-benedict-0.8.0/PKG-INFO` & `python-benedict-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: python-benedict
-Version: 0.8.0
+Version: 0.9.0
 Summary: The Python dictionary for humans dealing with evil/complex data.
 Home-page: https://github.com/fabiocaccamo/python-benedict
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 License: MIT
-Download-URL: https://github.com/fabiocaccamo/python-benedict/archive/0.8.0.tar.gz
+Download-URL: https://github.com/fabiocaccamo/python-benedict/archive/0.9.0.tar.gz
 Description: [![Build Status](https://travis-ci.org/fabiocaccamo/python-benedict.svg?branch=master)](https://travis-ci.org/fabiocaccamo/python-benedict)
         [![codecov](https://codecov.io/gh/fabiocaccamo/python-benedict/branch/master/graph/badge.svg)](https://codecov.io/gh/fabiocaccamo/python-benedict)
         [![Codacy Badge](https://api.codacy.com/project/badge/Grade/0dbd5cc2089f4dce80a0e49e6822be3c)](https://www.codacy.com/app/fabiocaccamo/python-benedict)
         [![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/fabiocaccamo/python-benedict/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/fabiocaccamo/python-benedict/?branch=master)
         [![Requirements Status](https://requires.io/github/fabiocaccamo/python-benedict/requirements.svg?branch=master)](https://requires.io/github/fabiocaccamo/python-benedict/requirements/?branch=master)
         [![PyPI version](https://badge.fury.io/py/python-benedict.svg)](https://badge.fury.io/py/python-benedict)
         [![PyPI downloads](https://img.shields.io/pypi/dm/python-benedict.svg)](https://img.shields.io/pypi/dm/python-benedict.svg)
@@ -30,17 +30,19 @@
                 -   [List keypaths](#list-keypaths)
                 -   [Custom keypath separator](#custom-keypath-separator)
                 -   [Disable keypath functionality](#disable-keypath-functionality)
         -   [API](#api)
             -   [I/O](#io)
                 -   [`from_json`](#from_json)
                 -   [`from_toml`](#from_toml)
+                -   [`from_xml`](#from_xml)
                 -   [`from_yaml`](#from_yaml)
                 -   [`to_json`](#to_json)
                 -   [`to_toml`](#to_toml)
+                -   [`to_xml`](#to_xml)
                 -   [`to_yaml`](#to_yaml)
             -   [Parse](#parse)
                 -   [`get_bool`](#get_bool)
                 -   [`get_bool_list`](#get_bool_list)
                 -   [`get_datetime`](#get_datetime)
                 -   [`get_datetime_list`](#get_datetime_list)
                 -   [`get_decimal`](#get_decimal)
@@ -68,15 +70,15 @@
                 -   [`remove`](#remove)
                 -   [`subset`](#subset)
         -   [Testing](#testing)
         -   [License](#license)
         
         ## Features
         -   Full **keypath** support *(using the dot syntax by default)*
-        -   Easy **I/O operations** with most common formats: `json`, `toml`, `yaml`
+        -   Easy **I/O operations** with most common formats: `json`, `toml`, `xml`, `yaml`
         -   Many **utility** and **parse methods** to retrieve data as needed *(all methods listed below)*
         -   Give **benediction** :) to `dict` values before they are returned *(they receive benedict casting)*
         -   100% **backward-compatible** *(you can replace existing dicts without pain)*
         
         ## Requirements
         -   Python 2.7, 3.4, 3.5, 3.6, 3.7
         
@@ -141,44 +143,53 @@
         d = benedict(existing_dict, keypath_separator='/')
         ```
         
         #### Disable keypath functionality
         You can disable the keypath functionality passing `keypath_separator=None` in the constructor.
         
         ```python
-        d = benedict(existing_dict, keypath_separator='/')
+        d = benedict(existing_dict, keypath_separator=None)
         ```
         
         ## API
         
         ### I/O
-        These methods simplify I/O operations with most common formats: `json`, `toml`, `yaml`
+        These methods simplify I/O operations with most common formats: `json`, `toml`, `xml`, `yaml`
         
         -   ##### from_json
         
         ```python
-        # Try to load/decode a json encoded string and return it as dict instance.
+        # Try to load/decode a json encoded data and return it as dict instance.
         # Accept as first argument: url, filepath or string.
         # A ValueError is raised in case of failure.
         benedict.from_json(s)
         ```
         
         -   ##### from_toml
         
         ```python
-        # Try to load/decode a toml encoded string and return it as dict instance.
+        # Try to load/decode a toml encoded data and return it as dict instance.
         # Accept as first argument: url, filepath or string.
         # A ValueError is raised in case of failure.
         benedict.from_toml(s)
         ```
         
+        -   ##### from_xml
+        
+        ```python
+        # Try to load/decode a xml encoded data and return it as dict instance.
+        # Accept as first argument: url, filepath or string.
+        # A ValueError is raised in case of failure.
+        benedict.from_xml(s)
+        ```
+        
         -   ##### from_yaml
         
         ```python
-        # Try to load/decode a yaml encoded string and return it as dict instance.
+        # Try to load/decode a yaml encoded data and return it as dict instance.
         # Accept as first argument: url, filepath or string.
         # A ValueError is raised in case of failure.
         benedict.from_yaml(s)
         ```
         
         -   ##### to_json
         
@@ -194,14 +205,23 @@
         ```python
         # Return the dict instance encoded in toml format and optionally save it at the specified filepath.
         # It's possible to pass custom options to the encoder using kwargs.
         # A ValueError is raised in case of failure.
         s = d.to_toml(filepath='', **kwargs)
         ```
         
+        -   ##### to_xml
+        
+        ```python
+        # Return the dict instance encoded in xml format and optionally save it at the specified filepath.
+        # It's possible to pass custom options to the encoder using kwargs.
+        # A ValueError is raised in case of failure.
+        s = d.to_xml(filepath='', **kwargs)
+        ```
+        
         -   ##### to_yaml
         
         ```python
         # Return the dict instance encoded in yaml format and optionally save it at the specified filepath.
         # It's possible to pass custom options to the encoder using kwargs.
         # A ValueError is raised in case of failure.
         s = d.to_yaml(filepath='', **kwargs)
```

### Comparing `python-benedict-0.8.0/python_benedict.egg-info/PKG-INFO` & `python-benedict-0.9.0/python_benedict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: python-benedict
-Version: 0.8.0
+Version: 0.9.0
 Summary: The Python dictionary for humans dealing with evil/complex data.
 Home-page: https://github.com/fabiocaccamo/python-benedict
 Author: Fabio Caccamo
 Author-email: fabio.caccamo@gmail.com
 License: MIT
-Download-URL: https://github.com/fabiocaccamo/python-benedict/archive/0.8.0.tar.gz
+Download-URL: https://github.com/fabiocaccamo/python-benedict/archive/0.9.0.tar.gz
 Description: [![Build Status](https://travis-ci.org/fabiocaccamo/python-benedict.svg?branch=master)](https://travis-ci.org/fabiocaccamo/python-benedict)
         [![codecov](https://codecov.io/gh/fabiocaccamo/python-benedict/branch/master/graph/badge.svg)](https://codecov.io/gh/fabiocaccamo/python-benedict)
         [![Codacy Badge](https://api.codacy.com/project/badge/Grade/0dbd5cc2089f4dce80a0e49e6822be3c)](https://www.codacy.com/app/fabiocaccamo/python-benedict)
         [![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/fabiocaccamo/python-benedict/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/fabiocaccamo/python-benedict/?branch=master)
         [![Requirements Status](https://requires.io/github/fabiocaccamo/python-benedict/requirements.svg?branch=master)](https://requires.io/github/fabiocaccamo/python-benedict/requirements/?branch=master)
         [![PyPI version](https://badge.fury.io/py/python-benedict.svg)](https://badge.fury.io/py/python-benedict)
         [![PyPI downloads](https://img.shields.io/pypi/dm/python-benedict.svg)](https://img.shields.io/pypi/dm/python-benedict.svg)
@@ -30,17 +30,19 @@
                 -   [List keypaths](#list-keypaths)
                 -   [Custom keypath separator](#custom-keypath-separator)
                 -   [Disable keypath functionality](#disable-keypath-functionality)
         -   [API](#api)
             -   [I/O](#io)
                 -   [`from_json`](#from_json)
                 -   [`from_toml`](#from_toml)
+                -   [`from_xml`](#from_xml)
                 -   [`from_yaml`](#from_yaml)
                 -   [`to_json`](#to_json)
                 -   [`to_toml`](#to_toml)
+                -   [`to_xml`](#to_xml)
                 -   [`to_yaml`](#to_yaml)
             -   [Parse](#parse)
                 -   [`get_bool`](#get_bool)
                 -   [`get_bool_list`](#get_bool_list)
                 -   [`get_datetime`](#get_datetime)
                 -   [`get_datetime_list`](#get_datetime_list)
                 -   [`get_decimal`](#get_decimal)
@@ -68,15 +70,15 @@
                 -   [`remove`](#remove)
                 -   [`subset`](#subset)
         -   [Testing](#testing)
         -   [License](#license)
         
         ## Features
         -   Full **keypath** support *(using the dot syntax by default)*
-        -   Easy **I/O operations** with most common formats: `json`, `toml`, `yaml`
+        -   Easy **I/O operations** with most common formats: `json`, `toml`, `xml`, `yaml`
         -   Many **utility** and **parse methods** to retrieve data as needed *(all methods listed below)*
         -   Give **benediction** :) to `dict` values before they are returned *(they receive benedict casting)*
         -   100% **backward-compatible** *(you can replace existing dicts without pain)*
         
         ## Requirements
         -   Python 2.7, 3.4, 3.5, 3.6, 3.7
         
@@ -141,44 +143,53 @@
         d = benedict(existing_dict, keypath_separator='/')
         ```
         
         #### Disable keypath functionality
         You can disable the keypath functionality passing `keypath_separator=None` in the constructor.
         
         ```python
-        d = benedict(existing_dict, keypath_separator='/')
+        d = benedict(existing_dict, keypath_separator=None)
         ```
         
         ## API
         
         ### I/O
-        These methods simplify I/O operations with most common formats: `json`, `toml`, `yaml`
+        These methods simplify I/O operations with most common formats: `json`, `toml`, `xml`, `yaml`
         
         -   ##### from_json
         
         ```python
-        # Try to load/decode a json encoded string and return it as dict instance.
+        # Try to load/decode a json encoded data and return it as dict instance.
         # Accept as first argument: url, filepath or string.
         # A ValueError is raised in case of failure.
         benedict.from_json(s)
         ```
         
         -   ##### from_toml
         
         ```python
-        # Try to load/decode a toml encoded string and return it as dict instance.
+        # Try to load/decode a toml encoded data and return it as dict instance.
         # Accept as first argument: url, filepath or string.
         # A ValueError is raised in case of failure.
         benedict.from_toml(s)
         ```
         
+        -   ##### from_xml
+        
+        ```python
+        # Try to load/decode a xml encoded data and return it as dict instance.
+        # Accept as first argument: url, filepath or string.
+        # A ValueError is raised in case of failure.
+        benedict.from_xml(s)
+        ```
+        
         -   ##### from_yaml
         
         ```python
-        # Try to load/decode a yaml encoded string and return it as dict instance.
+        # Try to load/decode a yaml encoded data and return it as dict instance.
         # Accept as first argument: url, filepath or string.
         # A ValueError is raised in case of failure.
         benedict.from_yaml(s)
         ```
         
         -   ##### to_json
         
@@ -194,14 +205,23 @@
         ```python
         # Return the dict instance encoded in toml format and optionally save it at the specified filepath.
         # It's possible to pass custom options to the encoder using kwargs.
         # A ValueError is raised in case of failure.
         s = d.to_toml(filepath='', **kwargs)
         ```
         
+        -   ##### to_xml
+        
+        ```python
+        # Return the dict instance encoded in xml format and optionally save it at the specified filepath.
+        # It's possible to pass custom options to the encoder using kwargs.
+        # A ValueError is raised in case of failure.
+        s = d.to_xml(filepath='', **kwargs)
+        ```
+        
         -   ##### to_yaml
         
         ```python
         # Return the dict instance encoded in yaml format and optionally save it at the specified filepath.
         # It's possible to pass custom options to the encoder using kwargs.
         # A ValueError is raised in case of failure.
         s = d.to_yaml(filepath='', **kwargs)
```

### Comparing `python-benedict-0.8.0/python_benedict.egg-info/SOURCES.txt` & `python-benedict-0.9.0/python_benedict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-benedict-0.8.0/README.md` & `python-benedict-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,19 @@
         -   [List keypaths](#list-keypaths)
         -   [Custom keypath separator](#custom-keypath-separator)
         -   [Disable keypath functionality](#disable-keypath-functionality)
 -   [API](#api)
     -   [I/O](#io)
         -   [`from_json`](#from_json)
         -   [`from_toml`](#from_toml)
+        -   [`from_xml`](#from_xml)
         -   [`from_yaml`](#from_yaml)
         -   [`to_json`](#to_json)
         -   [`to_toml`](#to_toml)
+        -   [`to_xml`](#to_xml)
         -   [`to_yaml`](#to_yaml)
     -   [Parse](#parse)
         -   [`get_bool`](#get_bool)
         -   [`get_bool_list`](#get_bool_list)
         -   [`get_datetime`](#get_datetime)
         -   [`get_datetime_list`](#get_datetime_list)
         -   [`get_decimal`](#get_decimal)
@@ -59,15 +61,15 @@
         -   [`remove`](#remove)
         -   [`subset`](#subset)
 -   [Testing](#testing)
 -   [License](#license)
 
 ## Features
 -   Full **keypath** support *(using the dot syntax by default)*
--   Easy **I/O operations** with most common formats: `json`, `toml`, `yaml`
+-   Easy **I/O operations** with most common formats: `json`, `toml`, `xml`, `yaml`
 -   Many **utility** and **parse methods** to retrieve data as needed *(all methods listed below)*
 -   Give **benediction** :) to `dict` values before they are returned *(they receive benedict casting)*
 -   100% **backward-compatible** *(you can replace existing dicts without pain)*
 
 ## Requirements
 -   Python 2.7, 3.4, 3.5, 3.6, 3.7
 
@@ -132,44 +134,53 @@
 d = benedict(existing_dict, keypath_separator='/')
 ```
 
 #### Disable keypath functionality
 You can disable the keypath functionality passing `keypath_separator=None` in the constructor.
 
 ```python
-d = benedict(existing_dict, keypath_separator='/')
+d = benedict(existing_dict, keypath_separator=None)
 ```
 
 ## API
 
 ### I/O
-These methods simplify I/O operations with most common formats: `json`, `toml`, `yaml`
+These methods simplify I/O operations with most common formats: `json`, `toml`, `xml`, `yaml`
 
 -   ##### from_json
 
 ```python
-# Try to load/decode a json encoded string and return it as dict instance.
+# Try to load/decode a json encoded data and return it as dict instance.
 # Accept as first argument: url, filepath or string.
 # A ValueError is raised in case of failure.
 benedict.from_json(s)
 ```
 
 -   ##### from_toml
 
 ```python
-# Try to load/decode a toml encoded string and return it as dict instance.
+# Try to load/decode a toml encoded data and return it as dict instance.
 # Accept as first argument: url, filepath or string.
 # A ValueError is raised in case of failure.
 benedict.from_toml(s)
 ```
 
+-   ##### from_xml
+
+```python
+# Try to load/decode a xml encoded data and return it as dict instance.
+# Accept as first argument: url, filepath or string.
+# A ValueError is raised in case of failure.
+benedict.from_xml(s)
+```
+
 -   ##### from_yaml
 
 ```python
-# Try to load/decode a yaml encoded string and return it as dict instance.
+# Try to load/decode a yaml encoded data and return it as dict instance.
 # Accept as first argument: url, filepath or string.
 # A ValueError is raised in case of failure.
 benedict.from_yaml(s)
 ```
 
 -   ##### to_json
 
@@ -185,14 +196,23 @@
 ```python
 # Return the dict instance encoded in toml format and optionally save it at the specified filepath.
 # It's possible to pass custom options to the encoder using kwargs.
 # A ValueError is raised in case of failure.
 s = d.to_toml(filepath='', **kwargs)
 ```
 
+-   ##### to_xml
+
+```python
+# Return the dict instance encoded in xml format and optionally save it at the specified filepath.
+# It's possible to pass custom options to the encoder using kwargs.
+# A ValueError is raised in case of failure.
+s = d.to_xml(filepath='', **kwargs)
+```
+
 -   ##### to_yaml
 
 ```python
 # Return the dict instance encoded in yaml format and optionally save it at the specified filepath.
 # It's possible to pass custom options to the encoder using kwargs.
 # A ValueError is raised in case of failure.
 s = d.to_yaml(filepath='', **kwargs)
```

### Comparing `python-benedict-0.8.0/setup.py` & `python-benedict-0.9.0/setup.py`

 * *Files identical despite different names*

