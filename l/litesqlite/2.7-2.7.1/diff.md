# Comparing `tmp/litesqlite-2.7.tar.gz` & `tmp/litesqlite-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litesqlite-2.7.tar", last modified: Wed Jun 14 17:30:07 2023, max compression
+gzip compressed data, was "litesqlite-2.7.1.tar", last modified: Sat Jun 17 15:18:49 2023, max compression
```

## Comparing `litesqlite-2.7.tar` & `litesqlite-2.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 17:30:07.731193 litesqlite-2.7/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.7/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      626 2023-06-14 17:30:07.731193 litesqlite-2.7/PKG-INFO
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1735 2023-06-14 17:26:48.000000 litesqlite-2.7/README.md
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 17:30:07.727193 litesqlite-2.7/litesqlite/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.7/litesqlite/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.7/litesqlite/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8905 2023-06-14 17:06:04.000000 litesqlite-2.7/litesqlite/lite_sqlite.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-14 17:30:07.731193 litesqlite-2.7/litesqlite.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      626 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-14 17:30:07.000000 litesqlite-2.7/litesqlite.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-14 17:30:07.731193 litesqlite-2.7/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      780 2023-06-14 17:29:45.000000 litesqlite-2.7/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-17 15:18:49.052738 litesqlite-2.7.1/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 litesqlite-2.7.1/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-17 15:18:49.048738 litesqlite-2.7.1/PKG-INFO
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     1735 2023-06-14 17:26:48.000000 litesqlite-2.7.1/README.md
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-17 15:18:49.048738 litesqlite-2.7.1/litesqlite/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      100 2023-06-10 21:17:16.000000 litesqlite-2.7.1/litesqlite/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     4330 2023-06-11 17:09:48.000000 litesqlite-2.7.1/litesqlite/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     8985 2023-06-17 15:16:56.000000 litesqlite-2.7.1/litesqlite/lite_sqlite.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-17 15:18:49.048738 litesqlite-2.7.1/litesqlite.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      628 2023-06-17 15:18:48.000000 litesqlite-2.7.1/litesqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      268 2023-06-17 15:18:48.000000 litesqlite-2.7.1/litesqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-17 15:18:48.000000 litesqlite-2.7.1/litesqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-17 15:18:48.000000 litesqlite-2.7.1/litesqlite.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       11 2023-06-17 15:18:48.000000 litesqlite-2.7.1/litesqlite.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-17 15:18:49.052738 litesqlite-2.7.1/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      782 2023-06-17 15:16:56.000000 litesqlite-2.7.1/setup.py
```

### Comparing `litesqlite-2.7/LICENSE` & `litesqlite-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `litesqlite-2.7/PKG-INFO` & `litesqlite-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.7
+Version: 2.7.1
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.7/README.md` & `litesqlite-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `litesqlite-2.7/litesqlite/datatypes.py` & `litesqlite-2.7.1/litesqlite/datatypes.py`

 * *Files identical despite different names*

### Comparing `litesqlite-2.7/litesqlite/lite_sqlite.py` & `litesqlite-2.7.1/litesqlite/lite_sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,17 @@
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
     def open_conn(self) -> None:
-        self.__conn = sqlite3.connect(self.__db_name)
-        self.__cursor = self.__conn.cursor()
+        if self.__conn is None:
+            self.__conn = sqlite3.connect(self.__db_name)
+            self.__cursor = self.__conn.cursor()
 
     def __enter__(self) -> 'Sqlite':
         self.open_conn()
         return self
 
     def create_table(self,
                      table_name: str,
@@ -118,16 +119,17 @@
     def __init__(self,
                  db_name: str) -> None:
         self.__db_name = db_name
         self.__conn = None
         self.__cursor = None
 
     async def open_conn(self) -> None:
-        self.__conn = await aiosqlite.connect(self.__db_name)
-        self.__cursor = await self.__conn.cursor()
+        if self.__conn is None:
+            self.__conn = await aiosqlite.connect(self.__db_name)
+            self.__cursor = await self.__conn.cursor()
 
     async def __aenter__(self) -> 'AioSqlite':
         await self.open_conn()
         return self
 
     async def create_table(self,
                            table_name: str,
```

### Comparing `litesqlite-2.7/litesqlite.egg-info/PKG-INFO` & `litesqlite-2.7.1/litesqlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litesqlite
-Version: 2.7
+Version: 2.7.1
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/FREVOD/litesqlite
 Author: FREVOD
 Author-email: frevod_dev@mail.ru
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `litesqlite-2.7/setup.py` & `litesqlite-2.7.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='litesqlite',
-    version='2.7',
+    version='2.7.1',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/FREVOD/litesqlite',
     author='FREVOD',
     author_email='frevod_dev@mail.ru',
     license='GPLv3',
     packages=['litesqlite'],
     install_requires=[
```

