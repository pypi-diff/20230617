# Comparing `tmp/finops-0.1.0.tar.gz` & `tmp/finops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops-0.1.0.tar", last modified: Fri Jun 16 23:13:26 2023, max compression
+gzip compressed data, was "finops-0.1.1.tar", last modified: Sat Jun 17 11:58:35 2023, max compression
```

## Comparing `finops-0.1.0.tar` & `finops-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-16 23:13:16.000000 finops-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 23:13:26.561515 finops-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-16 23:13:16.000000 finops-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/finops/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-16 23:13:16.000000 finops-0.1.0/finops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-16 23:13:16.000000 finops-0.1.0/finops/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-16 23:13:16.000000 finops-0.1.0/finops/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-16 23:13:16.000000 finops-0.1.0/finops/tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-16 23:13:16.000000 finops-0.1.0/finops/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/finops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:16.000000 finops-0.1.0/finops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-16 23:13:16.000000 finops-0.1.0/finops/utils/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-16 23:13:16.000000 finops-0.1.0/finops/utils/base_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-16 23:13:16.000000 finops-0.1.0/finops/utils/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/finops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 23:13:26.000000 finops-0.1.0/finops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 23:13:26.561515 finops-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-16 23:13:16.000000 finops-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:16.000000 finops-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_tehran_stock_exchange.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:26.561515 finops-0.1.0/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_utils/test_base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-16 23:13:16.000000 finops-0.1.0/tests/test_utils/test_base_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.537871 finops-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-17 11:58:26.000000 finops-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-17 11:58:35.537871 finops-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-17 11:58:26.000000 finops-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.533871 finops-0.1.1/finops/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-17 11:58:26.000000 finops-0.1.1/finops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-17 11:58:26.000000 finops-0.1.1/finops/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 11:58:26.000000 finops-0.1.1/finops/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-17 11:58:26.000000 finops-0.1.1/finops/tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-17 11:58:26.000000 finops-0.1.1/finops/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.533871 finops-0.1.1/finops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.000000 finops-0.1.1/finops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-17 11:58:26.000000 finops-0.1.1/finops/utils/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-17 11:58:26.000000 finops-0.1.1/finops/utils/base_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-17 11:58:26.000000 finops-0.1.1/finops/utils/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.533871 finops-0.1.1/finops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 11:58:35.000000 finops-0.1.1/finops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 11:58:35.537871 finops-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-17 11:58:26.000000 finops-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.537871 finops-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.000000 finops-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_tehran_stock_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:35.537871 finops-0.1.1/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_utils/test_base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-17 11:58:26.000000 finops-0.1.1/tests/test_utils/test_base_scraper.py
```

### Comparing `finops-0.1.0/LICENSE` & `finops-0.1.1/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-Copyright (c) 2005-2023, FinOps Developers.
+BSD 3-Clause License
+Copyright (c) 2021 - 2023, FinOps
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are
-met:
+modification, are permitted provided that the following conditions are met:
 
-    * Redistributions of source code must retain the above copyright
-       notice, this list of conditions and the following disclaimer.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
-    * Redistributions in binary form must reproduce the above
-       copyright notice, this list of conditions and the following
-       disclaimer in the documentation and/or other materials provided
-       with the distribution.
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
 
-    * Neither the name of the FinOps Developers nor the names of any
-       contributors may be used to endorse or promote products derived
-       from this software without specific prior written permission.
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
 
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `finops-0.1.0/PKG-INFO` & `finops-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.0
+Version: 0.1.1
 Summary: Financial tools for the rest of us.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `finops-0.1.0/finops/config.py` & `finops-0.1.1/finops/config.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.0/finops/tehran_stock_exchange.py` & `finops-0.1.1/finops/tehran_stock_exchange.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -68,17 +68,17 @@
     ):
         Ticker(ticker_index).get_shareholder_data(
             start_date, end_date, store_path, log_path
         )
 
     def get_shareholders_data(
         self,
-        tickers_index_list,
         start_date,
         end_date,
+        tickers_index_list,
         store_path,
         log_path,
         n_threads=1,
     ):
         if tickers_index_list is None:
             tickers_index_list = self.get_stock_tickers_index_list()
         with concurrent.futures.ThreadPoolExecutor(max_workers=n_threads) as executor:
```

### Comparing `finops-0.1.0/finops/ticker.py` & `finops-0.1.1/finops/ticker.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,27 +5,28 @@
     SHAREHOLDER_DATA_COLUMNS,
     PRICE_HISTORY_DATA_COLUMNS,
     LOG_COLUMNS,
     USER_AGENT,
     PRICE_HISTORY_FIELD_MAP,
     SHAREHOLDER_FIELD_MAP,
 )
+from finops.utils.wrappers import catch
 from finops.logger import logger
 from finops.utils.base_scraper import BaseScraper
 
 
 class Ticker(BaseScraper):
     def __init__(self, ticker_index, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.ticker_index = ticker_index
 
     def _preprocess_shareholder_data(self, parsed_response, date):
-        preprocessed_response = parsed_response.get("shareShareholder", [])
-        if not preprocessed_response:
-            return None
+        preprocessed_response = parsed_response["shareShareholder"]
+        if len(preprocessed_response) == 0:
+            return pd.DataFrame(columns=SHAREHOLDER_DATA_COLUMNS)
 
         preprocessed_response = (
             pd.DataFrame(preprocessed_response)
             .rename(columns=SHAREHOLDER_FIELD_MAP)
             .assign(ticker_index=self.ticker_index)
             .assign(req_date=date)
             .drop(["change", "change_amount"], axis=1)
@@ -48,14 +49,15 @@
         )
         return ticker_price_history
 
     def get_traded_dates(self):
         price_history = self.get_price_history()
         return price_history.date.tolist()
 
+    @catch
     def get_shareholder_data_one_day(self, date):
         url = SHAREHOLDER_URL.format(
             ticker_index=self.ticker_index, date=date.strftime("%Y%m%d")
         )
         response = self._download(url, user_agent=USER_AGENT)
         parsed_response = self._parse_json_response(response)
         return self._preprocess_shareholder_data(parsed_response, date)
```

### Comparing `finops-0.1.0/finops/utils/base_downloader.py` & `finops-0.1.1/finops/utils/base_downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.0/finops/utils/base_scraper.py` & `finops-0.1.1/finops/utils/base_scraper.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.0/finops.egg-info/PKG-INFO` & `finops-0.1.1/finops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops
-Version: 0.1.0
+Version: 0.1.1
 Summary: Financial tools for the rest of us.
 Home-page: https://github.com/nixuri/FinOps
 Author: Alireza Nilgaran
 Author-email: alireza.nilgaran@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `finops-0.1.0/finops.egg-info/SOURCES.txt` & `finops-0.1.1/finops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finops-0.1.0/setup.py` & `finops-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='finops',
-    version='0.1.0',
+    version='0.1.1',
     description='Financial tools for the rest of us.',
     author='Alireza Nilgaran',
     author_email='alireza.nilgaran@gmail.com',
     url='https://github.com/nixuri/FinOps',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `finops-0.1.0/tests/test_tehran_stock_exchange.py` & `finops-0.1.1/tests/test_tehran_stock_exchange.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.0/tests/test_ticker.py` & `finops-0.1.1/tests/test_ticker.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,8 @@
         )
         self.assertIsInstance(result, pd.DataFrame)
         pd.testing.assert_frame_equal(result, expected_result)
 
     def test_get_traded_dates(self):
         traded_dates = self.ticker.get_traded_dates()
         self.assertIsInstance(traded_dates, list)
-        self.assertTrue(all(isinstance(date, datetime) for date in traded_dates))
+        self.assertTrue(all(isinstance(date, datetime) for date in traded_dates))
```

### Comparing `finops-0.1.0/tests/test_utils/test_base_downloader.py` & `finops-0.1.1/tests/test_utils/test_base_downloader.py`

 * *Files identical despite different names*

### Comparing `finops-0.1.0/tests/test_utils/test_base_scraper.py` & `finops-0.1.1/tests/test_utils/test_base_scraper.py`

 * *Files identical despite different names*

