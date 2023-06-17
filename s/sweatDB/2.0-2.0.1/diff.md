# Comparing `tmp/sweatDB-2.0.tar.gz` & `tmp/sweatDB-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweatDB-2.0.tar", last modified: Sat Jun 17 13:44:43 2023, max compression
+gzip compressed data, was "sweatDB-2.0.1.tar", last modified: Sat Jun 17 13:56:30 2023, max compression
```

## Comparing `sweatDB-2.0.tar` & `sweatDB-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-17 13:44:43.713583 sweatDB-2.0/
--rw-r--r--   0 sweat     (1000) sweat     (1000)      284 2023-06-17 13:44:43.709583 sweatDB-2.0/PKG-INFO
--rw-r--r--   0 sweat     (1000) sweat     (1000)       81 2023-06-17 12:33:57.000000 sweatDB-2.0/pyproject.toml
--rw-r--r--   0 sweat     (1000) sweat     (1000)       38 2023-06-17 13:44:43.713583 sweatDB-2.0/setup.cfg
--rw-r--r--   0 sweat     (1000) sweat     (1000)      533 2023-06-17 13:43:58.000000 sweatDB-2.0/setup.py
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-17 13:44:43.709583 sweatDB-2.0/sweatDB/
--rw-r--r--   0 sweat     (1000) sweat     (1000)     2680 2023-06-17 13:41:44.000000 sweatDB-2.0/sweatDB/__init__.py
--rw-r--r--   0 sweat     (1000) sweat     (1000)     2249 2023-06-17 12:39:49.000000 sweatDB-2.0/sweatDB/sweatDB.py
-drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-17 13:44:43.709583 sweatDB-2.0/sweatDB.egg-info/
--rw-r--r--   0 sweat     (1000) sweat     (1000)      284 2023-06-17 13:44:43.000000 sweatDB-2.0/sweatDB.egg-info/PKG-INFO
--rw-r--r--   0 sweat     (1000) sweat     (1000)      186 2023-06-17 13:44:43.000000 sweatDB-2.0/sweatDB.egg-info/SOURCES.txt
--rw-r--r--   0 sweat     (1000) sweat     (1000)        1 2023-06-17 13:44:43.000000 sweatDB-2.0/sweatDB.egg-info/dependency_links.txt
--rw-r--r--   0 sweat     (1000) sweat     (1000)        8 2023-06-17 13:44:43.000000 sweatDB-2.0/sweatDB.egg-info/top_level.txt
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-17 13:56:30.137601 sweatDB-2.0.1/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-17 13:56:30.137601 sweatDB-2.0.1/PKG-INFO
+-rw-r--r--   0 sweat     (1000) sweat     (1000)       81 2023-06-17 12:33:57.000000 sweatDB-2.0.1/pyproject.toml
+-rw-r--r--   0 sweat     (1000) sweat     (1000)       38 2023-06-17 13:56:30.137601 sweatDB-2.0.1/setup.cfg
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      535 2023-06-17 13:55:57.000000 sweatDB-2.0.1/setup.py
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-17 13:56:30.137601 sweatDB-2.0.1/sweatDB/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)     2694 2023-06-17 13:54:20.000000 sweatDB-2.0.1/sweatDB/__init__.py
+-rw-r--r--   0 sweat     (1000) sweat     (1000)     2249 2023-06-17 12:39:49.000000 sweatDB-2.0.1/sweatDB/sweatDB.py
+drwxr-xr-x   0 sweat     (1000) sweat     (1000)        0 2023-06-17 13:56:30.137601 sweatDB-2.0.1/sweatDB.egg-info/
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      286 2023-06-17 13:56:30.000000 sweatDB-2.0.1/sweatDB.egg-info/PKG-INFO
+-rw-r--r--   0 sweat     (1000) sweat     (1000)      186 2023-06-17 13:56:30.000000 sweatDB-2.0.1/sweatDB.egg-info/SOURCES.txt
+-rw-r--r--   0 sweat     (1000) sweat     (1000)        1 2023-06-17 13:56:30.000000 sweatDB-2.0.1/sweatDB.egg-info/dependency_links.txt
+-rw-r--r--   0 sweat     (1000) sweat     (1000)        8 2023-06-17 13:56:30.000000 sweatDB-2.0.1/sweatDB.egg-info/top_level.txt
```

### Comparing `sweatDB-2.0/setup.py` & `sweatDB-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup(
     name="sweatDB",
-    version='2.0',
+    version='2.0.1',
     author="0xsweat",
     author_email="<0x.sweat@tutanota.com>",
     description='A python3 DBMS',
     long_description_content_type="text/markdown",
     long_description='A database management system with an easier syntax than SQL',
     packages=find_packages(),
     install_requires=[],
```

### Comparing `sweatDB-2.0/sweatDB/__init__.py` & `sweatDB-2.0.1/sweatDB/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import datetime
 import os
-version = "v1.0"
+version = "v2.0"
 e = os.path.isfile
 
 class actions :
     
     # Create a database.
     
     def create(db):
         if e(db):
             raise Exception(f"{db} already exists")
         else:
             open(db,'w').write(f"DATABASE NAME : {db} TIME CREATED : {datetime.datetime.utcnow()} CREATED WITH https://pypi.org/project/sweatDB/ {version}\n")
     
     # Delete an item or database.
     
-    def delete(ttd,db,item=''):
-        if e(name) != True:
+    def delete(db,delete_type,item=''):
+        if e(db) != True:
             return f"Database : {name} doesn't exist"
-        if ttd == "db":
+        if delete_type == "db":
             os.remove(db)
         elif item == '':
             raise Exception('No item specified')
             a = open(db, 'r').read().split("\n")
             open(db, 'w').write("".join([f"{x}\n" for x in a if x.startswith(f'{item} ') == False])[:-1])
 
     # Add an item to a database.
```

### Comparing `sweatDB-2.0/sweatDB/sweatDB.py` & `sweatDB-2.0.1/sweatDB/sweatDB.py`

 * *Files identical despite different names*

