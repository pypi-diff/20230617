# Comparing `tmp/pygame_ui_controls-1.0.0.tar.gz` & `tmp/pygame_ui_controls-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_ui_controls-1.0.0.tar", last modified: Sat Jun 17 07:22:18 2023, max compression
+gzip compressed data, was "pygame_ui_controls-1.0.1.tar", last modified: Sat Jun 17 07:36:07 2023, max compression
```

## Comparing `pygame_ui_controls-1.0.0.tar` & `pygame_ui_controls-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-17 07:22:18.307148 pygame_ui_controls-1.0.0/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    35149 2023-06-13 19:42:58.000000 pygame_ui_controls-1.0.0/LICENSE
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      659 2023-06-17 07:22:18.307148 pygame_ui_controls-1.0.0/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      478 2023-06-17 06:57:42.000000 pygame_ui_controls-1.0.0/README.md
--rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-17 07:22:18.307148 pygame_ui_controls-1.0.0/setup.cfg
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      789 2023-06-17 07:13:39.000000 pygame_ui_controls-1.0.0/setup.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-17 07:22:18.303148 pygame_ui_controls-1.0.0/src/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-14 20:26:51.000000 pygame_ui_controls-1.0.0/src/__init__.py
-drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-17 07:22:18.307148 pygame_ui_controls-1.0.0/src/pygame_ui_controls.egg-info/
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      659 2023-06-17 07:22:18.000000 pygame_ui_controls-1.0.0/src/pygame_ui_controls.egg-info/PKG-INFO
--rw-rw-r--   0 arthur    (1000) arthur    (1000)      290 2023-06-17 07:22:18.000000 pygame_ui_controls-1.0.0/src/pygame_ui_controls.egg-info/SOURCES.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-17 07:22:18.000000 pygame_ui_controls-1.0.0/src/pygame_ui_controls.egg-info/dependency_links.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        7 2023-06-17 07:22:18.000000 pygame_ui_controls-1.0.0/src/pygame_ui_controls.egg-info/requires.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-17 07:22:18.000000 pygame_ui_controls-1.0.0/src/pygame_ui_controls.egg-info/top_level.txt
--rw-rw-r--   0 arthur    (1000) arthur    (1000)    23070 2023-06-17 06:31:42.000000 pygame_ui_controls-1.0.0/src/ui_controls.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-17 07:36:07.671228 pygame_ui_controls-1.0.1/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    35149 2023-06-13 19:42:58.000000 pygame_ui_controls-1.0.1/LICENSE
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      659 2023-06-17 07:36:07.671228 pygame_ui_controls-1.0.1/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      478 2023-06-17 06:57:42.000000 pygame_ui_controls-1.0.1/README.md
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)       38 2023-06-17 07:36:07.671228 pygame_ui_controls-1.0.1/setup.cfg
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      789 2023-06-17 07:35:46.000000 pygame_ui_controls-1.0.1/setup.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-17 07:36:07.671228 pygame_ui_controls-1.0.1/src/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        0 2023-06-14 20:26:51.000000 pygame_ui_controls-1.0.1/src/__init__.py
+drwxrwxr-x   0 arthur    (1000) arthur    (1000)        0 2023-06-17 07:36:07.671228 pygame_ui_controls-1.0.1/src/pygame_ui_controls.egg-info/
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      659 2023-06-17 07:36:07.000000 pygame_ui_controls-1.0.1/src/pygame_ui_controls.egg-info/PKG-INFO
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)      297 2023-06-17 07:36:07.000000 pygame_ui_controls-1.0.1/src/pygame_ui_controls.egg-info/SOURCES.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-17 07:36:07.000000 pygame_ui_controls-1.0.1/src/pygame_ui_controls.egg-info/dependency_links.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        7 2023-06-17 07:36:07.000000 pygame_ui_controls-1.0.1/src/pygame_ui_controls.egg-info/requires.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)        1 2023-06-17 07:36:07.000000 pygame_ui_controls-1.0.1/src/pygame_ui_controls.egg-info/top_level.txt
+-rw-rw-r--   0 arthur    (1000) arthur    (1000)    23070 2023-06-17 07:27:58.000000 pygame_ui_controls-1.0.1/src/pygame_ui_controls.py
```

### Comparing `pygame_ui_controls-1.0.0/LICENSE` & `pygame_ui_controls-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_ui_controls-1.0.0/PKG-INFO` & `pygame_ui_controls-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_ui_controls
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pygame UI controls
 Home-page: https://github.com/ArthurLeFloch/PygameUI
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygame_ui_controls-1.0.0/setup.py` & `pygame_ui_controls-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='pygame_ui_controls',
-    version='1.0.0',
+    version='1.0.1',
     author='Arthur Le Floch',
     author_email='alf.github@gmail.com',
     description='Pygame UI controls',
     long_description='UI controls for Pygame (Button, ImageButton, CheckBox, Slider, Text)',
     url='https://github.com/ArthurLeFloch/PygameUI',
     packages=[''],
     package_dir={'': 'src'},
```

### Comparing `pygame_ui_controls-1.0.0/src/pygame_ui_controls.egg-info/PKG-INFO` & `pygame_ui_controls-1.0.1/src/pygame_ui_controls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-ui-controls
-Version: 1.0.0
+Version: 1.0.1
 Summary: Pygame UI controls
 Home-page: https://github.com/ArthurLeFloch/PygameUI
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `pygame_ui_controls-1.0.0/src/ui_controls.py` & `pygame_ui_controls-1.0.1/src/pygame_ui_controls.py`

 * *Files identical despite different names*

