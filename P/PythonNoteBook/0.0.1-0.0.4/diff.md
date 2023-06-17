# Comparing `tmp/PythonNoteBook-0.0.1.tar.gz` & `tmp/PythonNoteBook-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonNoteBook-0.0.1.tar", last modified: Sat Jun 17 18:06:47 2023, max compression
+gzip compressed data, was "PythonNoteBook-0.0.4.tar", last modified: Sat Jun 17 18:17:37 2023, max compression
```

## Comparing `PythonNoteBook-0.0.1.tar` & `PythonNoteBook-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:06:47.817146 PythonNoteBook-0.0.1/
--rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PythonNoteBook-0.0.1/LICENSE
--rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PythonNoteBook-0.0.1/MANIFEST.in
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:06:47.815603 PythonNoteBook-0.0.1/NoteBook/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      202 2023-06-17 17:58:12.000000 PythonNoteBook-0.0.1/NoteBook/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 17:45:31.000000 PythonNoteBook-0.0.1/NoteBook/__version__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      157 2023-06-17 17:58:50.000000 PythonNoteBook-0.0.1/NoteBook/engine.py
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:06:47.816178 PythonNoteBook-0.0.1/NoteBook/variable/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PythonNoteBook-0.0.1/NoteBook/variable/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      317 2023-06-17 17:58:03.000000 PythonNoteBook-0.0.1/NoteBook/variable/variable.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      688 2023-06-17 18:06:47.817023 PythonNoteBook-0.0.1/PKG-INFO
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:06:47.816844 PythonNoteBook-0.0.1/PythonNoteBook.egg-info/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      688 2023-06-17 18:06:47.000000 PythonNoteBook-0.0.1/PythonNoteBook.egg-info/PKG-INFO
--rw-r--r--   0 huangjiabao   (501) staff       (20)      314 2023-06-17 18:06:47.000000 PythonNoteBook-0.0.1/PythonNoteBook.egg-info/SOURCES.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-17 18:06:47.000000 PythonNoteBook-0.0.1/PythonNoteBook.egg-info/dependency_links.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-17 18:06:47.000000 PythonNoteBook-0.0.1/PythonNoteBook.egg-info/top_level.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)       13 2023-06-17 17:50:58.000000 PythonNoteBook-0.0.1/README.md
--rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-17 18:06:47.817191 PythonNoteBook-0.0.1/setup.cfg
--rw-r--r--   0 huangjiabao   (501) staff       (20)     3898 2023-06-17 18:06:45.000000 PythonNoteBook-0.0.1/setup.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:17:37.345449 PythonNoteBook-0.0.4/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PythonNoteBook-0.0.4/LICENSE
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PythonNoteBook-0.0.4/MANIFEST.in
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:17:37.344089 PythonNoteBook-0.0.4/NoteBook/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      202 2023-06-17 17:58:12.000000 PythonNoteBook-0.0.4/NoteBook/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 18:16:29.000000 PythonNoteBook-0.0.4/NoteBook/__version__.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:17:37.344358 PythonNoteBook-0.0.4/NoteBook/variable/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PythonNoteBook-0.0.4/NoteBook/variable/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      316 2023-06-17 18:13:53.000000 PythonNoteBook-0.0.4/NoteBook/variable/variable.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      688 2023-06-17 18:17:37.345317 PythonNoteBook-0.0.4/PKG-INFO
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:17:37.345099 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      688 2023-06-17 18:17:37.000000 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/PKG-INFO
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      295 2023-06-17 18:17:37.000000 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/SOURCES.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-17 18:17:37.000000 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/dependency_links.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-17 18:17:37.000000 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/top_level.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       13 2023-06-17 17:50:58.000000 PythonNoteBook-0.0.4/README.md
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-17 18:17:37.345499 PythonNoteBook-0.0.4/setup.cfg
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     3898 2023-06-17 18:16:37.000000 PythonNoteBook-0.0.4/setup.py
```

### Comparing `PythonNoteBook-0.0.1/LICENSE` & `PythonNoteBook-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonNoteBook-0.0.1/NoteBook/__version__.py` & `PythonNoteBook-0.0.4/NoteBook/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 # @Software: PyCharm
 # @Blog    ：https://bornforthis.cn/
 # 8b    d8 Yb  dP 88""Yb    db     dP""b8 88  dP    db     dP""b8 888888
 # 88b  d88  YbdP  88__dP   dPYb   dP   `" 88odP    dPYb   dP   `" 88__
 # 88YbdP88   8P   88"""   dP__Yb  Yb      88"Yb   dP__Yb  Yb  "88 88""
 # 88 YY 88  dP    88     dP""""Yb  YboodP 88  Yb dP""""Yb  YboodP 888888
 
-VERSION = (0, 0, 1)
+VERSION = (0, 0, 4)
 
 __version__ = '.'.join(map(str, VERSION))
```

### Comparing `PythonNoteBook-0.0.1/PKG-INFO` & `PythonNoteBook-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonNoteBook
-Version: 0.0.1
+Version: 0.0.4
 Summary: 方便学员查询 Python 相关知识点,辅助考试。
 Home-page: https://github.com/AndersonHJB/PyNoteBook
 Author: Bornforthis
 Author-email: bornforthis@bornforthis.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PythonNoteBook-0.0.1/PythonNoteBook.egg-info/PKG-INFO` & `PythonNoteBook-0.0.4/PythonNoteBook.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonNoteBook
-Version: 0.0.1
+Version: 0.0.4
 Summary: 方便学员查询 Python 相关知识点,辅助考试。
 Home-page: https://github.com/AndersonHJB/PyNoteBook
 Author: Bornforthis
 Author-email: bornforthis@bornforthis.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `PythonNoteBook-0.0.1/setup.py` & `PythonNoteBook-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'PythonNoteBook'
 DESCRIPTION = '方便学员查询 Python 相关知识点,辅助考试。'
 URL = 'https://github.com/AndersonHJB/PyNoteBook'
 EMAIL = 'bornforthis@bornforthis.com'
 AUTHOR = 'Bornforthis'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.1'
+VERSION = '0.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

