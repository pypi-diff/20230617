# Comparing `tmp/specialStr-0.0.1.tar.gz` & `tmp/specialStr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specialStr-0.0.1.tar", last modified: Sun Jun 11 12:00:02 2023, max compression
+gzip compressed data, was "specialStr-0.0.2.tar", last modified: Sat Jun 17 15:01:33 2023, max compression
```

## Comparing `specialStr-0.0.1.tar` & `specialStr-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 12:00:02.436352 specialStr-0.0.1/
--rw-rw-rw-   0        0        0      819 2023-06-11 12:00:02.435352 specialStr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      107 2023-06-11 10:43:10.000000 specialStr-0.0.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-11 12:00:02.436352 specialStr-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1041 2023-06-11 10:44:01.000000 specialStr-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 12:00:02.427352 specialStr-0.0.1/specialStr/
--rw-rw-rw-   0        0        0      537 2023-06-11 05:30:11.000000 specialStr-0.0.1/specialStr/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-06-11 11:58:30.000000 specialStr-0.0.1/specialStr/checker.py
--rw-rw-rw-   0        0        0     6266 2023-06-11 11:58:05.000000 specialStr-0.0.1/specialStr/main.py
-drwxrwxrwx   0        0        0        0 2023-06-11 12:00:02.434352 specialStr-0.0.1/specialStr.egg-info/
--rw-rw-rw-   0        0        0      819 2023-06-11 12:00:02.000000 specialStr-0.0.1/specialStr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-11 12:00:02.000000 specialStr-0.0.1/specialStr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 12:00:02.000000 specialStr-0.0.1/specialStr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-11 12:00:02.000000 specialStr-0.0.1/specialStr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-11 12:00:02.000000 specialStr-0.0.1/specialStr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 15:01:33.730479 specialStr-0.0.2/
+-rw-rw-rw-   0        0        0      819 2023-06-17 15:01:33.730479 specialStr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2023-06-11 10:43:10.000000 specialStr-0.0.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-17 15:01:33.730479 specialStr-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1041 2023-06-17 15:01:27.000000 specialStr-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:01:33.720478 specialStr-0.0.2/specialStr/
+-rw-rw-rw-   0        0        0      537 2023-06-11 05:30:11.000000 specialStr-0.0.2/specialStr/__init__.py
+-rw-rw-rw-   0        0        0     1924 2023-06-17 15:01:09.000000 specialStr-0.0.2/specialStr/checker.py
+-rw-rw-rw-   0        0        0     6266 2023-06-11 11:58:05.000000 specialStr-0.0.2/specialStr/main.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:01:33.728480 specialStr-0.0.2/specialStr.egg-info/
+-rw-rw-rw-   0        0        0      819 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-17 15:01:33.000000 specialStr-0.0.2/specialStr.egg-info/top_level.txt
```

### Comparing `specialStr-0.0.1/PKG-INFO` & `specialStr-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialStr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Manage strings more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: string
 Platform: windows
```

### Comparing `specialStr-0.0.1/setup.py` & `specialStr-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'specialStr',
-    version = '0.0.1',
+    version = '0.0.2',
     keywords = ['string'],
     description = 'Manage strings more easily',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
```

### Comparing `specialStr-0.0.1/specialStr/__init__.py` & `specialStr-0.0.2/specialStr/__init__.py`

 * *Files identical despite different names*

### Comparing `specialStr-0.0.1/specialStr/checker.py` & `specialStr-0.0.2/specialStr/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from typing import List,Dict,Tuple
 __all__=["UrlChecker","PathChecker","EmailChecker","Checker"]
 class Checker(object):
     tester=[] #type: List[re.Pattern]
     finder={} #type: Dict[Tuple[str,...],re.Pattern]
     
 class UrlChecker(Checker):
-    tester=[re.compile(r"^[^/\\\.&\?\#]*://(?:[^/\\\.&\?\#]+\.)+[^/\\\.&\?\#]+(?::[0-9]+)?(?:(?:/[^/\\\.&\?\#]+)*/?)(?:\?(?:(?:[^/\\\.&\?\#]+=[^/\\\.&\?\#]*)&?)+)?(?:#[^&\?\#]*)?$")]
+    tester=[re.compile(r"^[^/\\\.&\?\#]*://(?:[^/\\\.&\?\#]+\.)+[^/\\\.&\?\#]+(?::[0-9]+)?(?:(?:/[^/\\&\?\#]+)*/?)(?:\?(?:(?:[^/\\\.&\?\#]+=[^/\\\.&\?\#]*)&?)+)?(?:#[^&\?\#]*)?$")]
     finder={
         (
             "scheme","domain","port","path","paramstr","anchor"
-        ):re.compile(r"^([^/\\\.&\?\#]*)://((?:[^/\\\.&\?\#]+\.)+[^/\\\.&\?\#]+)((?::[0-9]+)?)((?:(?:/[^/\\\.&\?\#]+)*/?))((?:\?(?:(?:[^/\\\.&\?\#]+=[^/\\\.&\?\#]*)&?)+)?)((?:#[^&\?\#]*)?)$")
+        ):re.compile(r"^([^/\\\.&\?\#]*)://((?:[^/\\\.&\?\#]+\.)+[^/\\\.&\?\#]+)((?::[0-9]+)?)((?:(?:/[^/\\&\?\#]+)*/?))((?:\?(?:(?:[^/\\\.&\?\#]+=[^/\\\.&\?\#]*)&?)+)?)((?:#[^&\?\#]*)?)$")
     }
     
 class PathChecker(Checker):
     tester=[re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)/(?:[^/\\\*\?]+/?)*$")]
     driverFinder=re.compile(r"^((?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+))/(?:[^/\\\*\?]+/?)*$")
     pathFinder=re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)(/(?:[^/\\\*\?]+/?)*)$")
     finder={
```

### Comparing `specialStr-0.0.1/specialStr/main.py` & `specialStr-0.0.2/specialStr/main.py`

 * *Files identical despite different names*

### Comparing `specialStr-0.0.1/specialStr.egg-info/PKG-INFO` & `specialStr-0.0.2/specialStr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialStr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Manage strings more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: string
 Platform: windows
```

