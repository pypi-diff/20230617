# Comparing `tmp/robin_stocks-3.0.1.tar.gz` & `tmp/robin_stocks-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_stocks-3.0.1.tar", last modified: Mon May 22 03:03:17 2023, max compression
+gzip compressed data, was "robin_stocks-3.0.2.tar", last modified: Sat Jun 17 02:18:30 2023, max compression
```

## Comparing `robin_stocks-3.0.1.tar` & `robin_stocks-3.0.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.538196 robin_stocks-3.0.1/
--rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.1/LICENSE.txt
--rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.1/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-05-22 03:03:17.537774 robin_stocks-3.0.1/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/README.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.518837 robin_stocks-3.0.1/robin_stocks/
--rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.524616 robin_stocks-3.0.1/robin_stocks/gemini/
--rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/account.py
--rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.530730 robin_stocks-3.0.1/robin_stocks/robinhood/
--rw-r--r--   0 josh       (501) staff       (20)     5012 2021-02-23 04:31:10.000000 robin_stocks-3.0.1/robin_stocks/robinhood/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.1/robin_stocks/robinhood/account.py
--rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.1/robin_stocks/robinhood/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.1/robin_stocks/robinhood/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.1/robin_stocks/robinhood/export.py
--rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/robinhood/globals.py
--rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.1/robin_stocks/robinhood/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.1/robin_stocks/robinhood/markets.py
--rw-r--r--   0 josh       (501) staff       (20)    20319 2023-05-22 00:46:39.000000 robin_stocks-3.0.1/robin_stocks/robinhood/options.py
--rw-r--r--   0 josh       (501) staff       (20)    63387 2023-05-22 01:12:04.000000 robin_stocks-3.0.1/robin_stocks/robinhood/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.1/robin_stocks/robinhood/profiles.py
--rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.1/robin_stocks/robinhood/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     7567 2023-05-22 02:23:50.000000 robin_stocks-3.0.1/robin_stocks/robinhood/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.534925 robin_stocks-3.0.1/robin_stocks/tda/
--rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/accounts.py
--rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/helper.py
--rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/markets.py
--rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/orders.py
--rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.1/robin_stocks/tda/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.520827 robin_stocks-3.0.1/robin_stocks.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1330 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.1/robin_stocks.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)       42 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       19 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-05-22 03:03:17.538312 robin_stocks-3.0.1/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      931 2023-05-22 03:00:44.000000 robin_stocks-3.0.1/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.537151 robin_stocks-3.0.1/tests/
--rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.1/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.1/tests/app_tests.py
--rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/tests/test_gemini.py
--rw-r--r--   0 josh       (501) staff       (20)    32945 2023-05-22 02:32:23.000000 robin_stocks-3.0.1/tests/test_robinhood.py
--rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/tests/test_tda.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.044574 robin_stocks-3.0.2/
+-rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.2/LICENSE.txt
+-rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.2/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 02:18:30.044156 robin_stocks-3.0.2/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/README.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.026703 robin_stocks-3.0.2/robin_stocks/
+-rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.031605 robin_stocks-3.0.2/robin_stocks/gemini/
+-rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.037597 robin_stocks-3.0.2/robin_stocks/robinhood/
+-rw-r--r--   0 josh       (501) staff       (20)     5012 2021-02-23 04:31:10.000000 robin_stocks-3.0.2/robin_stocks/robinhood/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.2/robin_stocks/robinhood/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.2/robin_stocks/robinhood/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.2/robin_stocks/robinhood/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.2/robin_stocks/robinhood/export.py
+-rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/robinhood/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.2/robin_stocks/robinhood/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.2/robin_stocks/robinhood/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)    19807 2023-06-17 02:17:53.000000 robin_stocks-3.0.2/robin_stocks/robinhood/options.py
+-rw-r--r--   0 josh       (501) staff       (20)    63700 2023-06-17 02:17:53.000000 robin_stocks-3.0.2/robin_stocks/robinhood/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.2/robin_stocks/robinhood/profiles.py
+-rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.2/robin_stocks/robinhood/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     7621 2023-06-17 02:17:53.000000 robin_stocks-3.0.2/robin_stocks/robinhood/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.041455 robin_stocks-3.0.2/robin_stocks/tda/
+-rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/accounts.py
+-rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.2/robin_stocks/tda/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.028450 robin_stocks-3.0.2/robin_stocks.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1330 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.2/robin_stocks.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)       42 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       19 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-06-17 02:18:30.044722 robin_stocks-3.0.2/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      931 2023-06-17 02:17:53.000000 robin_stocks-3.0.2/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.043573 robin_stocks-3.0.2/tests/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.2/tests/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.2/tests/app_tests.py
+-rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/tests/test_gemini.py
+-rw-r--r--   0 josh       (501) staff       (20)    32945 2023-05-22 02:32:23.000000 robin_stocks-3.0.2/tests/test_robinhood.py
+-rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/tests/test_tda.py
```

### Comparing `robin_stocks-3.0.1/LICENSE.txt` & `robin_stocks-3.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/PKG-INFO` & `robin_stocks-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_stocks
-Version: 3.0.1
+Version: 3.0.2
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.1/README.rst` & `robin_stocks-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/gemini/__init__.py` & `robin_stocks-3.0.2/robin_stocks/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/gemini/account.py` & `robin_stocks-3.0.2/robin_stocks/gemini/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/gemini/authentication.py` & `robin_stocks-3.0.2/robin_stocks/gemini/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/gemini/crypto.py` & `robin_stocks-3.0.2/robin_stocks/gemini/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/gemini/globals.py` & `robin_stocks-3.0.2/robin_stocks/gemini/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/gemini/helper.py` & `robin_stocks-3.0.2/robin_stocks/gemini/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/gemini/orders.py` & `robin_stocks-3.0.2/robin_stocks/gemini/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/gemini/urls.py` & `robin_stocks-3.0.2/robin_stocks/gemini/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/__init__.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/account.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/authentication.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/crypto.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/export.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/export.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/globals.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/helper.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/markets.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/options.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -330,51 +330,23 @@
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
     :returns: Returns a dictionary of key/value pairs for the stock. \
     If info parameter is provided, the value of the key that matches info is extracted.
 
     """
     instrument = get_option_instrument_data_by_id(id)
-    url = marketdata_options_url()
-    payload = {
-        "instruments" : instrument['url']
-    }
-    data = request_get(url, 'results', payload)
-
-    if not data:
-        data= {
-        'adjusted_mark_price':'',
-        'ask_price':'',
-        'ask_size':'',
-        'bid_price':'',
-        'bid_size':'',
-        'break_even_price':'',
-        'high_price':'',
-        'instrument':'',
-        'last_trade_price':'',
-        'last_trade_size':'',
-        'low_price':'',
-        'mark_price':'',
-        'open_interest':'',
-        'previous_close_date':'',
-        'previous_close_price':'',
-        'volume':'',
-        'chance_of_profit_long':'',
-        'chance_of_profit_short':'',
-        'delta':'',
-        'gamma':'',
-        'implied_volatility':'',
-        'rho':'',
-        'theta':'',
-        'vega':'',
-        'high_fill_rate_buy_price':'',
-        'high_fill_rate_sell_price':'',
-        'low_fill_rate_buy_price':'',
-        'low_fill_rate_sell_price':''
-        }
+    if instrument is None:
+      # e.g. 503 Server Error: Service Unavailable for url: https://api.robinhood.com/options/instruments/d1058013-09a2-4063-b6b0-92717e17d0c0/
+      return None  # just return None which the caller can easily check; do NOT use faked empty data, it will only cause future problem
+    else:
+      payload = {
+          "instruments" : instrument['url']
+      }
+      url = marketdata_options_url()
+      data = request_get(url, 'results', payload)
 
     return(filter_data(data, info))
 
 @login_required
 def get_option_market_data(inputSymbols, expirationDate, strikePrice, optionType, info=None):
     """Returns the option market data for the stock option, including the greeks,
     open interest, change of profit, and adjusted mark price.
```

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/orders.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/orders.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,24 +67,24 @@
 
     data = [item for item in data if item['cancel'] is not None]
 
     return(filter_data(data, info))
 
 
 @login_required
-def get_all_open_option_orders(info=None):
+def get_all_open_option_orders(info=None, account_number=None):
     """Returns a list of all the orders that are currently open.
 
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
     :returns: Returns a list of dictionaries of key/value pairs for each order. If info parameter is provided, \
     a list of strings is returned where the strings are the value of the key that matches info.
 
     """
-    url = option_orders_url()
+    url = option_orders_url(account_number=account_number)
     data = request_get(url, 'pagination')
 
     data = [item for item in data if item['cancel_url'] is not None]
 
     return(filter_data(data, info))
 
 
@@ -373,15 +373,15 @@
     if amountInDollars < 1:
         print("ERROR: Fractional share price should meet minimum 1.00.", file=get_output())
         return None
 
     # turn the money amount into decimal number of shares
     price = next(iter(get_latest_price(symbol, 'ask_price', extendedHours)), 0.00)
     fractional_shares = 0 if (price == 0.00) else round_price(amountInDollars/float(price))
-
+    
     return order(symbol, fractional_shares, "buy", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_buy_limit(symbol, quantity, limitPrice, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a limit order to be executed once a certain price is reached.
 
@@ -823,14 +823,19 @@
         'type': orderType,
         'stop_price': stopPrice,
         'time_in_force': timeInForce,
         'trigger': trigger,
         'side': side,
         'extended_hours': extendedHours
     }
+    # BEGIN PATCH FOR NEW ROBINHOOD BUY FORM (GuitarGuyChrisB 5/26/2023)
+    if side == "buy":
+        payload['order_form_version'] = "2"
+        payload['preset_percent_limit'] = "0.05"
+    # END PATCH FOR NEW ROBINHOOD BUY FORM (GuitarGuyChrisB 5/26/2023)
 
     url = orders_url()
 
 
     data = request_post(url, payload, jsonify_data=jsonify)
 
     return(data)
```

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/profiles.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/profiles.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/stocks.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/robinhood/urls.py` & `robin_stocks-3.0.2/robin_stocks/robinhood/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -207,19 +207,22 @@
 def option_instruments_url(id=None):
     if id:
         return('https://api.robinhood.com/options/instruments/{0}/'.format(id))
     else:
         return('https://api.robinhood.com/options/instruments/')
 
 
-def option_orders_url(orderID=None):
+def option_orders_url(orderID=None, account_number=None):
+    url = 'https://api.robinhood.com/options/orders/'
     if orderID:
-        return('https://api.robinhood.com/options/orders/{0}/'.format(orderID))
-    else:
-        return('https://api.robinhood.com/options/orders/')
+        url += '{0}/'.format(orderID)
+    if account_number:
+        url += ('?account_numbers='+account_number)
+
+    return url
 
 
 def option_positions_url(account_number):
     if account_number:
         return('https://api.robinhood.com/options/positions/?account_numbers='+account_number)
     else:
         return('https://api.robinhood.com/options/positions/')
```

### Comparing `robin_stocks-3.0.1/robin_stocks/tda/__init__.py` & `robin_stocks-3.0.2/robin_stocks/tda/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/tda/accounts.py` & `robin_stocks-3.0.2/robin_stocks/tda/accounts.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/tda/authentication.py` & `robin_stocks-3.0.2/robin_stocks/tda/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/tda/globals.py` & `robin_stocks-3.0.2/robin_stocks/tda/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/tda/helper.py` & `robin_stocks-3.0.2/robin_stocks/tda/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/tda/markets.py` & `robin_stocks-3.0.2/robin_stocks/tda/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/tda/orders.py` & `robin_stocks-3.0.2/robin_stocks/tda/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/tda/stocks.py` & `robin_stocks-3.0.2/robin_stocks/tda/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks/tda/urls.py` & `robin_stocks-3.0.2/robin_stocks/tda/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/robin_stocks.egg-info/PKG-INFO` & `robin_stocks-3.0.2/robin_stocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-stocks
-Version: 3.0.1
+Version: 3.0.2
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.1/robin_stocks.egg-info/SOURCES.txt` & `robin_stocks-3.0.2/robin_stocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/setup.py` & `robin_stocks-3.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='robin_stocks',
-      version='3.0.1',
+      version='3.0.2',
       description='A Python wrapper around the Robinhood API',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       url='https://github.com/jmfernandes/robin_stocks',
       author='Josh Fernandes',
       author_email='joshfernandes@mac.com',
       keywords=['robinhood','robin stocks','finance app','stocks','options','trading','investing'],
```

### Comparing `robin_stocks-3.0.1/tests/app_tests.py` & `robin_stocks-3.0.2/tests/app_tests.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/tests/test_gemini.py` & `robin_stocks-3.0.2/tests/test_gemini.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/tests/test_robinhood.py` & `robin_stocks-3.0.2/tests/test_robinhood.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.1/tests/test_tda.py` & `robin_stocks-3.0.2/tests/test_tda.py`

 * *Files identical despite different names*

