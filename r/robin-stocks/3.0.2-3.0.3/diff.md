# Comparing `tmp/robin_stocks-3.0.2.tar.gz` & `tmp/robin_stocks-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_stocks-3.0.2.tar", last modified: Sat Jun 17 02:18:30 2023, max compression
+gzip compressed data, was "robin_stocks-3.0.3.tar", last modified: Sat Jun 17 04:53:44 2023, max compression
```

## Comparing `robin_stocks-3.0.2.tar` & `robin_stocks-3.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.044574 robin_stocks-3.0.2/
--rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.2/LICENSE.txt
--rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.2/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 02:18:30.044156 robin_stocks-3.0.2/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/README.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.026703 robin_stocks-3.0.2/robin_stocks/
--rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.031605 robin_stocks-3.0.2/robin_stocks/gemini/
--rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/account.py
--rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/gemini/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.037597 robin_stocks-3.0.2/robin_stocks/robinhood/
--rw-r--r--   0 josh       (501) staff       (20)     5012 2021-02-23 04:31:10.000000 robin_stocks-3.0.2/robin_stocks/robinhood/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.2/robin_stocks/robinhood/account.py
--rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.2/robin_stocks/robinhood/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.2/robin_stocks/robinhood/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.2/robin_stocks/robinhood/export.py
--rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/robinhood/globals.py
--rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.2/robin_stocks/robinhood/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.2/robin_stocks/robinhood/markets.py
--rw-r--r--   0 josh       (501) staff       (20)    19807 2023-06-17 02:17:53.000000 robin_stocks-3.0.2/robin_stocks/robinhood/options.py
--rw-r--r--   0 josh       (501) staff       (20)    63700 2023-06-17 02:17:53.000000 robin_stocks-3.0.2/robin_stocks/robinhood/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.2/robin_stocks/robinhood/profiles.py
--rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.2/robin_stocks/robinhood/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     7621 2023-06-17 02:17:53.000000 robin_stocks-3.0.2/robin_stocks/robinhood/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.041455 robin_stocks-3.0.2/robin_stocks/tda/
--rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/accounts.py
--rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/helper.py
--rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/markets.py
--rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/orders.py
--rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.2/robin_stocks/tda/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/robin_stocks/tda/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.028450 robin_stocks-3.0.2/robin_stocks.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1330 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.2/robin_stocks.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)       42 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       19 2023-06-17 02:18:29.000000 robin_stocks-3.0.2/robin_stocks.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-06-17 02:18:30.044722 robin_stocks-3.0.2/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      931 2023-06-17 02:17:53.000000 robin_stocks-3.0.2/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 02:18:30.043573 robin_stocks-3.0.2/tests/
--rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.2/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.2/tests/app_tests.py
--rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/tests/test_gemini.py
--rw-r--r--   0 josh       (501) staff       (20)    32945 2023-05-22 02:32:23.000000 robin_stocks-3.0.2/tests/test_robinhood.py
--rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.2/tests/test_tda.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.038479 robin_stocks-3.0.3/
+-rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.3/LICENSE.txt
+-rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.3/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 04:53:44.038055 robin_stocks-3.0.3/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/README.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.019691 robin_stocks-3.0.3/robin_stocks/
+-rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.025204 robin_stocks-3.0.3/robin_stocks/gemini/
+-rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.031423 robin_stocks-3.0.3/robin_stocks/robinhood/
+-rw-r--r--   0 josh       (501) staff       (20)     5012 2021-02-23 04:31:10.000000 robin_stocks-3.0.3/robin_stocks/robinhood/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.3/robin_stocks/robinhood/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.3/robin_stocks/robinhood/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.3/robin_stocks/robinhood/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.3/robin_stocks/robinhood/export.py
+-rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/robinhood/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.3/robin_stocks/robinhood/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.3/robin_stocks/robinhood/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)    19807 2023-06-17 02:17:53.000000 robin_stocks-3.0.3/robin_stocks/robinhood/options.py
+-rw-r--r--   0 josh       (501) staff       (20)    65100 2023-06-17 04:52:06.000000 robin_stocks-3.0.3/robin_stocks/robinhood/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.3/robin_stocks/robinhood/profiles.py
+-rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.3/robin_stocks/robinhood/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     7621 2023-06-17 02:17:53.000000 robin_stocks-3.0.3/robin_stocks/robinhood/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.035377 robin_stocks-3.0.3/robin_stocks/tda/
+-rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/accounts.py
+-rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.3/robin_stocks/tda/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.021814 robin_stocks-3.0.3/robin_stocks.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1330 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.3/robin_stocks.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)       42 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       19 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-06-17 04:53:44.038661 robin_stocks-3.0.3/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      931 2023-06-17 04:52:30.000000 robin_stocks-3.0.3/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.037494 robin_stocks-3.0.3/tests/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.3/tests/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.3/tests/app_tests.py
+-rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/tests/test_gemini.py
+-rw-r--r--   0 josh       (501) staff       (20)    32945 2023-05-22 02:32:23.000000 robin_stocks-3.0.3/tests/test_robinhood.py
+-rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/tests/test_tda.py
```

### Comparing `robin_stocks-3.0.2/LICENSE.txt` & `robin_stocks-3.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/PKG-INFO` & `robin_stocks-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_stocks
-Version: 3.0.2
+Version: 3.0.3
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.2/README.rst` & `robin_stocks-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/gemini/__init__.py` & `robin_stocks-3.0.3/robin_stocks/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/gemini/account.py` & `robin_stocks-3.0.3/robin_stocks/gemini/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/gemini/authentication.py` & `robin_stocks-3.0.3/robin_stocks/gemini/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/gemini/crypto.py` & `robin_stocks-3.0.3/robin_stocks/gemini/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/gemini/globals.py` & `robin_stocks-3.0.3/robin_stocks/gemini/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/gemini/helper.py` & `robin_stocks-3.0.3/robin_stocks/gemini/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/gemini/orders.py` & `robin_stocks-3.0.3/robin_stocks/gemini/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/gemini/urls.py` & `robin_stocks-3.0.3/robin_stocks/gemini/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/__init__.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/account.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/authentication.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/crypto.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/export.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/export.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/globals.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/helper.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/markets.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/options.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/options.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/orders.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/orders.py`

 * *Files 3% similar despite different names*

```diff
@@ -295,48 +295,50 @@
         request_post(item['cancel_url'])
 
     print('All Crypto Orders Cancelled', file=get_output())
     return(data)
 
 
 @login_required
-def order_buy_market(symbol, quantity, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order_buy_market(symbol, quantity, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param quantity: The number of stocks to buy.
     :type quantity: int
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_buy_fractional_by_quantity(symbol, quantity, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param quantity: The amount of the fractional shares you want to buy.
     :type quantity: float
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
@@ -353,16 +355,16 @@
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param amountInDollars: The amount in dollars of the fractional shares you want to buy.
     :type amountInDollars: float
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
@@ -378,88 +380,94 @@
     price = next(iter(get_latest_price(symbol, 'ask_price', extendedHours)), 0.00)
     fractional_shares = 0 if (price == 0.00) else round_price(amountInDollars/float(price))
     
     return order(symbol, fractional_shares, "buy", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_buy_limit(symbol, quantity, limitPrice, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order_buy_limit(symbol, quantity, limitPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a limit order to be executed once a certain price is reached.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param quantity: The number of stocks to buy.
     :type quantity: int
     :param limitPrice: The price to trigger the buy order.
     :type limitPrice: float
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", limitPrice, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", account_number, limitPrice, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_buy_stop_loss(symbol, quantity, stopPrice, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order_buy_stop_loss(symbol, quantity, stopPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a stop order to be turned into a market order once a certain stop price is reached.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param quantity: The number of stocks to buy.
     :type quantity: int
     :param stopPrice: The price to trigger the market order.
     :type stopPrice: float
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", None, stopPrice, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", account_number, None, stopPrice, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_buy_stop_limit(symbol, quantity, limitPrice, stopPrice, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order_buy_stop_limit(symbol, quantity, limitPrice, stopPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a stop order to be turned into a limit order once a certain stop price is reached.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param quantity: The number of stocks to buy.
     :type quantity: int
     :param limitPrice: The price to trigger the market order.
     :type limitPrice: float
     :param stopPrice: The price to trigger the limit order.
     :type stopPrice: float
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", limitPrice, stopPrice, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", account_number, limitPrice, stopPrice, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_buy_trailing_stop(symbol, quantity, trailAmount, trailType='percentage', timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a trailing stop buy order to be turned into a market order when traling stop price reached.
 
     :param symbol: The stock ticker of the stock to buy.
@@ -485,48 +493,50 @@
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
     return order_trailing_stop(symbol, quantity, "buy", trailAmount, trailType, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_sell_market(symbol, quantity, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order_sell_market(symbol, quantity, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately.
 
     :param symbol: The stock ticker of the stock to sell.
     :type symbol: str
     :param quantity: The number of stocks to sell.
     :type quantity: int
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_sell_fractional_by_quantity(symbol, quantity, account_number=None, timeInForce='gfd', priceType='bid_price', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param quantity: The amount of the fractional shares you want to buy.
     :type quantity: float
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
@@ -543,14 +553,16 @@
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param amountInDollars: The amount in dollars of the fractional shares you want to buy.
     :type amountInDollars: float
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
@@ -565,88 +577,94 @@
     price = next(iter(get_latest_price(symbol, 'bid_price', extendedHours)), 0.00)
     fractional_shares = 0 if (price == 0.00) else round_price(amountInDollars/float(price))
 
     return order(symbol, fractional_shares, "sell", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_sell_limit(symbol, quantity, limitPrice, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order_sell_limit(symbol, quantity, limitPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a limit order to be executed once a certain price is reached.
 
     :param symbol: The stock ticker of the stock to sell.
     :type symbol: str
     :param quantity: The number of stocks to sell.
     :type quantity: int
     :param limitPrice: The price to trigger the sell order.
     :type limitPrice: float
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", limitPrice, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", account_number, limitPrice, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_sell_stop_loss(symbol, quantity, stopPrice, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order_sell_stop_loss(symbol, quantity, stopPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a stop order to be turned into a market order once a certain stop price is reached.
 
     :param symbol: The stock ticker of the stock to sell.
     :type symbol: str
     :param quantity: The number of stocks to sell.
     :type quantity: int
     :param stopPrice: The price to trigger the market order.
     :type stopPrice: float
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", None, stopPrice, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", account_number, None, stopPrice, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_sell_stop_limit(symbol, quantity, limitPrice, stopPrice, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order_sell_stop_limit(symbol, quantity, limitPrice, stopPrice, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a stop order to be turned into a limit order once a certain stop price is reached.
 
     :param symbol: The stock ticker of the stock to sell.
     :type symbol: str
     :param quantity: The number of stocks to sell.
     :type quantity: int
     :param limitPrice: The price to trigger the market order.
     :type limitPrice: float
     :param stopPrice: The price to trigger the limit order.
     :type stopPrice: float
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", limitPrice, stopPrice, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", account_number, limitPrice, stopPrice, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_sell_trailing_stop(symbol, quantity, trailAmount, trailType='percentage', timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a trailing stop sell order to be turned into a market order when traling stop price reached.
 
     :param symbol: The stock ticker of the stock to sell.
@@ -672,27 +690,29 @@
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
     return order_trailing_stop(symbol, quantity, "sell", trailAmount, trailType, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_trailing_stop(symbol, quantity, side, trailAmount, trailType='percentage', timeInForce='gtc', extendedHours=False, jsonify=True):
+def order_trailing_stop(symbol, quantity, side, trailAmount, trailType='percentage', account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a trailing stop order to be turned into a market order when traling stop price reached.
 
     :param symbol: The stock ticker of the stock to trade.
     :type symbol: str
     :param quantity: The number of stocks to trade.
     :type quantity: int
     :param side: buy or sell
     :type side: str
     :param trailAmount: how much to trail by; could be percentage or dollar value depending on trailType
     :type trailAmount: float
     :param trailType: could be "amount" or "percentage"
     :type trailType: str
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
@@ -722,15 +742,15 @@
         print('ERROR: {}'.format(e))
         return None
 
     stopPrice = stock_price + margin if side == "buy" else stock_price - margin
     stopPrice = round_price(stopPrice)
 
     payload = {
-        'account': load_account_profile(info='url'),
+        'account': load_account_profile(account_number=account_number, info='url'),
         'instrument': get_instruments_by_symbols(symbol, info='url')[0],
         'symbol': symbol,
         'quantity': quantity,
         'ref_id': str(uuid4()),
         'type': 'market',
         'stop_price': stopPrice,
         'time_in_force': timeInForce,
@@ -751,29 +771,29 @@
     url = orders_url()
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return (data)
 
 
 @login_required
-def order(symbol, quantity, side, account_number=None, limitPrice=None, stopPrice=None, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order(symbol, quantity, side, limitPrice=None, stopPrice=None, account_number=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """A generic order function.
 
     :param symbol: The stock ticker of the stock to sell.
     :type symbol: str
     :param quantity: The number of stocks to sell.
     :type quantity: int
     :param side: Either 'buy' or 'sell'
     :type side: str
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
     :param limitPrice: The price to trigger the market order.
     :type limitPrice: float
     :param stopPrice: The price to trigger the limit or market order.
     :type stopPrice: float
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: str
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
@@ -858,16 +878,16 @@
         - effect: This should be 'open' or 'close'.\n
         - action: This should be 'buy' or 'sell'.
     :type spread: dict
     :param timeInForce: Changes how long the order will be in effect for. \
      'gtc' = good until cancelled. \
      'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' = execute at opening.
     :type timeInForce: Optional[str]
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
     return(order_option_spread("credit", price, symbol, quantity, spread, timeInForce, account_number, jsonify))
@@ -890,27 +910,27 @@
         - effect: This should be 'open' or 'close'.\n
         - action: This should be 'buy' or 'sell'.
     :type spread: dict
     :param timeInForce: Changes how long the order will be in effect for.
      'gtc' = good until cancelled. \
      'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
     return(order_option_spread("debit", price, symbol, quantity, spread, timeInForce, account_number, jsonify))
 
 
 @login_required
-def order_option_spread(direction, price, symbol, quantity, spread, timeInForce='gtc', account_number=None, jsonify=True):
+def order_option_spread(direction, price, symbol, quantity, spread, account_number=None, timeInForce='gtc', jsonify=True):
     """Submits a limit order for an option spread. i.e. place a debit / credit spread
 
     :param direction: Can be "credit" or "debit".
     :type direction: str
     :param price: The limit price to trigger a trade of the option.
     :type price: float
     :param symbol: The stock ticker of the stock to trade.
@@ -920,22 +940,22 @@
     :param spread: A dictionary of spread options with the following keys: \n
         - expirationDate: The expiration date of the option in 'YYYY-MM-DD' format.\n
         - strike: The strike price of the option.\n
         - optionType: This should be 'call' or 'put'.\n
         - effect: This should be 'open' or 'close'.\n
         - action: This should be 'buy' or 'sell'.
     :type spread: dict
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for.
      'gtc' = good until cancelled. \
      'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """ 
     try:
         symbol = symbol.upper().strip()
     except AttributeError as message:
@@ -969,15 +989,15 @@
     url = option_orders_url()
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return(data)
 
 
 @login_required
-def order_buy_option_limit(positionEffect, creditOrDebit, price, symbol, quantity, expirationDate, strike, optionType='both', timeInForce='gtc', account_number=None, jsonify=True):
+def order_buy_option_limit(positionEffect, creditOrDebit, price, symbol, quantity, expirationDate, strike, optionType='both', account_number=None, timeInForce='gtc', jsonify=True):
     """Submits a limit order for an option. i.e. place a long call or a long put.
 
     :param positionEffect: Either 'open' for a buy to open effect or 'close' for a buy to close effect.
     :type positionEffect: str
     :param creditOrDebit: Either 'debit' or 'credit'.
     :type creditOrDebit: str
     :param price: The limit price to trigger a buy of the option.
@@ -988,19 +1008,19 @@
     :type quantity: int
     :param expirationDate: The expiration date of the option in 'YYYY-MM-DD' format.
     :type expirationDate: str
     :param strike: The strike price of the option.
     :type strike: float
     :param optionType: This should be 'call' or 'put'
     :type optionType: str
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the buying of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
@@ -1032,15 +1052,15 @@
     url = option_orders_url()
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return(data)
 
 
 @login_required
-def order_buy_option_stop_limit(positionEffect, creditOrDebit, limitPrice, stopPrice, symbol, quantity, expirationDate, strike, optionType='both', timeInForce='gtc', jsonify=True):
+def order_buy_option_stop_limit(positionEffect, creditOrDebit, limitPrice, stopPrice, symbol, quantity, expirationDate, strike, optionType='both', account_number=None, timeInForce='gtc', jsonify=True):
     """Submits a stop order to be turned into a limit order once a certain stop price is reached.
 
     :param positionEffect: Either 'open' for a buy to open effect or 'close' for a buy to close effect.
     :type positionEffect: str
     :param creditOrDebit: Either 'debit' or 'credit'.
     :type creditOrDebit: str
     :param limitPrice: The limit price to trigger a buy of the option.
@@ -1053,19 +1073,19 @@
     :type quantity: int
     :param expirationDate: The expiration date of the option in 'YYYY-MM-DD' format.
     :type expirationDate: str
     :param strike: The strike price of the option.
     :type strike: float
     :param optionType: This should be 'call' or 'put'
     :type optionType: str
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the buying of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
@@ -1074,15 +1094,15 @@
     except AttributeError as message:
         print(message, file=get_output())
         return None
 
     optionID = id_for_option(symbol, expirationDate, strike, optionType)
 
     payload = {
-        'account': load_account_profile(info='url'),
+        'account': load_account_profile(account_number=account_number, info='url'),
         'direction': creditOrDebit,
         'time_in_force': timeInForce,
         'legs': [
             {'position_effect': positionEffect, 'side': 'buy',
                 'ratio_quantity': 1, 'option': option_instruments_url(optionID)},
         ],
         'type': 'limit',
@@ -1097,15 +1117,15 @@
 
     url = option_orders_url()
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return(data)
 
 
-def order_sell_option_stop_limit(positionEffect, creditOrDebit, limitPrice, stopPrice, symbol, quantity, expirationDate, strike, optionType='both', timeInForce='gtc', jsonify=True):
+def order_sell_option_stop_limit(positionEffect, creditOrDebit, limitPrice, stopPrice, symbol, quantity, expirationDate, strike, optionType='both', account_number=None, timeInForce='gtc', jsonify=True):
     """Submits a stop order to be turned into a limit order once a certain stop price is reached.
 
     :param positionEffect: Either 'open' for a buy to open effect or 'close' for a buy to close effect.
     :type positionEffect: str
     :param creditOrDebit: Either 'debit' or 'credit'.
     :type creditOrDebit: str
     :param limitPrice: The limit price to trigger a buy of the option.
@@ -1118,19 +1138,19 @@
     :type quantity: int
     :param expirationDate: The expiration date of the option in 'YYYY-MM-DD' format.
     :type expirationDate: str
     :param strike: The strike price of the option.
     :type strike: float
     :param optionType: This should be 'call' or 'put'
     :type optionType: str
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the buying of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
@@ -1139,15 +1159,15 @@
     except AttributeError as message:
         print(message, file=get_output())
         return None
 
     optionID = id_for_option(symbol, expirationDate, strike, optionType)
 
     payload = {
-        'account': load_account_profile(info='url'),
+        'account': load_account_profile(account_number=account_number, info='url'),
         'direction': creditOrDebit,
         'time_in_force': timeInForce,
         'legs': [
             {'position_effect': positionEffect, 'side': 'sell',
                 'ratio_quantity': 1, 'option': option_instruments_url(optionID)},
         ],
         'type': 'limit',
@@ -1163,15 +1183,15 @@
     url = option_orders_url()
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return(data)
 
 
 @login_required
-def order_sell_option_limit(positionEffect, creditOrDebit, price, symbol, quantity, expirationDate, strike, optionType='both', timeInForce='gtc', account_number=None, jsonify=True):
+def order_sell_option_limit(positionEffect, creditOrDebit, price, symbol, quantity, expirationDate, strike, optionType='both', account_number=None, timeInForce='gtc', jsonify=True):
     """Submits a limit order for an option. i.e. place a short call or a short put.
 
     :param positionEffect: Either 'open' for a sell to open effect or 'close' for a sell to close effect.
     :type positionEffect: str
     :param creditOrDebit: Either 'debit' or 'credit'.
     :type creditOrDebit: str
     :param price: The limit price to trigger a sell of the option.
@@ -1182,19 +1202,19 @@
     :type quantity: int
     :param expirationDate: The expiration date of the option in 'YYYY-MM-DD' format.
     :type expirationDate: str
     :param strike: The strike price of the option.
     :type strike: float
     :param optionType: This should be 'call' or 'put'
     :type optionType: str
+    :param account_number: the robinhood account number.
+    :type account_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
-    :param acccount_number: the robinhood account number.
-    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """
```

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/profiles.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/profiles.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/stocks.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/robinhood/urls.py` & `robin_stocks-3.0.3/robin_stocks/robinhood/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/tda/__init__.py` & `robin_stocks-3.0.3/robin_stocks/tda/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/tda/accounts.py` & `robin_stocks-3.0.3/robin_stocks/tda/accounts.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/tda/authentication.py` & `robin_stocks-3.0.3/robin_stocks/tda/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/tda/globals.py` & `robin_stocks-3.0.3/robin_stocks/tda/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/tda/helper.py` & `robin_stocks-3.0.3/robin_stocks/tda/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/tda/markets.py` & `robin_stocks-3.0.3/robin_stocks/tda/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/tda/orders.py` & `robin_stocks-3.0.3/robin_stocks/tda/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/tda/stocks.py` & `robin_stocks-3.0.3/robin_stocks/tda/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks/tda/urls.py` & `robin_stocks-3.0.3/robin_stocks/tda/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/robin_stocks.egg-info/PKG-INFO` & `robin_stocks-3.0.3/robin_stocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-stocks
-Version: 3.0.2
+Version: 3.0.3
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.2/robin_stocks.egg-info/SOURCES.txt` & `robin_stocks-3.0.3/robin_stocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/setup.py` & `robin_stocks-3.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='robin_stocks',
-      version='3.0.2',
+      version='3.0.3',
       description='A Python wrapper around the Robinhood API',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       url='https://github.com/jmfernandes/robin_stocks',
       author='Josh Fernandes',
       author_email='joshfernandes@mac.com',
       keywords=['robinhood','robin stocks','finance app','stocks','options','trading','investing'],
```

### Comparing `robin_stocks-3.0.2/tests/app_tests.py` & `robin_stocks-3.0.3/tests/app_tests.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/tests/test_gemini.py` & `robin_stocks-3.0.3/tests/test_gemini.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/tests/test_robinhood.py` & `robin_stocks-3.0.3/tests/test_robinhood.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.2/tests/test_tda.py` & `robin_stocks-3.0.3/tests/test_tda.py`

 * *Files identical despite different names*

