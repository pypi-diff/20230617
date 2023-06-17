# Comparing `tmp/pywalc-1.0.2.tar.gz` & `tmp/pywalc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywalc-1.0.2.tar", last modified: Sat Jun 17 14:46:10 2023, max compression
+gzip compressed data, was "pywalc-1.0.3.tar", last modified: Sat Jun 17 16:06:31 2023, max compression
```

## Comparing `pywalc-1.0.2.tar` & `pywalc-1.0.3.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/
--rw-r--r--   0 png       (1000) png261    (1000)       84 2023-06-16 16:41:58.000000 pywalc-1.0.2/.gitignore
--rw-r--r--   0 png       (1000) png261    (1000)       86 2023-06-16 14:17:37.000000 pywalc-1.0.2/.gitmodules
--rw-r--r--   0 png       (1000) png261    (1000)      233 2023-06-17 09:16:42.000000 pywalc-1.0.2/.pypirc
--rw-r--r--   0 png       (1000) png261    (1000)     1070 2023-06-16 14:10:31.000000 pywalc-1.0.2/LICENSE
--rw-r--r--   0 png       (1000) png261    (1000)      110 2023-06-17 14:45:01.000000 pywalc-1.0.2/MANIFEST.in
--rw-r--r--   0 png       (1000) png261    (1000)     1567 2023-06-17 14:46:10.329613 pywalc-1.0.2/PKG-INFO
--rw-r--r--   0 png       (1000) png261    (1000)      901 2023-06-16 14:10:31.000000 pywalc-1.0.2/README.md
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.326280 pywalc-1.0.2/pywalc/
--rw-r--r--   0 png       (1000) png261    (1000)      267 2023-06-17 06:25:24.000000 pywalc-1.0.2/pywalc/__init__.py
--rw-r--r--   0 png       (1000) png261    (1000)      361 2023-06-17 08:33:01.000000 pywalc-1.0.2/pywalc/__main__.py
--rw-r--r--   0 png       (1000) png261    (1000)      661 2023-06-17 07:28:43.000000 pywalc-1.0.2/pywalc/colors.py
--rw-r--r--   0 png       (1000) png261    (1000)     2821 2023-06-17 08:28:11.000000 pywalc-1.0.2/pywalc/server.py
--rw-r--r--   0 png       (1000) png261    (1000)      480 2023-06-17 04:15:10.000000 pywalc-1.0.2/pywalc/settings.py
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.326280 pywalc-1.0.2/pywalc/static/
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/pywalc/static/css/
--rw-r--r--   0 png       (1000) png261    (1000)     4575 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/css/style.css
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/pywalc/static/js/
--rw-r--r--   0 png       (1000) png261    (1000)      825 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/Actions.js
--rw-r--r--   0 png       (1000) png261    (1000)      790 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/Color.js
--rw-r--r--   0 png       (1000) png261    (1000)      209 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/Sys.js
--rw-r--r--   0 png       (1000) png261    (1000)      794 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/Theme.js
--rw-r--r--   0 png       (1000) png261    (1000)     1284 2023-06-17 08:21:42.000000 pywalc-1.0.2/pywalc/static/js/Wallpaper.js
--rw-r--r--   0 png       (1000) png261    (1000)      675 2023-06-17 08:18:19.000000 pywalc-1.0.2/pywalc/static/js/api.js
--rw-r--r--   0 png       (1000) png261    (1000)      356 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/connect.js
--rw-r--r--   0 png       (1000) png261    (1000)     1636 2023-06-17 08:13:04.000000 pywalc-1.0.2/pywalc/static/js/data.js
--rw-r--r--   0 png       (1000) png261    (1000)      669 2023-06-17 07:42:58.000000 pywalc-1.0.2/pywalc/static/js/helper.js
--rw-r--r--   0 png       (1000) png261    (1000)      537 2023-06-17 08:28:15.000000 pywalc-1.0.2/pywalc/static/js/main.js
--rw-r--r--   0 png       (1000) png261    (1000)      667 2023-06-17 08:36:08.000000 pywalc-1.0.2/pywalc/system.py
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/pywalc/templates/
--rw-r--r--   0 png       (1000) png261    (1000)     3493 2023-06-17 08:35:11.000000 pywalc-1.0.2/pywalc/templates/index.html
--rw-r--r--   0 png       (1000) png261    (1000)      760 2023-06-16 14:53:07.000000 pywalc-1.0.2/pywalc/theme.py
--rw-r--r--   0 png       (1000) png261    (1000)      533 2023-06-17 08:33:00.000000 pywalc-1.0.2/pywalc/util.py
--rw-r--r--   0 png       (1000) png261    (1000)     1451 2023-06-17 08:25:28.000000 pywalc-1.0.2/pywalc/wallpaper.py
-drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 14:46:10.329613 pywalc-1.0.2/pywalc.egg-info/
--rw-r--r--   0 png       (1000) png261    (1000)     1567 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/PKG-INFO
--rw-r--r--   0 png       (1000) png261    (1000)      746 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/SOURCES.txt
--rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/dependency_links.txt
--rw-r--r--   0 png       (1000) png261    (1000)       48 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/entry_points.txt
--rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-17 14:44:05.000000 pywalc-1.0.2/pywalc.egg-info/not-zip-safe
--rw-r--r--   0 png       (1000) png261    (1000)        7 2023-06-17 14:46:10.000000 pywalc-1.0.2/pywalc.egg-info/top_level.txt
--rw-r--r--   0 png       (1000) png261    (1000)       62 2023-06-17 09:07:38.000000 pywalc-1.0.2/requirements.txt
--rw-r--r--   0 png       (1000) png261    (1000)       38 2023-06-17 14:46:10.329613 pywalc-1.0.2/setup.cfg
--rw-r--r--   0 png       (1000) png261    (1000)     1031 2023-06-17 14:46:02.000000 pywalc-1.0.2/setup.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 16:06:31.276616 pywalc-1.0.3/
+-rw-r--r--   0 png       (1000) png261    (1000)       84 2023-06-16 16:41:58.000000 pywalc-1.0.3/.gitignore
+-rw-r--r--   0 png       (1000) png261    (1000)       86 2023-06-16 14:17:37.000000 pywalc-1.0.3/.gitmodules
+-rw-r--r--   0 png       (1000) png261    (1000)      233 2023-06-17 09:16:42.000000 pywalc-1.0.3/.pypirc
+-rw-r--r--   0 png       (1000) png261    (1000)     1070 2023-06-16 14:10:31.000000 pywalc-1.0.3/LICENSE
+-rw-r--r--   0 png       (1000) png261    (1000)      110 2023-06-17 14:45:01.000000 pywalc-1.0.3/MANIFEST.in
+-rw-r--r--   0 png       (1000) png261    (1000)     1567 2023-06-17 16:06:31.276616 pywalc-1.0.3/PKG-INFO
+-rw-r--r--   0 png       (1000) png261    (1000)      901 2023-06-16 14:10:31.000000 pywalc-1.0.3/README.md
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 16:06:31.276616 pywalc-1.0.3/pywalc/
+-rw-r--r--   0 png       (1000) png261    (1000)      214 2023-06-17 14:53:09.000000 pywalc-1.0.3/pywalc/__init__.py
+-rw-r--r--   0 png       (1000) png261    (1000)      553 2023-06-17 16:06:06.000000 pywalc-1.0.3/pywalc/__main__.py
+-rw-r--r--   0 png       (1000) png261    (1000)      572 2023-06-17 15:52:02.000000 pywalc-1.0.3/pywalc/colors.py
+-rw-r--r--   0 png       (1000) png261    (1000)     4457 2023-06-17 15:53:35.000000 pywalc-1.0.3/pywalc/server.py
+-rw-r--r--   0 png       (1000) png261    (1000)      401 2023-06-17 15:32:38.000000 pywalc-1.0.3/pywalc/settings.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 16:06:31.273283 pywalc-1.0.3/pywalc/static/
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 16:06:31.276616 pywalc-1.0.3/pywalc/static/css/
+-rw-r--r--   0 png       (1000) png261    (1000)     4575 2023-06-17 07:42:58.000000 pywalc-1.0.3/pywalc/static/css/style.css
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 16:06:31.276616 pywalc-1.0.3/pywalc/static/js/
+-rw-r--r--   0 png       (1000) png261    (1000)      825 2023-06-17 07:42:58.000000 pywalc-1.0.3/pywalc/static/js/Actions.js
+-rw-r--r--   0 png       (1000) png261    (1000)      790 2023-06-17 07:42:58.000000 pywalc-1.0.3/pywalc/static/js/Color.js
+-rw-r--r--   0 png       (1000) png261    (1000)      209 2023-06-17 07:42:58.000000 pywalc-1.0.3/pywalc/static/js/Sys.js
+-rw-r--r--   0 png       (1000) png261    (1000)      794 2023-06-17 07:42:58.000000 pywalc-1.0.3/pywalc/static/js/Theme.js
+-rw-r--r--   0 png       (1000) png261    (1000)     1284 2023-06-17 08:21:42.000000 pywalc-1.0.3/pywalc/static/js/Wallpaper.js
+-rw-r--r--   0 png       (1000) png261    (1000)      675 2023-06-17 08:18:19.000000 pywalc-1.0.3/pywalc/static/js/api.js
+-rw-r--r--   0 png       (1000) png261    (1000)     1636 2023-06-17 08:13:04.000000 pywalc-1.0.3/pywalc/static/js/data.js
+-rw-r--r--   0 png       (1000) png261    (1000)      352 2023-06-17 16:05:08.000000 pywalc-1.0.3/pywalc/static/js/helper.js
+-rw-r--r--   0 png       (1000) png261    (1000)      537 2023-06-17 16:02:00.000000 pywalc-1.0.3/pywalc/static/js/main.js
+-rw-r--r--   0 png       (1000) png261    (1000)      426 2023-06-17 15:52:35.000000 pywalc-1.0.3/pywalc/system.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 16:06:31.276616 pywalc-1.0.3/pywalc/templates/
+-rw-r--r--   0 png       (1000) png261    (1000)     3496 2023-06-17 14:51:07.000000 pywalc-1.0.3/pywalc/templates/index.html
+-rw-r--r--   0 png       (1000) png261    (1000)      738 2023-06-17 15:52:13.000000 pywalc-1.0.3/pywalc/theme.py
+-rw-r--r--   0 png       (1000) png261    (1000)     1812 2023-06-17 16:01:13.000000 pywalc-1.0.3/pywalc/util.py
+-rw-r--r--   0 png       (1000) png261    (1000)     1306 2023-06-17 16:05:13.000000 pywalc-1.0.3/pywalc/wallpaper.py
+drwxr-xr-x   0 png       (1000) png261    (1000)        0 2023-06-17 16:06:31.276616 pywalc-1.0.3/pywalc.egg-info/
+-rw-r--r--   0 png       (1000) png261    (1000)     1567 2023-06-17 16:06:31.000000 pywalc-1.0.3/pywalc.egg-info/PKG-INFO
+-rw-r--r--   0 png       (1000) png261    (1000)      718 2023-06-17 16:06:31.000000 pywalc-1.0.3/pywalc.egg-info/SOURCES.txt
+-rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-17 16:06:31.000000 pywalc-1.0.3/pywalc.egg-info/dependency_links.txt
+-rw-r--r--   0 png       (1000) png261    (1000)       48 2023-06-17 16:06:31.000000 pywalc-1.0.3/pywalc.egg-info/entry_points.txt
+-rw-r--r--   0 png       (1000) png261    (1000)        1 2023-06-17 14:44:05.000000 pywalc-1.0.3/pywalc.egg-info/not-zip-safe
+-rw-r--r--   0 png       (1000) png261    (1000)        7 2023-06-17 16:06:31.000000 pywalc-1.0.3/pywalc.egg-info/top_level.txt
+-rw-r--r--   0 png       (1000) png261    (1000)       62 2023-06-17 09:07:38.000000 pywalc-1.0.3/requirements.txt
+-rw-r--r--   0 png       (1000) png261    (1000)       38 2023-06-17 16:06:31.276616 pywalc-1.0.3/setup.cfg
+-rw-r--r--   0 png       (1000) png261    (1000)     1031 2023-06-17 16:06:23.000000 pywalc-1.0.3/setup.py
```

### Comparing `pywalc-1.0.2/LICENSE` & `pywalc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/PKG-INFO` & `pywalc-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pywalc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Change pywal color online
 Home-page: https://github.com/png261/pwy
-Download-URL: https://github.com/png261/pwy/archive/1.0.2.tar.gz
+Download-URL: https://github.com/png261/pwy/archive/1.0.3.tar.gz
 Author: Phuong Nguyen
 Author-email: nhphuong.code@gmail.com
 License: MIT
 Keywords: pywalc wal colorscheme terminal-emulators changing-colorschemes
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pywalc-1.0.2/README.md` & `pywalc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/pywalc/static/css/style.css` & `pywalc-1.0.3/pywalc/static/css/style.css`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/pywalc/static/js/Actions.js` & `pywalc-1.0.3/pywalc/static/js/Actions.js`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/pywalc/static/js/Color.js` & `pywalc-1.0.3/pywalc/static/js/Color.js`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/pywalc/static/js/Theme.js` & `pywalc-1.0.3/pywalc/static/js/Theme.js`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/pywalc/static/js/Wallpaper.js` & `pywalc-1.0.3/pywalc/static/js/Wallpaper.js`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/pywalc/static/js/api.js` & `pywalc-1.0.3/pywalc/static/js/api.js`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/pywalc/static/js/data.js` & `pywalc-1.0.3/pywalc/static/js/data.js`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/pywalc/static/js/main.js` & `pywalc-1.0.3/pywalc/static/js/main.js`

 * *Files identical despite different names*

### Comparing `pywalc-1.0.2/pywalc/templates/index.html` & `pywalc-1.0.3/pywalc/templates/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
     <meta charset="UTF-8" />
-    <title>pwy</title>
+    <title>Pywalc</title>
     <link href="{{ url_for('static', path='/css/style.css') }}" rel="stylesheet">
 </head>
 
 <body class="home-page">
     <section id="sys">
         <div class="container">
             <div class="sys__inner">
```

### Comparing `pywalc-1.0.2/pywalc/theme.py` & `pywalc-1.0.3/pywalc/theme.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 import os
 import json
 import pywal
-from fastapi import APIRouter
 from .settings import MODULE_DIR
 
-dark_themes = [
-    theme.name.replace(".json", "") for theme in pywal.theme.list_themes()
-]
-light_themes = [
-    theme.name.replace(".json", "")
-    for theme in pywal.theme.list_themes(dark=False)
-]
-
-THEME = {"dark": dark_themes, "light": light_themes}
-
-
-themeRouter = APIRouter()
-
-
-@themeRouter.get("/theme", tags=["theme"])
-def get_themes():
-    return THEME
-
-
-@themeRouter.get("/theme/{category}/{name}", tags=["theme"])
-def set_theme(name, category):
-    themes_path = os.path.join(
-        MODULE_DIR, "colorschemes", category, name + ".json"
-    )
-    with open(themes_path) as file:
-        themes = json.loads(file.read())
-    return themes["colors"]
+class Theme:
+    def __init__(self):
+        dark_themes = [
+            theme.name.replace(".json", "") for theme in pywal.theme.list_themes()
+        ]
+        light_themes = [
+            theme.name.replace(".json", "")
+            for theme in pywal.theme.list_themes(dark=False)
+        ]
+
+        self.data = {"dark": dark_themes, "light": light_themes}
+
+    def get(self):
+        return self.data
+
+    def set(self, name, category):
+        themes_path = os.path.join(
+            MODULE_DIR, "colorschemes", category, name + ".json"
+        )
+        with open(themes_path) as file:
+            themes = json.loads(file.read())
+        return themes["colors"]
```

### Comparing `pywalc-1.0.2/pywalc.egg-info/PKG-INFO` & `pywalc-1.0.3/pywalc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pywalc
-Version: 1.0.2
+Version: 1.0.3
 Summary: Change pywal color online
 Home-page: https://github.com/png261/pwy
-Download-URL: https://github.com/png261/pwy/archive/1.0.2.tar.gz
+Download-URL: https://github.com/png261/pwy/archive/1.0.3.tar.gz
 Author: Phuong Nguyen
 Author-email: nhphuong.code@gmail.com
 License: MIT
 Keywords: pywalc wal colorscheme terminal-emulators changing-colorschemes
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pywalc-1.0.2/pywalc.egg-info/SOURCES.txt` & `pywalc-1.0.3/pywalc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,12 +24,11 @@
 pywalc/static/css/style.css
 pywalc/static/js/Actions.js
 pywalc/static/js/Color.js
 pywalc/static/js/Sys.js
 pywalc/static/js/Theme.js
 pywalc/static/js/Wallpaper.js
 pywalc/static/js/api.js
-pywalc/static/js/connect.js
 pywalc/static/js/data.js
 pywalc/static/js/helper.js
 pywalc/static/js/main.js
 pywalc/templates/index.html
```

### Comparing `pywalc-1.0.2/setup.py` & `pywalc-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """pwy - setup.py"""
 import setuptools
 
 LONG_DESC = open('README.md').read()
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 DOWNLOAD = "https://github.com/png261/pwy/archive/%s.tar.gz" % VERSION
 
 setuptools.setup(
     name="pywalc",
     version=VERSION,
     author="Phuong Nguyen",
     author_email="nhphuong.code@gmail.com",
```

