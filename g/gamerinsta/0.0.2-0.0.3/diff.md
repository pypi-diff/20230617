# Comparing `tmp/gamerinsta-0.0.2.tar.gz` & `tmp/gamerinsta-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamerinsta-0.0.2.tar", last modified: Tue Jun  6 11:49:47 2023, max compression
+gzip compressed data, was "gamerinsta-0.0.3.tar", last modified: Sat Jun 17 10:46:42 2023, max compression
```

## Comparing `gamerinsta-0.0.2.tar` & `gamerinsta-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 11:49:47.912848 gamerinsta-0.0.2/
--rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 gamerinsta-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      617 2023-06-06 11:49:47.912848 gamerinsta-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 11:49:47.897228 gamerinsta-0.0.2/gamerinsta/
--rw-rw-rw-   0        0        0     6962 2023-06-06 11:15:20.000000 gamerinsta-0.0.2/gamerinsta/__init__.py
--rw-rw-rw-   0        0        0     6247 2023-06-06 11:07:28.000000 gamerinsta-0.0.2/gamerinsta/tokens.py
-drwxrwxrwx   0        0        0        0 2023-06-06 11:49:47.912848 gamerinsta-0.0.2/gamerinsta.egg-info/
--rw-rw-rw-   0        0        0      617 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 11:49:47.000000 gamerinsta-0.0.2/gamerinsta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 11:49:47.912848 gamerinsta-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      918 2023-06-06 11:07:28.000000 gamerinsta-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 10:46:42.855710 gamerinsta-0.0.3/
+-rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 gamerinsta-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      617 2023-06-17 10:46:42.855710 gamerinsta-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 10:46:42.792712 gamerinsta-0.0.3/gamerinsta/
+-rw-rw-rw-   0        0        0    11036 2023-06-17 10:43:23.000000 gamerinsta-0.0.3/gamerinsta/__init__.py
+-rw-rw-rw-   0        0        0     6436 2023-06-17 10:28:19.000000 gamerinsta-0.0.3/gamerinsta/tokens.py
+drwxrwxrwx   0        0        0        0 2023-06-17 10:46:42.855710 gamerinsta-0.0.3/gamerinsta.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-17 10:46:42.000000 gamerinsta-0.0.3/gamerinsta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 10:46:42.855710 gamerinsta-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      918 2023-06-17 10:43:23.000000 gamerinsta-0.0.3/setup.py
```

### Comparing `gamerinsta-0.0.2/LICENSE` & `gamerinsta-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gamerinsta-0.0.2/PKG-INFO` & `gamerinsta-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamerinsta
-Version: 0.0.2
+Version: 0.0.3
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamerinsta-0.0.2/gamerinsta/tokens.py` & `gamerinsta-0.0.3/gamerinsta/tokens.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,20 +100,28 @@
                 'Ig-Intended-User-Id': str(self.UserId),
                 'Host': 'b.i.instagram.com',
 
             }
             headers = {key: updict.get(key, self.headers[key]) for key in self.headers}
             response = httpx.post('https://b.i.instagram.com/api/v1/zr/dual_tokens/', headers=self.headers,
                                      data=data)
-            self.claim = response.headers['x-ig-set-www-claim']
-            self.shbid = response.headers['ig-set-ig-u-shbid']
-            self.igid = self.shbid.split(',')[0]
-            self.shbi=self.shbid.split(':')[1]
-            self.shbts = response.headers['ig-set-ig-u-shbts']
             self.urur = response.headers['ig-set-ig-u-rur'].split(':')[1]
+            self.claim = response.headers['x-ig-set-www-claim']
+            try:
+                self.shbid = response.headers['ig-set-ig-u-shbid']
+                self.igid = self.shbid.split(',')[0]
+                self.shbi=self.shbid.split(':')[1]
+                self.shbts = response.headers['ig-set-ig-u-shbts']
+            except:
+                self.shbid=None
+                self.igid=None
+                self.shbi=None
+                self.shbts=None
+
+
 
             return self.claim,self.shbi,self.igid,self.shbts,self.urur
         except Exception as e:
             print(e)
             Tokens.Cooki2(self)
```

### Comparing `gamerinsta-0.0.2/gamerinsta.egg-info/PKG-INFO` & `gamerinsta-0.0.3/gamerinsta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamerinsta
-Version: 0.0.2
+Version: 0.0.3
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamerinsta-0.0.2/setup.py` & `gamerinsta-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Instagram Android Api For Login '
 LONG_DESCRIPTION = 'A python library that helps you to login in instagram do various task and automaiton'
 
 # Setting up
 setup(
     name="gamerinsta",
     version=VERSION,
```

