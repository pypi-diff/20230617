# Comparing `tmp/finops-0.1.1.tar.gz` & `tmp/finops-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.1.1.tar", last modified: Sat Jun 17 11:58:35 2023, max compression
+gzip compressed data, was "finops-0.1.2.tar", last modified: Sat Jun 17 12:20:03 2023, max compression
```

## Comparing `finops-0.1.1.tar` & `finops-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.537871 finops-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-17 11:58:26.000000 finops-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-17 11:58:35.537871 finops-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-17 11:58:26.000000 finops-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.533871 finops-0.1.1/finops/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 11:58:26.000000 finops-0.1.1/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-17 11:58:26.000000 finops-0.1.1/finops/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 11:58:26.000000 finops-0.1.1/finops/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-17 11:58:26.000000 finops-0.1.1/finops/tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-17 11:58:26.000000 finops-0.1.1/finops/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.533871 finops-0.1.1/finops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.000000 finops-0.1.1/finops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-17 11:58:26.000000 finops-0.1.1/finops/utils/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-17 11:58:26.000000 finops-0.1.1/finops/utils/base_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 11:58:26.000000 finops-0.1.1/finops/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.533871 finops-0.1.1/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 11:58:35.537871 finops-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-17 11:58:26.000000 finops-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.537871 finops-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.000000 finops-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.537871 finops-0.1.1/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_utils/test_base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_utils/test_base_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-17 12:19:51.000000 finops-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-17 12:20:03.773547 finops-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-17 12:19:51.000000 finops-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 12:19:51.000000 finops-0.1.2/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-17 12:19:51.000000 finops-0.1.2/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 12:19:51.000000 finops-0.1.2/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-17 12:19:51.000000 finops-0.1.2/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-17 12:19:51.000000 finops-0.1.2/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 12:19:51.000000 finops-0.1.2/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-17 12:19:51.000000 finops-0.1.2/finops/utils/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-17 12:19:51.000000 finops-0.1.2/finops/utils/base_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 12:19:51.000000 finops-0.1.2/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 12:20:03.000000 finops-0.1.2/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 12:20:03.773547 finops-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-17 12:19:51.000000 finops-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 12:19:51.000000 finops-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 12:20:03.773547 finops-0.1.2/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_utils/test_base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-17 12:19:51.000000 finops-0.1.2/tests/test_utils/test_base_scraper.py
```

### Comparing `finops-0.1.1/LICENSE` & `finops-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/README.md` & `finops-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 FinOps is a python package for financial operations.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contributing](#contributing)
-- [License](#license)
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install finops.
 
 ```pip install finops```
```

### Comparing `finops-0.1.1/finops/config.py` & `finops-0.1.2/finops/config.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/finops/tehran_stock_exchange.py` & `finops-0.1.2/finops/tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/finops/ticker.py` & `finops-0.1.2/finops/ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/finops/utils/base_downloader.py` & `finops-0.1.2/finops/utils/base_downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/finops/utils/base_scraper.py` & `finops-0.1.2/finops/utils/base_scraper.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/finops.egg-info/SOURCES.txt` & `finops-0.1.2/finops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/tests/test_tehran_stock_exchange.py` & `finops-0.1.2/tests/test_tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/tests/test_ticker.py` & `finops-0.1.2/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/tests/test_utils/test_base_downloader.py` & `finops-0.1.2/tests/test_utils/test_base_downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.1/tests/test_utils/test_base_scraper.py` & `finops-0.1.2/tests/test_utils/test_base_scraper.py`

 * *Files identical despite different names*

