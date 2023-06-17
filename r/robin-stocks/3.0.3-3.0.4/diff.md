# Comparing `tmp/robin_stocks-3.0.3.tar.gz` & `tmp/robin_stocks-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin_stocks-3.0.3.tar", last modified: Sat Jun 17 04:53:44 2023, max compression
+gzip compressed data, was "robin_stocks-3.0.4.tar", last modified: Sat Jun 17 05:01:07 2023, max compression
```

## Comparing `robin_stocks-3.0.3.tar` & `robin_stocks-3.0.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.038479 robin_stocks-3.0.3/
--rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.3/LICENSE.txt
--rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.3/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 04:53:44.038055 robin_stocks-3.0.3/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/README.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.019691 robin_stocks-3.0.3/robin_stocks/
--rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.025204 robin_stocks-3.0.3/robin_stocks/gemini/
--rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/account.py
--rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/gemini/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.031423 robin_stocks-3.0.3/robin_stocks/robinhood/
--rw-r--r--   0 josh       (501) staff       (20)     5012 2021-02-23 04:31:10.000000 robin_stocks-3.0.3/robin_stocks/robinhood/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.3/robin_stocks/robinhood/account.py
--rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.3/robin_stocks/robinhood/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.3/robin_stocks/robinhood/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.3/robin_stocks/robinhood/export.py
--rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/robinhood/globals.py
--rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.3/robin_stocks/robinhood/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.3/robin_stocks/robinhood/markets.py
--rw-r--r--   0 josh       (501) staff       (20)    19807 2023-06-17 02:17:53.000000 robin_stocks-3.0.3/robin_stocks/robinhood/options.py
--rw-r--r--   0 josh       (501) staff       (20)    65100 2023-06-17 04:52:06.000000 robin_stocks-3.0.3/robin_stocks/robinhood/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.3/robin_stocks/robinhood/profiles.py
--rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.3/robin_stocks/robinhood/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     7621 2023-06-17 02:17:53.000000 robin_stocks-3.0.3/robin_stocks/robinhood/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.035377 robin_stocks-3.0.3/robin_stocks/tda/
--rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/accounts.py
--rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/helper.py
--rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/markets.py
--rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/orders.py
--rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.3/robin_stocks/tda/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/robin_stocks/tda/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.021814 robin_stocks-3.0.3/robin_stocks.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1330 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.3/robin_stocks.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)       42 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       19 2023-06-17 04:53:43.000000 robin_stocks-3.0.3/robin_stocks.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-06-17 04:53:44.038661 robin_stocks-3.0.3/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      931 2023-06-17 04:52:30.000000 robin_stocks-3.0.3/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 04:53:44.037494 robin_stocks-3.0.3/tests/
--rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.3/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.3/tests/app_tests.py
--rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/tests/test_gemini.py
--rw-r--r--   0 josh       (501) staff       (20)    32945 2023-05-22 02:32:23.000000 robin_stocks-3.0.3/tests/test_robinhood.py
--rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.3/tests/test_tda.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.416613 robin_stocks-3.0.4/
+-rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.4/LICENSE.txt
+-rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.4/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 05:01:07.416217 robin_stocks-3.0.4/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/README.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.398390 robin_stocks-3.0.4/robin_stocks/
+-rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.403811 robin_stocks-3.0.4/robin_stocks/gemini/
+-rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/gemini/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.409840 robin_stocks-3.0.4/robin_stocks/robinhood/
+-rw-r--r--   0 josh       (501) staff       (20)     5064 2023-06-17 04:58:36.000000 robin_stocks-3.0.4/robin_stocks/robinhood/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.4/robin_stocks/robinhood/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.4/robin_stocks/robinhood/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.4/robin_stocks/robinhood/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.4/robin_stocks/robinhood/export.py
+-rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/robinhood/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.4/robin_stocks/robinhood/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.4/robin_stocks/robinhood/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)    20412 2023-06-17 04:58:36.000000 robin_stocks-3.0.4/robin_stocks/robinhood/options.py
+-rw-r--r--   0 josh       (501) staff       (20)    65100 2023-06-17 04:52:06.000000 robin_stocks-3.0.4/robin_stocks/robinhood/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.4/robin_stocks/robinhood/profiles.py
+-rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.4/robin_stocks/robinhood/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     7621 2023-06-17 02:17:53.000000 robin_stocks-3.0.4/robin_stocks/robinhood/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.413592 robin_stocks-3.0.4/robin_stocks/tda/
+-rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/accounts.py
+-rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.4/robin_stocks/tda/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/robin_stocks/tda/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.400360 robin_stocks-3.0.4/robin_stocks.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1330 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.4/robin_stocks.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)       42 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       19 2023-06-17 05:01:07.000000 robin_stocks-3.0.4/robin_stocks.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-06-17 05:01:07.416724 robin_stocks-3.0.4/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      931 2023-06-17 05:00:40.000000 robin_stocks-3.0.4/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-06-17 05:01:07.415647 robin_stocks-3.0.4/tests/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.4/tests/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.4/tests/app_tests.py
+-rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/tests/test_gemini.py
+-rw-r--r--   0 josh       (501) staff       (20)    32945 2023-05-22 02:32:23.000000 robin_stocks-3.0.4/tests/test_robinhood.py
+-rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.4/tests/test_tda.py
```

### Comparing `robin_stocks-3.0.3/LICENSE.txt` & `robin_stocks-3.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/PKG-INFO` & `robin_stocks-3.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_stocks
-Version: 3.0.3
+Version: 3.0.4
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.3/README.rst` & `robin_stocks-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/gemini/__init__.py` & `robin_stocks-3.0.4/robin_stocks/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/gemini/account.py` & `robin_stocks-3.0.4/robin_stocks/gemini/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/gemini/authentication.py` & `robin_stocks-3.0.4/robin_stocks/gemini/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/gemini/crypto.py` & `robin_stocks-3.0.4/robin_stocks/gemini/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/gemini/globals.py` & `robin_stocks-3.0.4/robin_stocks/gemini/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/gemini/helper.py` & `robin_stocks-3.0.4/robin_stocks/gemini/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/gemini/orders.py` & `robin_stocks-3.0.4/robin_stocks/gemini/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/gemini/urls.py` & `robin_stocks-3.0.4/robin_stocks/gemini/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/__init__.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
                       get_market_next_open_hours_after_date,
                       get_market_today_hours, get_markets, get_top_100,
                       get_top_movers, get_top_movers_sp500)
 from .options import (find_options_by_expiration,
                       find_options_by_expiration_and_strike,
                       find_options_by_specific_profitability,
                       find_options_by_strike, find_tradable_options,
+                      get_aggregate_open_positions,
                       get_aggregate_positions, get_all_option_positions,
                       get_chains, get_market_options,
                       get_open_option_positions, get_option_historicals,
                       get_option_instrument_data,
                       get_option_instrument_data_by_id, get_option_market_data,
                       get_option_market_data_by_id)
 from .orders import (cancel_all_crypto_orders, cancel_all_option_orders,
```

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/account.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/authentication.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/crypto.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/export.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/export.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/globals.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/helper.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/markets.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/options.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,29 @@
     a list of strings is returned where the strings are the value of the key that matches info.
 
     """
     url = aggregate_url()
     data = request_get(url, 'pagination')
     return(filter_data(data, info))
 
+@login_required
+def get_aggregate_open_positions(info=None):
+    """Collapses all open option positions for a stock into a single dictionary.
+
+    :param info: Will filter the results to get a specific value.
+    :type info: Optional[str]
+    :returns: Returns a list of dictionaries of key/value pairs for each order. If info parameter is provided, \
+    a list of strings is returned where the strings are the value of the key that matches info.
+
+    """
+    url = aggregate_url()
+    payload = {'nonzero': 'True'}
+    data = request_get(url, 'pagination', payload)
+    return(filter_data(data, info))
+
 
 @login_required
 def get_market_options(info=None):
     """Returns a list of all options.
 
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
```

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/orders.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/profiles.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/profiles.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/stocks.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/robinhood/urls.py` & `robin_stocks-3.0.4/robin_stocks/robinhood/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/tda/__init__.py` & `robin_stocks-3.0.4/robin_stocks/tda/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/tda/accounts.py` & `robin_stocks-3.0.4/robin_stocks/tda/accounts.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/tda/authentication.py` & `robin_stocks-3.0.4/robin_stocks/tda/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/tda/globals.py` & `robin_stocks-3.0.4/robin_stocks/tda/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/tda/helper.py` & `robin_stocks-3.0.4/robin_stocks/tda/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/tda/markets.py` & `robin_stocks-3.0.4/robin_stocks/tda/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/tda/orders.py` & `robin_stocks-3.0.4/robin_stocks/tda/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/tda/stocks.py` & `robin_stocks-3.0.4/robin_stocks/tda/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks/tda/urls.py` & `robin_stocks-3.0.4/robin_stocks/tda/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/robin_stocks.egg-info/PKG-INFO` & `robin_stocks-3.0.4/robin_stocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-stocks
-Version: 3.0.3
+Version: 3.0.4
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Requires: requests
```

### Comparing `robin_stocks-3.0.3/robin_stocks.egg-info/SOURCES.txt` & `robin_stocks-3.0.4/robin_stocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/setup.py` & `robin_stocks-3.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='robin_stocks',
-      version='3.0.3',
+      version='3.0.4',
       description='A Python wrapper around the Robinhood API',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       url='https://github.com/jmfernandes/robin_stocks',
       author='Josh Fernandes',
       author_email='joshfernandes@mac.com',
       keywords=['robinhood','robin stocks','finance app','stocks','options','trading','investing'],
```

### Comparing `robin_stocks-3.0.3/tests/app_tests.py` & `robin_stocks-3.0.4/tests/app_tests.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/tests/test_gemini.py` & `robin_stocks-3.0.4/tests/test_gemini.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/tests/test_robinhood.py` & `robin_stocks-3.0.4/tests/test_robinhood.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.3/tests/test_tda.py` & `robin_stocks-3.0.4/tests/test_tda.py`

 * *Files identical despite different names*

