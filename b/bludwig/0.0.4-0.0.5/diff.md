# Comparing `tmp/bludwig-0.0.4.tar.gz` & `tmp/bludwig-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bludwig-0.0.4.tar", last modified: Wed Jun 14 04:33:37 2023, max compression
+gzip compressed data, was "bludwig-0.0.5.tar", last modified: Sat Jun 17 19:40:01 2023, max compression
```

## Comparing `bludwig-0.0.4.tar` & `bludwig-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:33:37.167999 bludwig-0.0.4/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bludwig-0.0.4/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)      488 2023-06-14 04:33:37.167999 bludwig-0.0.4/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)       58 2023-06-14 04:32:55.000000 bludwig-0.0.4/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1124 2023-06-14 04:32:40.000000 bludwig-0.0.4/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-14 04:33:37.167999 bludwig-0.0.4/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:33:37.163999 bludwig-0.0.4/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:33:37.167999 bludwig-0.0.4/src/bludwig/
--rw-r--r--   0 me        (1000) me        (1000)    13727 2023-06-13 20:10:46.000000 bludwig-0.0.4/src/bludwig/LudwigJob.py
--rw-r--r--   0 me        (1000) me        (1000)       82 2023-06-11 18:48:52.000000 bludwig-0.0.4/src/bludwig/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      197 2023-06-10 09:59:04.000000 bludwig-0.0.4/src/bludwig/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)     3798 2023-06-11 20:20:52.000000 bludwig-0.0.4/src/bludwig/helper.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:33:37.167999 bludwig-0.0.4/src/bludwig.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)      488 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      339 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       50 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       17 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)        8 2023-06-14 04:33:37.000000 bludwig-0.0.4/src/bludwig.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 19:40:01.219388 bludwig-0.0.5/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 bludwig-0.0.5/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)      488 2023-06-17 19:40:01.219388 bludwig-0.0.5/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)       58 2023-06-17 19:38:54.000000 bludwig-0.0.5/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1124 2023-06-17 19:38:03.000000 bludwig-0.0.5/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-17 19:40:01.219388 bludwig-0.0.5/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 19:40:01.199388 bludwig-0.0.5/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 19:40:01.219388 bludwig-0.0.5/src/bludwig/
+-rw-r--r--   0 me        (1000) me        (1000)    13727 2023-06-13 20:10:46.000000 bludwig-0.0.5/src/bludwig/LudwigJob.py
+-rw-r--r--   0 me        (1000) me        (1000)       82 2023-06-11 18:48:52.000000 bludwig-0.0.5/src/bludwig/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      197 2023-06-10 09:59:04.000000 bludwig-0.0.5/src/bludwig/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)    16867 2023-06-17 14:54:42.000000 bludwig-0.0.5/src/bludwig/helper.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 19:40:01.219388 bludwig-0.0.5/src/bludwig.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)      488 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/PKG-INFO
+-rw-rw-r--   0 me        (1000) me        (1000)      339 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/SOURCES.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        1 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/dependency_links.txt
+-rw-rw-r--   0 me        (1000) me        (1000)       50 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       17 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/requires.txt
+-rw-rw-r--   0 me        (1000) me        (1000)        8 2023-06-17 19:40:01.000000 bludwig-0.0.5/src/bludwig.egg-info/top_level.txt
```

### Comparing `bludwig-0.0.4/LICENSE` & `bludwig-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bludwig-0.0.4/pyproject.toml` & `bludwig-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyproject.toml
 
 
 [project]
 name            = "bludwig"
-version         = "0.0.4"        
+version         = "0.0.5"        
 
 requires-python = ">=3.9"
 dependencies    = ['pandasklar','munch']
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
 description     = "Some helper for Ludwig AI"
 readme          = "README.md"
```

### Comparing `bludwig-0.0.4/src/bludwig/LudwigJob.py` & `bludwig-0.0.5/src/bludwig/LudwigJob.py`

 * *Files identical despite different names*

