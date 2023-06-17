# Comparing `tmp/python-utils-3.6.0.tar.gz` & `tmp/python-utils-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-utils-3.6.0.tar", last modified: Mon May 29 00:59:15 2023, max compression
+gzip compressed data, was "/Volumes/workspace/python-utils/dist/.tmp-5x_ekkqi/python-utils-3.6.1.tar", last modified: Sat Jun 17 11:33:55 2023, max compression
```

## Comparing `python-utils-3.6.0.tar` & `python-utils-3.6.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-29 00:59:15.642409 python-utils-3.6.0/
--rw-r--r--   0 rick       (501) staff       (20)     1501 2021-10-31 01:51:48.000000 python-utils-3.6.0/LICENSE
--rw-r--r--   0 rick       (501) staff       (20)      281 2022-10-29 20:47:53.000000 python-utils-3.6.0/MANIFEST.in
--rw-r--r--   0 rick       (501) staff       (20)     9086 2023-05-29 00:59:15.642876 python-utils-3.6.0/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)     8642 2023-05-29 00:58:50.000000 python-utils-3.6.0/README.rst
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-29 00:59:15.605651 python-utils-3.6.0/_python_utils_tests/
--rw-r--r--   0 rick       (501) staff       (20)        0 2023-05-29 00:58:48.000000 python-utils-3.6.0/_python_utils_tests/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       12 2021-12-16 15:50:12.000000 python-utils-3.6.0/_python_utils_tests/requirements.txt
--rw-r--r--   0 rick       (501) staff       (20)      508 2023-05-29 00:58:50.000000 python-utils-3.6.0/_python_utils_tests/test_aio.py
--rw-r--r--   0 rick       (501) staff       (20)      592 2023-02-08 16:44:13.000000 python-utils-3.6.0/_python_utils_tests/test_containers.py
--rw-r--r--   0 rick       (501) staff       (20)      897 2022-05-29 21:48:50.000000 python-utils-3.6.0/_python_utils_tests/test_decorators.py
--rw-r--r--   0 rick       (501) staff       (20)     1669 2022-05-30 22:13:21.000000 python-utils-3.6.0/_python_utils_tests/test_generators.py
--rw-r--r--   0 rick       (501) staff       (20)     1431 2022-05-29 21:48:50.000000 python-utils-3.6.0/_python_utils_tests/test_import.py
--rw-r--r--   0 rick       (501) staff       (20)      362 2022-05-29 02:02:55.000000 python-utils-3.6.0/_python_utils_tests/test_logger.py
--rw-r--r--   0 rick       (501) staff       (20)      271 2022-05-29 21:48:50.000000 python-utils-3.6.0/_python_utils_tests/test_python_utils.py
--rw-r--r--   0 rick       (501) staff       (20)     4326 2022-10-29 19:12:20.000000 python-utils-3.6.0/_python_utils_tests/test_time.py
--rw-r--r--   0 rick       (501) staff       (20)       50 2021-10-31 01:51:48.000000 python-utils-3.6.0/coverage.rc
--rw-r--r--   0 rick       (501) staff       (20)      391 2023-05-29 00:58:50.000000 python-utils-3.6.0/pyproject.toml
--rw-r--r--   0 rick       (501) staff       (20)      253 2023-05-29 00:58:50.000000 python-utils-3.6.0/pytest.ini
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-29 00:59:15.623605 python-utils-3.6.0/python_utils/
--rw-r--r--   0 rick       (501) staff       (20)      385 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/__about__.py
--rw-r--r--   0 rick       (501) staff       (20)     1705 2023-05-29 00:58:48.000000 python-utils-3.6.0/python_utils/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)      544 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/aio.py
--rw-r--r--   0 rick       (501) staff       (20)        0 2016-05-31 10:02:50.000000 python-utils-3.6.0/python_utils/compat.py
--rw-r--r--   0 rick       (501) staff       (20)     9783 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/containers.py
--rw-r--r--   0 rick       (501) staff       (20)    11404 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/converters.py
--rw-r--r--   0 rick       (501) staff       (20)     4061 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/decorators.py
--rw-r--r--   0 rick       (501) staff       (20)      617 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/exceptions.py
--rw-r--r--   0 rick       (501) staff       (20)     5015 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/formatters.py
--rw-r--r--   0 rick       (501) staff       (20)     2609 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/generators.py
--rw-r--r--   0 rick       (501) staff       (20)     3165 2022-05-29 21:48:50.000000 python-utils-3.6.0/python_utils/import_.py
--rw-r--r--   0 rick       (501) staff       (20)     3132 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/logger.py
--rw-r--r--   0 rick       (501) staff       (20)      358 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/loguru.py
--rw-r--r--   0 rick       (501) staff       (20)        0 2022-10-29 19:12:20.000000 python-utils-3.6.0/python_utils/py.typed
--rw-r--r--   0 rick       (501) staff       (20)     4711 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/terminal.py
--rw-r--r--   0 rick       (501) staff       (20)    11304 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/time.py
--rw-r--r--   0 rick       (501) staff       (20)     3652 2023-05-29 00:58:50.000000 python-utils-3.6.0/python_utils/types.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-05-29 00:59:15.641745 python-utils-3.6.0/python_utils.egg-info/
--rw-r--r--   0 rick       (501) staff       (20)     9086 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)     1069 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rick       (501) staff       (20)        1 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rick       (501) staff       (20)      160 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/requires.txt
--rw-r--r--   0 rick       (501) staff       (20)       13 2023-05-29 00:59:15.000000 python-utils-3.6.0/python_utils.egg-info/top_level.txt
--rw-r--r--   0 rick       (501) staff       (20)        2 2023-02-09 15:13:53.000000 python-utils-3.6.0/requirements.txt
--rw-r--r--   0 rick       (501) staff       (20)      611 2023-05-29 00:59:15.646852 python-utils-3.6.0/setup.cfg
--rw-r--r--   0 rick       (501) staff       (20)     1594 2023-05-29 00:58:50.000000 python-utils-3.6.0/setup.py
--rw-r--r--   0 rick       (501) staff       (20)     1440 2023-05-29 00:58:50.000000 python-utils-3.6.0/tox.ini
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-17 11:33:55.052707 python-utils-3.6.1/
+-rw-r--r--   0 rick       (501) staff       (20)     1501 2021-10-31 01:51:48.000000 python-utils-3.6.1/LICENSE
+-rw-r--r--   0 rick       (501) staff       (20)      281 2022-10-29 20:47:53.000000 python-utils-3.6.1/MANIFEST.in
+-rw-r--r--   0 rick       (501) staff       (20)     9086 2023-06-17 11:33:55.052829 python-utils-3.6.1/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)     8642 2023-05-29 00:58:50.000000 python-utils-3.6.1/README.rst
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-17 11:33:55.040573 python-utils-3.6.1/_python_utils_tests/
+-rw-r--r--   0 rick       (501) staff       (20)        0 2023-06-17 11:33:41.000000 python-utils-3.6.1/_python_utils_tests/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       12 2021-12-16 15:50:12.000000 python-utils-3.6.1/_python_utils_tests/requirements.txt
+-rw-r--r--   0 rick       (501) staff       (20)      508 2023-05-29 00:58:50.000000 python-utils-3.6.1/_python_utils_tests/test_aio.py
+-rw-r--r--   0 rick       (501) staff       (20)      592 2023-02-08 16:44:13.000000 python-utils-3.6.1/_python_utils_tests/test_containers.py
+-rw-r--r--   0 rick       (501) staff       (20)      897 2022-05-29 21:48:50.000000 python-utils-3.6.1/_python_utils_tests/test_decorators.py
+-rw-r--r--   0 rick       (501) staff       (20)     1669 2022-05-30 22:13:21.000000 python-utils-3.6.1/_python_utils_tests/test_generators.py
+-rw-r--r--   0 rick       (501) staff       (20)     1431 2022-05-29 21:48:50.000000 python-utils-3.6.1/_python_utils_tests/test_import.py
+-rw-r--r--   0 rick       (501) staff       (20)      362 2022-05-29 02:02:55.000000 python-utils-3.6.1/_python_utils_tests/test_logger.py
+-rw-r--r--   0 rick       (501) staff       (20)      271 2022-05-29 21:48:50.000000 python-utils-3.6.1/_python_utils_tests/test_python_utils.py
+-rw-r--r--   0 rick       (501) staff       (20)     4326 2022-10-29 19:12:20.000000 python-utils-3.6.1/_python_utils_tests/test_time.py
+-rw-r--r--   0 rick       (501) staff       (20)       50 2021-10-31 01:51:48.000000 python-utils-3.6.1/coverage.rc
+-rw-r--r--   0 rick       (501) staff       (20)      391 2023-05-29 00:58:50.000000 python-utils-3.6.1/pyproject.toml
+-rw-r--r--   0 rick       (501) staff       (20)      253 2023-05-29 00:58:50.000000 python-utils-3.6.1/pytest.ini
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-17 11:33:55.050628 python-utils-3.6.1/python_utils/
+-rw-r--r--   0 rick       (501) staff       (20)      385 2023-06-17 11:33:42.000000 python-utils-3.6.1/python_utils/__about__.py
+-rw-r--r--   0 rick       (501) staff       (20)     1705 2023-06-17 11:33:41.000000 python-utils-3.6.1/python_utils/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)      544 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/aio.py
+-rw-r--r--   0 rick       (501) staff       (20)        0 2016-05-31 10:02:50.000000 python-utils-3.6.1/python_utils/compat.py
+-rw-r--r--   0 rick       (501) staff       (20)     9783 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/containers.py
+-rw-r--r--   0 rick       (501) staff       (20)    11404 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/converters.py
+-rw-r--r--   0 rick       (501) staff       (20)     4061 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/decorators.py
+-rw-r--r--   0 rick       (501) staff       (20)      617 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/exceptions.py
+-rw-r--r--   0 rick       (501) staff       (20)     5015 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/formatters.py
+-rw-r--r--   0 rick       (501) staff       (20)     2609 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/generators.py
+-rw-r--r--   0 rick       (501) staff       (20)     3165 2022-05-29 21:48:50.000000 python-utils-3.6.1/python_utils/import_.py
+-rw-r--r--   0 rick       (501) staff       (20)     3132 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/logger.py
+-rw-r--r--   0 rick       (501) staff       (20)      358 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/loguru.py
+-rw-r--r--   0 rick       (501) staff       (20)        0 2022-10-29 19:12:20.000000 python-utils-3.6.1/python_utils/py.typed
+-rw-r--r--   0 rick       (501) staff       (20)     4711 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/terminal.py
+-rw-r--r--   0 rick       (501) staff       (20)    11304 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/time.py
+-rw-r--r--   0 rick       (501) staff       (20)     3652 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/types.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-17 11:33:55.052464 python-utils-3.6.1/python_utils.egg-info/
+-rw-r--r--   0 rick       (501) staff       (20)     9086 2023-06-17 11:33:54.000000 python-utils-3.6.1/python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)     1069 2023-06-17 11:33:55.000000 python-utils-3.6.1/python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rick       (501) staff       (20)        1 2023-06-17 11:33:54.000000 python-utils-3.6.1/python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rick       (501) staff       (20)      169 2023-06-17 11:33:54.000000 python-utils-3.6.1/python_utils.egg-info/requires.txt
+-rw-r--r--   0 rick       (501) staff       (20)       13 2023-06-17 11:33:54.000000 python-utils-3.6.1/python_utils.egg-info/top_level.txt
+-rw-r--r--   0 rick       (501) staff       (20)        2 2023-02-09 15:13:53.000000 python-utils-3.6.1/requirements.txt
+-rw-r--r--   0 rick       (501) staff       (20)      611 2023-06-17 11:33:55.054330 python-utils-3.6.1/setup.cfg
+-rw-r--r--   0 rick       (501) staff       (20)     1603 2023-06-17 11:33:42.000000 python-utils-3.6.1/setup.py
+-rw-r--r--   0 rick       (501) staff       (20)     1440 2023-05-29 00:58:50.000000 python-utils-3.6.1/tox.ini
```

### Comparing `python-utils-3.6.0/LICENSE` & `python-utils-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/PKG-INFO` & `python-utils-3.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-utils
-Version: 3.6.0
+Version: 3.6.1
 Summary: Python Utils is a module with some convenient utilities not included with the standard Python install
 Home-page: https://github.com/WoLpH/python-utils
 Author: Rick van Hattem
 Author-email: Wolph@wol.ph
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >3.8.0
```

### Comparing `python-utils-3.6.0/README.rst` & `python-utils-3.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/_python_utils_tests/test_containers.py` & `python-utils-3.6.1/_python_utils_tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/_python_utils_tests/test_decorators.py` & `python-utils-3.6.1/_python_utils_tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/_python_utils_tests/test_generators.py` & `python-utils-3.6.1/_python_utils_tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/_python_utils_tests/test_import.py` & `python-utils-3.6.1/_python_utils_tests/test_import.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/_python_utils_tests/test_time.py` & `python-utils-3.6.1/_python_utils_tests/test_time.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/__init__.py` & `python-utils-3.6.1/python_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/aio.py` & `python-utils-3.6.1/python_utils/aio.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/containers.py` & `python-utils-3.6.1/python_utils/containers.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/converters.py` & `python-utils-3.6.1/python_utils/converters.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/decorators.py` & `python-utils-3.6.1/python_utils/decorators.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/exceptions.py` & `python-utils-3.6.1/python_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/formatters.py` & `python-utils-3.6.1/python_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/generators.py` & `python-utils-3.6.1/python_utils/generators.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/import_.py` & `python-utils-3.6.1/python_utils/import_.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/logger.py` & `python-utils-3.6.1/python_utils/logger.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/terminal.py` & `python-utils-3.6.1/python_utils/terminal.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/time.py` & `python-utils-3.6.1/python_utils/time.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils/types.py` & `python-utils-3.6.1/python_utils/types.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/python_utils.egg-info/PKG-INFO` & `python-utils-3.6.1/python_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-utils
-Version: 3.6.0
+Version: 3.6.1
 Summary: Python Utils is a module with some convenient utilities not included with the standard Python install
 Home-page: https://github.com/WoLpH/python-utils
 Author: Rick van Hattem
 Author-email: Wolph@wol.ph
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >3.8.0
```

### Comparing `python-utils-3.6.0/python_utils.egg-info/SOURCES.txt` & `python-utils-3.6.1/python_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/setup.cfg` & `python-utils-3.6.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.0/setup.py` & `python-utils-3.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         url=about['__url__'],
         license='BSD',
         packages=setuptools.find_packages(
             exclude=['_python_utils_tests', '*.__pycache__'],
         ),
         package_data={'python_utils': ['py.typed']},
         long_description=long_description,
-        install_requires=['typing_extensions'],
+        install_requires=['typing_extensions>3.10.0.2'],
         tests_require=['pytest'],
         extras_require={
             'loguru': [
                 'loguru',
             ],
             'docs': [
                 'mock',
```

### Comparing `python-utils-3.6.0/tox.ini` & `python-utils-3.6.1/tox.ini`

 * *Files identical despite different names*

