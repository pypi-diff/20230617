# Comparing `tmp/nft_market-1.8.tar.gz` & `tmp/nft_market-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nft_market-1.8.tar", last modified: Thu Apr 28 01:01:26 2022, max compression
+gzip compressed data, was "nft_market-1.9.tar", last modified: Fri Apr 29 01:40:53 2022, max compression
```

## Comparing `nft_market-1.8.tar` & `nft_market-1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ukaznil    (501) staff       (20)        0 2022-04-28 01:01:26.170862 nft_market-1.8/
--rw-r--r--   0 ukaznil    (501) staff       (20)     1072 2022-04-08 02:40:29.000000 nft_market-1.8/LICENSE
--rw-r--r--   0 ukaznil    (501) staff       (20)     6529 2022-04-28 01:01:26.170681 nft_market-1.8/PKG-INFO
--rw-r--r--   0 ukaznil    (501) staff       (20)     6002 2022-04-28 01:00:56.000000 nft_market-1.8/README.md
-drwxr-xr-x   0 ukaznil    (501) staff       (20)        0 2022-04-28 01:01:26.156613 nft_market-1.8/nft_market/
--rw-r--r--   0 ukaznil    (501) staff       (20)      100 2022-04-09 23:28:42.000000 nft_market-1.8/nft_market/__init__.py
--rw-r--r--   0 ukaznil    (501) staff       (20)      396 2022-04-28 01:00:56.000000 nft_market-1.8/nft_market/market.py
--rw-r--r--   0 ukaznil    (501) staff       (20)     4173 2022-04-28 01:00:56.000000 nft_market-1.8/nft_market/nftinfo.py
--rw-r--r--   0 ukaznil    (501) staff       (20)    22872 2022-04-28 01:00:56.000000 nft_market-1.8/nft_market/retriever.py
-drwxr-xr-x   0 ukaznil    (501) staff       (20)        0 2022-04-28 01:01:26.170356 nft_market-1.8/nft_market.egg-info/
--rw-r--r--   0 ukaznil    (501) staff       (20)     6529 2022-04-28 01:01:25.000000 nft_market-1.8/nft_market.egg-info/PKG-INFO
--rw-r--r--   0 ukaznil    (501) staff       (20)      285 2022-04-28 01:01:25.000000 nft_market-1.8/nft_market.egg-info/SOURCES.txt
--rw-r--r--   0 ukaznil    (501) staff       (20)        1 2022-04-28 01:01:25.000000 nft_market-1.8/nft_market.egg-info/dependency_links.txt
--rw-r--r--   0 ukaznil    (501) staff       (20)       27 2022-04-28 01:01:25.000000 nft_market-1.8/nft_market.egg-info/requires.txt
--rw-r--r--   0 ukaznil    (501) staff       (20)       11 2022-04-28 01:01:25.000000 nft_market-1.8/nft_market.egg-info/top_level.txt
--rw-r--r--   0 ukaznil    (501) staff       (20)       38 2022-04-28 01:01:26.170918 nft_market-1.8/setup.cfg
--rw-r--r--   0 ukaznil    (501) staff       (20)      845 2022-04-28 01:00:56.000000 nft_market-1.8/setup.py
+drwxr-xr-x   0 ukaznil    (501) staff       (20)        0 2022-04-29 01:40:53.599743 nft_market-1.9/
+-rw-r--r--   0 ukaznil    (501) staff       (20)     1072 2022-04-08 02:40:29.000000 nft_market-1.9/LICENSE
+-rw-r--r--   0 ukaznil    (501) staff       (20)     6529 2022-04-29 01:40:53.599538 nft_market-1.9/PKG-INFO
+-rw-r--r--   0 ukaznil    (501) staff       (20)     6002 2022-04-28 01:00:56.000000 nft_market-1.9/README.md
+drwxr-xr-x   0 ukaznil    (501) staff       (20)        0 2022-04-29 01:40:53.574993 nft_market-1.9/nft_market/
+-rw-r--r--   0 ukaznil    (501) staff       (20)      100 2022-04-09 23:28:42.000000 nft_market-1.9/nft_market/__init__.py
+-rw-r--r--   0 ukaznil    (501) staff       (20)      396 2022-04-28 01:00:56.000000 nft_market-1.9/nft_market/market.py
+-rw-r--r--   0 ukaznil    (501) staff       (20)     4173 2022-04-28 01:00:56.000000 nft_market-1.9/nft_market/nftinfo.py
+-rw-r--r--   0 ukaznil    (501) staff       (20)    22876 2022-04-29 01:40:35.000000 nft_market-1.9/nft_market/retriever.py
+drwxr-xr-x   0 ukaznil    (501) staff       (20)        0 2022-04-29 01:40:53.599214 nft_market-1.9/nft_market.egg-info/
+-rw-r--r--   0 ukaznil    (501) staff       (20)     6529 2022-04-29 01:40:53.000000 nft_market-1.9/nft_market.egg-info/PKG-INFO
+-rw-r--r--   0 ukaznil    (501) staff       (20)      285 2022-04-29 01:40:53.000000 nft_market-1.9/nft_market.egg-info/SOURCES.txt
+-rw-r--r--   0 ukaznil    (501) staff       (20)        1 2022-04-29 01:40:53.000000 nft_market-1.9/nft_market.egg-info/dependency_links.txt
+-rw-r--r--   0 ukaznil    (501) staff       (20)       27 2022-04-29 01:40:53.000000 nft_market-1.9/nft_market.egg-info/requires.txt
+-rw-r--r--   0 ukaznil    (501) staff       (20)       11 2022-04-29 01:40:53.000000 nft_market-1.9/nft_market.egg-info/top_level.txt
+-rw-r--r--   0 ukaznil    (501) staff       (20)       38 2022-04-29 01:40:53.599801 nft_market-1.9/setup.cfg
+-rw-r--r--   0 ukaznil    (501) staff       (20)      845 2022-04-29 01:40:35.000000 nft_market-1.9/setup.py
```

### Comparing `nft_market-1.8/LICENSE` & `nft_market-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nft_market-1.8/PKG-INFO` & `nft_market-1.9/nft_market.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nft_market
-Version: 1.8
+Name: nft-market
+Version: 1.9
 Summary: NFT market is in your hands.
 Home-page: https://github.com/ukaznil/nft-market
 Author: ukaznil
 Author-email: ukaznil@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ukaznil/nft-market/issues
 Platform: UNKNOWN
```

### Comparing `nft_market-1.8/README.md` & `nft_market-1.9/README.md`

 * *Files identical despite different names*

### Comparing `nft_market-1.8/nft_market/nftinfo.py` & `nft_market-1.9/nft_market/nftinfo.py`

 * *Files identical despite different names*

### Comparing `nft_market-1.8/nft_market/retriever.py` & `nft_market-1.9/nft_market/retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,19 +314,19 @@
 
         nft = None
         try:
             with _WebFetcher(url, **self.option) as driver:
                 error = None
 
                 nft = NFTInfoBuilder(driver, id) \
-                    .name('//*[@id="app"]/div/div[2]/div[2]/div[1]/div/div[1]/div/div[1]/div[1]/div') \
-                    .num_listing('//*[@id="app"]/div/div[2]/div[2]/div[1]/div/div[2]/div/div[1]/div[3]/div[1]/div[2]/div[1]',
+                    .name('//*[@id="app"]/div/div[3]/div[2]/div[1]/div/div[1]/div/div[1]/div[1]/div') \
+                    .num_listing('//*[@id="app"]/div/div[3]/div[2]/div[1]/div/div[2]/div/div[1]/div[3]/div[1]/div[2]/div[1]',
                                  lambda s: s.replace('results', '')) \
-                    .floor('//*[@id="app"]/div/div[2]/div[2]/div[1]/div/div[1]/div/div[1]/div[2]/span[3]/span[2]') \
-                    .volume('//*[@id="app"]/div/div[2]/div[2]/div[1]/div/div[1]/div/div[1]/div[2]/span[1]/span[2]') \
+                    .floor('//*[@id="app"]/div/div[3]/div[2]/div[1]/div/div[1]/div/div[1]/div[2]/span[3]/span[2]') \
+                    .volume('//*[@id="app"]/div/div[3]/div[2]/div[1]/div/div[1]/div/div[1]/div[2]/span[1]/span[2]') \
                     .build()
             # endwith
         except Exception as e:
             error = e
         # endtry
 
         return nft, error
@@ -334,24 +334,24 @@
 
     def _retrieve_looksrare(self, id: str) -> Tuple[NFTInfo, Exception]:
         url = f'https://looksrare.org/collections/{id}'
 
         nft = None
         try:
             with _WebFetcher(url, **self.option) as driver:
-                for c_name, c_listing in itertools.product([4, 5], [6, 7]):
+                for c_name, c_other in itertools.product([4, 5], [6, 7]):
                     error = None
 
                     try:
                         nft = NFTInfoBuilder(driver, id) \
-                            .name(f'//*[@id="__next"]/div[2]/div/div/div[1]/div[2]/div[2]/div[2]/div[{c_name}]/div/div[2]/div[1]/h1') \
-                            .num_listing(f'//*[@id="__next"]/div[2]/div/div/div[1]/div[2]/div[2]/div[2]/div[{c_listing}]/div/div/div/div[3]/div[2]') \
-                            .num_owners(f'//*[@id="__next"]/div[2]/div/div/div[1]/div[2]/div[2]/div[2]/div[{c_listing}]/div/div/div/div[4]/div[2]') \
-                            .floor(f'//*[@id="__next"]/div[2]/div/div/div[1]/div[2]/div[2]/div[2]/div[{c_listing}]/div/div/div/div[1]/div[2]/div[1]') \
-                            .volume(f'//*[@id="__next"]/div[2]/div/div/div[1]/div[2]/div[2]/div[2]/div[{c_listing}]/div/div/div/div[2]/div[2]/div') \
+                            .name(f'//*[@id="__next"]/div[2]/div/div/div/div[1]/div[2]/div[2]/div[2]/div[{c_name}]/div/div[2]/div[1]/h1') \
+                            .num_listing(f'//*[@id="__next"]/div[2]/div/div/div/div[1]/div[2]/div[2]/div[2]/div[{c_other}]/div/div/div/div[3]/div[2]') \
+                            .num_owners(f'//*[@id="__next"]/div[2]/div/div/div/div[1]/div[2]/div[2]/div[2]/div[{c_other}]/div/div/div/div[4]/div[2]') \
+                            .floor(f'//*[@id="__next"]/div[2]/div/div/div/div[3]/div[2]/div[2]/div[2]/div[1]/div[1]/a/div[1]/div[3]/div[1]/div') \
+                            .volume(f'//*[@id="__next"]/div[2]/div/div/div/div[1]/div[2]/div[2]/div[2]/div[{c_other}]/div/div/div/div[2]/div[2]/div ') \
                             .build()
                         break
                     except NoSuchElementException as e:
                         error = e
                         continue
                     # endtry
                 # endfor
@@ -471,16 +471,16 @@
                 error = None
 
                 nft = NFTInfoBuilder(driver, id) \
                     .name('//*[@id="root"]/section/section/main/div/div[2]/div[1]/div[1]') \
                     .num_supply('//*[@id="root"]/section/section/main/div/div[2]/div[1]/div[3]/div[5]/div/div/div/div[1]') \
                     .num_listing('//*[@id="root"]/section/section/main/div/div[2]/div[1]/div[3]/div[1]/div/div/div/div[1]') \
                     .num_owners('//*[@id="root"]/section/section/main/div/div[2]/div[1]/div[3]/div[2]/div/div/div/div[1]') \
-                    .floor('//*[@id="root"]/section/section/main/div/div[2]/div[1]/div[3]/div[4]/div/div/div/div[1]/div/div') \
-                    .volume('//*[@id="root"]/section/section/main/div/div[2]/div[1]/div[3]/div[3]/div/div/div/div[1]/div/div') \
+                    .floor('//*[@id="root"]/section/section/main/div/div[2]/div[1]/div[3]/div[3]/div/div/div/div[1]/div/div') \
+                    .volume('//*[@id="root"]/section/section/main/div/div[2]/div[1]/div[3]/div[4]/div/div/div/div[1]/div/div') \
                     .build()
             # endwith
         except Exception as e:
             error = e
         # endtry
 
         return nft, error
```

### Comparing `nft_market-1.8/nft_market.egg-info/PKG-INFO` & `nft_market-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nft-market
-Version: 1.8
+Name: nft_market
+Version: 1.9
 Summary: NFT market is in your hands.
 Home-page: https://github.com/ukaznil/nft-market
 Author: ukaznil
 Author-email: ukaznil@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ukaznil/nft-market/issues
 Platform: UNKNOWN
```

### Comparing `nft_market-1.8/setup.py` & `nft_market-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nft_market",
-    version="1.8",
+    version="1.9",
     author="ukaznil",
     author_email="ukaznil@gmail.com",
     description="NFT market is in your hands.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ukaznil/nft-market",
     project_urls={
```

