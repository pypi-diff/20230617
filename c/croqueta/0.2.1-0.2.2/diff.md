# Comparing `tmp/croqueta-0.2.1.tar.gz` & `tmp/croqueta-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croqueta-0.2.1.tar", last modified: Sat Jun 17 09:59:12 2023, max compression
+gzip compressed data, was "croqueta-0.2.2.tar", last modified: Sat Jun 17 16:23:06 2023, max compression
```

## Comparing `croqueta-0.2.1.tar` & `croqueta-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 09:59:12.911116 croqueta-0.2.1/
--rw-r--r--   0 juanluis   (502) staff       (20)    11357 2022-03-30 10:50:05.000000 croqueta-0.2.1/LICENSE
--rw-r--r--   0 juanluis   (502) staff       (20)      473 2023-06-17 09:59:12.911225 croqueta-0.2.1/PKG-INFO
--rw-r--r--   0 juanluis   (502) staff       (20)      139 2023-06-17 09:53:59.000000 croqueta-0.2.1/README.md
-drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 09:59:12.910436 croqueta-0.2.1/croqueta/
--rw-r--r--   0 juanluis   (502) staff       (20)      181 2023-06-17 09:38:35.000000 croqueta-0.2.1/croqueta/__init__.py
--rw-r--r--   0 juanluis   (502) staff       (20)     1321 2023-06-17 09:24:30.000000 croqueta-0.2.1/croqueta/obj.py
--rw-r--r--   0 juanluis   (502) staff       (20)     9056 2022-03-30 14:37:52.000000 croqueta-0.2.1/croqueta/pandas.py
--rw-r--r--   0 juanluis   (502) staff       (20)      764 2023-06-17 09:39:27.000000 croqueta-0.2.1/croqueta/str.py
--rw-r--r--   0 juanluis   (502) staff       (20)     1126 2023-06-17 09:22:55.000000 croqueta-0.2.1/croqueta/viz.py
-drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 09:59:12.910940 croqueta-0.2.1/croqueta.egg-info/
--rw-r--r--   0 juanluis   (502) staff       (20)      473 2023-06-17 09:59:12.000000 croqueta-0.2.1/croqueta.egg-info/PKG-INFO
--rw-r--r--   0 juanluis   (502) staff       (20)      252 2023-06-17 09:59:12.000000 croqueta-0.2.1/croqueta.egg-info/SOURCES.txt
--rw-r--r--   0 juanluis   (502) staff       (20)        1 2023-06-17 09:59:12.000000 croqueta-0.2.1/croqueta.egg-info/dependency_links.txt
--rw-r--r--   0 juanluis   (502) staff       (20)        9 2023-06-17 09:59:12.000000 croqueta-0.2.1/croqueta.egg-info/top_level.txt
--rw-r--r--   0 juanluis   (502) staff       (20)      103 2023-06-17 09:59:12.911541 croqueta-0.2.1/setup.cfg
--rw-r--r--   0 juanluis   (502) staff       (20)      673 2023-06-17 09:59:03.000000 croqueta-0.2.1/setup.py
+drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 16:23:06.957148 croqueta-0.2.2/
+-rw-r--r--   0 juanluis   (502) staff       (20)    11357 2022-03-30 10:50:05.000000 croqueta-0.2.2/LICENSE
+-rw-r--r--   0 juanluis   (502) staff       (20)      588 2023-06-17 16:23:06.957217 croqueta-0.2.2/PKG-INFO
+-rw-r--r--   0 juanluis   (502) staff       (20)      254 2023-06-17 16:17:55.000000 croqueta-0.2.2/README.md
+drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 16:23:06.956399 croqueta-0.2.2/croqueta/
+-rw-r--r--   0 juanluis   (502) staff       (20)      215 2023-06-17 16:07:12.000000 croqueta-0.2.2/croqueta/__init__.py
+-rw-r--r--   0 juanluis   (502) staff       (20)      879 2023-06-17 16:06:27.000000 croqueta-0.2.2/croqueta/maps.py
+-rw-r--r--   0 juanluis   (502) staff       (20)     1321 2023-06-17 09:24:30.000000 croqueta-0.2.2/croqueta/obj.py
+-rw-r--r--   0 juanluis   (502) staff       (20)     9806 2023-06-17 16:21:30.000000 croqueta-0.2.2/croqueta/pd.py
+-rw-r--r--   0 juanluis   (502) staff       (20)      764 2023-06-17 09:39:27.000000 croqueta-0.2.2/croqueta/str.py
+-rw-r--r--   0 juanluis   (502) staff       (20)     1162 2023-06-17 15:19:25.000000 croqueta-0.2.2/croqueta/viz.py
+drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 16:23:06.957039 croqueta-0.2.2/croqueta.egg-info/
+-rw-r--r--   0 juanluis   (502) staff       (20)      588 2023-06-17 16:23:06.000000 croqueta-0.2.2/croqueta.egg-info/PKG-INFO
+-rw-r--r--   0 juanluis   (502) staff       (20)      265 2023-06-17 16:23:06.000000 croqueta-0.2.2/croqueta.egg-info/SOURCES.txt
+-rw-r--r--   0 juanluis   (502) staff       (20)        1 2023-06-17 16:23:06.000000 croqueta-0.2.2/croqueta.egg-info/dependency_links.txt
+-rw-r--r--   0 juanluis   (502) staff       (20)        9 2023-06-17 16:23:06.000000 croqueta-0.2.2/croqueta.egg-info/top_level.txt
+-rw-r--r--   0 juanluis   (502) staff       (20)      103 2023-06-17 16:23:06.957474 croqueta-0.2.2/setup.cfg
+-rw-r--r--   0 juanluis   (502) staff       (20)      673 2023-06-17 16:07:46.000000 croqueta-0.2.2/setup.py
```

### Comparing `croqueta-0.2.1/LICENSE` & `croqueta-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `croqueta-0.2.1/croqueta/obj.py` & `croqueta-0.2.2/croqueta/obj.py`

 * *Files identical despite different names*

### Comparing `croqueta-0.2.1/croqueta/pandas.py` & `croqueta-0.2.2/croqueta/pd.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,30 @@
 import pandas as pd
 import numpy as np
 
 
 def filter_df(df, filter_dict, filter_type='and', filter_iterable_values = True):
     """
     Filter a dataframe with a dictionary of filters.
+
+    Args:
+        df (pandas.DataFrame): The dataframe to be filtered.
+        filter_dict (dict): A dictionary of filters, where the keys represent the column names
+            and the values represent the filter values.
+        filter_type (str, optional): The type of filter to apply. Valid values are 'and' (default) and 'or'.
+        filter_iterable_values (bool, optional): Determines whether iterable values should be treated as
+            multiple filter values. Defaults to True.
+
+    Returns:
+        pandas.DataFrame: The filtered dataframe.
+
+    Example:
+        df = pd.DataFrame({'A': [1, 2, 3, 4], 'B': ['x', 'y', 'z', 'w']})
+        filters = {'A': [2, 3], 'B': 'x'}
+        filtered_df = filter_df(df, filters, filter_type = "or")
     """
     views = []
     for key, value in filter_dict.items():
         if filter_iterable_values and not isinstance(value, str) and isinstance(value, Iterable):
             views.append(df[df[key].isin(value)])
         else:
             views.append(df[df[key] == value])
```

### Comparing `croqueta-0.2.1/croqueta/str.py` & `croqueta-0.2.2/croqueta/str.py`

 * *Files identical despite different names*

### Comparing `croqueta-0.2.1/croqueta/viz.py` & `croqueta-0.2.2/croqueta/viz.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from matplotlib.axes import Axes
 from pathlib import Path
 
-def savefig(fig, filename : str, path = None, size = None):
+def savefig(fig, filename : str, path = None, size = None, dpi: int =300):
     """
     Save a figure to a file.
 
     Parameters:
         - fig: The figure or axes object to save.
         - filename: The filename to save the figure as.
         - path: Optional. The directory path to save the figure in.
@@ -26,8 +26,9 @@
         path = Path()
     elif isinstance(path,str):
         path = Path(path)
     if not filename.endswith('.png'):
         filename = filename + '.png'
     if isinstance(size, tuple):
         fig.set_size_inches(size)
+    fig.set_dpi(dpi)
     fig.savefig(path / filename)
```

### Comparing `croqueta-0.2.1/setup.py` & `croqueta-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="croqueta", # Replace with your own username
-    version="0.2.1",
+    version="0.2.2",
     author="juanluisrto",
     author_email="juanluis.rto@gmail.com",
     description="A bunch of utilities to code even faster.",
     url="https://github.com/juanluisrto/croqueta",
     packages= setuptools.find_packages(),
     python_requires='>=3.8',
     include_package_data=True,
```

