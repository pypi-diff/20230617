# Comparing `tmp/mykit-2.0.4.tar.gz` & `tmp/mykit-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-1_d_1_xn/mykit-2.0.4.tar", last modified: Fri Jun 16 13:06:15 2023, max compression
+gzip compressed data, was "/home/runner/work/mykit/mykit/dist/.tmp-tgo56sui/mykit-3.0.0.tar", last modified: Sat Jun 17 17:20:30 2023, max compression
```

## Comparing `mykit-2.0.4.tar` & `mykit-3.0.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 13:05:51.000000 mykit-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-16 13:06:15.000000 mykit-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-16 13:05:51.000000 mykit-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/app/
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/arrow.py
--rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/button.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/app/complex/
--rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/complex/biplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    17112 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/complex/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/label.py
--rw-r--r--   0 runner    (1001) docker     (123)    27032 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/app/slider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/color.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/fast_visualizations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/fast_visualizations/static/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/fast_visualizations/static/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/ffmpeg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/keycrate/
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/keycrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit/kit/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/neuralnet/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/neuralnet/genetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-16 13:05:51.000000 mykit-2.0.4/mykit/kit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-16 13:06:15.000000 mykit-2.0.4/mykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-16 13:05:51.000000 mykit-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 13:06:15.000000 mykit-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 13:05:51.000000 mykit-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-17 17:20:10.000000 mykit-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-17 17:20:30.000000 mykit-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-17 17:20:10.000000 mykit-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/button.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/app/complex/
+-rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/complex/biplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17112 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/complex/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27032 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/app/slider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/color.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/fast_visualizations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/fast_visualizations/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/fast_visualizations/static/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/ffmpeg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/keycrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/keycrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit/kit/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/neuralnet/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14840 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/neuralnet/genetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-17 17:20:10.000000 mykit-3.0.0/mykit/kit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-17 17:20:30.000000 mykit-3.0.0/mykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-17 17:20:10.000000 mykit-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 17:20:30.000000 mykit-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-17 17:20:10.000000 mykit-3.0.0/setup.py
```

### Comparing `mykit-2.0.4/LICENSE` & `mykit-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/PKG-INFO` & `mykit-3.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.4
+Version: 3.0.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -61,16 +61,22 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 3.0.0 (June 17, 2023):
+    - Breaking changes:
+        - Changed `title` arg to `name` in `.app.App`
+        - Now `/kit/keycrate` must be a .txt file, and the file must exist
+        - Added `export` method to `.kit.keycrate.KeyCrate`
+    - Added test suite for `.kit.keycrate.KeyCrate`
 - 2.0.4 (June 16, 2023):
-    - Now `move` method of `Button`, `Label`, `_Slider` and will return self
+    - Now `move` method of `Button`, `Label`, and `_Slider` will return self
 - 2.0.3 (June 16, 2023):
     - Now `.app.complex.plot.Plot` and `.app.complex.plot.Biplot` can be used even if no points is specified
     - Added `add_background_processes` to `.app.App`
 - 2.0.2 (June 14, 2023):
     - finished updating all type hints
     - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
```

### Comparing `mykit-2.0.4/README.md` & `mykit-3.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,16 +34,22 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 3.0.0 (June 17, 2023):
+    - Breaking changes:
+        - Changed `title` arg to `name` in `.app.App`
+        - Now `/kit/keycrate` must be a .txt file, and the file must exist
+        - Added `export` method to `.kit.keycrate.KeyCrate`
+    - Added test suite for `.kit.keycrate.KeyCrate`
 - 2.0.4 (June 16, 2023):
-    - Now `move` method of `Button`, `Label`, `_Slider` and will return self
+    - Now `move` method of `Button`, `Label`, and `_Slider` will return self
 - 2.0.3 (June 16, 2023):
     - Now `.app.complex.plot.Plot` and `.app.complex.plot.Biplot` can be used even if no points is specified
     - Added `add_background_processes` to `.app.App`
 - 2.0.2 (June 14, 2023):
     - finished updating all type hints
     - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
```

### Comparing `mykit-2.0.4/mykit/__main__.py` & `mykit-3.0.0/mykit/__main__.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/app/__init__.py` & `mykit-3.0.0/mykit/app/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,23 @@
 
     ---
 
     ## Limitations
     - currently available only in fullscreen mode
     """
 
-    def __init__(self, title: str = 'app', bg: str = '#111111') -> None:
-        
+    def __init__(
+        self,
+        name: str = 'app',
+        bg: str = '#111111'
+    ) -> None:
+
         self.root = _tk.Tk()
         self.root.attributes('-fullscreen', True)
-        self.root.title(title)
+        self.root.title(name)
 
         page = _tk.Canvas(
             master=self.root,
             width=self.root.winfo_screenwidth(),
             height=self.root.winfo_screenheight(),
             background=bg,
             borderwidth=0, highlightthickness=0
```

### Comparing `mykit-2.0.4/mykit/app/arrow.py` & `mykit-3.0.0/mykit/app/arrow.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/app/button.py` & `mykit-3.0.0/mykit/app/button.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/app/complex/biplot.py` & `mykit-3.0.0/mykit/app/complex/biplot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/app/complex/plot.py` & `mykit-3.0.0/mykit/app/complex/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/app/label.py` & `mykit-3.0.0/mykit/app/label.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/app/slider.py` & `mykit-3.0.0/mykit/app/slider.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/color.py` & `mykit-3.0.0/mykit/kit/color.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/fast_visualizations/static/plot.py` & `mykit-3.0.0/mykit/kit/fast_visualizations/static/plot.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/ffmpeg.py` & `mykit-3.0.0/mykit/kit/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/keycrate/__init__.py` & `mykit-3.0.0/mykit/kit/keycrate/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re as _re
+import os as _os
 from typing import (
     Any as _Any,
+    Dict as _Dict,
     List as _List,
     NoReturn as _NoReturn,
     Optional as _Optional
 )
 
 from mykit.kit.path import open_file as _open_file
 from mykit.kit.utils import is_valid_var_name as _is_valid_var_name
@@ -36,28 +38,38 @@
         - `file_pth`: full path to the .txt file that holds the key-value pairs
         - `key_is_var`: if `True`, all keys must be valid as variable name
         - `eval_value`: if `True`, all values must be evaluatable by `eval()`
         - `only_keys`: only keys specified by `only_keys` are allowed in `file_pth`
         - `need_keys`: keys that specified by `need_keys` must exist in `file_pth`
 
         ## Exceptions
+        - `ValueError`: if `file_pth` is not a .txt file
+        - `FileNotFoundError`: if `file_pth` is not a file
         - `AttributeError`: if trying to access a nonexistent key
         - see `self.parse` exceptions
 
         ## Demo 1
         >>> kc = KeyCrate('config.txt', eval_value=True)
         >>> fps = kc.fps  # or kc['fps']
         >>> output_dir = kc['output folder']
 
         ## Demo 2
         >>> settings = KeyCrate('settings.txt', key_is_var=True, only_keys=['fps', 'dur'])
         >>> fps = settings.fps
         >>> dur = settings.dur
         """
 
+        ## keycrate file should be a .txt file
+        if not file_pth.endswith('.txt'):
+            raise ValueError(f'KeyCrate file {repr(file_pth)} should be a .txt file.')
+
+        ## keycrate file must exist
+        if not _os.path.isfile(file_pth):
+            raise FileNotFoundError(f'KeyCrate file {repr(file_pth)} is not found.')
+
         ## added the prefix "_kc__" to prevent conflicts with the keys
         self._kc__file_pth = file_pth
         self._kc__key_is_var = key_is_var
         self._kc__eval_value = eval_value
         self._kc__only_keys = only_keys
         self._kc__need_keys = need_keys
 
@@ -168,8 +180,19 @@
                 raise AssertionError(
                     f'KeyCrate file {repr(self._kc__file_pth)} is missing keys: '
                     + ', '.join(map(repr, _need_keys))
                 )
 
     def open(self) -> None:
         """open the .txt file"""
-        _open_file(self._kc__file_pth)
+        _open_file(self._kc__file_pth)
+    
+    def export(self) -> _Dict[str, _Any]:
+        """Return all the key-value pairs as dictionary."""
+
+        force_copy = eval(str(self.__dict__), {})  # not sure gonna copy all the things deeply
+
+        out = {
+            key: force_copy[key]
+            for key in filter(lambda key: not key.startswith('_kc__'), force_copy.keys())
+        }
+        return out
```

### Comparing `mykit-2.0.4/mykit/kit/math.py` & `mykit-3.0.0/mykit/kit/math.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/neuralnet/dense.py` & `mykit-3.0.0/mykit/kit/neuralnet/dense.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/neuralnet/genetic.py` & `mykit-3.0.0/mykit/kit/neuralnet/genetic.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/noise.py` & `mykit-3.0.0/mykit/kit/noise.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/path.py` & `mykit-3.0.0/mykit/kit/path.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/time.py` & `mykit-3.0.0/mykit/kit/time.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit/kit/utils.py` & `mykit-3.0.0/mykit/kit/utils.py`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/mykit.egg-info/PKG-INFO` & `mykit-3.0.0/mykit.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mykit
-Version: 2.0.4
+Version: 3.0.0
 Summary: Python utility library
 Home-page: https://nvfp.github.io/mykit
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/mykit/docs
 Project-URL: report bugs, https://github.com/nvfp/mykit/issues
@@ -61,16 +61,22 @@
 ## FAQ
 
 - 
 
 
 ## Changelog
 
+- 3.0.0 (June 17, 2023):
+    - Breaking changes:
+        - Changed `title` arg to `name` in `.app.App`
+        - Now `/kit/keycrate` must be a .txt file, and the file must exist
+        - Added `export` method to `.kit.keycrate.KeyCrate`
+    - Added test suite for `.kit.keycrate.KeyCrate`
 - 2.0.4 (June 16, 2023):
-    - Now `move` method of `Button`, `Label`, `_Slider` and will return self
+    - Now `move` method of `Button`, `Label`, and `_Slider` will return self
 - 2.0.3 (June 16, 2023):
     - Now `.app.complex.plot.Plot` and `.app.complex.plot.Biplot` can be used even if no points is specified
     - Added `add_background_processes` to `.app.App`
 - 2.0.2 (June 14, 2023):
     - finished updating all type hints
     - Added visibility functionality to `/app/complex/plot.py`
 - 2.0.1 (June 14, 2023):
```

### Comparing `mykit-2.0.4/mykit.egg-info/SOURCES.txt` & `mykit-3.0.0/mykit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mykit-2.0.4/pyproject.toml` & `mykit-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mykit"
-version = "2.0.4"
+version = "3.0.0"
 description = "Python utility library"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

