# Comparing `tmp/trulia_rapidapi-0.1.0.tar.gz` & `tmp/trulia_rapidapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trulia_rapidapi-0.1.0.tar", last modified: Wed Jun 14 20:09:06 2023, max compression
+gzip compressed data, was "trulia_rapidapi-0.1.1.tar", last modified: Sat Jun 17 09:38:53 2023, max compression
```

## Comparing `trulia_rapidapi-0.1.0.tar` & `trulia_rapidapi-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 20:09:06.722861 trulia_rapidapi-0.1.0/
--rw-rw-rw-   0        0        0     1588 2023-06-14 20:09:06.723863 trulia_rapidapi-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1232 2023-06-14 20:04:25.000000 trulia_rapidapi-0.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-06-14 20:09:06.725869 trulia_rapidapi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-06-14 20:03:14.000000 trulia_rapidapi-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:09:06.699868 trulia_rapidapi-0.1.0/trulia_rapidapi/
-drwxrwxrwx   0        0        0        0 2023-06-14 20:09:06.714863 trulia_rapidapi-0.1.0/trulia_rapidapi/src/
--rw-rw-rw-   0        0        0     6456 2023-06-14 19:52:46.000000 trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_api.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:09:06.721864 trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_models/
--rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_models/base.py
--rw-rw-rw-   0        0        0     3175 2023-06-14 19:13:10.000000 trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_models/enums.py
--rw-rw-rw-   0        0        0     1497 2023-06-14 18:52:49.000000 trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_models/listing_model.py
--rw-rw-rw-   0        0        0      539 2023-06-14 19:49:05.000000 trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_models/search_token_model.py
--rw-rw-rw-   0        0        0     1808 2023-06-14 19:58:12.000000 trulia_rapidapi-0.1.0/trulia_rapidapi/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:09:06.713862 trulia_rapidapi-0.1.0/trulia_rapidapi.egg-info/
--rw-rw-rw-   0        0        0     1588 2023-06-14 20:09:06.000000 trulia_rapidapi-0.1.0/trulia_rapidapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-06-14 20:09:06.000000 trulia_rapidapi-0.1.0/trulia_rapidapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 20:09:06.000000 trulia_rapidapi-0.1.0/trulia_rapidapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-14 20:08:36.000000 trulia_rapidapi-0.1.0/trulia_rapidapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-06-14 20:09:06.000000 trulia_rapidapi-0.1.0/trulia_rapidapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.923941 trulia_rapidapi-0.1.1/
+-rw-rw-rw-   0        0        0     1848 2023-06-17 09:38:53.923941 trulia_rapidapi-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1232 2023-06-14 20:14:23.000000 trulia_rapidapi-0.1.1/README.md
+-rw-rw-rw-   0        0        0      399 2023-06-17 09:38:53.925942 trulia_rapidapi-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      625 2023-06-17 09:36:05.000000 trulia_rapidapi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.902941 trulia_rapidapi-0.1.1/trulia_rapidapi/
+drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.918940 trulia_rapidapi-0.1.1/trulia_rapidapi/src/
+-rw-rw-rw-   0        0        0     6458 2023-06-17 08:53:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_api.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.922941 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/
+-rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/base.py
+-rw-rw-rw-   0        0        0     3175 2023-06-14 19:13:10.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/enums.py
+-rw-rw-rw-   0        0        0     1497 2023-06-14 18:52:49.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/listing_model.py
+-rw-rw-rw-   0        0        0      539 2023-06-14 19:49:05.000000 trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/search_token_model.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:38:53.917944 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/
+-rw-rw-rw-   0        0        0     1848 2023-06-17 09:38:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2023-06-17 09:38:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 09:38:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-14 20:08:36.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-06-17 09:38:53.000000 trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/top_level.txt
```

### Comparing `trulia_rapidapi-0.1.0/PKG-INFO` & `trulia_rapidapi-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: trulia_rapidapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Trulia Real Estate API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/trulia-real-estate-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
+Project-URL: Documentation, https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper/
+Project-URL: Bug Reports, https://github.com/letsscrape/python_trulia_rapidapi/issues
+Project-URL: Source Code, https://github.com/letsscrape/python_trulia_rapidapi
 Keywords: trulia,real estate api,trulia real estate,trulia api,parsing,scraper
 Description-Content-Type: text/markdown
 
-# trulia API on RapidAPI
+# Trulia API on RapidAPI
 
 ## Available on [PyPi](https://pypi.org/project/trulia_rapidapi/)
 ## Read more on [main project page](https://letsscrape.com/scrapers/trulia-real-estate-api/)
 ## See on [RapidAPI](https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper)
 
 ## Install
 ### using pip
```

### Comparing `trulia_rapidapi-0.1.0/README.md` & `trulia_rapidapi-0.1.1/README.md`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,8 @@
-# trulia API on RapidAPI
+# Trulia API on RapidAPI
 
 ## Available on [PyPi](https://pypi.org/project/trulia_rapidapi/)
 ## Read more on [main project page](https://letsscrape.com/scrapers/trulia-real-estate-api/)
 ## See on [RapidAPI](https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper)
 
 ## Install
 ### using pip
```

### Comparing `trulia_rapidapi-0.1.0/setup.py` & `trulia_rapidapi-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='trulia_rapidapi',
-    version='0.1.0',
+    version='0.1.1',
     description='Trulia Real Estate API on RapidAPI',
     packages=['trulia_rapidapi', 'trulia_rapidapi.src', 'trulia_rapidapi.src.trulia_models'],
     author_email='hello@letsscrape.com',
     zip_safe=False,
     author='LetsScrape',
     keywords=['trulia', 'real estate api', 'trulia real estate', 'trulia api', 'parsing', 'scraper'],
     classifiers=[],
```

### Comparing `trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_api.py` & `trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
         Parameters:
         page (int): The page number you want to work with. If you want the first page, pass in 1.
         """
         token = await self.get_search_token(search_type, place)
 
         if len(token.data.places) == 0:
-            return ListingModel(data=[], status=200, description="No places have been found!")
+            return ListingModel(data=None, status=200, description="No places have been found!")
 
         return await self.search_by_token(search_type, token.data.places[0].search_token, page, sort, beds, min_price, max_price,
             house_type, for_sale_by_agent, for_sale_by_owner, new_construction)
 
     async def search_by_token(self, search_type:TruliaSearchType, token: str, page: int, 
         sort: TruliaSort=None, beds: TruliaBeds=None,
         min_price: TruliaPriceRange=None, max_price: TruliaPriceRange=None,
```

### Comparing `trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_models/enums.py` & `trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/enums.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_models/listing_model.py` & `trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/listing_model.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.0/trulia_rapidapi/src/trulia_models/search_token_model.py` & `trulia_rapidapi-0.1.1/trulia_rapidapi/src/trulia_models/search_token_model.py`

 * *Files identical despite different names*

### Comparing `trulia_rapidapi-0.1.0/trulia_rapidapi.egg-info/PKG-INFO` & `trulia_rapidapi-0.1.1/trulia_rapidapi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: trulia-rapidapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Trulia Real Estate API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/trulia-real-estate-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
+Project-URL: Documentation, https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper/
+Project-URL: Bug Reports, https://github.com/letsscrape/python_trulia_rapidapi/issues
+Project-URL: Source Code, https://github.com/letsscrape/python_trulia_rapidapi
 Keywords: trulia,real estate api,trulia real estate,trulia api,parsing,scraper
 Description-Content-Type: text/markdown
 
-# trulia API on RapidAPI
+# Trulia API on RapidAPI
 
 ## Available on [PyPi](https://pypi.org/project/trulia_rapidapi/)
 ## Read more on [main project page](https://letsscrape.com/scrapers/trulia-real-estate-api/)
 ## See on [RapidAPI](https://rapidapi.com/letsscrape/api/trulia-real-estate-scraper)
 
 ## Install
 ### using pip
```

