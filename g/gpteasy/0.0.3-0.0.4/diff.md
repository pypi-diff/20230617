# Comparing `tmp/gpteasy-0.0.3.tar.gz` & `tmp/gpteasy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpteasy-0.0.3.tar", last modified: Sat Jun 17 08:31:51 2023, max compression
+gzip compressed data, was "gpteasy-0.0.4.tar", last modified: Sat Jun 17 09:11:53 2023, max compression
```

## Comparing `gpteasy-0.0.3.tar` & `gpteasy-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 08:31:51.182370 gpteasy-0.0.3/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-0.0.3/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)     5686 2023-06-17 08:31:51.181780 gpteasy-0.0.3/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     3833 2023-06-17 08:31:40.000000 gpteasy-0.0.3/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 08:31:51.176741 gpteasy-0.0.3/gpteasy/
--rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-0.0.3/gpteasy/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4289 2023-06-16 09:38:51.000000 gpteasy-0.0.3/gpteasy/commands.py
--rw-r--r--   0 hp         (501) staff       (20)     5919 2023-03-24 22:31:36.000000 gpteasy-0.0.3/gpteasy/day.py
--rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-0.0.3/gpteasy/display.py
--rw-r--r--   0 hp         (501) staff       (20)    12500 2023-06-17 08:13:14.000000 gpteasy-0.0.3/gpteasy/gpt.py
--rw-r--r--   0 hp         (501) staff       (20)     2365 2022-10-11 21:46:52.000000 gpteasy-0.0.3/gpteasy/period.py
--rw-r--r--   0 hp         (501) staff       (20)     1192 2023-06-16 09:38:41.000000 gpteasy-0.0.3/gpteasy/repl.py
--rw-r--r--   0 hp         (501) staff       (20)     3757 2023-06-16 09:08:00.000000 gpteasy-0.0.3/gpteasy/settings.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 08:31:51.180885 gpteasy-0.0.3/gpteasy.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     5686 2023-06-17 08:31:51.000000 gpteasy-0.0.3/gpteasy.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      329 2023-06-17 08:31:51.000000 gpteasy-0.0.3/gpteasy.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 08:31:51.000000 gpteasy-0.0.3/gpteasy.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)       52 2023-06-17 08:31:51.000000 gpteasy-0.0.3/gpteasy.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 08:31:51.000000 gpteasy-0.0.3/gpteasy.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)     1066 2023-06-17 08:31:40.000000 gpteasy-0.0.3/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 08:31:51.182521 gpteasy-0.0.3/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 09:11:53.758711 gpteasy-0.0.4/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 gpteasy-0.0.4/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 09:11:53.758383 gpteasy-0.0.4/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     3335 2023-06-17 09:11:45.000000 gpteasy-0.0.4/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 09:11:53.755452 gpteasy-0.0.4/gpteasy/
+-rw-r--r--   0 hp         (501) staff       (20)      118 2023-06-16 09:28:57.000000 gpteasy-0.0.4/gpteasy/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4289 2023-06-16 09:38:51.000000 gpteasy-0.0.4/gpteasy/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)      572 2023-06-16 09:08:00.000000 gpteasy-0.0.4/gpteasy/display.py
+-rw-r--r--   0 hp         (501) staff       (20)    12500 2023-06-17 08:13:14.000000 gpteasy-0.0.4/gpteasy/gpt.py
+-rw-r--r--   0 hp         (501) staff       (20)     1192 2023-06-16 09:38:41.000000 gpteasy-0.0.4/gpteasy/repl.py
+-rw-r--r--   0 hp         (501) staff       (20)     3757 2023-06-16 09:08:00.000000 gpteasy-0.0.4/gpteasy/settings.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2023-06-17 09:11:53.757880 gpteasy-0.0.4/gpteasy.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     5188 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      296 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)       52 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        8 2023-06-17 09:11:53.000000 gpteasy-0.0.4/gpteasy.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)     1066 2023-06-17 09:11:45.000000 gpteasy-0.0.4/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2023-06-17 09:11:53.758804 gpteasy-0.0.4/setup.cfg
```

### Comparing `gpteasy-0.0.3/LICENSE` & `gpteasy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gpteasy-0.0.3/gpteasy/commands.py` & `gpteasy-0.0.4/gpteasy/commands.py`

 * *Files identical despite different names*

### Comparing `gpteasy-0.0.3/gpteasy/display.py` & `gpteasy-0.0.4/gpteasy/display.py`

 * *Files identical despite different names*

### Comparing `gpteasy-0.0.3/gpteasy/gpt.py` & `gpteasy-0.0.4/gpteasy/gpt.py`

 * *Files identical despite different names*

### Comparing `gpteasy-0.0.3/gpteasy/repl.py` & `gpteasy-0.0.4/gpteasy/repl.py`

 * *Files identical despite different names*

### Comparing `gpteasy-0.0.3/gpteasy/settings.py` & `gpteasy-0.0.4/gpteasy/settings.py`

 * *Files identical despite different names*

### Comparing `gpteasy-0.0.3/pyproject.toml` & `gpteasy-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpteasy"
-version = "0.0.3"
+version = "0.0.4"
 description = "Makes working with OpenAi's GPT API super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

