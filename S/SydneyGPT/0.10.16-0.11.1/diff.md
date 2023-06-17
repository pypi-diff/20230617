# Comparing `tmp/SydneyGPT-0.10.16.tar.gz` & `tmp/SydneyGPT-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SydneyGPT-0.10.16.tar", last modified: Thu Jun 15 10:05:10 2023, max compression
+gzip compressed data, was "SydneyGPT-0.11.1.tar", last modified: Sat Jun 17 16:10:06 2023, max compression
```

## Comparing `SydneyGPT-0.10.16.tar` & `SydneyGPT-0.11.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:05:10.013564 SydneyGPT-0.10.16/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-15 10:05:10.013564 SydneyGPT-0.10.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-15 10:05:10.013564 SydneyGPT-0.10.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:05:10.009564 SydneyGPT-0.10.16/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:05:10.009564 SydneyGPT-0.10.16/src/SydneyGPT/
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/SydneyGPT.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/SydneyGPTUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/conversation_style.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-15 10:04:36.000000 SydneyGPT-0.10.16/src/SydneyGPT/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 10:05:10.013564 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-15 10:05:09.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-15 10:05:10.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 10:05:09.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 10:05:09.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-15 10:05:10.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-15 10:05:10.000000 SydneyGPT-0.10.16/src/SydneyGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:10:06.170879 SydneyGPT-0.11.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-17 16:09:40.000000 SydneyGPT-0.11.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-17 16:10:06.170879 SydneyGPT-0.11.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-17 16:09:40.000000 SydneyGPT-0.11.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-17 16:10:06.174879 SydneyGPT-0.11.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-17 16:09:40.000000 SydneyGPT-0.11.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:10:06.166879 SydneyGPT-0.11.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:10:06.170879 SydneyGPT-0.11.1/src/SydneyGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-06-17 16:09:40.000000 SydneyGPT-0.11.1/src/SydneyGPT/SydneyGPT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-17 16:09:40.000000 SydneyGPT-0.11.1/src/SydneyGPT/SydneyGPTUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-17 16:09:40.000000 SydneyGPT-0.11.1/src/SydneyGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-17 16:09:40.000000 SydneyGPT-0.11.1/src/SydneyGPT/conversation_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-17 16:09:40.000000 SydneyGPT-0.11.1/src/SydneyGPT/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:10:06.170879 SydneyGPT-0.11.1/src/SydneyGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-17 16:10:06.000000 SydneyGPT-0.11.1/src/SydneyGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-17 16:10:06.000000 SydneyGPT-0.11.1/src/SydneyGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:10:06.000000 SydneyGPT-0.11.1/src/SydneyGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-17 16:10:06.000000 SydneyGPT-0.11.1/src/SydneyGPT.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-17 16:10:06.000000 SydneyGPT-0.11.1/src/SydneyGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-17 16:10:06.000000 SydneyGPT-0.11.1/src/SydneyGPT.egg-info/top_level.txt
```

### Comparing `SydneyGPT-0.10.16/LICENSE` & `SydneyGPT-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.10.16/PKG-INFO` & `SydneyGPT-0.11.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SydneyGPT
-Version: 0.10.16
+Version: 0.11.1
 Summary: Reverse engineered Sydney Bing Chat API
 Home-page: https://github.com/rafaelcalleja/SydneyGPT
 Author: Rafael Calleja
 Author-email: rafaelcalleja@gmail.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/rafaelcalleja/SydneyGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

### Comparing `SydneyGPT-0.10.16/README.md` & `SydneyGPT-0.11.1/README.md`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.10.16/setup.py` & `SydneyGPT-0.11.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="SydneyGPT",
-    version="0.10.16",
+    version="0.11.1",
     license="GNU General Public License v2.0",
     author="Rafael Calleja",
     author_email="rafaelcalleja@gmail.com",
     description="Reverse engineered Sydney Bing Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/rafaelcalleja/SydneyGPT",
```

### Comparing `SydneyGPT-0.10.16/src/SydneyGPT/SydneyGPT.py` & `SydneyGPT-0.11.1/src/SydneyGPT/SydneyGPT.py`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.10.16/src/SydneyGPT/SydneyGPTUtils.py` & `SydneyGPT-0.11.1/src/SydneyGPT/SydneyGPTUtils.py`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.10.16/src/SydneyGPT/conversation_style.py` & `SydneyGPT-0.11.1/src/SydneyGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `SydneyGPT-0.10.16/src/SydneyGPT.egg-info/PKG-INFO` & `SydneyGPT-0.11.1/src/SydneyGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SydneyGPT
-Version: 0.10.16
+Version: 0.11.1
 Summary: Reverse engineered Sydney Bing Chat API
 Home-page: https://github.com/rafaelcalleja/SydneyGPT
 Author: Rafael Calleja
 Author-email: rafaelcalleja@gmail.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/rafaelcalleja/SydneyGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
```

