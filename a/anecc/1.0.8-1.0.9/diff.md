# Comparing `tmp/anecc-1.0.8-py3.11.egg` & `tmp/anecc-1.0.9-py3.11.egg`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 16791 bytes, number of entries: 13
--rw-r--r--  2.0 unx      118 b- defN 23-Jun-17 17:39 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      215 b- defN 23-Jun-17 17:39 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-17 17:39 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       40 b- defN 23-Jun-17 17:39 EGG-INFO/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-17 17:39 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Jun-17 17:39 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-17 17:39 EGG-INFO/zip-safe
--rw-r--r--  2.0 unx     9581 b- defN 23-Jun-17 17:39 anecc/__init__.py
+Zip file size: 16792 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      118 b- defN 23-Jun-17 17:42 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      215 b- defN 23-Jun-17 17:42 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-17 17:42 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-17 17:42 EGG-INFO/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-17 17:42 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-17 17:42 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-17 17:42 EGG-INFO/zip-safe
+-rw-r--r--  2.0 unx     9581 b- defN 23-Jun-17 17:40 anecc/__init__.py
 -rw-r--r--  2.0 unx      841 b- defN 23-Jun-17 17:30 anecc/anect_run.py
--rw-r--r--  2.0 unx      844 b- defN 23-Jun-17 17:36 anecc/run.py
--rw-r--r--  2.0 unx    19791 b- defN 23-Jun-17 17:39 anecc/__pycache__/__init__.cpython-311.pyc
--rw-r--r--  2.0 unx     1593 b- defN 23-Jun-17 17:39 anecc/__pycache__/anect_run.cpython-311.pyc
--rw-r--r--  2.0 unx     1593 b- defN 23-Jun-17 17:39 anecc/__pycache__/run.cpython-311.pyc
-13 files, 34640 bytes uncompressed, 15141 bytes compressed:  56.3%
+-rw-r--r--  2.0 unx      844 b- defN 23-Jun-17 17:40 anecc/run.py
+-rw-r--r--  2.0 unx    19791 b- defN 23-Jun-17 17:42 anecc/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--  2.0 unx     1593 b- defN 23-Jun-17 17:42 anecc/__pycache__/anect_run.cpython-311.pyc
+-rw-r--r--  2.0 unx     1593 b- defN 23-Jun-17 17:42 anecc/__pycache__/run.cpython-311.pyc
+13 files, 34640 bytes uncompressed, 15142 bytes compressed:  56.3%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,6 +1,6 @@
 Metadata-Version: 2.1
 Name: anecc
-Version: 1.0.8
+Version: 1.0.9
 Summary: ANE converter
 Author: Eileen Yoon
 Author-email: eyn@gmx.com
```

## anecc/__pycache__/__init__.cpython-311.pyc

### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x34718d64 (Sat Jun 17 08:39:16 2023 UTC)
+moddate:  0x6a718d64 (Sat Jun 17 08:40:10 2023 UTC)
 files sz: 9581
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 15
    flags     : 0
    code
```

## anecc/__pycache__/run.cpython-311.pyc

### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xa8708d64 (Sat Jun 17 08:36:56 2023 UTC)
+moddate:  0x6a718d64 (Sat Jun 17 08:40:10 2023 UTC)
 files sz: 844
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 13
    flags     : 0
    code
```

