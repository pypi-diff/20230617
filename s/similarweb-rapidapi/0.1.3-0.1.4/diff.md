# Comparing `tmp/similarweb_rapidapi-0.1.3.tar.gz` & `tmp/similarweb_rapidapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarweb_rapidapi-0.1.3.tar", last modified: Wed Jun  7 13:57:51 2023, max compression
+gzip compressed data, was "similarweb_rapidapi-0.1.4.tar", last modified: Sat Jun 17 09:46:22 2023, max compression
```

## Comparing `similarweb_rapidapi-0.1.3.tar` & `similarweb_rapidapi-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 13:57:51.503379 similarweb_rapidapi-0.1.3/
--rw-rw-rw-   0        0        0     2005 2023-06-07 13:57:51.503379 similarweb_rapidapi-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1670 2023-06-07 13:28:15.000000 similarweb_rapidapi-0.1.3/README.md
--rw-rw-rw-   0        0        0       86 2023-06-07 13:57:51.506381 similarweb_rapidapi-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      579 2023-06-07 13:26:38.000000 similarweb_rapidapi-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 13:57:51.455380 similarweb_rapidapi-0.1.3/similarweb_rapidapi/
--rw-rw-rw-   0        0        0       35 2023-05-24 11:11:54.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/__init__.py
--rw-rw-rw-   0        0        0     7814 2023-06-07 13:55:22.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/api.py
--rw-rw-rw-   0        0        0      149 2023-05-25 19:47:56.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/logger_mock.py
-drwxrwxrwx   0        0        0        0 2023-06-07 13:57:51.502380 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/
--rw-rw-rw-   0        0        0        8 2023-05-24 11:46:32.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/__init__.py
--rw-rw-rw-   0        0        0     3305 2023-06-07 13:48:59.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/additional_domain_data.py
--rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/base.py
--rw-rw-rw-   0        0        0     1440 2023-05-24 20:09:52.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/basic_domain_data.py
--rw-rw-rw-   0        0        0      216 2023-05-25 18:31:28.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/cancel_task.py
--rw-rw-rw-   0        0        0      283 2023-05-24 18:52:53.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/complete_data_task.py
--rw-rw-rw-   0        0        0      530 2023-05-24 20:09:30.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/my_tasks.py
--rw-rw-rw-   0        0        0     7562 2023-05-25 19:07:43.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/task.py
--rw-rw-rw-   0        0        0      307 2023-05-24 20:04:34.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/task_status.py
-drwxrwxrwx   0        0        0        0 2023-06-07 13:57:51.484380 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/
--rw-rw-rw-   0        0        0     2005 2023-06-07 13:57:51.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      727 2023-06-07 13:57:51.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 13:57:51.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 14:10:40.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-06-07 13:57:51.000000 similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 09:46:22.255035 similarweb_rapidapi-0.1.4/
+-rw-rw-rw-   0        0        0     2268 2023-06-17 09:46:22.255035 similarweb_rapidapi-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1670 2023-06-07 13:28:15.000000 similarweb_rapidapi-0.1.4/README.md
+-rw-rw-rw-   0        0        0      394 2023-06-17 09:46:22.257039 similarweb_rapidapi-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      579 2023-06-17 09:46:18.000000 similarweb_rapidapi-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:46:22.220032 similarweb_rapidapi-0.1.4/similarweb_rapidapi/
+-rw-rw-rw-   0        0        0       35 2023-05-24 11:11:54.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/__init__.py
+-rw-rw-rw-   0        0        0     7814 2023-06-07 13:55:22.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/api.py
+-rw-rw-rw-   0        0        0      149 2023-05-25 19:47:56.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/logger_mock.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:46:22.254042 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/
+-rw-rw-rw-   0        0        0        8 2023-05-24 11:46:32.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/__init__.py
+-rw-rw-rw-   0        0        0     3305 2023-06-07 13:48:59.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/additional_domain_data.py
+-rw-rw-rw-   0        0        0      110 2023-05-24 11:23:07.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/base.py
+-rw-rw-rw-   0        0        0     1440 2023-05-24 20:09:52.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/basic_domain_data.py
+-rw-rw-rw-   0        0        0      216 2023-05-25 18:31:28.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/cancel_task.py
+-rw-rw-rw-   0        0        0      283 2023-05-24 18:52:53.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/complete_data_task.py
+-rw-rw-rw-   0        0        0      530 2023-05-24 20:09:30.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/my_tasks.py
+-rw-rw-rw-   0        0        0     7562 2023-05-25 19:07:43.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/task.py
+-rw-rw-rw-   0        0        0      307 2023-05-24 20:04:34.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/task_status.py
+drwxrwxrwx   0        0        0        0 2023-06-17 09:46:22.238041 similarweb_rapidapi-0.1.4/similarweb_rapidapi.egg-info/
+-rw-rw-rw-   0        0        0     2268 2023-06-17 09:46:22.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-06-17 09:46:22.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 09:46:22.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-17 09:46:00.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       20 2023-06-17 09:46:22.000000 similarweb_rapidapi-0.1.4/similarweb_rapidapi.egg-info/top_level.txt
```

### Comparing `similarweb_rapidapi-0.1.3/PKG-INFO` & `similarweb_rapidapi-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: similarweb_rapidapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: SimilarWeb API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/similarweb-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
+Project-URL: Documentation, https://rapidapi.com/letsscrape/api/similarweb-working-api
+Project-URL: Bug Reports, https://github.com/letsscrape/python_similarweb_rapidapi/issues
+Project-URL: Source Code, https://github.com/letsscrape/python_similarweb_rapidapi
 Keywords: rapidapi,similarweb,similarweb api,scraping,parsing,scraper
 Description-Content-Type: text/markdown
 
 # SimilarWeb API on RapidAPI
 
 ## Available on [PyPi](https://pypi.org/project/similarweb_rapidapi/)
 ## Read more on [main project page](https://letsscrape.com/scrapers/similarweb-api/)
```

### Comparing `similarweb_rapidapi-0.1.3/README.md` & `similarweb_rapidapi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.3/setup.py` & `similarweb_rapidapi-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='similarweb_rapidapi',
-    version='0.1.3',
+    version='0.1.4',
     description='SimilarWeb API on RapidAPI',
     packages=['similarweb_rapidapi', 'similarweb_rapidapi.schemas'],
     author_email='hello@letsscrape.com',
     zip_safe=False,
     author='LetsScrape',
     keywords=['rapidapi', 'similarweb', 'similarweb api', 'scraping', 'parsing', 'scraper'],
     classifiers=[],
```

### Comparing `similarweb_rapidapi-0.1.3/similarweb_rapidapi/api.py` & `similarweb_rapidapi-0.1.4/similarweb_rapidapi/api.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/additional_domain_data.py` & `similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/additional_domain_data.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/basic_domain_data.py` & `similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/basic_domain_data.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/my_tasks.py` & `similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/my_tasks.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.3/similarweb_rapidapi/schemas/task.py` & `similarweb_rapidapi-0.1.4/similarweb_rapidapi/schemas/task.py`

 * *Files identical despite different names*

### Comparing `similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/PKG-INFO` & `similarweb_rapidapi-0.1.4/similarweb_rapidapi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: similarweb-rapidapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: SimilarWeb API on RapidAPI
 Home-page: https://letsscrape.com/scrapers/similarweb-api/
 Author: LetsScrape
 Author-email: hello@letsscrape.com
+Project-URL: Documentation, https://rapidapi.com/letsscrape/api/similarweb-working-api
+Project-URL: Bug Reports, https://github.com/letsscrape/python_similarweb_rapidapi/issues
+Project-URL: Source Code, https://github.com/letsscrape/python_similarweb_rapidapi
 Keywords: rapidapi,similarweb,similarweb api,scraping,parsing,scraper
 Description-Content-Type: text/markdown
 
 # SimilarWeb API on RapidAPI
 
 ## Available on [PyPi](https://pypi.org/project/similarweb_rapidapi/)
 ## Read more on [main project page](https://letsscrape.com/scrapers/similarweb-api/)
```

### Comparing `similarweb_rapidapi-0.1.3/similarweb_rapidapi.egg-info/SOURCES.txt` & `similarweb_rapidapi-0.1.4/similarweb_rapidapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

