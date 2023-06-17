# Comparing `tmp/RolexReserver-1.0.4.tar.gz` & `tmp/RolexReserver-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RolexReserver-1.0.4.tar", last modified: Tue Jun 13 13:01:54 2023, max compression
+gzip compressed data, was "RolexReserver-1.0.5.tar", last modified: Sat Jun 17 01:36:36 2023, max compression
```

## Comparing `RolexReserver-1.0.4.tar` & `RolexReserver-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.325291 RolexReserver-1.0.4/
--rw-rw-rw-   0        0        0      887 2023-06-13 13:01:54.325291 RolexReserver-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-05-09 13:04:12.000000 RolexReserver-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.300284 RolexReserver-1.0.4/RolexReserver/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.308289 RolexReserver-1.0.4/RolexReserver/Getter/
-drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.310288 RolexReserver-1.0.4/RolexReserver/Getter/Base/
--rw-rw-rw-   0        0        0     1417 2023-05-09 13:09:11.000000 RolexReserver-1.0.4/RolexReserver/Getter/Base/baseGetter.py
--rw-rw-rw-   0        0        0     7479 2023-06-13 13:00:37.000000 RolexReserver-1.0.4/RolexReserver/Getter/getter_rolexReserve.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.322292 RolexReserver-1.0.4/RolexReserver/Library/
--rw-rw-rw-   0        0        0     4820 2023-05-23 13:18:26.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverConfig.py
--rw-rw-rw-   0        0        0      704 2023-05-13 05:47:49.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverConfiger.py
--rw-rw-rw-   0        0        0     1538 2023-05-10 13:23:34.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverController.py
--rw-rw-rw-   0        0        0      164 2023-05-09 12:52:25.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverDeclare.py
--rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverException.py
--rw-rw-rw-   0        0        0      573 2023-05-09 13:01:02.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverGlobals.py
--rw-rw-rw-   0        0        0     4731 2023-05-09 13:01:02.000000 RolexReserver-1.0.4/RolexReserver/Library/rolexReserverMailer.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.323300 RolexReserver-1.0.4/RolexReserver/Models/
--rw-rw-rw-   0        0        0      669 2023-06-13 12:51:31.000000 RolexReserver-1.0.4/RolexReserver/Models/log_reserve.py
--rw-rw-rw-   0        0        0      261 2023-06-13 13:01:42.000000 RolexReserver-1.0.4/RolexReserver/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:01:54.306285 RolexReserver-1.0.4/RolexReserver.egg-info/
--rw-rw-rw-   0        0        0      887 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      784 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0      105 2023-06-13 13:01:54.000000 RolexReserver-1.0.4/RolexReserver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 13:01:54.326295 RolexReserver-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2523 2023-05-09 12:42:27.000000 RolexReserver-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 01:36:36.229146 RolexReserver-1.0.5/
+-rw-rw-rw-   0        0        0      887 2023-06-17 01:36:36.228142 RolexReserver-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-05-09 13:04:12.000000 RolexReserver-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 01:36:36.155604 RolexReserver-1.0.5/RolexReserver/
+drwxrwxrwx   0        0        0        0 2023-06-17 01:36:36.173133 RolexReserver-1.0.5/RolexReserver/Getter/
+drwxrwxrwx   0        0        0        0 2023-06-17 01:36:36.177145 RolexReserver-1.0.5/RolexReserver/Getter/Base/
+-rw-rw-rw-   0        0        0     1417 2023-05-09 13:09:11.000000 RolexReserver-1.0.5/RolexReserver/Getter/Base/baseGetter.py
+-rw-rw-rw-   0        0        0     7479 2023-06-13 13:08:49.000000 RolexReserver-1.0.5/RolexReserver/Getter/getter_rolexReserve.py
+drwxrwxrwx   0        0        0        0 2023-06-17 01:36:36.222148 RolexReserver-1.0.5/RolexReserver/Library/
+-rw-rw-rw-   0        0        0     4820 2023-05-23 13:18:26.000000 RolexReserver-1.0.5/RolexReserver/Library/rolexReserverConfig.py
+-rw-rw-rw-   0        0        0      704 2023-05-13 05:47:49.000000 RolexReserver-1.0.5/RolexReserver/Library/rolexReserverConfiger.py
+-rw-rw-rw-   0        0        0     1538 2023-05-10 13:23:34.000000 RolexReserver-1.0.5/RolexReserver/Library/rolexReserverController.py
+-rw-rw-rw-   0        0        0      164 2023-05-09 12:52:25.000000 RolexReserver-1.0.5/RolexReserver/Library/rolexReserverDeclare.py
+-rw-rw-rw-   0        0        0     2092 2023-01-06 13:54:01.000000 RolexReserver-1.0.5/RolexReserver/Library/rolexReserverException.py
+-rw-rw-rw-   0        0        0      573 2023-05-09 13:01:02.000000 RolexReserver-1.0.5/RolexReserver/Library/rolexReserverGlobals.py
+-rw-rw-rw-   0        0        0     4731 2023-05-09 13:01:02.000000 RolexReserver-1.0.5/RolexReserver/Library/rolexReserverMailer.py
+drwxrwxrwx   0        0        0        0 2023-06-17 01:36:36.224146 RolexReserver-1.0.5/RolexReserver/Models/
+-rw-rw-rw-   0        0        0      669 2023-06-13 13:08:49.000000 RolexReserver-1.0.5/RolexReserver/Models/log_reserve.py
+drwxrwxrwx   0        0        0        0 2023-06-17 01:36:36.227142 RolexReserver-1.0.5/RolexReserver/Register/
+-rw-rw-rw-   0        0        0      446 2023-06-13 13:08:49.000000 RolexReserver-1.0.5/RolexReserver/Register/register_LogReserve.py
+-rw-rw-rw-   0        0        0      261 2023-06-17 01:36:19.000000 RolexReserver-1.0.5/RolexReserver/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 01:36:36.171615 RolexReserver-1.0.5/RolexReserver.egg-info/
+-rw-rw-rw-   0        0        0      887 2023-06-17 01:36:35.000000 RolexReserver-1.0.5/RolexReserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-06-17 01:36:36.000000 RolexReserver-1.0.5/RolexReserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 01:36:35.000000 RolexReserver-1.0.5/RolexReserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      784 2023-06-17 01:36:35.000000 RolexReserver-1.0.5/RolexReserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      128 2023-06-17 01:36:36.000000 RolexReserver-1.0.5/RolexReserver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 01:36:36.230146 RolexReserver-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2618 2023-06-17 01:36:13.000000 RolexReserver-1.0.5/setup.py
```

### Comparing `RolexReserver-1.0.4/PKG-INFO` & `RolexReserver-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RolexReserver
-Version: 1.0.4
+Version: 1.0.5
 Summary: RolexReserver Package
 Home-page: https://github.com/kaioman/RolexReserver.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: RolexReserver
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RolexReserver-1.0.4/RolexReserver/Getter/Base/baseGetter.py` & `RolexReserver-1.0.5/RolexReserver/Getter/Base/baseGetter.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/RolexReserver/Getter/getter_rolexReserve.py` & `RolexReserver-1.0.5/RolexReserver/Getter/getter_rolexReserve.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverConfig.py` & `RolexReserver-1.0.5/RolexReserver/Library/rolexReserverConfig.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverConfiger.py` & `RolexReserver-1.0.5/RolexReserver/Library/rolexReserverConfiger.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverController.py` & `RolexReserver-1.0.5/RolexReserver/Library/rolexReserverController.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverException.py` & `RolexReserver-1.0.5/RolexReserver/Library/rolexReserverException.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverGlobals.py` & `RolexReserver-1.0.5/RolexReserver/Library/rolexReserverGlobals.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/RolexReserver/Library/rolexReserverMailer.py` & `RolexReserver-1.0.5/RolexReserver/Library/rolexReserverMailer.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/RolexReserver/Models/log_reserve.py` & `RolexReserver-1.0.5/RolexReserver/Models/log_reserve.py`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/RolexReserver.egg-info/PKG-INFO` & `RolexReserver-1.0.5/RolexReserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RolexReserver
-Version: 1.0.4
+Version: 1.0.5
 Summary: RolexReserver Package
 Home-page: https://github.com/kaioman/RolexReserver.git
 Author: unchainworks
 Author-email: kajin0318@gmail.com
 License: BSD-3-Clause
 Keywords: RolexReserver
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `RolexReserver-1.0.4/RolexReserver.egg-info/SOURCES.txt` & `RolexReserver-1.0.5/RolexReserver.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 RolexReserver/Library/rolexReserverConfig.py
 RolexReserver/Library/rolexReserverConfiger.py
 RolexReserver/Library/rolexReserverController.py
 RolexReserver/Library/rolexReserverDeclare.py
 RolexReserver/Library/rolexReserverException.py
 RolexReserver/Library/rolexReserverGlobals.py
 RolexReserver/Library/rolexReserverMailer.py
-RolexReserver/Models/log_reserve.py
+RolexReserver/Models/log_reserve.py
+RolexReserver/Register/register_LogReserve.py
```

### Comparing `RolexReserver-1.0.4/RolexReserver.egg-info/requires.txt` & `RolexReserver-1.0.5/RolexReserver.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `RolexReserver-1.0.4/setup.py` & `RolexReserver-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 
 package_name = 'RolexReserver'
 subPackage_name_getter = 'Getter'
 subPackage_name_getter_base = 'Getter/Base'
 subPackage_name_library = 'Library'
 subPackage_name_models = 'Models'
+subPackage_name_register = 'Register'
 
 root_dir = path.abspath(path.dirname(__file__))
 
 def _requirements():
     return [name.rstrip() for name in open(path.join(root_dir, 'requirements.txt')).readlines()]
 
 
@@ -40,14 +41,15 @@
     name=package_name,
     packages=[
         package_name + '/',
         package_name + '/' + subPackage_name_getter,
         package_name + '/' + subPackage_name_getter_base,
         package_name + '/' + subPackage_name_library,
         package_name + '/' + subPackage_name_models,
+        package_name + '/' + subPackage_name_register,
     ],
 
     version=version,
 
     license=license,
 
     install_requires=_requirements(),
```

