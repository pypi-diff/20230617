# Comparing `tmp/phub-2.2.tar.gz` & `tmp/phub-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-2.2.tar", last modified: Tue Jun 13 07:52:50 2023, max compression
+gzip compressed data, was "phub-2.3.tar", last modified: Sat Jun 17 09:53:43 2023, max compression
```

## Comparing `phub-2.2.tar` & `phub-2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:50.160314 phub-2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 07:52:40.000000 phub-2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-13 07:52:50.160314 phub-2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-13 07:52:40.000000 phub-2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 07:52:40.000000 phub-2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 07:52:50.160314 phub-2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-13 07:52:40.000000 phub-2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:50.156314 phub-2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:50.160314 phub-2.2/src/phub/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 07:52:40.000000 phub-2.2/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17284 2023-06-13 07:52:40.000000 phub-2.2/src/phub/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-13 07:52:40.000000 phub-2.2/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-06-13 07:52:40.000000 phub-2.2/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-13 07:52:40.000000 phub-2.2/src/phub/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-13 07:52:40.000000 phub-2.2/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:52:50.160314 phub-2.2/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 07:52:50.000000 phub-2.2/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:53:43.305211 phub-2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 09:53:33.000000 phub-2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-17 09:53:43.305211 phub-2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-17 09:53:33.000000 phub-2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-17 09:53:33.000000 phub-2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 09:53:43.305211 phub-2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-17 09:53:33.000000 phub-2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:53:43.305211 phub-2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:53:43.305211 phub-2.3/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-17 09:53:33.000000 phub-2.3/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17284 2023-06-17 09:53:33.000000 phub-2.3/src/phub/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-17 09:53:33.000000 phub-2.3/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-17 09:53:33.000000 phub-2.3/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-17 09:53:33.000000 phub-2.3/src/phub/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-06-17 09:53:33.000000 phub-2.3/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 09:53:43.305211 phub-2.3/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-17 09:53:43.000000 phub-2.3/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-17 09:53:43.000000 phub-2.3/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 09:53:43.000000 phub-2.3/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-17 09:53:43.000000 phub-2.3/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-17 09:53:43.000000 phub-2.3/src/phub.egg-info/top_level.txt
```

### Comparing `phub-2.2/LICENSE` & `phub-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-2.2/PKG-INFO` & `phub-2.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.2
+Version: 2.3
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
@@ -16,17 +16,19 @@
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PHUB](https://github.com/Egsagon/PHUB/blob/master/assets/banner.png)
 
-# PHUB - An API for `pornhub.com`.
+# PHUB - An API for PornHub.
 PHUB is an API wrapper for PornHub. It is able to fetch, search and download videos and supports account connections, achieved with efficient web scrapping using requests and regexes.
 
+> :warning: **Early development: bugs may occur** (also i'm a terrible programer)
+
 ## Installation
 - Install using pip:
 ```sh
 pip install --upgrade phub
 ```
 
 - Or using this repository to get latest features:
@@ -52,13 +54,11 @@
 
 # Display all videos (careful if there is a lot of results)
 for video in record:
   print(video.title)
 ```
 
 ## Documentation
-TODO
+See the [wiki](https://github.com/Egsagon/PHUB/wiki).
 
 ## Why?
 This project was made as an enhancement for [pfetch](https://github.com/Egsagon/pornhub-fetch), which aimed at downloading videos from PornHub.
-
-I do not plan to maintain this much, so if there are any errors clone the repository and update the regexes in `src/phub/consts` in the `regexes` class.
```

### Comparing `phub-2.2/README.md` & `phub-2.3/src/phub.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,34 @@
+Metadata-Version: 2.1
+Name: phub
+Version: 2.3
+Summary: An API for PornHub
+Home-page: https://github.com/Egsagon/PHUB/
+Author: Egsagon
+Author-email: egsagon12@gmail.com
+License: GPLv3
+Platform: unix
+Platform: linux
+Platform: win32
+Platform: cygwin
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Education
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![PHUB](https://github.com/Egsagon/PHUB/blob/master/assets/banner.png)
 
-# PHUB - An API for `pornhub.com`.
+# PHUB - An API for PornHub.
 PHUB is an API wrapper for PornHub. It is able to fetch, search and download videos and supports account connections, achieved with efficient web scrapping using requests and regexes.
 
+> :warning: **Early development: bugs may occur** (also i'm a terrible programer)
+
 ## Installation
 - Install using pip:
 ```sh
 pip install --upgrade phub
 ```
 
 - Or using this repository to get latest features:
@@ -32,13 +54,11 @@
 
 # Display all videos (careful if there is a lot of results)
 for video in record:
   print(video.title)
 ```
 
 ## Documentation
-TODO
+See the [wiki](https://github.com/Egsagon/PHUB/wiki).
 
 ## Why?
 This project was made as an enhancement for [pfetch](https://github.com/Egsagon/pornhub-fetch), which aimed at downloading videos from PornHub.
-
-I do not plan to maintain this much, so if there are any errors clone the repository and update the regexes in `src/phub/consts` in the `regexes` class.
```

### Comparing `phub-2.2/setup.cfg` & `phub-2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phub
-version = 2.2
+version = 2.3
 description = An API for PornHub
 author = Egsagon
 author_email = egsagon12@gmail.com
 url = https://github.com/Egsagon/PHUB/
 license = GPLv3
 license_file = LICENSE
 long_description = file: README.md
```

### Comparing `phub-2.2/src/phub/__init__.py` & `phub-2.3/src/phub/__init__.py`

 * *Files identical despite different names*

### Comparing `phub-2.2/src/phub/classes.py` & `phub-2.3/src/phub/classes.py`

 * *Files identical despite different names*

### Comparing `phub-2.2/src/phub/consts.py` & `phub-2.3/src/phub/consts.py`

 * *Files identical despite different names*

### Comparing `phub-2.2/src/phub/core.py` & `phub-2.3/src/phub/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,35 +90,38 @@
     Represents a Client capable of interacting with PornHub.
     '''
     
     def __init__(self,
                  username: str = None,
                  password: str = None,
                  session: requests.Session = None,
+                 language: str = 'en,en-US',
                  autologin: bool = False) -> None:
         '''
         #### Initialise a new client. #####
         -----------------------------------
         
         Arguments
-        - `username`   (=`None`) -- Account to connect to username.
-        - `password`   (=`None`) -- Account to connect to password.
-        - `session`    (=`None`) -- Recovery requests session.
-        - `autologin` (=`False`) -- Whether to login after initialisation.
+        - `username`     (=`None`) -- Account to connect to username.
+        - `password`     (=`None`) -- Account to connect to password.
+        - `session`      (=`None`) -- Recovery requests session.
+        - `language` (=`en,en-US`) -- Language of the client session.
+        - `autologin`   (=`False`) -- Whether to login after initialisation.
         
         -----------------------------------
         Returns a `Client` object.
         '''
         
         # Initialise session
         self.session = session or requests.Session()
         self.session.cookies.set('accessAgeDisclaimerPH', '1')
         
         self.creds = {'username': username, 'password': password}
         self._intents_to_login = bool(username)
+        self.language = {'Accept-Language': language}
         
         # Connect Account object
         self.account: Account | None = Account(self)
         
         # Autologin
         self.logged = False
         if autologin: self.login()
@@ -198,15 +201,15 @@
               if simple_url else func
         
         log('client', f'Sending request at {utils.shortify(url, 25)}', level = 6)
         
         response = self.session.request(
             method = method,
             url = url,
-            headers = consts.HEADERS | headers,
+            headers = consts.HEADERS | headers | self.language,
             data = data
         )
         
         log('client', 'Request passed with status', response.status_code, level = 6)
         
         if throw and not response.ok:
             raise ConnectionError(f'Request `{func}` failed:' + \
```

### Comparing `phub-2.2/src/phub/parser.py` & `phub-2.3/src/phub/parser.py`

 * *Files identical despite different names*

### Comparing `phub-2.2/src/phub/utils.py` & `phub-2.3/src/phub/utils.py`

 * *Files identical despite different names*

