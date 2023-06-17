# Comparing `tmp/FinGen-0.2.tar.gz` & `tmp/FinGen-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinGen-0.2.tar", last modified: Tue Mar  7 02:32:18 2023, max compression
+gzip compressed data, was "FinGen-0.3.tar", last modified: Sat Jun 17 03:58:14 2023, max compression
```

## Comparing `FinGen-0.2.tar` & `FinGen-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 02:32:18.095531 FinGen-0.2/
-drwxrwxrwx   0        0        0        0 2023-03-07 02:32:18.082435 FinGen-0.2/FinGen/
--rw-rw-rw-   0        0        0     3082 2023-03-07 02:23:14.000000 FinGen-0.2/FinGen/FindingsGenerator.py
--rw-rw-rw-   0        0        0     1440 2023-02-01 01:25:37.000000 FinGen-0.2/FinGen/Loader.py
--rw-rw-rw-   0        0        0        0 2023-02-01 01:30:43.000000 FinGen-0.2/FinGen/__init__.py
--rw-rw-rw-   0        0        0      196 2023-03-07 02:15:39.000000 FinGen-0.2/FinGen/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 02:32:18.093526 FinGen-0.2/FinGen.egg-info/
--rw-rw-rw-   0        0        0      595 2023-03-07 02:32:17.000000 FinGen-0.2/FinGen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-03-07 02:32:17.000000 FinGen-0.2/FinGen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 02:32:17.000000 FinGen-0.2/FinGen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-07 02:32:17.000000 FinGen-0.2/FinGen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-07 02:32:17.000000 FinGen-0.2/FinGen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-02-01 01:18:31.000000 FinGen-0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      595 2023-03-07 02:32:18.095531 FinGen-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-03-07 02:32:18.096530 FinGen-0.2/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-03-07 02:28:25.000000 FinGen-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 03:58:14.138520 FinGen-0.3/
+drwxrwxrwx   0        0        0        0 2023-06-17 03:58:14.122953 FinGen-0.3/FinGen/
+-rw-rw-rw-   0        0        0     4914 2023-06-17 03:56:41.000000 FinGen-0.3/FinGen/FindingsGenerator.py
+-rw-rw-rw-   0        0        0     1440 2023-02-01 01:25:37.000000 FinGen-0.3/FinGen/Loader.py
+-rw-rw-rw-   0        0        0        0 2023-02-01 01:30:43.000000 FinGen-0.3/FinGen/__init__.py
+-rw-rw-rw-   0        0        0      196 2023-03-07 02:15:39.000000 FinGen-0.3/FinGen/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 03:58:14.137516 FinGen-0.3/FinGen.egg-info/
+-rw-rw-rw-   0        0        0      595 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 03:58:13.000000 FinGen-0.3/FinGen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-02-01 01:18:31.000000 FinGen-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      595 2023-06-17 03:58:14.138520 FinGen-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-06-17 03:58:14.139517 FinGen-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-06-17 03:57:43.000000 FinGen-0.3/setup.py
```

### Comparing `FinGen-0.2/FinGen/Loader.py` & `FinGen-0.3/FinGen/Loader.py`

 * *Files identical despite different names*

### Comparing `FinGen-0.2/FinGen.egg-info/PKG-INFO` & `FinGen-0.3/FinGen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinGen
-Version: 0.2
+Version: 0.3
 Summary: A penetration testing findings generator using ChatGPT.
 Home-page: https://github.com/Stratus-Security/FinGen
 Author: Stratus Security
 Author-email: contact@stratussecurity.com
 License: GPLv3
 Keywords: ChatGPT,Pentesting,Penetration Testing,Findings Generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FinGen-0.2/LICENSE.txt` & `FinGen-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FinGen-0.2/PKG-INFO` & `FinGen-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinGen
-Version: 0.2
+Version: 0.3
 Summary: A penetration testing findings generator using ChatGPT.
 Home-page: https://github.com/Stratus-Security/FinGen
 Author: Stratus Security
 Author-email: contact@stratussecurity.com
 License: GPLv3
 Keywords: ChatGPT,Pentesting,Penetration Testing,Findings Generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `FinGen-0.2/setup.py` & `FinGen-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'FinGen',
   packages = ['FinGen'],
-  version = '0.2',
+  version = '0.3',
   license='GPLv3',
   description = 'A penetration testing findings generator using ChatGPT.',
   author = 'Stratus Security',
   author_email = 'contact@stratussecurity.com',
   url = 'https://github.com/Stratus-Security/FinGen',
   keywords = ['ChatGPT', 'Pentesting', 'Penetration Testing', 'Findings Generator'],
   install_requires=[
```

