# Comparing `tmp/pywalc-1.0.1.tar.gz` & `tmp/pywalc-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywalc-1.0.1.tar", last modified: Sat Jun 17 14:14:43 2023, max compression
+gzip compressed data, was "pywalc-1.0.2.tar", last modified: Sat Jun 17 14:46:10 2023, max compression
```

## Comparing `pywalc-1.0.1.tar` & `pywalc-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,44 @@
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:14:43.193445 pywalc-1.0.1/
--rw-r--r--   0 png       (1000) png261    (1000)     1070 2023-06-16 14:10:31.000000 pywalc-1.0.1/LICENSE
--rw-r--r--   0 png       (1000) png261    (1000)      110 2023-06-17 07:59:06.000000 pywalc-1.0.1/MANIFEST.in
--rw-r--r--   0 png       (1000) png261    (1000)     1567 2023-06-17 14:14:43.193445 pywalc-1.0.1/PKG-INFO
--rw-r--r--   0 png       (1000) png261    (1000)      901 2023-06-16 14:10:31.000000 pywalc-1.0.1/README.md
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:14:43.193445 pywalc-1.0.1/pywalc/
--rw-r--r--   0 png       (1000) png261    (1000)      267 2023-06-17 06:25:24.000000 pywalc-1.0.1/pywalc/__init__.py
--rw-r--r--   0 png       (1000) png261    (1000)      361 2023-06-17 08:33:01.000000 pywalc-1.0.1/pywalc/__main__.py
--rw-r--r--   0 png       (1000) png261    (1000)      661 2023-06-17 07:28:43.000000 pywalc-1.0.1/pywalc/colors.py
--rw-r--r--   0 png       (1000) png261    (1000)     2821 2023-06-17 08:28:11.000000 pywalc-1.0.1/pywalc/server.py
--rw-r--r--   0 png       (1000) png261    (1000)      480 2023-06-17 04:15:10.000000 pywalc-1.0.1/pywalc/settings.py
--rw-r--r--   0 png       (1000) png261    (1000)      667 2023-06-17 08:36:08.000000 pywalc-1.0.1/pywalc/system.py
--rw-r--r--   0 png       (1000) png261    (1000)      760 2023-06-16 14:53:07.000000 pywalc-1.0.1/pywalc/theme.py
--rw-r--r--   0 png       (1000) png261    (1000)      533 2023-06-17 08:33:00.000000 pywalc-1.0.1/pywalc/util.py
--rw-r--r--   0 png       (1000) png261    (1000)     1451 2023-06-17 08:25:28.000000 pywalc-1.0.1/pywalc/wallpaper.py
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:14:43.193445 pywalc-1.0.1/pywalc.egg-info/
--rw-r--r--   0 png       (1000) png261    (1000)     1567 2023-06-17 14:14:43.000000 pywalc-1.0.1/pywalc.egg-info/PKG-INFO
--rw-r--r--   0 png       (1000) png261    (1000)      379 2023-06-17 14:14:43.000000 pywalc-1.0.1/pywalc.egg-info/SOURCES.txt
--rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-17 14:14:43.000000 pywalc-1.0.1/pywalc.egg-info/dependency_links.txt
--rw-r--r--   0 png       (1000) png261    (1000)       48 2023-06-17 14:14:43.000000 pywalc-1.0.1/pywalc.egg-info/entry_points.txt
--rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-17 14:14:43.000000 pywalc-1.0.1/pywalc.egg-info/not-zip-safe
--rw-r--r--   0 png       (1000) png261    (1000)        7 2023-06-17 14:14:43.000000 pywalc-1.0.1/pywalc.egg-info/top_level.txt
--rw-r--r--   0 png       (1000) png261    (1000)       38 2023-06-17 14:14:43.193445 pywalc-1.0.1/setup.cfg
--rw-r--r--   0 png       (1000) png261    (1000)     1031 2023-06-17 14:09:41.000000 pywalc-1.0.1/setup.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/
+-rw-r--r--   0 png       (1000) png261    (1000)       84 2023-06-16 16:41:58.000000 pywalc-1.0.2/.gitignore
+-rw-r--r--   0 png       (1000) png261    (1000)       86 2023-06-16 14:17:37.000000 pywalc-1.0.2/.gitmodules
+-rw-r--r--   0 png       (1000) png261    (1000)      233 2023-06-17 09:16:42.000000 pywalc-1.0.2/.pypirc
+-rw-r--r--   0 png       (1000) png261    (1000)     1070 2023-06-16 14:10:31.000000 pywalc-1.0.2/LICENSE
+-rw-r--r--   0 png       (1000) png261    (1000)      110 2023-06-17 14:45:01.000000 pywalc-1.0.2/MANIFEST.in
+-rw-r--r--   0 png       (1000) png261    (1000)     1567 2023-06-17 14:46:10.329613 pywalc-1.0.2/PKG-INFO
+-rw-r--r--   0 png       (1000) png261    (1000)      901 2023-06-16 14:10:31.000000 pywalc-1.0.2/README.md
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.326280 pywalc-1.0.2/pywalc/
+-rw-r--r--   0 png       (1000) png261    (1000)      267 2023-06-17 06:25:24.000000 pywalc-1.0.2/pywalc/__init__.py
+-rw-r--r--   0 png       (1000) png261    (1000)      361 2023-06-17 08:33:01.000000 pywalc-1.0.2/pywalc/__main__.py
+-rw-r--r--   0 png       (1000) png261    (1000)      661 2023-06-17 07:28:43.000000 pywalc-1.0.2/pywalc/colors.py
+-rw-r--r--   0 png       (1000) png261    (1000)     2821 2023-06-17 08:28:11.000000 pywalc-1.0.2/pywalc/server.py
+-rw-r--r--   0 png       (1000) png261    (1000)      480 2023-06-17 04:15:10.000000 pywalc-1.0.2/pywalc/settings.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.326280 pywalc-1.0.2/pywalc/static/
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/pywalc/static/css/
+-rw-r--r--   0 png       (1000) png261    (1000)     4575 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/css/style.css
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/pywalc/static/js/
+-rw-r--r--   0 png       (1000) png261    (1000)      825 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/Actions.js
+-rw-r--r--   0 png       (1000) png261    (1000)      790 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/Color.js
+-rw-r--r--   0 png       (1000) png261    (1000)      209 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/Sys.js
+-rw-r--r--   0 png       (1000) png261    (1000)      794 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/Theme.js
+-rw-r--r--   0 png       (1000) png261    (1000)     1284 2023-06-17 08:21:42.000000 pywalc-1.0.2/pywalc/static/js/Wallpaper.js
+-rw-r--r--   0 png       (1000) png261    (1000)      675 2023-06-17 08:18:19.000000 pywalc-1.0.2/pywalc/static/js/api.js
+-rw-r--r--   0 png       (1000) png261    (1000)      356 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/connect.js
+-rw-r--r--   0 png       (1000) png261    (1000)     1636 2023-06-17 08:13:04.000000 pywalc-1.0.2/pywalc/static/js/data.js
+-rw-r--r--   0 png       (1000) png261    (1000)      669 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/helper.js
+-rw-r--r--   0 png       (1000) png261    (1000)      537 2023-06-17 08:28:15.000000 pywalc-1.0.2/pywalc/static/js/main.js
+-rw-r--r--   0 png       (1000) png261    (1000)      667 2023-06-17 08:36:08.000000 pywalc-1.0.2/pywalc/system.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/pywalc/templates/
+-rw-r--r--   0 png       (1000) png261    (1000)     3493 2023-06-17 08:35:11.000000 pywalc-1.0.2/pywalc/templates/index.html
+-rw-r--r--   0 png       (1000) png261    (1000)      760 2023-06-16 14:53:07.000000 pywalc-1.0.2/pywalc/theme.py
+-rw-r--r--   0 png       (1000) png261    (1000)      533 2023-06-17 08:33:00.000000 pywalc-1.0.2/pywalc/util.py
+-rw-r--r--   0 png       (1000) png261    (1000)     1451 2023-06-17 08:25:28.000000 pywalc-1.0.2/pywalc/wallpaper.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/pywalc.egg-info/
+-rw-r--r--   0 png       (1000) png261    (1000)     1567 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/PKG-INFO
+-rw-r--r--   0 png       (1000) png261    (1000)      746 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/SOURCES.txt
+-rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/dependency_links.txt
+-rw-r--r--   0 png       (1000) png261    (1000)       48 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/entry_points.txt
+-rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-17 14:44:05.000000 pywalc-1.0.2/pywalc.egg-info/not-zip-safe
+-rw-r--r--   0 png       (1000) png261    (1000)        7 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/top_level.txt
+-rw-r--r--   0 png       (1000) png261    (1000)       62 2023-06-17 09:07:38.000000 pywalc-1.0.2/requirements.txt
+-rw-r--r--   0 png       (1000) png261    (1000)       38 2023-06-17 14:46:10.329613 pywalc-1.0.2/setup.cfg
+-rw-r--r--   0 png       (1000) png261    (1000)     1031 2023-06-17 14:46:02.000000 pywalc-1.0.2/setup.py
```

### Comparing `pywalc-1.0.1/LICENSE` & `pywalc-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.1/PKG-INFO` & `pywalc-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pywalc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Change pywal color online
 Home-page: https://github.com/png261/pwy
-Download-URL: https://github.com/png261/pwy/archive/1.0.1.tar.gz
+Download-URL: https://github.com/png261/pwy/archive/1.0.2.tar.gz
 Author: Phuong Nguyen
 Author-email: nhphuong.code@gmail.com
 License: MIT
 Keywords: pywalc wal colorscheme terminal-emulators changing-colorschemes
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pywalc-1.0.1/README.md` & `pywalc-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.1/pywalc/colors.py` & `pywalc-1.0.2/pywalc/colors.py`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.1/pywalc/server.py` & `pywalc-1.0.2/pywalc/server.py`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.1/pywalc/system.py` & `pywalc-1.0.2/pywalc/system.py`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.1/pywalc/theme.py` & `pywalc-1.0.2/pywalc/theme.py`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.1/pywalc/util.py` & `pywalc-1.0.2/pywalc/util.py`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.1/pywalc/wallpaper.py` & `pywalc-1.0.2/pywalc/wallpaper.py`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.1/pywalc.egg-info/PKG-INFO` & `pywalc-1.0.2/pywalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pywalc
-Version: 1.0.1
+Version: 1.0.2
 Summary: Change pywal color online
 Home-page: https://github.com/png261/pwy
-Download-URL: https://github.com/png261/pwy/archive/1.0.1.tar.gz
+Download-URL: https://github.com/png261/pwy/archive/1.0.2.tar.gz
 Author: Phuong Nguyen
 Author-email: nhphuong.code@gmail.com
 License: MIT
 Keywords: pywalc wal colorscheme terminal-emulators changing-colorschemes
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pywalc-1.0.1/setup.py` & `pywalc-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """pwy - setup.py"""
 import setuptools
 
 LONG_DESC = open('README.md').read()
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 DOWNLOAD = "https://github.com/png261/pwy/archive/%s.tar.gz" % VERSION
 
 setuptools.setup(
     name="pywalc",
     version=VERSION,
     author="Phuong Nguyen",
     author_email="nhphuong.code@gmail.com",
```

