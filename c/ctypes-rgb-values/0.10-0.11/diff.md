# Comparing `tmp/ctypes_rgb_values-0.10.tar.gz` & `tmp/ctypes_rgb_values-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctypes_rgb_values-0.10.tar", last modified: Thu Dec 22 08:39:04 2022, max compression
+gzip compressed data, was "ctypes_rgb_values-0.11.tar", last modified: Sat Jun 17 14:17:16 2023, max compression
```

## Comparing `ctypes_rgb_values-0.10.tar` & `ctypes_rgb_values-0.11.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-12-22 08:39:04.530303 ctypes_rgb_values-0.10/
--rw-rw-rw-   0        0        0     1148 2022-12-22 08:38:59.000000 ctypes_rgb_values-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      157 2022-12-22 08:38:58.000000 ctypes_rgb_values-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2834 2022-12-22 08:39:04.530303 ctypes_rgb_values-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1896 2022-12-22 08:34:30.000000 ctypes_rgb_values-0.10/README.md
-drwxrwxrwx   0        0        0        0 2022-12-22 08:39:04.527399 ctypes_rgb_values-0.10/ctypes_rgb_values/
--rw-rw-rw-   0        0        0     1069 2022-10-02 04:27:48.000000 ctypes_rgb_values-0.10/ctypes_rgb_values/LICENSE
--rw-rw-rw-   0        0        0     1896 2022-12-22 08:34:30.000000 ctypes_rgb_values-0.10/ctypes_rgb_values/README.MD
--rw-rw-rw-   0        0        0     3316 2022-12-22 08:31:52.000000 ctypes_rgb_values-0.10/ctypes_rgb_values/__init__.py
--rw-rw-rw-   0        0        0        4 2022-12-22 08:39:03.000000 ctypes_rgb_values-0.10/ctypes_rgb_values/requirements.txt
--rw-rw-rw-   0        0        0        2 2022-12-22 08:39:03.000000 ctypes_rgb_values-0.10/ctypes_rgb_values/thirdparty.json
-drwxrwxrwx   0        0        0        0 2022-12-22 08:39:04.529327 ctypes_rgb_values-0.10/ctypes_rgb_values.egg-info/
--rw-rw-rw-   0        0        0     2834 2022-12-22 08:39:04.000000 ctypes_rgb_values-0.10/ctypes_rgb_values.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2022-12-22 08:39:04.000000 ctypes_rgb_values-0.10/ctypes_rgb_values.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-22 08:39:04.000000 ctypes_rgb_values-0.10/ctypes_rgb_values.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2022-12-22 08:39:04.000000 ctypes_rgb_values-0.10/ctypes_rgb_values.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-12-22 08:39:04.000000 ctypes_rgb_values-0.10/ctypes_rgb_values.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-12-22 08:39:04.530303 ctypes_rgb_values-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1388 2022-12-22 08:39:03.000000 ctypes_rgb_values-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 14:17:16.310884 ctypes_rgb_values-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-06-17 14:17:10.000000 ctypes_rgb_values-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      157 2023-06-17 14:17:09.000000 ctypes_rgb_values-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2528 2023-06-17 14:17:16.310884 ctypes_rgb_values-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1896 2023-04-15 00:18:08.000000 ctypes_rgb_values-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 14:17:16.306895 ctypes_rgb_values-0.11/ctypes_rgb_values/
+-rw-rw-rw-   0        0        0     1069 2023-04-15 00:18:08.000000 ctypes_rgb_values-0.11/ctypes_rgb_values/LICENSE
+-rw-rw-rw-   0        0        0     1896 2023-04-15 00:18:08.000000 ctypes_rgb_values-0.11/ctypes_rgb_values/README.MD
+-rw-rw-rw-   0        0        0     3752 2023-06-17 14:10:46.000000 ctypes_rgb_values-0.11/ctypes_rgb_values/__init__.py
+-rw-rw-rw-   0        0        0        4 2023-06-17 14:17:15.000000 ctypes_rgb_values-0.11/ctypes_rgb_values/requirements.txt
+-rw-rw-rw-   0        0        0     1183 2023-06-17 14:17:15.000000 ctypes_rgb_values-0.11/ctypes_rgb_values/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-06-17 14:17:16.309887 ctypes_rgb_values-0.11/ctypes_rgb_values.egg-info/
+-rw-rw-rw-   0        0        0     2528 2023-06-17 14:17:16.000000 ctypes_rgb_values-0.11/ctypes_rgb_values.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-06-17 14:17:16.000000 ctypes_rgb_values-0.11/ctypes_rgb_values.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 14:17:16.000000 ctypes_rgb_values-0.11/ctypes_rgb_values.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-17 14:17:16.000000 ctypes_rgb_values-0.11/ctypes_rgb_values.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-17 14:17:16.000000 ctypes_rgb_values-0.11/ctypes_rgb_values.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-17 14:17:16.310884 ctypes_rgb_values-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2023-06-17 14:17:15.000000 ctypes_rgb_values-0.11/setup.py
```

### Comparing `ctypes_rgb_values-0.10/LICENSE.rst` & `ctypes_rgb_values-0.11/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
  The MIT License (MIT)
- Copyright (c) 2022 Johannes Fischer
+ Copyright (c) 2023 Johannes Fischer
  
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `ctypes_rgb_values-0.10/PKG-INFO` & `ctypes_rgb_values-0.11/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,41 @@
-Metadata-Version: 2.1
-Name: ctypes_rgb_values
-Version: 0.10
-Summary: Get rgb values at mouse position
-Home-page: https://github.com/hansalemaos/ctypes_rgb_values
-Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
-License: MIT
-Keywords: ctypes,windows,rgb,screenshot
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-
-### Get rgb values at mouse position
-
-
-```python
-pip install ctypes-rgb-values
-
-from ctypes_rgb_values import get_rgb_values
-cols = get_rgb_values(
-    sleeptime=0.0,
-    on_left_click=False,  # if True: only captures when left  mouse button is pressed
-    on_right_click=False,  # if True: only captures when right mouse button is pressed
-    rgb_values=True,  # if True: rgb will be returned
-    rgba_values=True,  # if True: rgba will be returned
-    coords=True,  # if True: coords of each color will be returned
-    time_value=True,  # if True: time of each color change will be returned
-)
-# Press ctrl+c when you are done!
-
-"""
-[((107, 107, 107), (107, 107, 107, 0), (1356, 1051), 1671697419.8177068),
- ((99, 99, 99), (99, 99, 99, 0), (1357, 1049), 1671697419.8401546),
- ((99, 99, 99), (99, 99, 99, 0), (1359, 1041), 1671697419.8508923),
- ((99, 99, 99), (99, 99, 99, 0), (1361, 1038), 1671697419.8670166),
- ((99, 99, 99), (99, 99, 99, 0), (1363, 1033), 1671697419.8836083),
- ((99, 99, 99), (99, 99, 99, 0), (1364, 1029), 1671697419.9011772),
- ((99, 99, 99), (99, 99, 99, 0), (1365, 1028), 1671697419.9167929),
- ((99, 99, 99), (99, 99, 99, 0), (1365, 1028), 1671697419.9333844),
- ((99, 99, 99), (99, 99, 99, 0), (1365, 1028), 1671697419.9499762),
- ((99, 99, 99), (99, 99, 99, 0), (1365, 1028), 1671697419.9675448),
- ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697419.9831607),
- ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0007331),
- ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0182958),
- ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0329359),
- ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0505047),
- ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0705392),
- ((250, 250, 250), (250, 250, 250, 0), (1368, 1027), 1671697420.0851743),
- ....
- """
-
-```
-
+### Get rgb values at mouse position
+
+
+```python
+pip install ctypes-rgb-values
+
+from ctypes_rgb_values import get_rgb_values
+cols = get_rgb_values(
+    sleeptime=0.0,
+    on_left_click=False,  # if True: only captures when left  mouse button is pressed
+    on_right_click=False,  # if True: only captures when right mouse button is pressed
+    rgb_values=True,  # if True: rgb will be returned
+    rgba_values=True,  # if True: rgba will be returned
+    coords=True,  # if True: coords of each color will be returned
+    time_value=True,  # if True: time of each color change will be returned
+)
+# Press ctrl+c when you are done!
+
+"""
+[((107, 107, 107), (107, 107, 107, 0), (1356, 1051), 1671697419.8177068),
+ ((99, 99, 99), (99, 99, 99, 0), (1357, 1049), 1671697419.8401546),
+ ((99, 99, 99), (99, 99, 99, 0), (1359, 1041), 1671697419.8508923),
+ ((99, 99, 99), (99, 99, 99, 0), (1361, 1038), 1671697419.8670166),
+ ((99, 99, 99), (99, 99, 99, 0), (1363, 1033), 1671697419.8836083),
+ ((99, 99, 99), (99, 99, 99, 0), (1364, 1029), 1671697419.9011772),
+ ((99, 99, 99), (99, 99, 99, 0), (1365, 1028), 1671697419.9167929),
+ ((99, 99, 99), (99, 99, 99, 0), (1365, 1028), 1671697419.9333844),
+ ((99, 99, 99), (99, 99, 99, 0), (1365, 1028), 1671697419.9499762),
+ ((99, 99, 99), (99, 99, 99, 0), (1365, 1028), 1671697419.9675448),
+ ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697419.9831607),
+ ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0007331),
+ ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0182958),
+ ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0329359),
+ ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0505047),
+ ((117, 117, 117), (117, 117, 117, 0), (1365, 1028), 1671697420.0705392),
+ ((250, 250, 250), (250, 250, 250, 0), (1368, 1027), 1671697420.0851743),
+ ....
+ """
+
+```
+
```

### Comparing `ctypes_rgb_values-0.10/README.md` & `ctypes_rgb_values-0.11/ctypes_rgb_values/README.MD`

 * *Files identical despite different names*

### Comparing `ctypes_rgb_values-0.10/ctypes_rgb_values/LICENSE` & `ctypes_rgb_values-0.11/ctypes_rgb_values/LICENSE`

 * *Files identical despite different names*

### Comparing `ctypes_rgb_values-0.10/ctypes_rgb_values/__init__.py` & `ctypes_rgb_values-0.11/ctypes_rgb_values/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-from ctypes import windll, Structure, byref
-from ctypes.wintypes import LONG
+import ctypes
+from ctypes import Structure, byref
+from ctypes.wintypes import LONG, HGDIOBJ, BOOL
 from ansi.colour.rgb import rgb256
 from ansi.colour import fg, bg, fx
 from time import time, sleep
+windll = ctypes.LibraryLoader(ctypes.WinDLL)
+windll.shcore.SetProcessDpiAwareness(2)
+user32 = ctypes.WinDLL("user32", use_last_error=True)
+psapi = ctypes.WinDLL("psapi", use_last_error=True)
+gdi32 = ctypes.WinDLL("gdi32", use_last_error=True)
+gdi32.DeleteObject.argtypes = [HGDIOBJ]
+gdi32.DeleteObject.restypes = BOOL
+DeleteObject = gdi32.DeleteObject
 
-user32 = windll.user32
-gdi32 = windll.gdi32
 LM_BUTTON = 0x01
 RM_BUTTON = 0x02
 
 
 def print_full_col(text, colour):
     return "".join(
         list(
@@ -40,14 +47,19 @@
     user32.GetCursorPos(byref(pos))
     return pos.x, pos.y
 
 
 def get_pixel(x, y, hdc=0):
     dc = user32.GetDC(hdc)
     colorref = gdi32.GetPixel(dc, x, y)
+    try:
+        DeleteObject(dc)
+    except Exception as faq:
+        print(faq)
+        pass
     return colorref
 
 
 def is_right_mouse_button_pressed():
     return get_key_state(RM_BUTTON) > 1
```

### Comparing `ctypes_rgb_values-0.10/setup.py` & `ctypes_rgb_values-0.11/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import setup, find_packages
 import codecs
 import os
-
-#change to dict
+# 
 here = os.path.abspath(os.path.dirname(__file__))
+# 
+with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()\
 
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
+from pathlib import Path
+this_directory = Path(__file__).parent
+#long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.10'
-DESCRIPTION = "Get rgb values at mouse position"
+VERSION = '''0.11'''
+DESCRIPTION = '''Get rgb values at mouse position'''
 
 # Setting up
 setup(
     name="ctypes_rgb_values",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/ctypes_rgb_values',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=['ansi'],
     keywords=['ctypes', 'windows', 'rgb', 'screenshot'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.9', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Text Editors :: Text Processing', 'Topic :: Text Processing :: General', 'Topic :: Text Processing :: Indexing', 'Topic :: Text Processing :: Filters', 'Topic :: Utilities'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=['ansi'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

