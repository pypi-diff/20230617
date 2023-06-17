# Comparing `tmp/pymultithreading-0.0.0.tar.gz` & `tmp/pymultithreading-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymultithreading-0.0.0.tar", last modified: Sat Jun 17 10:21:57 2023, max compression
+gzip compressed data, was "pymultithreading-0.1.0.tar", last modified: Sat Jun 17 15:09:30 2023, max compression
```

## Comparing `pymultithreading-0.0.0.tar` & `pymultithreading-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 10:21:57.305412 pymultithreading-0.0.0/
--rw-rw-rw-   0        0        0       98 2023-06-17 10:21:57.000000 pymultithreading-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2045 2023-06-17 10:21:57.305412 pymultithreading-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.0.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-17 10:21:57.291411 pymultithreading-0.0.0/multithreading/
--rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.0.0/multithreading/__init__.py
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 pymultithreading-0.0.0/multithreading/base.py
--rw-rw-rw-   0        0        0      220 2023-06-17 10:20:04.000000 pymultithreading-0.0.0/multithreading/document.py
--rw-rw-rw-   0        0        0     4789 2023-06-17 10:19:47.000000 pymultithreading-0.0.0/multithreading/process.py
-drwxrwxrwx   0        0        0        0 2023-06-17 10:21:57.304414 pymultithreading-0.0.0/pymultithreading.egg-info/
--rw-rw-rw-   0        0        0     2045 2023-06-17 10:21:57.000000 pymultithreading-0.0.0/pymultithreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-06-17 10:21:57.000000 pymultithreading-0.0.0/pymultithreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 10:21:57.000000 pymultithreading-0.0.0/pymultithreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-17 10:21:57.000000 pymultithreading-0.0.0/pymultithreading.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-17 10:21:57.000000 pymultithreading-0.0.0/pymultithreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      635 2023-06-17 10:21:57.000000 pymultithreading-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 10:21:57.305412 pymultithreading-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1561 2023-06-17 10:21:46.000000 pymultithreading-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:09:30.915073 pymultithreading-0.1.0/
+-rw-rw-rw-   0        0        0       98 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2045 2023-06-17 15:09:30.914075 pymultithreading-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1243 2023-06-17 10:16:35.000000 pymultithreading-0.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 pymultithreading-0.1.0/build.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:09:30.899039 pymultithreading-0.1.0/multithreading/
+-rw-rw-rw-   0        0        0       53 2023-06-17 10:18:28.000000 pymultithreading-0.1.0/multithreading/__init__.py
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 pymultithreading-0.1.0/multithreading/base.py
+-rw-rw-rw-   0        0        0      220 2023-06-17 10:20:04.000000 pymultithreading-0.1.0/multithreading/document.py
+-rw-rw-rw-   0        0        0    10505 2023-06-17 14:58:52.000000 pymultithreading-0.1.0/multithreading/process.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:09:30.913104 pymultithreading-0.1.0/pymultithreading.egg-info/
+-rw-rw-rw-   0        0        0     2045 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pymultithreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      635 2023-06-17 15:09:30.000000 pymultithreading-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       20 2023-05-30 09:10:35.000000 pymultithreading-0.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 09:09:27.000000 pymultithreading-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 15:09:30.915073 pymultithreading-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1561 2023-06-17 15:09:21.000000 pymultithreading-0.1.0/setup.py
```

### Comparing `pymultithreading-0.0.0/PKG-INFO` & `pymultithreading-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.0.0
+Version: 0.1.0
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.0.0/README.md` & `pymultithreading-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.0.0/build.py` & `pymultithreading-0.1.0/build.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.0.0/multithreading/base.py` & `pymultithreading-0.1.0/multithreading/base.py`

 * *Files identical despite different names*

### Comparing `pymultithreading-0.0.0/pymultithreading.egg-info/PKG-INFO` & `pymultithreading-0.1.0/pymultithreading.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymultithreading
-Version: 0.0.0
+Version: 0.1.0
 Summary: A python module for creating multithreading processes easily, in a more Pythonic way.
 Home-page: https://github.com/Shahaf-F-S/multithreading
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymultithreading-0.0.0/pyproject.toml` & `pymultithreading-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pymultithreading'
-version = '0.0.0'
+version = '0.1.0'
 description = 'A python module for creating multithreading processes easily, in a more Pythonic way.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pymultithreading-0.0.0/setup.py` & `pymultithreading-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             "__pycache__",
             "*.pyc"
         ],
         include=[],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pymultithreading',
-        version='0.0.0',
+        version='0.1.0',
         description=(
             "A python module for creating multithreading "
             "processes easily, in a more Pythonic way."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

