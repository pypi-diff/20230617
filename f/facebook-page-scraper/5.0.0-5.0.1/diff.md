# Comparing `tmp/facebook_page_scraper-5.0.0.tar.gz` & `tmp/facebook_page_scraper-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facebook_page_scraper-5.0.0.tar", last modified: Sun Jun  4 12:42:06 2023, max compression
+gzip compressed data, was "facebook_page_scraper-5.0.1.tar", last modified: Sat Jun 17 12:07:47 2023, max compression
```

## Comparing `facebook_page_scraper-5.0.0.tar` & `facebook_page_scraper-5.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 12:42:06.834387 facebook_page_scraper-5.0.0/
--rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-5.0.0/LICENSE
--rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-5.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    12291 2023-06-04 12:42:06.833386 facebook_page_scraper-5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    10970 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 12:42:06.808408 facebook_page_scraper-5.0.0/facebook_page_scraper/
--rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/driver_initialization.py
--rw-rw-rw-   0        0        0     7853 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/driver_utilities.py
--rw-rw-rw-   0        0        0    17022 2023-02-19 06:31:55.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/element_finder.py
--rw-rw-rw-   0        0        0    15742 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/scraper.py
--rw-rw-rw-   0        0        0     5248 2022-10-05 09:29:57.000000 facebook_page_scraper-5.0.0/facebook_page_scraper/scraping_utilities.py
-drwxrwxrwx   0        0        0        0 2023-06-04 12:42:06.832387 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/
--rw-rw-rw-   0        0        0    12291 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-04 12:42:06.000000 facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 12:42:06.834387 facebook_page_scraper-5.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1726 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 12:07:47.191515 facebook_page_scraper-5.0.1/
+-rw-rw-rw-   0        0        0     1090 2021-01-01 03:52:50.000000 facebook_page_scraper-5.0.1/LICENSE
+-rw-rw-rw-   0        0        0       17 2022-04-14 08:09:34.000000 facebook_page_scraper-5.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    12291 2023-06-17 12:07:47.191515 facebook_page_scraper-5.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10970 2023-06-17 12:06:17.000000 facebook_page_scraper-5.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 12:07:47.156507 facebook_page_scraper-5.0.1/facebook_page_scraper/
+-rw-rw-rw-   0        0        0      322 2022-08-20 06:31:28.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/driver_initialization.py
+-rw-rw-rw-   0        0        0     7853 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/driver_utilities.py
+-rw-rw-rw-   0        0        0    17022 2023-02-19 06:31:55.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/element_finder.py
+-rw-rw-rw-   0        0        0    15742 2023-06-04 12:41:04.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/scraper.py
+-rw-rw-rw-   0        0        0     5248 2022-10-05 09:29:57.000000 facebook_page_scraper-5.0.1/facebook_page_scraper/scraping_utilities.py
+drwxrwxrwx   0        0        0        0 2023-06-17 12:07:47.189514 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/
+-rw-rw-rw-   0        0        0    12291 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-17 12:07:46.000000 facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 12:07:47.192515 facebook_page_scraper-5.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1726 2023-06-17 12:06:44.000000 facebook_page_scraper-5.0.1/setup.py
```

### Comparing `facebook_page_scraper-5.0.0/LICENSE` & `facebook_page_scraper-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.0/PKG-INFO` & `facebook_page_scraper-5.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook_page_scraper
-Version: 5.0.0
+Version: 5.0.1
 Summary: Python package to scrap facebook's pages front end with no limitations
 Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium facebook facebook-pages
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1> Facebook Page Scraper </h1>
 
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https://github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
@@ -72,15 +72,15 @@
 </details>
 
 <!--TABLE of contents //-->
 
 <h2 id="Prerequisites"> Prerequisites </h2>
 
 - Internet Connection
-- Python 3.6+
+- Python 3.7+
 - Chrome or Firefox browser installed on your machine
 <br>
 
 <hr>
 <h2 id="Installation">Installation:</h2>
 
 <h3 id="sourceInstallation"> Installing from source: </h3>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.0 Summary:
+Metadata-Version: 2.1 Name: facebook_page_scraper Version: 5.0.1 Summary:
 Python package to scrap facebook's pages front end with no limitations Home-
 page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
 MacOS Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.6 Description-
+Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** Facebook Page Scraper ******
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https:/
 /github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity) [!
 [PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://
 opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/
 python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
@@ -38,15 +38,15 @@
                 # Scrape_in_CSV_format
                       # Parameters_for_scrape_to_csv()_method
                 # Keys_of_the_output_data
    3. Tech
    4. License
 
 ***** Prerequisites *****
-- Internet Connection - Python 3.6+ - Chrome or Firefox browser installed on
+- Internet Connection - Python 3.7+ - Chrome or Firefox browser installed on
 your machine
 ===============================================================================
 ***** Installation: *****
 **** Installing from source: ****
 ``` git clone https://github.com/shaikhsajid1111/facebook_page_scraper ```
 *** Inside project's directory ***
 ``` python3 setup.py install ```
```

### Comparing `facebook_page_scraper-5.0.0/README.md` & `facebook_page_scraper-5.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 </details>
 
 <!--TABLE of contents //-->
 
 <h2 id="Prerequisites"> Prerequisites </h2>
 
 - Internet Connection
-- Python 3.6+
+- Python 3.7+
 - Chrome or Firefox browser installed on your machine
 <br>
 
 <hr>
 <h2 id="Installation">Installation:</h2>
 
 <h3 id="sourceInstallation"> Installing from source: </h3>
```

#### html2text {}

```diff
@@ -21,15 +21,15 @@
                 # Scrape_in_CSV_format
                       # Parameters_for_scrape_to_csv()_method
                 # Keys_of_the_output_data
    3. Tech
    4. License
 
 ***** Prerequisites *****
-- Internet Connection - Python 3.6+ - Chrome or Firefox browser installed on
+- Internet Connection - Python 3.7+ - Chrome or Firefox browser installed on
 your machine
 ===============================================================================
 ***** Installation: *****
 **** Installing from source: ****
 ``` git clone https://github.com/shaikhsajid1111/facebook_page_scraper ```
 *** Inside project's directory ***
 ``` python3 setup.py install ```
```

### Comparing `facebook_page_scraper-5.0.0/facebook_page_scraper/driver_initialization.py` & `facebook_page_scraper-5.0.1/facebook_page_scraper/driver_initialization.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.0/facebook_page_scraper/driver_utilities.py` & `facebook_page_scraper-5.0.1/facebook_page_scraper/driver_utilities.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.0/facebook_page_scraper/element_finder.py` & `facebook_page_scraper-5.0.1/facebook_page_scraper/element_finder.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.0/facebook_page_scraper/scraper.py` & `facebook_page_scraper-5.0.1/facebook_page_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.0/facebook_page_scraper/scraping_utilities.py` & `facebook_page_scraper-5.0.1/facebook_page_scraper/scraping_utilities.py`

 * *Files identical despite different names*

### Comparing `facebook_page_scraper-5.0.0/facebook_page_scraper.egg-info/PKG-INFO` & `facebook_page_scraper-5.0.1/facebook_page_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facebook-page-scraper
-Version: 5.0.0
+Version: 5.0.1
 Summary: Python package to scrap facebook's pages front end with no limitations
 Home-page: https://github.com/shaikhsajid1111/facebook_page_scraper
 Author: Sajid Shaikh
 Author-email: shaikhsajid3732@gmail.com
 License: MIT
 Keywords: web-scraping selenium facebook facebook-pages
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Internet :: WWW/HTTP
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1> Facebook Page Scraper </h1>
 
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https://github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity)
 [![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
@@ -72,15 +72,15 @@
 </details>
 
 <!--TABLE of contents //-->
 
 <h2 id="Prerequisites"> Prerequisites </h2>
 
 - Internet Connection
-- Python 3.6+
+- Python 3.7+
 - Chrome or Firefox browser installed on your machine
 <br>
 
 <hr>
 <h2 id="Installation">Installation:</h2>
 
 <h3 id="sourceInstallation"> Installing from source: </h3>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: facebook-page-scraper Version: 5.0.0 Summary:
+Metadata-Version: 2.1 Name: facebook-page-scraper Version: 5.0.1 Summary:
 Python package to scrap facebook's pages front end with no limitations Home-
 page: https://github.com/shaikhsajid1111/facebook_page_scraper Author: Sajid
 Shaikh Author-email: shaikhsajid3732@gmail.com License: MIT Keywords: web-
 scraping selenium facebook facebook-pages Classifier: Development Status :: 4 -
 Beta Classifier: Environment :: Console Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 Natural Language :: English Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux Classifier: Operating System ::
 MacOS Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.6 Description-
+Classifier: Topic :: Internet :: WWW/HTTP Requires-Python: >=3.7 Description-
 Content-Type: text/markdown License-File: LICENSE
 ****** Facebook Page Scraper ******
 [![Maintenance](https://img.shields.io/badge/Maintained-Yes-green.svg)](https:/
 /github.com/shaikhsajid1111/facebook_page_scraper/graphs/commit-activity) [!
 [PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://
 opensource.org/licenses/MIT) [![Python >=3.6.9](https://img.shields.io/badge/
 python-3.6+-blue.svg)](https://www.python.org/downloads/release/python-360/)
@@ -38,15 +38,15 @@
                 # Scrape_in_CSV_format
                       # Parameters_for_scrape_to_csv()_method
                 # Keys_of_the_output_data
    3. Tech
    4. License
 
 ***** Prerequisites *****
-- Internet Connection - Python 3.6+ - Chrome or Firefox browser installed on
+- Internet Connection - Python 3.7+ - Chrome or Firefox browser installed on
 your machine
 ===============================================================================
 ***** Installation: *****
 **** Installing from source: ****
 ``` git clone https://github.com/shaikhsajid1111/facebook_page_scraper ```
 *** Inside project's directory ***
 ``` python3 setup.py install ```
```

### Comparing `facebook_page_scraper-5.0.0/setup.py` & `facebook_page_scraper-5.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 requirements = ['selenium==4.1.0',
                 'webdriver-manager==3.2.2',
-                'selenium-wire==4.3.1',
+                'selenium-wire==5.1.0',
                 'python-dateutil==2.8.2']
 
 
 setuptools.setup(
     name="facebook_page_scraper",
-    version="5.0.0",
+    version="5.0.1",
     author="Sajid Shaikh",
     author_email="shaikhsajid3732@gmail.com",
     description="Python package to scrap facebook's pages front end with no limitations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/shaikhsajid1111/facebook_page_scraper",
@@ -37,10 +37,10 @@
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Internet :: WWW/HTTP"
 
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=requirements
 )
```

