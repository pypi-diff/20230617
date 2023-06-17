# Comparing `tmp/pygrb_lc-0.0.2.tar.gz` & `tmp/pygrb_lc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrb_lc-0.0.2.tar", last modified: Sat Jun 17 10:38:38 2023, max compression
+gzip compressed data, was "pygrb_lc-0.0.6.tar", last modified: Sat Jun 17 11:11:27 2023, max compression
```

## Comparing `pygrb_lc-0.0.2.tar` & `pygrb_lc-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 georgiy    (501) staff       (20)        0 2023-06-17 10:38:38.033595 pygrb_lc-0.0.2/
--rw-r--r--   0 georgiy    (501) staff       (20)     1073 2023-06-06 22:50:33.000000 pygrb_lc-0.0.2/LICENSE
--rw-r--r--   0 georgiy    (501) staff       (20)      687 2023-06-17 10:38:38.033703 pygrb_lc-0.0.2/PKG-INFO
--rw-r--r--   0 georgiy    (501) staff       (20)      176 2023-06-06 22:50:33.000000 pygrb_lc-0.0.2/README.md
--rw-r--r--   0 georgiy    (501) staff       (20)      182 2023-06-17 09:45:37.000000 pygrb_lc-0.0.2/pyproject.toml
--rw-r--r--   0 georgiy    (501) staff       (20)      669 2023-06-17 10:38:38.033995 pygrb_lc-0.0.2/setup.cfg
--rw-r--r--   0 georgiy    (501) staff       (20)       68 2023-06-17 09:38:49.000000 pygrb_lc-0.0.2/setup.py
-drwxr-xr-x   0 georgiy    (501) staff       (20)        0 2023-06-17 10:38:38.029251 pygrb_lc-0.0.2/src/
-drwxr-xr-x   0 georgiy    (501) staff       (20)        0 2023-06-17 10:38:38.032318 pygrb_lc-0.0.2/src/pygrb_lc/
--rw-r--r--   0 georgiy    (501) staff       (20)        0 2023-06-06 22:50:33.000000 pygrb_lc-0.0.2/src/pygrb_lc/__init__.py
--rw-r--r--   0 georgiy    (501) staff       (20)     5315 2023-06-06 22:50:33.000000 pygrb_lc-0.0.2/src/pygrb_lc/blind_search.py
--rw-r--r--   0 georgiy    (501) staff       (20)     1416 2023-06-17 09:12:43.000000 pygrb_lc-0.0.2/src/pygrb_lc/config.py
--rw-r--r--   0 georgiy    (501) staff       (20)     1026 2023-06-06 22:50:33.000000 pygrb_lc-0.0.2/src/pygrb_lc/crossmatching.py
--rw-r--r--   0 georgiy    (501) staff       (20)     6266 2023-06-11 21:59:33.000000 pygrb_lc-0.0.2/src/pygrb_lc/furie.py
--rw-r--r--   0 georgiy    (501) staff       (20)    32935 2023-06-17 10:01:41.000000 pygrb_lc-0.0.2/src/pygrb_lc/light_curves.py
--rw-r--r--   0 georgiy    (501) staff       (20)     4155 2023-06-06 22:50:33.000000 pygrb_lc-0.0.2/src/pygrb_lc/time.py
--rw-r--r--   0 georgiy    (501) staff       (20)     2641 2023-06-06 22:50:33.000000 pygrb_lc-0.0.2/src/pygrb_lc/utils.py
-drwxr-xr-x   0 georgiy    (501) staff       (20)        0 2023-06-17 10:38:38.033043 pygrb_lc-0.0.2/src/pygrb_lc.egg-info/
--rw-r--r--   0 georgiy    (501) staff       (20)      687 2023-06-17 10:38:38.000000 pygrb_lc-0.0.2/src/pygrb_lc.egg-info/PKG-INFO
--rw-r--r--   0 georgiy    (501) staff       (20)      497 2023-06-17 10:38:38.000000 pygrb_lc-0.0.2/src/pygrb_lc.egg-info/SOURCES.txt
--rw-r--r--   0 georgiy    (501) staff       (20)        1 2023-06-17 10:38:38.000000 pygrb_lc-0.0.2/src/pygrb_lc.egg-info/dependency_links.txt
--rw-r--r--   0 georgiy    (501) staff       (20)       26 2023-06-17 10:38:38.000000 pygrb_lc-0.0.2/src/pygrb_lc.egg-info/requires.txt
--rw-r--r--   0 georgiy    (501) staff       (20)        9 2023-06-17 10:38:38.000000 pygrb_lc-0.0.2/src/pygrb_lc.egg-info/top_level.txt
-drwxr-xr-x   0 georgiy    (501) staff       (20)        0 2023-06-17 10:38:38.033348 pygrb_lc-0.0.2/tests/
--rw-r--r--   0 georgiy    (501) staff       (20)        0 2023-06-17 09:30:18.000000 pygrb_lc-0.0.2/tests/test_light_curves.py
--rw-r--r--   0 georgiy    (501) staff       (20)        0 2023-06-17 09:29:48.000000 pygrb_lc-0.0.2/tests/test_time.py
--rw-r--r--   0 georgiy    (501) staff       (20)      684 2023-06-17 09:35:05.000000 pygrb_lc-0.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:11:27.596065 pygrb_lc-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-17 11:11:27.596065 pygrb_lc-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-17 11:11:27.596065 pygrb_lc-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:11:27.588065 pygrb_lc-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:11:27.592065 pygrb_lc-0.0.6/src/pygrb_lc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/src/pygrb_lc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/src/pygrb_lc/blind_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/src/pygrb_lc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/src/pygrb_lc/crossmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/src/pygrb_lc/furie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32933 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/src/pygrb_lc/light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/src/pygrb_lc/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/src/pygrb_lc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:11:27.592065 pygrb_lc-0.0.6/src/pygrb_lc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-17 11:11:27.000000 pygrb_lc-0.0.6/src/pygrb_lc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-17 11:11:27.000000 pygrb_lc-0.0.6/src/pygrb_lc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 11:11:27.000000 pygrb_lc-0.0.6/src/pygrb_lc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-17 11:11:27.000000 pygrb_lc-0.0.6/src/pygrb_lc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 11:11:27.596065 pygrb_lc-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/tests/test_light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-17 11:11:18.000000 pygrb_lc-0.0.6/tests/test_utils.py
```

### Comparing `pygrb_lc-0.0.2/LICENSE` & `pygrb_lc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.2/setup.cfg` & `pygrb_lc-0.0.6/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 [metadata]
 name = pygrb_lc
-version = 0.0.2
+version = 0.0.6
 author = Mozgunov Georgiy
 author_email = georgiy99@bk.ru
 description = Python package for GRB analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/Jorezzz/pygrb
+url = https://github.com/Jorezzz/pygrb_lc
 project_urls = 
-	Bug Tracker = https://github.com/Jorezzz/pygrb/issues
+	Bug Tracker = https://github.com/Jorezzz/pygrb_lc/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
 
-[options.extras_require]
-test = 
-	pytest
-	pytest-cov
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pygrb_lc-0.0.2/src/pygrb_lc/blind_search.py` & `pygrb_lc-0.0.6/src/pygrb_lc/blind_search.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.2/src/pygrb_lc/config.py` & `pygrb_lc-0.0.6/src/pygrb_lc/config.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.2/src/pygrb_lc/crossmatching.py` & `pygrb_lc-0.0.6/src/pygrb_lc/crossmatching.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.2/src/pygrb_lc/furie.py` & `pygrb_lc-0.0.6/src/pygrb_lc/furie.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.2/src/pygrb_lc/light_curves.py` & `pygrb_lc-0.0.6/src/pygrb_lc/light_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 class SPI_ACS_LightCurve(LightCurve):
     '''
     Class for light curves from SPI-ACS/INTEGRAL
     '''
     def __init__(self, 
                  event_time: str,
                  duration: int, 
-                 loading_method: str = 'local',
+                 loading_method: str = 'web',
                  scale: str = 'utc',
                  **kwargs):
         '''
         Args:
             event_time (str): date and time of event in ISO 8601 format
             duration (int): duration of light curve in seconds
             loading_method (str, optional): 'local' or 'web'
```

### Comparing `pygrb_lc-0.0.2/src/pygrb_lc/time.py` & `pygrb_lc-0.0.6/src/pygrb_lc/time.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.2/src/pygrb_lc/utils.py` & `pygrb_lc-0.0.6/src/pygrb_lc/utils.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.0.2/tests/test_utils.py` & `pygrb_lc-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

