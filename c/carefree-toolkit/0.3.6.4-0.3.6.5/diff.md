# Comparing `tmp/carefree-toolkit-0.3.6.4.tar.gz` & `tmp/carefree-toolkit-0.3.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-toolkit-0.3.6.4.tar", last modified: Sat Jun 17 03:37:11 2023, max compression
+gzip compressed data, was "carefree-toolkit-0.3.6.5.tar", last modified: Sat Jun 17 13:29:45 2023, max compression
```

## Comparing `carefree-toolkit-0.3.6.4.tar` & `carefree-toolkit-0.3.6.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 03:37:11.424605 carefree-toolkit-0.3.6.4/
--rw-rw-rw-   0        0        0     1090 2019-09-25 20:51:10.000000 carefree-toolkit-0.3.6.4/LICENSE
--rw-rw-rw-   0        0        0     9010 2023-06-17 03:37:11.420615 carefree-toolkit-0.3.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     8579 2022-06-27 01:36:51.000000 carefree-toolkit-0.3.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 03:37:11.340762 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/
--rw-rw-rw-   0        0        0     9010 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-17 03:37:11.000000 carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-17 03:37:11.406588 carefree-toolkit-0.3.6.4/cftool/
--rw-rw-rw-   0        0        0        0 2020-11-05 10:59:33.000000 carefree-toolkit-0.3.6.4/cftool/__init__.py
--rw-rw-rw-   0        0        0    22677 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/array.py
--rw-rw-rw-   0        0        0       58 2023-05-18 01:18:59.000000 carefree-toolkit-0.3.6.4/cftool/constants.py
--rw-rw-rw-   0        0        0     8445 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/cv.py
--rw-rw-rw-   0        0        0    17747 2023-06-17 03:34:51.000000 carefree-toolkit-0.3.6.4/cftool/data_structures.py
-drwxrwxrwx   0        0        0        0 2023-06-17 03:37:11.414632 carefree-toolkit-0.3.6.4/cftool/dist/
--rw-rw-rw-   0        0        0       28 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/dist/__init__.py
--rw-rw-rw-   0        0        0    21842 2022-08-08 17:03:13.000000 carefree-toolkit-0.3.6.4/cftool/dist/core.py
--rw-rw-rw-   0        0        0     9983 2023-06-05 15:51:28.000000 carefree-toolkit-0.3.6.4/cftool/geometry.py
--rw-rw-rw-   0        0        0    25320 2022-08-08 17:03:13.000000 carefree-toolkit-0.3.6.4/cftool/manage.py
--rw-rw-rw-   0        0        0    85083 2023-05-18 01:18:59.000000 carefree-toolkit-0.3.6.4/cftool/misc.py
--rw-rw-rw-   0        0        0     6451 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/pipeline.py
--rw-rw-rw-   0        0        0     1004 2023-04-03 14:14:29.000000 carefree-toolkit-0.3.6.4/cftool/types.py
--rw-rw-rw-   0        0        0     2237 2023-05-18 01:18:59.000000 carefree-toolkit-0.3.6.4/cftool/web.py
--rw-rw-rw-   0        0        0       42 2023-06-17 03:37:11.425601 carefree-toolkit-0.3.6.4/setup.cfg
--rw-rw-rw-   0        0        0      905 2023-06-17 03:37:04.000000 carefree-toolkit-0.3.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:29:45.253143 carefree-toolkit-0.3.6.5/
+-rw-rw-rw-   0        0        0     1090 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/LICENSE
+-rw-rw-rw-   0        0        0     9010 2023-06-17 13:29:45.253143 carefree-toolkit-0.3.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8579 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 13:29:45.246160 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     9010 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 13:29:45.000000 carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 13:29:45.251636 carefree-toolkit-0.3.6.5/cftool/
+-rw-rw-rw-   0        0        0        0 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/cftool/__init__.py
+-rw-rw-rw-   0        0        0    22677 2023-03-28 02:09:10.000000 carefree-toolkit-0.3.6.5/cftool/array.py
+-rw-rw-rw-   0        0        0       58 2023-05-17 12:47:47.000000 carefree-toolkit-0.3.6.5/cftool/constants.py
+-rw-rw-rw-   0        0        0     8445 2023-03-28 02:09:18.000000 carefree-toolkit-0.3.6.5/cftool/cv.py
+-rw-rw-rw-   0        0        0    17747 2023-06-17 08:20:53.000000 carefree-toolkit-0.3.6.5/cftool/data_structures.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:29:45.251636 carefree-toolkit-0.3.6.5/cftool/dist/
+-rw-rw-rw-   0        0        0       28 2023-03-05 03:09:06.000000 carefree-toolkit-0.3.6.5/cftool/dist/__init__.py
+-rw-rw-rw-   0        0        0    21842 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/cftool/dist/core.py
+-rw-rw-rw-   0        0        0     9983 2023-05-31 06:56:25.000000 carefree-toolkit-0.3.6.5/cftool/geometry.py
+-rw-rw-rw-   0        0        0    25320 2023-01-17 02:58:51.000000 carefree-toolkit-0.3.6.5/cftool/manage.py
+-rw-rw-rw-   0        0        0    85225 2023-06-17 13:29:03.000000 carefree-toolkit-0.3.6.5/cftool/misc.py
+-rw-rw-rw-   0        0        0     6451 2023-03-21 11:08:09.000000 carefree-toolkit-0.3.6.5/cftool/pipeline.py
+-rw-rw-rw-   0        0        0     1004 2023-03-28 02:09:02.000000 carefree-toolkit-0.3.6.5/cftool/types.py
+-rw-rw-rw-   0        0        0     2237 2023-05-17 12:54:11.000000 carefree-toolkit-0.3.6.5/cftool/web.py
+-rw-rw-rw-   0        0        0       42 2023-06-17 13:29:45.253143 carefree-toolkit-0.3.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      905 2023-06-17 13:29:43.000000 carefree-toolkit-0.3.6.5/setup.py
```

### Comparing `carefree-toolkit-0.3.6.4/LICENSE` & `carefree-toolkit-0.3.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/PKG-INFO` & `carefree-toolkit-0.3.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-toolkit
-Version: 0.3.6.4
+Version: 0.3.6.5
 Summary: Some commonly used functions and modules
 Home-page: https://github.com/carefree0910/carefree-toolkit
-Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.4.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.5.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python numpy data-science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-toolkit
```

### Comparing `carefree-toolkit-0.3.6.4/README.md` & `carefree-toolkit-0.3.6.5/README.md`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/carefree_toolkit.egg-info/PKG-INFO` & `carefree-toolkit-0.3.6.5/carefree_toolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-toolkit
-Version: 0.3.6.4
+Version: 0.3.6.5
 Summary: Some commonly used functions and modules
 Home-page: https://github.com/carefree0910/carefree-toolkit
-Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.4.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-toolkit/archive/v0.3.6.5.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python numpy data-science
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # carefree-toolkit
```

### Comparing `carefree-toolkit-0.3.6.4/cftool/array.py` & `carefree-toolkit-0.3.6.5/cftool/array.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/cftool/cv.py` & `carefree-toolkit-0.3.6.5/cftool/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/cftool/data_structures.py` & `carefree-toolkit-0.3.6.5/cftool/data_structures.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/cftool/dist/core.py` & `carefree-toolkit-0.3.6.5/cftool/dist/core.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/cftool/geometry.py` & `carefree-toolkit-0.3.6.5/cftool/geometry.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/cftool/manage.py` & `carefree-toolkit-0.3.6.5/cftool/manage.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/cftool/misc.py` & `carefree-toolkit-0.3.6.5/cftool/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,19 +299,22 @@
 def prefix_dict(d: Dict[str, Any], prefix: str):
     """Prefix every key in dict `d` with `prefix`."""
 
     return {f"{prefix}_{k}": v for k, v in d.items()}
 
 
 def shallow_copy_dict(d: dict) -> dict:
-    d = d.copy()
-    for k, v in d.items():
-        if isinstance(v, dict):
-            d[k] = shallow_copy_dict(v)
-    return d
+    def _copy(d_: Union[dict, list]) -> Union[dict, list]:
+        if isinstance(d_, list):
+            return [_copy(item) for item in d_]
+        if isinstance(d_, dict):
+            return {k: _copy(v) for k, v in d_.items()}
+        return d_
+
+    return _copy(d)
 
 
 def update_dict(src_dict: dict, tgt_dict: dict) -> dict:
     """
     Update tgt_dict with src_dict.
     * Notice that changes will happen only on keys which src_dict holds.
```

### Comparing `carefree-toolkit-0.3.6.4/cftool/pipeline.py` & `carefree-toolkit-0.3.6.5/cftool/pipeline.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/cftool/types.py` & `carefree-toolkit-0.3.6.5/cftool/types.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/cftool/web.py` & `carefree-toolkit-0.3.6.5/cftool/web.py`

 * *Files identical despite different names*

### Comparing `carefree-toolkit-0.3.6.4/setup.py` & `carefree-toolkit-0.3.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.3.6.4"
+VERSION = "0.3.6.5"
 
 DESCRIPTION = "Some commonly used functions and modules"
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 INSTALL_REQUIRES = [
     "dill",
```

