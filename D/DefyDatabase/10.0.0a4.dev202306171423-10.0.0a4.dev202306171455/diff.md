# Comparing `tmp/DefyDatabase-10.0.0a4.dev202306171423.tar.gz` & `tmp/DefyDatabase-10.0.0a4.dev202306171455.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DefyDatabase-10.0.0a4.dev202306171423.tar", last modified: Sat Jun 17 06:44:02 2023, max compression
+gzip compressed data, was "DefyDatabase-10.0.0a4.dev202306171455.tar", last modified: Sat Jun 17 06:55:14 2023, max compression
```

## Comparing `DefyDatabase-10.0.0a4.dev202306171423.tar` & `DefyDatabase-10.0.0a4.dev202306171455.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 06:44:02.665207 DefyDatabase-10.0.0a4.dev202306171423/
-drwxrwxrwx   0        0        0        0 2023-06-17 06:44:02.663364 DefyDatabase-10.0.0a4.dev202306171423/DefyDatabase.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-17 06:44:02.000000 DefyDatabase-10.0.0a4.dev202306171423/DefyDatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-06-17 06:44:02.000000 DefyDatabase-10.0.0a4.dev202306171423/DefyDatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 06:44:02.000000 DefyDatabase-10.0.0a4.dev202306171423/DefyDatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-17 06:44:02.000000 DefyDatabase-10.0.0a4.dev202306171423/DefyDatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      567 2023-06-17 06:44:02.665207 DefyDatabase-10.0.0a4.dev202306171423/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202306171423/README.md
--rw-rw-rw-   0        0        0     5605 2023-06-17 06:26:30.000000 DefyDatabase-10.0.0a4.dev202306171423/defy.py
--rw-rw-rw-   0        0        0       42 2023-06-17 06:44:02.666209 DefyDatabase-10.0.0a4.dev202306171423/setup.cfg
--rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a4.dev202306171423/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:55:14.767928 DefyDatabase-10.0.0a4.dev202306171455/
+drwxrwxrwx   0        0        0        0 2023-06-17 06:55:14.765924 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-17 06:55:14.000000 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-06-17 06:55:14.000000 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 06:55:14.000000 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-17 06:55:14.000000 DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      567 2023-06-17 06:55:14.767928 DefyDatabase-10.0.0a4.dev202306171455/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-06-10 10:00:40.000000 DefyDatabase-10.0.0a4.dev202306171455/README.md
+-rw-rw-rw-   0        0        0     5625 2023-06-17 06:53:04.000000 DefyDatabase-10.0.0a4.dev202306171455/defy.py
+-rw-rw-rw-   0        0        0       42 2023-06-17 06:55:14.767928 DefyDatabase-10.0.0a4.dev202306171455/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-06-10 11:32:14.000000 DefyDatabase-10.0.0a4.dev202306171455/setup.py
```

### Comparing `DefyDatabase-10.0.0a4.dev202306171423/DefyDatabase.egg-info/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202306171455/DefyDatabase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202306171423
+Version: 10.0.0a4.dev202306171455
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202306171423/PKG-INFO` & `DefyDatabase-10.0.0a4.dev202306171455/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DefyDatabase
-Version: 10.0.0a4.dev202306171423
+Version: 10.0.0a4.dev202306171455
 Summary: Database for personal data based on SQLite
 Author: Defymen
 Author-email: vmuonline@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DefyDatabase-10.0.0a4.dev202306171423/defy.py` & `DefyDatabase-10.0.0a4.dev202306171455/defy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #Rules are meant to break by proudest ones.
 '''
 这是亮天计划的数据库官方API。
 '''
 import sqlite3,sys,os,datetime,io
 
 tor='DefyDatabase'
-version='10.0.0a4.dev202306171423'
+version='10.0.0a4.dev202306171455'
 
 commands=[
     'SELECT COUNT(*) FROM LIGHTSKY',
     'SELECT UID,BIND FROM BIND WHERE UID = "{}"',
     'SELECT UID, GRADE, JOB ,ABOUT FROM LIGHTSKY WHERE UID = "{}"',
     'SELECT UID, GRADE, JOB ,ABOUT from LIGHTSKY WHERE rowid={}',
     'SELECT COUNT(*) FROM BIND',
@@ -56,15 +56,17 @@
         self.code=code
     def __repr__(self):
         return str(self.code)
     def __eq__(self,value,/):
         return self.code==value
     def __int__(self):
         return self.code
-    
+
+KEEP=DefyStatus(280)
+
 #数据库管理对象。
 class __DefyProject(io.IOBase):   
     def __reset(self):
         self.__con=sqlite3.connect(self.__file)
         self.__cur=self.__con.cursor()
         self.__fro=0
```

### Comparing `DefyDatabase-10.0.0a4.dev202306171423/setup.py` & `DefyDatabase-10.0.0a4.dev202306171455/setup.py`

 * *Files identical despite different names*

