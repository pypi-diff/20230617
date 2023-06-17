# Comparing `tmp/auto-screener-0.2.0.tar.gz` & `tmp/auto-screener-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-0.2.0.tar", last modified: Sat Jun 17 10:42:21 2023, max compression
+gzip compressed data, was "auto-screener-1.0.0.tar", last modified: Sat Jun 17 11:15:03 2023, max compression
```

## Comparing `auto-screener-0.2.0.tar` & `auto-screener-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 10:42:21.932310 auto-screener-0.2.0/
--rw-rw-rw-   0        0        0       98 2023-06-17 10:42:21.000000 auto-screener-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-06-17 10:42:21.931313 auto-screener-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 10:42:21.926311 auto-screener-0.2.0/auto_screener/
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.2.0/auto_screener/base.py
--rw-rw-rw-   0        0        0    17233 2023-06-15 21:24:06.000000 auto-screener-0.2.0/auto_screener/collect.py
--rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-0.2.0/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-0.2.0/auto_screener/document.py
--rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-0.2.0/auto_screener/exchanges.py
--rw-rw-rw-   0        0        0    26654 2023-06-17 10:31:17.000000 auto-screener-0.2.0/auto_screener/feed.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.2.0/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.2.0/auto_screener/interval.py
--rw-rw-rw-   0        0        0    33759 2023-06-17 10:31:17.000000 auto-screener-0.2.0/auto_screener/screener.py
--rw-rw-rw-   0        0        0    32301 2023-06-17 10:33:08.000000 auto-screener-0.2.0/auto_screener/screening.py
--rw-rw-rw-   0        0        0    10070 2023-06-15 16:44:13.000000 auto-screener-0.2.0/auto_screener/symbols.py
-drwxrwxrwx   0        0        0        0 2023-06-17 10:42:21.930310 auto-screener-0.2.0/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-17 10:42:21.000000 auto-screener-0.2.0/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.2.0/build.py
--rw-rw-rw-   0        0        0      645 2023-06-17 10:42:21.000000 auto-screener-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       79 2023-06-17 10:23:38.000000 auto-screener-0.2.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       70 2023-06-17 10:23:38.000000 auto-screener-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 10:42:21.932310 auto-screener-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1564 2023-06-17 10:42:08.000000 auto-screener-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:15:03.253888 auto-screener-1.0.0/
+-rw-rw-rw-   0        0        0       98 2023-06-17 11:15:03.000000 auto-screener-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-06-17 11:15:03.253888 auto-screener-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 11:15:03.247886 auto-screener-1.0.0/auto_screener/
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-1.0.0/auto_screener/base.py
+-rw-rw-rw-   0        0        0    17233 2023-06-15 21:24:06.000000 auto-screener-1.0.0/auto_screener/collect.py
+-rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-1.0.0/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-1.0.0/auto_screener/document.py
+-rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-1.0.0/auto_screener/exchanges.py
+-rw-rw-rw-   0        0        0    26654 2023-06-17 10:31:17.000000 auto-screener-1.0.0/auto_screener/feed.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-1.0.0/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-1.0.0/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    33759 2023-06-17 10:31:17.000000 auto-screener-1.0.0/auto_screener/screener.py
+-rw-rw-rw-   0        0        0    32301 2023-06-17 10:33:08.000000 auto-screener-1.0.0/auto_screener/screening.py
+-rw-rw-rw-   0        0        0    10070 2023-06-15 16:44:13.000000 auto-screener-1.0.0/auto_screener/symbols.py
+drwxrwxrwx   0        0        0        0 2023-06-17 11:15:03.252888 auto-screener-1.0.0/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-17 11:15:03.000000 auto-screener-1.0.0/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-06-17 11:15:03.000000 auto-screener-1.0.0/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 11:15:03.000000 auto-screener-1.0.0/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-06-17 11:15:03.000000 auto-screener-1.0.0/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-17 11:15:03.000000 auto-screener-1.0.0/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-1.0.0/build.py
+-rw-rw-rw-   0        0        0      645 2023-06-17 11:15:03.000000 auto-screener-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       79 2023-06-17 10:23:38.000000 auto-screener-1.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       70 2023-06-17 10:23:38.000000 auto-screener-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 11:15:03.253888 auto-screener-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1564 2023-06-17 11:14:58.000000 auto-screener-1.0.0/setup.py
```

### Comparing `auto-screener-0.2.0/PKG-INFO` & `auto-screener-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.2.0
+Version: 1.0.0
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.2.0/README.md` & `auto-screener-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener/base.py` & `auto-screener-1.0.0/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener/collect.py` & `auto-screener-1.0.0/auto_screener/collect.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener/dataset.py` & `auto-screener-1.0.0/auto_screener/dataset.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener/document.py` & `auto-screener-1.0.0/auto_screener/document.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener/feed.py` & `auto-screener-1.0.0/auto_screener/feed.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener/interval.py` & `auto-screener-1.0.0/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener/screener.py` & `auto-screener-1.0.0/auto_screener/screener.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener/screening.py` & `auto-screener-1.0.0/auto_screener/screening.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener/symbols.py` & `auto-screener-1.0.0/auto_screener/symbols.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/auto_screener.egg-info/PKG-INFO` & `auto-screener-1.0.0/auto_screener.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.2.0
+Version: 1.0.0
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.2.0/auto_screener.egg-info/SOURCES.txt` & `auto-screener-1.0.0/auto_screener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/build.py` & `auto-screener-1.0.0/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.2.0/pyproject.toml` & `auto-screener-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '0.2.0'
+version = '1.0.0'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-0.2.0/setup.py` & `auto-screener-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='0.2.0',
+        version='1.0.0',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

