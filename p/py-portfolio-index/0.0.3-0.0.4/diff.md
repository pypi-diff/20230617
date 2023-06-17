# Comparing `tmp/py-portfolio-index-0.0.3.tar.gz` & `tmp/py-portfolio-index-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-index-0.0.3.tar", last modified: Fri Jun 16 17:13:29 2023, max compression
+gzip compressed data, was "py-portfolio-index-0.0.4.tar", last modified: Sat Jun 17 15:34:38 2023, max compression
```

## Comparing `py-portfolio-index-0.0.3.tar` & `py-portfolio-index-0.0.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.643473 py-portfolio-index-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-16 17:13:29.643473 py-portfolio-index-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.631473 py-portfolio-index-0.0.3/py_portfolio_index/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.631473 py-portfolio-index-0.0.3/py_portfolio_index/bin/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.635474 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.639474 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/coal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/cruises.csv
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/fake_meat.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/meat_poultry.csv
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/non_ethical_conduct.csv
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/oil.csv
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/renewable.csv
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/semiconductor.csv
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/space.csv
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/vice.csv
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.643473 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/alpaca.py
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/alpaca_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/base_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/local_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/robinhood.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/py_portfolio_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 17:13:29.631473 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 17:13:29.000000 py-portfolio-index-0.0.3/py_portfolio_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 17:13:29.643473 py-portfolio-index-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-16 17:13:20.000000 py-portfolio-index-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:34:38.499866 py-portfolio-index-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-17 15:34:38.499866 py-portfolio-index-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:34:38.491865 py-portfolio-index-0.0.4/py_portfolio_index/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:34:38.495865 py-portfolio-index-0.0.4/py_portfolio_index/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:34:38.495865 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:34:38.499866 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/coal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/cruises.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/fake_meat.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/meat_poultry.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/non_ethical_conduct.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/oil.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/renewable.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/semiconductor.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/space.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/vice.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:34:38.499866 py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/alpaca_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/local_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/robinhood.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/py_portfolio_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:34:38.495865 py-portfolio-index-0.0.4/py_portfolio_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-06-17 15:34:38.000000 py-portfolio-index-0.0.4/py_portfolio_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-17 15:34:38.000000 py-portfolio-index-0.0.4/py_portfolio_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:34:38.000000 py-portfolio-index-0.0.4/py_portfolio_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-17 15:34:38.000000 py-portfolio-index-0.0.4/py_portfolio_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 15:34:38.000000 py-portfolio-index-0.0.4/py_portfolio_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:34:38.499866 py-portfolio-index-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-17 15:34:25.000000 py-portfolio-index-0.0.4/setup.py
```

### Comparing `py-portfolio-index-0.0.3/LICENSE.txt` & `py-portfolio-index-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/PKG-INFO` & `py-portfolio-index-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-index
-Version: 0.0.3
+Version: 0.0.4
 Summary: Build index portfolios.
 Home-page: 
 Author: 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-portfolio-index-0.0.3/README.md` & `py-portfolio-index-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/__init__.py` & `py-portfolio-index-0.0.4/py_portfolio_index/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from py_portfolio_index.portfolio_providers.alpaca import AlpacaProviderLegacy
 from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
 from py_portfolio_index.portfolio_providers.alpaca_v2 import AlpacaProvider
 from py_portfolio_index.config import get_providers
 
 AVAILABLE_PROVIDERS = get_providers()
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 __all__ = [
     "INDEXES",
     "STOCK_LISTS",
     "Logger",
     "compare_portfolios",
     "AlpacaProvider",
```

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2020_q4.csv` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2021_q4.csv` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2021_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q2.csv` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2022_q2.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q3.csv` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2022_q3.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2022_q4.csv` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2022_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/esgv_2023_q1.csv` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/esgv_2023_q1.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/inventory.py` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/inventory.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,21 @@
     loaded: dict[str, IdealPortfolio] = Field(default_factory = dict)
 
     @classmethod
     def from_path(cls, path):
         path = Path(path)
         if path.is_file():
             path = path.parent
-        keys = [f.stem for f in path.iterdir() if f.suffix== ".csv"]
+        keys = []
+        for f in path.iterdir():
+            try:
+                if f.suffix == ".csv":
+                    keys.append(f.stem)
+            except FileNotFoundError:
+                pass
         return IndexInventory(keys = keys, base = path)
 
     def __getitem__(self, item: str) -> IdealPortfolio:
         if item in self.keys:
             values = self.loaded.get(item, None)
             if values:
                 return values
```

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/qcln_2020_q4.csv` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/qcln_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/inventory.py` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/inventory.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,21 @@
     loaded: dict[str, List[str]] = Field(default_factory = dict)
 
     @classmethod
     def from_path(cls, path):
         path = Path(path)
         if path.is_file():
             path = path.parent
-        keys = [f.stem for f in path.iterdir() if f.suffix== ".csv"]
+        keys = []
+        for f in path.iterdir():
+            try:
+                if f.suffix == ".csv":
+                    keys.append(f.stem)
+            except FileNotFoundError:
+                pass
         return StocklistInventory(keys = keys, base = path)
     
     def __getitem__(self, item: str) -> List[str]:
         if item in self.keys:
             values = self.loaded.get(item, None)
             if values:
                 return values
```

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/bin/lists/oil.csv` & `py-portfolio-index-0.0.4/py_portfolio_index/bin/lists/oil.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/config.py` & `py-portfolio-index-0.0.4/py_portfolio_index/config.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/models.py` & `py-portfolio-index-0.0.4/py_portfolio_index/models.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/operators.py` & `py-portfolio-index-0.0.4/py_portfolio_index/operators.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/alpaca.py` & `py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/alpaca.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/alpaca_v2.py` & `py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/alpaca_v2.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/base_portfolio.py` & `py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/base_portfolio.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/local_dict.py` & `py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/local_dict.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index/portfolio_providers/robinhood.py` & `py-portfolio-index-0.0.4/py_portfolio_index/portfolio_providers/robinhood.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index.egg-info/PKG-INFO` & `py-portfolio-index-0.0.4/py_portfolio_index.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-index
-Version: 0.0.3
+Version: 0.0.4
 Summary: Build index portfolios.
 Home-page: 
 Author: 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `py-portfolio-index-0.0.3/py_portfolio_index.egg-info/SOURCES.txt` & `py-portfolio-index-0.0.4/py_portfolio_index.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.3/setup.py` & `py-portfolio-index-0.0.4/setup.py`

 * *Files identical despite different names*

