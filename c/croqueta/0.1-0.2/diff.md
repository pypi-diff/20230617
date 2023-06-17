# Comparing `tmp/croqueta-0.1.tar.gz` & `tmp/croqueta-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croqueta-0.1.tar", last modified: Wed Mar 30 12:55:43 2022, max compression
+gzip compressed data, was "croqueta-0.2.tar", last modified: Sat Jun 17 09:32:42 2023, max compression
```

## Comparing `croqueta-0.1.tar` & `croqueta-0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2022-03-30 12:55:43.015675 croqueta-0.1/
--rw-r--r--   0 juanluis   (502) staff       (20)    11357 2022-03-30 10:50:05.000000 croqueta-0.1/LICENSE
--rw-r--r--   0 juanluis   (502) staff       (20)      342 2022-03-30 12:55:43.015755 croqueta-0.1/PKG-INFO
--rw-r--r--   0 juanluis   (502) staff       (20)       10 2022-03-30 12:47:58.000000 croqueta-0.1/README.md
-drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2022-03-30 12:55:43.015008 croqueta-0.1/croqueta/
--rw-r--r--   0 juanluis   (502) staff       (20)       37 2022-03-30 12:46:27.000000 croqueta-0.1/croqueta/__init__.py
--rw-r--r--   0 juanluis   (502) staff       (20)      758 2022-03-30 12:31:46.000000 croqueta-0.1/croqueta/pandas.py
-drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2022-03-30 12:55:43.015571 croqueta-0.1/croqueta.egg-info/
--rw-r--r--   0 juanluis   (502) staff       (20)      342 2022-03-30 12:55:42.000000 croqueta-0.1/croqueta.egg-info/PKG-INFO
--rw-r--r--   0 juanluis   (502) staff       (20)      204 2022-03-30 12:55:42.000000 croqueta-0.1/croqueta.egg-info/SOURCES.txt
--rw-r--r--   0 juanluis   (502) staff       (20)        1 2022-03-30 12:55:42.000000 croqueta-0.1/croqueta.egg-info/dependency_links.txt
--rw-r--r--   0 juanluis   (502) staff       (20)        9 2022-03-30 12:55:42.000000 croqueta-0.1/croqueta.egg-info/top_level.txt
--rw-r--r--   0 juanluis   (502) staff       (20)      103 2022-03-30 12:55:43.016140 croqueta-0.1/setup.cfg
--rw-r--r--   0 juanluis   (502) staff       (20)      671 2022-03-30 12:48:46.000000 croqueta-0.1/setup.py
+drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 09:32:42.362080 croqueta-0.2/
+-rw-r--r--   0 juanluis   (502) staff       (20)    11357 2022-03-30 10:50:05.000000 croqueta-0.2/LICENSE
+-rw-r--r--   0 juanluis   (502) staff       (20)      398 2023-06-17 09:32:42.362171 croqueta-0.2/PKG-INFO
+-rw-r--r--   0 juanluis   (502) staff       (20)       66 2023-06-17 09:32:29.000000 croqueta-0.2/README.md
+drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 09:32:42.361211 croqueta-0.2/croqueta/
+-rw-r--r--   0 juanluis   (502) staff       (20)      172 2023-06-17 09:25:20.000000 croqueta-0.2/croqueta/__init__.py
+-rw-r--r--   0 juanluis   (502) staff       (20)     1321 2023-06-17 09:24:30.000000 croqueta-0.2/croqueta/obj.py
+-rw-r--r--   0 juanluis   (502) staff       (20)     9056 2022-03-30 14:37:52.000000 croqueta-0.2/croqueta/pandas.py
+-rw-r--r--   0 juanluis   (502) staff       (20)      787 2023-06-17 09:24:36.000000 croqueta-0.2/croqueta/str.py
+-rw-r--r--   0 juanluis   (502) staff       (20)     1126 2023-06-17 09:22:55.000000 croqueta-0.2/croqueta/viz.py
+drwxr-xr-x   0 juanluis   (502) staff       (20)        0 2023-06-17 09:32:42.361946 croqueta-0.2/croqueta.egg-info/
+-rw-r--r--   0 juanluis   (502) staff       (20)      398 2023-06-17 09:32:42.000000 croqueta-0.2/croqueta.egg-info/PKG-INFO
+-rw-r--r--   0 juanluis   (502) staff       (20)      252 2023-06-17 09:32:42.000000 croqueta-0.2/croqueta.egg-info/SOURCES.txt
+-rw-r--r--   0 juanluis   (502) staff       (20)        1 2023-06-17 09:32:42.000000 croqueta-0.2/croqueta.egg-info/dependency_links.txt
+-rw-r--r--   0 juanluis   (502) staff       (20)        9 2023-06-17 09:32:42.000000 croqueta-0.2/croqueta.egg-info/top_level.txt
+-rw-r--r--   0 juanluis   (502) staff       (20)      103 2023-06-17 09:32:42.362494 croqueta-0.2/setup.cfg
+-rw-r--r--   0 juanluis   (502) staff       (20)      671 2023-06-17 09:25:44.000000 croqueta-0.2/setup.py
```

### Comparing `croqueta-0.1/LICENSE` & `croqueta-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `croqueta-0.1/setup.py` & `croqueta-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="croqueta", # Replace with your own username
-    version="0.1",
+    version="0.2",
     author="juanluisrto",
     author_email="juanluis.rto@gmail.com",
     description="A bunch of utilities to code even faster.",
     url="https://github.com/juanluisrto/croqueta",
     packages= setuptools.find_packages(),
     python_requires='>=3.8',
     include_package_data=True,
```

