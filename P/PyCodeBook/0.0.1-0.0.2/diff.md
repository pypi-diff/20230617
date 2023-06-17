# Comparing `tmp/PyCodeBook-0.0.1.tar.gz` & `tmp/PyCodeBook-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCodeBook-0.0.1.tar", last modified: Sat Jun 17 18:30:07 2023, max compression
+gzip compressed data, was "PyCodeBook-0.0.2.tar", last modified: Sat Jun 17 18:32:31 2023, max compression
```

## Comparing `PyCodeBook-0.0.1.tar` & `PyCodeBook-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:30:07.538290 PyCodeBook-0.0.1/
--rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PyCodeBook-0.0.1/LICENSE
--rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PyCodeBook-0.0.1/MANIFEST.in
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:30:07.537115 PyCodeBook-0.0.1/NoteBook/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      234 2023-06-17 18:26:18.000000 PyCodeBook-0.0.1/NoteBook/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 18:16:29.000000 PyCodeBook-0.0.1/NoteBook/__version__.py
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:30:07.537481 PyCodeBook-0.0.1/NoteBook/variable/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PyCodeBook-0.0.1/NoteBook/variable/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      352 2023-01-07 02:10:39.000000 PyCodeBook-0.0.1/NoteBook/variable/__version__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      316 2023-06-17 18:13:53.000000 PyCodeBook-0.0.1/NoteBook/variable/variable.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      736 2023-06-17 18:30:07.538177 PyCodeBook-0.0.1/PKG-INFO
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:30:07.538006 PyCodeBook-0.0.1/PyCodeBook.egg-info/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      736 2023-06-17 18:30:07.000000 PyCodeBook-0.0.1/PyCodeBook.egg-info/PKG-INFO
--rw-r--r--   0 huangjiabao   (501) staff       (20)      312 2023-06-17 18:30:07.000000 PyCodeBook-0.0.1/PyCodeBook.egg-info/SOURCES.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-17 18:30:07.000000 PyCodeBook-0.0.1/PyCodeBook.egg-info/dependency_links.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-17 18:30:07.000000 PyCodeBook-0.0.1/PyCodeBook.egg-info/top_level.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)       64 2023-06-17 18:20:30.000000 PyCodeBook-0.0.1/README.md
--rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-17 18:30:07.538332 PyCodeBook-0.0.1/setup.cfg
--rw-r--r--   0 huangjiabao   (501) staff       (20)     3894 2023-06-17 18:29:53.000000 PyCodeBook-0.0.1/setup.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:32:31.454017 PyCodeBook-0.0.2/
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:32:31.452839 PyCodeBook-0.0.2/CodeBook/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      243 2023-06-17 18:32:13.000000 PyCodeBook-0.0.2/CodeBook/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 18:16:29.000000 PyCodeBook-0.0.2/CodeBook/__version__.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:32:31.453207 PyCodeBook-0.0.2/CodeBook/variable/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PyCodeBook-0.0.2/CodeBook/variable/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      352 2023-01-07 02:10:39.000000 PyCodeBook-0.0.2/CodeBook/variable/__version__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      316 2023-06-17 18:13:53.000000 PyCodeBook-0.0.2/CodeBook/variable/variable.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PyCodeBook-0.0.2/LICENSE
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PyCodeBook-0.0.2/MANIFEST.in
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-17 18:32:31.453903 PyCodeBook-0.0.2/PKG-INFO
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:32:31.453738 PyCodeBook-0.0.2/PyCodeBook.egg-info/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      732 2023-06-17 18:32:31.000000 PyCodeBook-0.0.2/PyCodeBook.egg-info/PKG-INFO
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      312 2023-06-17 18:32:31.000000 PyCodeBook-0.0.2/PyCodeBook.egg-info/SOURCES.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-17 18:32:31.000000 PyCodeBook-0.0.2/PyCodeBook.egg-info/dependency_links.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-17 18:32:31.000000 PyCodeBook-0.0.2/PyCodeBook.egg-info/top_level.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       60 2023-06-17 18:30:39.000000 PyCodeBook-0.0.2/README.md
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-17 18:32:31.454059 PyCodeBook-0.0.2/setup.cfg
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     3894 2023-06-17 18:32:24.000000 PyCodeBook-0.0.2/setup.py
```

### Comparing `PyCodeBook-0.0.1/LICENSE` & `PyCodeBook-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCodeBook-0.0.1/NoteBook/__version__.py` & `PyCodeBook-0.0.2/CodeBook/__version__.py`

 * *Files identical despite different names*

### Comparing `PyCodeBook-0.0.1/PKG-INFO` & `PyCodeBook-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCodeBook
-Version: 0.0.1
+Version: 0.0.2
 Summary: 方便学员查询 Python 相关知识点,辅助考试。
 Home-page: https://github.com/AndersonHJB/PyNoteBook
 Author: Bornforthis
 Author-email: bornforthis@bornforthis.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,9 +16,9 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PynoteBook
 
 ```python
-pip install --upgrade PythonNoteBook
+pip install --upgrade PyCodeBook
 ```
```

### Comparing `PyCodeBook-0.0.1/PyCodeBook.egg-info/PKG-INFO` & `PyCodeBook-0.0.2/PyCodeBook.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCodeBook
-Version: 0.0.1
+Version: 0.0.2
 Summary: 方便学员查询 Python 相关知识点,辅助考试。
 Home-page: https://github.com/AndersonHJB/PyNoteBook
 Author: Bornforthis
 Author-email: bornforthis@bornforthis.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,9 +16,9 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # PynoteBook
 
 ```python
-pip install --upgrade PythonNoteBook
+pip install --upgrade PyCodeBook
 ```
```

### Comparing `PyCodeBook-0.0.1/setup.py` & `PyCodeBook-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'PyCodeBook'
 DESCRIPTION = '方便学员查询 Python 相关知识点,辅助考试。'
 URL = 'https://github.com/AndersonHJB/PyNoteBook'
 EMAIL = 'bornforthis@bornforthis.com'
 AUTHOR = 'Bornforthis'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

