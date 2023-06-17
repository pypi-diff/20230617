# Comparing `tmp/evatr-client-0.0.4.tar.gz` & `tmp/evatr-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evatr-client-0.0.4.tar", last modified: Fri Jun 16 17:03:02 2023, max compression
+gzip compressed data, was "evatr-client-0.1.0.tar", last modified: Sat Jun 17 17:17:47 2023, max compression
```

## Comparing `evatr-client-0.0.4.tar` & `evatr-client-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-16 17:03:02.624590 evatr-client-0.0.4/
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1068 2023-06-16 08:34:10.000000 evatr-client-0.0.4/LICENSE.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      830 2023-06-16 17:03:02.624760 evatr-client-0.0.4/PKG-INFO
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1696 2023-06-16 08:34:10.000000 evatr-client-0.0.4/README.md
-drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-16 17:03:02.622306 evatr-client-0.0.4/evatr_client/
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      171 2023-06-16 17:00:00.000000 evatr-client-0.0.4/evatr_client/__init__.py
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     3579 2023-06-16 17:02:51.000000 evatr-client-0.0.4/evatr_client/client.py
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     4532 2023-06-16 08:34:10.000000 evatr-client-0.0.4/evatr_client/status_codes.py
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     2016 2023-06-16 17:01:52.000000 evatr-client-0.0.4/evatr_client/util.py
-drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-16 17:03:02.624212 evatr-client-0.0.4/evatr_client.egg-info/
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      830 2023-06-16 17:03:02.000000 evatr-client-0.0.4/evatr_client.egg-info/PKG-INFO
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)      317 2023-06-16 17:03:02.000000 evatr-client-0.0.4/evatr_client.egg-info/SOURCES.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)        1 2023-06-16 17:03:02.000000 evatr-client-0.0.4/evatr_client.egg-info/dependency_links.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)       32 2023-06-16 17:03:02.000000 evatr-client-0.0.4/evatr_client.egg-info/requires.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)       13 2023-06-16 17:03:02.000000 evatr-client-0.0.4/evatr_client.egg-info/top_level.txt
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)       79 2023-06-16 17:03:02.625652 evatr-client-0.0.4/setup.cfg
--rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1182 2023-06-16 16:47:00.000000 evatr-client-0.0.4/setup.py
+drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-17 17:17:47.334418 evatr-client-0.1.0/
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1068 2023-06-16 08:34:10.000000 evatr-client-0.1.0/LICENSE.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      863 2023-06-17 17:17:47.334579 evatr-client-0.1.0/PKG-INFO
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     3202 2023-06-16 21:31:12.000000 evatr-client-0.1.0/README.md
+drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-17 17:17:47.331919 evatr-client-0.1.0/evatr_client/
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      171 2023-06-16 17:00:00.000000 evatr-client-0.1.0/evatr_client/__init__.py
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     6070 2023-06-17 17:04:35.000000 evatr-client-0.1.0/evatr_client/client.py
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     4532 2023-06-17 16:38:13.000000 evatr-client-0.1.0/evatr_client/status_codes.py
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     5905 2023-06-17 17:01:59.000000 evatr-client-0.1.0/evatr_client/util.py
+drwxr-xr-x   0 cedricaltermatt   (501) staff       (20)        0 2023-06-17 17:17:47.334115 evatr-client-0.1.0/evatr_client.egg-info/
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      863 2023-06-17 17:17:47.000000 evatr-client-0.1.0/evatr_client.egg-info/PKG-INFO
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)      317 2023-06-17 17:17:47.000000 evatr-client-0.1.0/evatr_client.egg-info/SOURCES.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)        1 2023-06-17 17:17:47.000000 evatr-client-0.1.0/evatr_client.egg-info/dependency_links.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)       32 2023-06-17 17:17:47.000000 evatr-client-0.1.0/evatr_client.egg-info/requires.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)       13 2023-06-17 17:17:47.000000 evatr-client-0.1.0/evatr_client.egg-info/top_level.txt
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)       79 2023-06-17 17:17:47.335148 evatr-client-0.1.0/setup.cfg
+-rw-r--r--   0 cedricaltermatt   (501) staff       (20)     1221 2023-06-17 17:07:11.000000 evatr-client-0.1.0/setup.py
```

### Comparing `evatr-client-0.0.4/LICENSE.txt` & `evatr-client-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evatr-client-0.0.4/PKG-INFO` & `evatr-client-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: evatr-client
-Version: 0.0.4
+Version: 0.1.0
 Summary: A client for: https://evatr.bff-online.de/eVatR/
 Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.4.tar.gz
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.0.tar.gz
 Author: CeeDiii
 License: MIT
-Keywords: python,uid,vat,uid prüfung,vat validation,evatr
+Keywords: python,uid,vat,uid prüfung,vat validation,evatr,evatr client,evatr python client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
```

### Comparing `evatr-client-0.0.4/evatr_client/status_codes.py` & `evatr-client-0.1.0/evatr_client/status_codes.py`

 * *Files identical despite different names*

### Comparing `evatr-client-0.0.4/evatr_client.egg-info/PKG-INFO` & `evatr-client-0.1.0/evatr_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: evatr-client
-Version: 0.0.4
+Version: 0.1.0
 Summary: A client for: https://evatr.bff-online.de/eVatR/
 Home-page: https://github.com/CeeDiii/evatr-client
-Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.4.tar.gz
+Download-URL: https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.0.tar.gz
 Author: CeeDiii
 License: MIT
-Keywords: python,uid,vat,uid prüfung,vat validation,evatr
+Keywords: python,uid,vat,uid prüfung,vat validation,evatr,evatr client,evatr python client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.10
```

### Comparing `evatr-client-0.0.4/setup.py` & `evatr-client-0.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.1.0'
 DESCRIPTION = 'A client for: https://evatr.bff-online.de/eVatR/'
 LONG_DESCRIPTION = 'A client to validate EU-VAT numbers with the official German tool that can be found here: https://evatr.bff-online.de/eVatR/'
 
 # Setting up
 setup(
     name="evatr-client",
     version=VERSION,
     author="CeeDiii",
     description=DESCRIPTION,
     license='MIT',
     url='https://github.com/CeeDiii/evatr-client',
-    download_url='https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.0.4.tar.gz',
+    download_url='https://github.com/CeeDiii/evatr-client/archive/refs/tags/v0.1.0.tar.gz',
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    keywords=['python', 'uid', 'vat', 'uid prüfung', 'vat validation', 'evatr'],
+    keywords=['python', 'uid', 'vat', 'uid prüfung', 'vat validation', 'evatr', 'evatr client', 'evatr python client'],
     python_requires=">=3.10",
     install_requires=[
           'requests',
           'urllib3',
           'beautifulsoup4',
     ],
     classifiers=[
```

