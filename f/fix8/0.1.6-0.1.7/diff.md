# Comparing `tmp/fix8-0.1.6.tar.gz` & `tmp/fix8-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fix8-0.1.6.tar", last modified: Sat Jun 17 18:20:28 2023, max compression
+gzip compressed data, was "fix8-0.1.7.tar", last modified: Sat Jun 17 18:23:52 2023, max compression
```

## Comparing `fix8-0.1.6.tar` & `fix8-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-17 18:20:28.369139 fix8-0.1.6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-06-17 18:20:28.369139 fix8-0.1.6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-17 18:20:19.000000 fix8-0.1.6/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-17 18:20:28.369139 fix8-0.1.6/fix8.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      229 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-17 18:20:28.000000 fix8-0.1.6/fix8.egg-info/zip-safe
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    14750 2023-06-17 18:20:19.000000 fix8-0.1.6/fix8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      986 2023-06-17 18:20:28.369139 fix8-0.1.6/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1493 2023-06-17 18:20:19.000000 fix8-0.1.6/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-17 18:23:52.606634 fix8-0.1.7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2023-06-17 18:23:52.606634 fix8-0.1.7/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1584 2023-06-17 18:23:43.000000 fix8-0.1.7/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-17 18:23:52.606634 fix8-0.1.7/fix8.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2720 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      229 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-17 18:23:52.000000 fix8-0.1.7/fix8.egg-info/zip-safe
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    14750 2023-06-17 18:23:43.000000 fix8-0.1.7/fix8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      986 2023-06-17 18:23:52.606634 fix8-0.1.7/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1543 2023-06-17 18:23:43.000000 fix8-0.1.7/setup.py
```

### Comparing `fix8-0.1.6/PKG-INFO` & `fix8-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fix8
-Version: 0.1.6
+Version: 0.1.7
 Summary: Automatic fix for Python linting issues found by Flake8
 Home-page: https://github.com/PeterJCLaw/fix8
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/PeterJCLaw/fix8/blob/master/README.md
 Project-URL: Code, https://github.com/PeterJCLaw/fix8
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fix8-0.1.6/README.md` & `fix8-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fix8-0.1.6/fix8.egg-info/PKG-INFO` & `fix8-0.1.7/fix8.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fix8
-Version: 0.1.6
+Version: 0.1.7
 Summary: Automatic fix for Python linting issues found by Flake8
 Home-page: https://github.com/PeterJCLaw/fix8
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/PeterJCLaw/fix8/blob/master/README.md
 Project-URL: Code, https://github.com/PeterJCLaw/fix8
@@ -13,14 +13,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fix8-0.1.6/fix8.py` & `fix8-0.1.7/fix8.py`

 * *Files identical despite different names*

### Comparing `fix8-0.1.6/setup.cfg` & `fix8-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `fix8-0.1.6/setup.py` & `fix8-0.1.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup  # type: ignore[import]
 
 with open('README.md') as file:
     long_description = file.read()
 
 setup(
     name='fix8',
-    version='0.1.6',
+    version='0.1.7',
     url='https://github.com/PeterJCLaw/fix8',
     project_urls={
         'Documentation': 'https://github.com/PeterJCLaw/fix8/blob/master/README.md',
         'Code': 'https://github.com/PeterJCLaw/fix8',
         'Issue tracker': 'https://github.com/PeterJCLaw/fix8/issues',
     },
     description="Automatic fix for Python linting issues found by Flake8",
@@ -27,14 +27,15 @@
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Quality Assurance',
         'Topic :: Utilities',
     ],
     python_requires='>=3.7',
     install_requires=[
```

