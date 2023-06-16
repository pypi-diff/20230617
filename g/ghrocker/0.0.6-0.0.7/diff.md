# Comparing `tmp/ghrocker-0.0.6.tar.gz` & `tmp/ghrocker-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ghrocker-0.0.6.tar", last modified: Thu Feb 16 21:18:08 2023, max compression
+gzip compressed data, was "ghrocker-0.0.7.tar", last modified: Fri Jun 16 22:08:10 2023, max compression
```

## Comparing `ghrocker-0.0.6.tar` & `ghrocker-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-02-16 21:18:08.000000 ghrocker-0.0.6/
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      920 2023-02-16 21:15:45.000000 ghrocker-0.0.6/setup.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)    11358 2022-02-14 07:24:45.000000 ghrocker-0.0.6/LICENSE
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      333 2022-02-14 07:24:45.000000 ghrocker-0.0.6/README.md
--rw-r--r--   0 tfoote    (1000) tfoote    (1000)       38 2023-02-16 21:18:08.000000 ghrocker-0.0.6/setup.cfg
-drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-02-16 21:18:08.000000 ghrocker-0.0.6/src/
-drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-02-16 21:18:08.000000 ghrocker-0.0.6/src/ghrocker.egg-info/
--rw-r--r--   0 tfoote    (1000) tfoote    (1000)        1 2023-02-16 21:18:07.000000 ghrocker-0.0.6/src/ghrocker.egg-info/not-zip-safe
--rw-r--r--   0 tfoote    (1000) tfoote    (1000)      119 2023-02-16 21:18:07.000000 ghrocker-0.0.6/src/ghrocker.egg-info/entry_points.txt
--rw-r--r--   0 tfoote    (1000) tfoote    (1000)        1 2023-02-16 21:18:07.000000 ghrocker-0.0.6/src/ghrocker.egg-info/dependency_links.txt
--rw-r--r--   0 tfoote    (1000) tfoote    (1000)      416 2023-02-16 21:18:07.000000 ghrocker-0.0.6/src/ghrocker.egg-info/SOURCES.txt
--rw-r--r--   0 tfoote    (1000) tfoote    (1000)      651 2023-02-16 21:18:07.000000 ghrocker-0.0.6/src/ghrocker.egg-info/PKG-INFO
--rw-r--r--   0 tfoote    (1000) tfoote    (1000)       12 2023-02-16 21:18:07.000000 ghrocker-0.0.6/src/ghrocker.egg-info/requires.txt
--rw-r--r--   0 tfoote    (1000) tfoote    (1000)        9 2023-02-16 21:18:07.000000 ghrocker-0.0.6/src/ghrocker.egg-info/top_level.txt
-drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-02-16 21:18:08.000000 ghrocker-0.0.6/src/ghrocker/
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2669 2023-02-16 21:14:23.000000 ghrocker-0.0.6/src/ghrocker/ghrocker.py
-drwxr-xr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-02-16 21:18:08.000000 ghrocker-0.0.6/src/ghrocker/templates/
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      363 2023-02-16 21:14:38.000000 ghrocker-0.0.6/src/ghrocker/templates/ghpages_snippet.Dockerfile.em
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1661 2023-01-04 08:10:46.000000 ghrocker-0.0.6/src/ghrocker/ghpages_extension.py
--rw-rw-r--   0 tfoote    (1000) tfoote    (1000)        0 2022-02-14 07:24:45.000000 ghrocker-0.0.6/src/ghrocker/__init__.py
--rw-r--r--   0 tfoote    (1000) tfoote    (1000)      651 2023-02-16 21:18:08.000000 ghrocker-0.0.6/PKG-INFO
+drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-06-16 22:08:10.065273 ghrocker-0.0.7/
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      776 2023-06-16 22:08:10.065273 ghrocker-0.0.7/PKG-INFO
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      333 2023-06-16 21:46:59.000000 ghrocker-0.0.7/README.md
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)       38 2023-06-16 22:08:10.065273 ghrocker-0.0.7/setup.cfg
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      920 2023-06-16 22:06:34.000000 ghrocker-0.0.7/setup.py
+drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-06-16 22:08:10.065273 ghrocker-0.0.7/src/
+drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-06-16 22:08:10.065273 ghrocker-0.0.7/src/ghrocker/
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)        0 2023-06-16 21:46:59.000000 ghrocker-0.0.7/src/ghrocker/__init__.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     1661 2023-06-16 21:46:59.000000 ghrocker-0.0.7/src/ghrocker/ghpages_extension.py
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)     2669 2023-06-16 21:46:59.000000 ghrocker-0.0.7/src/ghrocker/ghrocker.py
+drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-06-16 22:08:10.065273 ghrocker-0.0.7/src/ghrocker/templates/
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      441 2023-06-16 22:04:03.000000 ghrocker-0.0.7/src/ghrocker/templates/ghpages_snippet.Dockerfile.em
+drwxrwxr-x   0 tfoote    (1000) tfoote    (1000)        0 2023-06-16 22:08:10.065273 ghrocker-0.0.7/src/ghrocker.egg-info/
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      776 2023-06-16 22:08:10.000000 ghrocker-0.0.7/src/ghrocker.egg-info/PKG-INFO
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      408 2023-06-16 22:08:10.000000 ghrocker-0.0.7/src/ghrocker.egg-info/SOURCES.txt
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)        1 2023-06-16 22:08:10.000000 ghrocker-0.0.7/src/ghrocker.egg-info/dependency_links.txt
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)      119 2023-06-16 22:08:10.000000 ghrocker-0.0.7/src/ghrocker.egg-info/entry_points.txt
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)        1 2023-06-16 22:06:12.000000 ghrocker-0.0.7/src/ghrocker.egg-info/not-zip-safe
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)       12 2023-06-16 22:08:10.000000 ghrocker-0.0.7/src/ghrocker.egg-info/requires.txt
+-rw-rw-r--   0 tfoote    (1000) tfoote    (1000)        9 2023-06-16 22:08:10.000000 ghrocker-0.0.7/src/ghrocker.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ghrocker-0.0.6/setup.py` & `ghrocker-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='ghrocker',
-    version="0.0.6",
+    version="0.0.7",
     packages=['ghrocker'],
     package_dir={'': 'src'},
     package_data={'ghrocker': ['templates/*.em']},
     author="Tully Foote",
     author_email="tfoote@osrfoundation.org",
     description="A rocker extension to locally test github pages.",
     long_description=long_description,
```

### Comparing `ghrocker-0.0.6/src/ghrocker/ghrocker.py` & `ghrocker-0.0.7/src/ghrocker/ghrocker.py`

 * *Files identical despite different names*

### Comparing `ghrocker-0.0.6/src/ghrocker/ghpages_extension.py` & `ghrocker-0.0.7/src/ghrocker/ghpages_extension.py`

 * *Files identical despite different names*

