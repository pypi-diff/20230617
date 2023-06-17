# Comparing `tmp/facebook_page_scraper-5.0.1.tar.gz` & `tmp/facebook_page_scraper-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_page_scraper-5.0.1.tar", last modified: Sat Jun 17 12:07:47 2023, max compression
+gzip compressed data, was "facebook_page_scraper-5.0.2.tar", last modified: Sat Jun 17 13:11:44 2023, max compression
```

## Comparing `facebook_page_scraper-5.0.1.tar` & `facebook_page_scraper-5.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 12:07:47.191515 facebook_page_scraper-5.0.1/
--rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-5.0.1/LICENSE
--rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-5.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    12291 2023-06-17 12:07:47.191515 facebook_page_scraper-5.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    10970 2023-06-17 12:06:17.000000 facebook_page_scraper-5.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 12:07:47.156507 facebook_page_scraper-5.0.1/facebook_page_scraper/
--rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/driver_initialization.py
--rw-rw-rw-   0        0        0     7853 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/driver_utilities.py
--rw-rw-rw-   0        0        0    17022 2023-02-19 06:31:55.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/element_finder.py
--rw-rw-rw-   0        0        0    15742 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/scraper.py
--rw-rw-rw-   0        0        0     5248 2022-10-05 09:29:57.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/scraping_utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-17 12:07:47.189514 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/
--rw-rw-rw-   0        0        0    12291 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 12:07:47.192515 facebook_page_scraper-5.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1726 2023-06-17 12:06:44.000000 facebook_page_scraper-5.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:11:44.440028 facebook_page_scraper-5.0.2/
+-rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-5.0.2/LICENSE
+-rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-5.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    12291 2023-06-17 13:11:44.439028 facebook_page_scraper-5.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10970 2023-06-17 13:08:13.000000 facebook_page_scraper-5.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 13:11:44.393438 facebook_page_scraper-5.0.2/facebook_page_scraper/
+-rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-5.0.2/facebook_page_scraper/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.2/facebook_page_scraper/driver_initialization.py
+-rw-rw-rw-   0        0        0     7853 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.2/facebook_page_scraper/driver_utilities.py
+-rw-rw-rw-   0        0        0    17022 2023-02-19 06:31:55.000000 facebook_page_scraper-5.0.2/facebook_page_scraper/element_finder.py
+-rw-rw-rw-   0        0        0    15740 2023-06-17 13:04:36.000000 facebook_page_scraper-5.0.2/facebook_page_scraper/scraper.py
+-rw-rw-rw-   0        0        0     5412 2023-06-17 13:04:26.000000 facebook_page_scraper-5.0.2/facebook_page_scraper/scraping_utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:11:44.437029 facebook_page_scraper-5.0.2/facebook_page_scraper.egg-info/
+-rw-rw-rw-   0        0        0    12291 2023-06-17 13:11:44.000000 facebook_page_scraper-5.0.2/facebook_page_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-06-17 13:11:44.000000 facebook_page_scraper-5.0.2/facebook_page_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 13:11:44.000000 facebook_page_scraper-5.0.2/facebook_page_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-17 13:11:44.000000 facebook_page_scraper-5.0.2/facebook_page_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-17 13:11:44.000000 facebook_page_scraper-5.0.2/facebook_page_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 13:11:44.440028 facebook_page_scraper-5.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1726 2023-06-17 13:07:55.000000 facebook_page_scraper-5.0.2/setup.py
```

### Comparing `facebook_page_scraper-5.0.1/LICENSE` & `facebook_page_scraper-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.1/PKG-INFO` & `facebook_page_scraper-5.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_page_scraper
-Version: 5.0.1
+Version: 5.0.2
 Summary: Python package to scrap facebook's pages front end with no limitations
 Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium facebook facebook-pages
 Classifier: Development Status :: 4 - Beta
@@ -27,15 +27,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1> Facebook Page Scraper </h1>
 
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https://github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity)
-[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 
 <p> No need of API key, No limitation on number of requests. Import the library and <b> Just Do It !<b> </p>
 
 <!--TABLE of contents-->
 <h2> Table of Contents </h2>
 <details open="open">
   <summary>Table of Contents</summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.1 Summary:
+Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.2 Summary:
 Python package to scrap facebook's pages front end with no limitations Home-
 page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** Facebook Page Scraper ******
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https:/
 /github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity) [!
 [PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://
 opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/
-python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
+python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 No need of API key, No limitation on number of requests. Import the library and
 Just Do It !
 ***** Table of Contents *****
  Table of Contents
    1. Getting_Started
           o Prerequisites
           o Installation
```

### Comparing `facebook_page_scraper-5.0.1/README.md` & `facebook_page_scraper-5.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1> Facebook Page Scraper </h1>
 
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https://github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity)
-[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 
 <p> No need of API key, No limitation on number of requests. Import the library and <b> Just Do It !<b> </p>
 
 <!--TABLE of contents-->
 <h2> Table of Contents </h2>
 <details open="open">
   <summary>Table of Contents</summary>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 ****** Facebook Page Scraper ******
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https:/
 /github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity) [!
 [PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://
 opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/
-python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
+python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 No need of API key, No limitation on number of requests. Import the library and
 Just Do It !
 ***** Table of Contents *****
  Table of Contents
    1. Getting_Started
           o Prerequisites
           o Installation
```

### Comparing `facebook_page_scraper-5.0.1/facebook_page_scraper/driver_initialization.py` & `facebook_page_scraper-5.0.2/facebook_page_scraper/driver_initialization.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.1/facebook_page_scraper/driver_utilities.py` & `facebook_page_scraper-5.0.2/facebook_page_scraper/driver_utilities.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.1/facebook_page_scraper/element_finder.py` & `facebook_page_scraper-5.0.2/facebook_page_scraper/element_finder.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.1/facebook_page_scraper/scraper.py` & `facebook_page_scraper-5.0.2/facebook_page_scraper/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,14 @@
                     l, "Sad")
                 # if Angry aria-label is in the list, than extract it and extract numbers from that text
                 angry = Scraping_utilities._Scraping_utilities__find_reaction_by_text(
                     l, "Angry")
                 # if Haha aria-label is in the list, than extract it and extract numbers from that text
                 haha = Scraping_utilities._Scraping_utilities__find_reaction_by_text(
                     l, "Haha")
-
                 # converting all reactions to numbers
                 # e,g reactions may contain counts like "5k","5m", so converting them to actual number
                 likes = Scraping_utilities._Scraping_utilities__value_to_float(
                     likes)
                 loves = Scraping_utilities._Scraping_utilities__value_to_float(
                     loves)
                 wow = Scraping_utilities._Scraping_utilities__value_to_float(
```

### Comparing `facebook_page_scraper-5.0.1/facebook_page_scraper/scraping_utilities.py` & `facebook_page_scraper-5.0.2/facebook_page_scraper/scraping_utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,17 +103,21 @@
         if 'm' in x:
             return float(x.replace('m', '')) * 1000000000
         return 0
 
     @staticmethod
     def __find_reaction_by_text(l, string):
         reaction = [substring for substring in l if string in substring]
+        if len(reaction) == 0:
+            return '0'
         reaction = re.findall(
-            "\d+", reaction[0])[0] if len(reaction) > 0 else "0"
-        return reaction
+            r"(\d+(?:\.\d+)?)([MmBbKk])?", reaction[0])
+        if len(reaction) > 0:
+            return ''.join(reaction[0]) #list of tuple, return first tuple's first result
+        return '0'
 
     @staticmethod
     def __convert_to_iso(t):
         past_date = "Failed to fetch!"
         if 'h' in t.lower() or "hr" in t.lower() or "hrs" in t.lower():
             hours_to_subract = re.sub("\D", '', t)
             # print(f"{hours_to_subract} subtracting hours\n")
```

### Comparing `facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/PKG-INFO` & `facebook_page_scraper-5.0.2/facebook_page_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-page-scraper
-Version: 5.0.1
+Version: 5.0.2
 Summary: Python package to scrap facebook's pages front end with no limitations
 Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium facebook facebook-pages
 Classifier: Development Status :: 4 - Beta
@@ -27,15 +27,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1> Facebook Page Scraper </h1>
 
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https://github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity)
-[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 
 <p> No need of API key, No limitation on number of requests. Import the library and <b> Just Do It !<b> </p>
 
 <!--TABLE of contents-->
 <h2> Table of Contents </h2>
 <details open="open">
   <summary>Table of Contents</summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: facebook-page-scraper Version: 5.0.1 Summary:
+Metadata-Version: 2.1 Name: facebook-page-scraper Version: 5.0.2 Summary:
 Python package to scrap facebook's pages front end with no limitations Home-
 page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** Facebook Page Scraper ******
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https:/
 /github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity) [!
 [PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://
 opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/
-python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
+python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-360/)
 No need of API key, No limitation on number of requests. Import the library and
 Just Do It !
 ***** Table of Contents *****
  Table of Contents
    1. Getting_Started
           o Prerequisites
           o Installation
```

### Comparing `facebook_page_scraper-5.0.1/setup.py` & `facebook_page_scraper-5.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                 'webdriver-manager==3.2.2',
                 'selenium-wire==5.1.0',
                 'python-dateutil==2.8.2']
 
 
 setuptools.setup(
     name="facebook_page_scraper",
-    version="5.0.1",
+    version="5.0.2",
     author="Sajid Shaikh",
     author_email="shaikhsajid3732@gmail.com",
     description="Python package to scrap facebook's pages front end with no limitations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/shaikhsajid1111/facebook_page_scraper",
```

