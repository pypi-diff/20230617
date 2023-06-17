# Comparing `tmp/PythonNoteBook-0.0.4.tar.gz` & `tmp/PythonNoteBook-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonNoteBook-0.0.4.tar", last modified: Sat Jun 17 18:17:37 2023, max compression
+gzip compressed data, was "PythonNoteBook-0.0.5.tar", last modified: Sat Jun 17 18:22:28 2023, max compression
```

## Comparing `PythonNoteBook-0.0.4.tar` & `PythonNoteBook-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:17:37.345449 PythonNoteBook-0.0.4/
--rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PythonNoteBook-0.0.4/LICENSE
--rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PythonNoteBook-0.0.4/MANIFEST.in
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:17:37.344089 PythonNoteBook-0.0.4/NoteBook/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      202 2023-06-17 17:58:12.000000 PythonNoteBook-0.0.4/NoteBook/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 18:16:29.000000 PythonNoteBook-0.0.4/NoteBook/__version__.py
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:17:37.344358 PythonNoteBook-0.0.4/NoteBook/variable/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PythonNoteBook-0.0.4/NoteBook/variable/__init__.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      316 2023-06-17 18:13:53.000000 PythonNoteBook-0.0.4/NoteBook/variable/variable.py
--rw-r--r--   0 huangjiabao   (501) staff       (20)      688 2023-06-17 18:17:37.345317 PythonNoteBook-0.0.4/PKG-INFO
-drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:17:37.345099 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/
--rw-r--r--   0 huangjiabao   (501) staff       (20)      688 2023-06-17 18:17:37.000000 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/PKG-INFO
--rw-r--r--   0 huangjiabao   (501) staff       (20)      295 2023-06-17 18:17:37.000000 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/SOURCES.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-17 18:17:37.000000 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/dependency_links.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-17 18:17:37.000000 PythonNoteBook-0.0.4/PythonNoteBook.egg-info/top_level.txt
--rw-r--r--   0 huangjiabao   (501) staff       (20)       13 2023-06-17 17:50:58.000000 PythonNoteBook-0.0.4/README.md
--rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-17 18:17:37.345499 PythonNoteBook-0.0.4/setup.cfg
--rw-r--r--   0 huangjiabao   (501) staff       (20)     3898 2023-06-17 18:16:37.000000 PythonNoteBook-0.0.4/setup.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:22:28.832751 PythonNoteBook-0.0.5/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     1067 2023-06-17 17:44:13.000000 PythonNoteBook-0.0.5/LICENSE
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       25 2023-06-17 17:43:01.000000 PythonNoteBook-0.0.5/MANIFEST.in
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:22:28.831522 PythonNoteBook-0.0.5/NoteBook/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      234 2023-06-17 18:21:48.000000 PythonNoteBook-0.0.5/NoteBook/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      516 2023-06-17 18:16:29.000000 PythonNoteBook-0.0.5/NoteBook/__version__.py
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:22:28.831923 PythonNoteBook-0.0.5/NoteBook/variable/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      162 2023-06-17 17:54:20.000000 PythonNoteBook-0.0.5/NoteBook/variable/__init__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      352 2023-01-07 02:10:39.000000 PythonNoteBook-0.0.5/NoteBook/variable/__version__.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      316 2023-06-17 18:13:53.000000 PythonNoteBook-0.0.5/NoteBook/variable/variable.py
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      740 2023-06-17 18:22:28.832630 PythonNoteBook-0.0.5/PKG-INFO
+drwxr-xr-x   0 huangjiabao   (501) staff       (20)        0 2023-06-17 18:22:28.832451 PythonNoteBook-0.0.5/PythonNoteBook.egg-info/
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      740 2023-06-17 18:22:28.000000 PythonNoteBook-0.0.5/PythonNoteBook.egg-info/PKG-INFO
+-rw-r--r--   0 huangjiabao   (501) staff       (20)      328 2023-06-17 18:22:28.000000 PythonNoteBook-0.0.5/PythonNoteBook.egg-info/SOURCES.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        1 2023-06-17 18:22:28.000000 PythonNoteBook-0.0.5/PythonNoteBook.egg-info/dependency_links.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)        9 2023-06-17 18:22:28.000000 PythonNoteBook-0.0.5/PythonNoteBook.egg-info/top_level.txt
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       64 2023-06-17 18:20:30.000000 PythonNoteBook-0.0.5/README.md
+-rw-r--r--   0 huangjiabao   (501) staff       (20)       38 2023-06-17 18:22:28.832797 PythonNoteBook-0.0.5/setup.cfg
+-rw-r--r--   0 huangjiabao   (501) staff       (20)     3898 2023-06-17 18:20:38.000000 PythonNoteBook-0.0.5/setup.py
```

### Comparing `PythonNoteBook-0.0.4/LICENSE` & `PythonNoteBook-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonNoteBook-0.0.4/NoteBook/__version__.py` & `PythonNoteBook-0.0.5/NoteBook/__version__.py`

 * *Files identical despite different names*

### Comparing `PythonNoteBook-0.0.4/setup.py` & `PythonNoteBook-0.0.5/setup.py`

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
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

