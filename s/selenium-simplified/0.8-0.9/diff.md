# Comparing `tmp/selenium-simplified-0.8.tar.gz` & `tmp/selenium-simplified-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selenium-simplified-0.8.tar", last modified: Thu Jun 15 16:56:02 2023, max compression
+gzip compressed data, was "selenium-simplified-0.9.tar", last modified: Thu Jun 15 17:03:48 2023, max compression
```

## Comparing `selenium-simplified-0.8.tar` & `selenium-simplified-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:56:02.672375 selenium-simplified-0.8/
--rw-rw-rw-   0        0        0     4488 2023-06-15 16:56:02.672375 selenium-simplified-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4006 2023-06-14 14:02:21.000000 selenium-simplified-0.8/README.md
--rw-rw-rw-   0        0        0      103 2023-06-15 16:03:52.000000 selenium-simplified-0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-15 16:56:02.662495 selenium-simplified-0.8/selenium_simplified.egg-info/
--rw-rw-rw-   0        0        0     4488 2023-06-15 16:56:02.000000 selenium-simplified-0.8/selenium_simplified.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-06-15 16:56:02.000000 selenium-simplified-0.8/selenium_simplified.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:56:02.000000 selenium-simplified-0.8/selenium_simplified.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-15 16:56:02.000000 selenium-simplified-0.8/selenium_simplified.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 16:56:02.000000 selenium-simplified-0.8/selenium_simplified.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 16:56:02.672375 selenium-simplified-0.8/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-15 16:52:53.000000 selenium-simplified-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:56:02.669193 selenium-simplified-0.8/simplified/
--rw-rw-rw-   0        0        0     1567 2023-06-15 16:32:34.000000 selenium-simplified-0.8/simplified/UserActivities.py
--rw-rw-rw-   0        0        0     1846 2023-06-15 16:15:59.000000 selenium-simplified-0.8/simplified/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:56:02.672375 selenium-simplified-0.8/simplified/locator/
--rw-rw-rw-   0        0        0      952 2023-06-15 16:35:30.000000 selenium-simplified-0.8/simplified/locator/TagsLocator.py
--rw-rw-rw-   0        0        0      476 2023-06-15 16:51:42.000000 selenium-simplified-0.8/simplified/locator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:03:48.651039 selenium-simplified-0.9/
+-rw-rw-rw-   0        0        0     4488 2023-06-15 17:03:48.651039 selenium-simplified-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4006 2023-06-14 14:02:21.000000 selenium-simplified-0.9/README.md
+-rw-rw-rw-   0        0        0      103 2023-06-15 16:03:52.000000 selenium-simplified-0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-15 17:03:48.634685 selenium-simplified-0.9/selenium_simplified.egg-info/
+-rw-rw-rw-   0        0        0     4488 2023-06-15 17:03:48.000000 selenium-simplified-0.9/selenium_simplified.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-06-15 17:03:48.000000 selenium-simplified-0.9/selenium_simplified.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 17:03:48.000000 selenium-simplified-0.9/selenium_simplified.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-15 17:03:48.000000 selenium-simplified-0.9/selenium_simplified.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-15 17:03:48.000000 selenium-simplified-0.9/selenium_simplified.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 17:03:48.651039 selenium-simplified-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-15 17:03:12.000000 selenium-simplified-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:03:48.645020 selenium-simplified-0.9/simplified/
+-rw-rw-rw-   0        0        0     1567 2023-06-15 16:32:34.000000 selenium-simplified-0.9/simplified/UserActivities.py
+-rw-rw-rw-   0        0        0     1846 2023-06-15 16:15:59.000000 selenium-simplified-0.9/simplified/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-15 17:03:48.649438 selenium-simplified-0.9/simplified/locator/
+-rw-rw-rw-   0        0        0      952 2023-06-15 16:35:30.000000 selenium-simplified-0.9/simplified/locator/TagsLocator.py
+-rw-rw-rw-   0        0        0      476 2023-06-15 16:51:42.000000 selenium-simplified-0.9/simplified/locator/__init__.py
```

### Comparing `selenium-simplified-0.8/PKG-INFO` & `selenium-simplified-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-simplified
-Version: 0.8
+Version: 0.9
 Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `selenium-simplified-0.8/README.md` & `selenium-simplified-0.9/README.md`

 * *Files identical despite different names*

### Comparing `selenium-simplified-0.8/selenium_simplified.egg-info/PKG-INFO` & `selenium-simplified-0.9/selenium_simplified.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-simplified
-Version: 0.8
+Version: 0.9
 Summary: A free, open-source web automation library for the Chrome browser using Selenium Python
 Home-page: https://github.com/raajrajnish/SeleniumSimplified.git
 Author: rajnish kumar
 Author-email: raajrajnish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `selenium-simplified-0.8/setup.py` & `selenium-simplified-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="selenium-simplified",
-    version="0.8",
+    version="0.9",
     author="rajnish kumar",
     author_email="raajrajnish@gmail.com",
     description="A free, open-source web automation library for the Chrome browser using Selenium Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raajrajnish/SeleniumSimplified.git",
     packages=setuptools.find_packages(),
```

### Comparing `selenium-simplified-0.8/simplified/UserActivities.py` & `selenium-simplified-0.9/simplified/UserActivities.py`

 * *Files identical despite different names*

### Comparing `selenium-simplified-0.8/simplified/__init__.py` & `selenium-simplified-0.9/simplified/__init__.py`

 * *Files identical despite different names*

### Comparing `selenium-simplified-0.8/simplified/locator/TagsLocator.py` & `selenium-simplified-0.9/simplified/locator/TagsLocator.py`

 * *Files identical despite different names*

