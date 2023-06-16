# Comparing `tmp/Lab93-Finance-0.0.1.2.tar.gz` & `tmp/Lab93-Finance-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lab93-Finance-0.0.1.2.tar", last modified: Fri Jun 16 20:58:52 2023, max compression
+gzip compressed data, was "Lab93-Finance-0.0.1.3.tar", last modified: Fri Jun 16 22:54:54 2023, max compression
```

## Comparing `Lab93-Finance-0.0.1.2.tar` & `Lab93-Finance-0.0.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.893568 Lab93-Finance-0.0.1.2/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 20:58:52.890235 Lab93-Finance-0.0.1.2/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      732 2023-06-16 20:57:27.000000 Lab93-Finance-0.0.1.2/pyproject.toml
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-06-16 20:58:52.893568 Lab93-Finance-0.0.1.2/setup.cfg
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.800233 Lab93-Finance-0.0.1.2/src/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.820233 Lab93-Finance-0.0.1.2/src/Lab93_Finance/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2059 2023-06-16 20:51:18.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2112 2023-06-16 20:57:11.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.840233 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     3542 2023-06-16 20:34:51.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.846900 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/assets/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1222 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/assets/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/assets/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.850234 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/positions/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1592 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/positions/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/positions/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.853567 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:51.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.860234 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/historic/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2724 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/historic/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/historic/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.863567 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1659 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.866901 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/stream/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1490 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/stream/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.870234 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.876901 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/CandlestickGraphs/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1984 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/CandlestickGraphs/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.880234 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/LinearRegression/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/LinearRegression/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/LinearRegression/__main__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.886901 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/MovingCrossAverage/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/MovingCrossAverage/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/MovingCrossAverage/__main__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/__init__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/__main__.py
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      977 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/old.__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.886901 Lab93-Finance-0.0.1.2/src/Lab93_Finance/reporting/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2027 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance/reporting/__init__.py
-drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:58:52.836900 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/PKG-INFO
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1328 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/SOURCES.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/dependency_links.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       62 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/requires.txt
--rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       14 2023-06-16 20:58:52.000000 Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/top_level.txt
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.719087 Lab93-Finance-0.0.1.3/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 22:54:54.712421 Lab93-Finance-0.0.1.3/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      732 2023-06-16 22:54:05.000000 Lab93-Finance-0.0.1.3/pyproject.toml
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       38 2023-06-16 22:54:54.719087 Lab93-Finance-0.0.1.3/setup.cfg
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.655754 Lab93-Finance-0.0.1.3/src/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.665754 Lab93-Finance-0.0.1.3/src/Lab93_Finance/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2401 2023-06-16 22:46:59.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2112 2023-06-16 20:57:11.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.675754 Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     3541 2023-06-16 22:52:53.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.679087 Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/assets/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1190 2023-06-16 22:39:31.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/assets/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/assets/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.682421 Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/positions/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1592 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/positions/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:52.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/positions/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.685754 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:51.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.689087 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/historic/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2724 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/historic/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:49.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/historic/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.692421 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/live/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1659 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/live/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/live/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.692421 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/live/stream/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1490 2023-06-16 20:34:50.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/live/stream/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.695754 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.702421 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/CandlestickGraphs/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1984 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/CandlestickGraphs/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.705754 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/LinearRegression/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/LinearRegression/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:54.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/LinearRegression/__main__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.709087 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/MovingCrossAverage/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/MovingCrossAverage/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/MovingCrossAverage/__main__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:53.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/__init__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/__main__.py
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      977 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/old.__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.709087 Lab93-Finance-0.0.1.3/src/Lab93_Finance/reporting/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     2027 2023-06-16 20:34:55.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance/reporting/__init__.py
+drwxr-xr-x   0 guyyatsu  (1000) guyyatsu  (1000)        0 2023-06-16 22:54:54.675754 Lab93-Finance-0.0.1.3/src/Lab93_Finance.egg-info/
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)      518 2023-06-16 22:54:54.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance.egg-info/PKG-INFO
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)     1328 2023-06-16 22:54:54.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance.egg-info/SOURCES.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)        1 2023-06-16 22:54:54.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance.egg-info/dependency_links.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       62 2023-06-16 22:54:54.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance.egg-info/requires.txt
+-rw-r--r--   0 guyyatsu  (1000) guyyatsu  (1000)       14 2023-06-16 22:54:54.000000 Lab93-Finance-0.0.1.3/src/Lab93_Finance.egg-info/top_level.txt
```

### Comparing `Lab93-Finance-0.0.1.2/PKG-INFO` & `Lab93-Finance-0.0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lab93-Finance
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: A library for handling and managing finance accounts algorithmically.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/Lab-93/Finance
 Project-URL: Bug Tracker, https://github.com/Lab-93/Finance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Lab93-Finance-0.0.1.2/pyproject.toml` & `Lab93-Finance-0.0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Lab93-Finance"
-version = "0.0.1.2"
+version = "0.0.1.3"
 authors = [
   { name="Hunter Dale", email="hunter@guyyatsu.me" },
 ]
 
 description = "A library for handling and managing finance accounts algorithmically."
 readme = "readme.md"
 requires-python = ">=3.7"
```

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 from Lab93_DatabaseSystem import AdministratorDatabase
 from datetime import datetime, timedelta
-from .graphing.CandlestickGraphs import drawCandlestick
-from .data.historic import Queries
+from graphing.CandlestickGraphs import drawCandlestick
+from data.historic import Queries
+from account import AccountDetails
 
 
 AdminDB = AdministratorDatabase()
 
 
 today = datetime.today()
 yesterday = today - timedelta(days=1)
 
 
+class AlpacaMarket:
+    def __init__(self):
+        self.account = AccountDetails(
+           ( AdminDB.Retrieve( user = "admin",
+                               platform = "alpaca_key" ),
+             AdminDB.Retrieve( user = "admin",
+                               platform = "alpaca_secret" ) ),
+        )
+
 class GraphingReports:
     def __init__(self, start=yesterday, end=today,
         output = "/server/front-end/assets/data-science/reports" ):
 
         # Collect High, Low, Open, Close, and Times for the given symbol.
         # TODO: Allow for custom symbol entries.
         # TODO: Allow for custom timeframes.
```

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/__main__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/__main__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 with your Alpaca.Markets account in an algorithmic
 manner.  
 """
 
 
 # Utilize the Alpaca-Py SDK to interact with money.
 from alpaca.trading.client import TradingClient
-from positions import Positions
-from assets import Assets
+from .positions import Positions
+from .assets import Assets
 
 
 class AccountDetails:
 
     def __init__(self, credentials: tuple) -> None:
 
         key, secret = credentials[0], credentials[1]
         client = TradingClient( key, secret,
                                 paper=False )
 
         self.data = client.get_account()
-
         self.assets    = Assets(   client )
         self.positions = Position( client )
 
 
     def Id( self ):
         return self.data\
                    .id
@@ -55,15 +54,15 @@
 
     def LastEquity( self ):
         return self.data\
                    .last_equity
 
     def Multiplier( self ):
         return self.data\
-                   ..multiplier
+                   .multiplier
 
     def AccruedFees( self ):
         return self.data\
                    .accrued_fees
 
     def BuyingPower( self ):
         return self.data\
@@ -135,15 +134,15 @@
 
     def DaytradeBuyingPower( self ):
         return self.data\
                    .daytrading_buying_power
 
     def TradeSuspendedByUser( self ):
         return self.data\
-                   ..trade_suspended_by_user
+                   .trade_suspended_by_user
 
     def LastMaintenanceMargin( self ):
         return self.data\
                    .last_maintenance_margin
 
     def NonMarginableBuyingPower( self ):
         return self.data\
```

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/assets/__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/assets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 # Utilize the Alpaca-Py SDK to interact with money.
 from alpaca.trading.requests import GetAssetsRequest
 from alpaca.trading.enums import AssetClass
 
 
 class Assets:
-        """
-        Curate a list of offerings available on the Alpaca market.
-  
-        Currently, we only display the cryptocurrency assets, as there are over
-        31,000 us_equity assets maintained by Alpaca.
-  
-        To display equity assets, the 31,000 should be broken up alphabetically
-        and given by the broker bot individually, piece by piece.
-        """
+    """
+    Curate a list of offerings available on the Alpaca market.
+
+    Currently, we only display the cryptocurrency assets, as there are over
+    31,000 us_equity assets maintained by Alpaca.
+
+    To display equity assets, the 31,000 should be broken up alphabetically
+    and given by the broker bot individually, piece by piece.
+    """
 
 
     def __init__( self, client ):
         self.client = client
 
 
     def Cryptocurrencies( self ):
```

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/account/positions/__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/account/positions/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/historic/__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/historic/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/live/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/data/live/stream/__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/data/live/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/CandlestickGraphs/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/graphing/old.__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/graphing/old.__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance/reporting/__init__.py` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/PKG-INFO` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lab93-Finance
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: A library for handling and managing finance accounts algorithmically.
 Author-email: Hunter Dale <hunter@guyyatsu.me>
 Project-URL: Homepage, https://github.com/Lab-93/Finance
 Project-URL: Bug Tracker, https://github.com/Lab-93/Finance/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `Lab93-Finance-0.0.1.2/src/Lab93_Finance.egg-info/SOURCES.txt` & `Lab93-Finance-0.0.1.3/src/Lab93_Finance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

