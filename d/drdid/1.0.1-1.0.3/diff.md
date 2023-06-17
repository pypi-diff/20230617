# Comparing `tmp/drdid-1.0.1.tar.gz` & `tmp/drdid-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drdid-1.0.1.tar", last modified: Sat Jun 17 01:23:18 2023, max compression
+gzip compressed data, was "drdid-1.0.3.tar", last modified: Sat Jun 17 01:29:07 2023, max compression
```

## Comparing `drdid-1.0.1.tar` & `drdid-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:23:18.315676 drdid-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-17 01:23:08.000000 drdid-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-17 01:23:18.315676 drdid-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:23:18.315676 drdid-1.0.1/drdid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:23:08.000000 drdid-1.0.1/drdid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-17 01:23:08.000000 drdid-1.0.1/drdid/_version_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-17 01:23:08.000000 drdid-1.0.1/drdid/drdid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-17 01:23:08.000000 drdid-1.0.1/drdid/ipwd_did.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-17 01:23:08.000000 drdid-1.0.1/drdid/reg_did.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-17 01:23:08.000000 drdid-1.0.1/drdid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:23:18.315676 drdid-1.0.1/drdid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-17 01:23:18.000000 drdid-1.0.1/drdid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-17 01:23:18.000000 drdid-1.0.1/drdid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:23:18.000000 drdid-1.0.1/drdid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 01:23:18.000000 drdid-1.0.1/drdid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 01:23:18.000000 drdid-1.0.1/drdid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:23:18.315676 drdid-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-17 01:23:08.000000 drdid-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:29:07.873012 drdid-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-17 01:28:57.000000 drdid-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-17 01:29:07.873012 drdid-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:29:07.873012 drdid-1.0.3/drdid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:28:57.000000 drdid-1.0.3/drdid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-17 01:28:57.000000 drdid-1.0.3/drdid/_version_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-06-17 01:28:57.000000 drdid-1.0.3/drdid/drdid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-17 01:28:57.000000 drdid-1.0.3/drdid/ipwd_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-17 01:28:57.000000 drdid-1.0.3/drdid/reg_did.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-17 01:28:57.000000 drdid-1.0.3/drdid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:29:07.873012 drdid-1.0.3/drdid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-17 01:29:07.000000 drdid-1.0.3/drdid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-17 01:29:07.000000 drdid-1.0.3/drdid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:29:07.000000 drdid-1.0.3/drdid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 01:29:07.000000 drdid-1.0.3/drdid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 01:29:07.000000 drdid-1.0.3/drdid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:29:07.873012 drdid-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-17 01:28:57.000000 drdid-1.0.3/setup.py
```

### Comparing `drdid-1.0.1/LICENSE` & `drdid-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drdid-1.0.1/drdid/drdid.py` & `drdid-1.0.3/drdid/drdid.py`

 * *Files identical despite different names*

### Comparing `drdid-1.0.1/drdid/ipwd_did.py` & `drdid-1.0.3/drdid/ipwd_did.py`

 * *Files identical despite different names*

### Comparing `drdid-1.0.1/drdid/reg_did.py` & `drdid-1.0.3/drdid/reg_did.py`

 * *Files identical despite different names*

### Comparing `drdid-1.0.1/drdid/utils.py` & `drdid-1.0.3/drdid/utils.py`

 * *Files identical despite different names*

