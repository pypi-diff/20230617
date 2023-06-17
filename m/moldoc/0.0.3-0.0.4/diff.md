# Comparing `tmp/moldoc-0.0.3.tar.gz` & `tmp/moldoc-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moldoc-0.0.3.tar", last modified: Thu Aug  5 11:44:34 2021, max compression
+gzip compressed data, was "moldoc-0.0.4.tar", last modified: Sat Jun 17 13:36:11 2023, max compression
```

## Comparing `moldoc-0.0.3.tar` & `moldoc-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2021-08-05 11:44:34.844851 moldoc-0.0.3/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1053 2021-07-30 16:38:58.000000 moldoc-0.0.3/LICENSE
--rw-r--r--   0 lukas     (1000) lukas     (1000)      272 2021-08-05 11:44:34.844851 moldoc-0.0.3/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5615 2021-08-05 11:42:04.000000 moldoc-0.0.3/README.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2021-08-05 11:44:34.844851 moldoc-0.0.3/setup.cfg
--rw-r--r--   0 lukas     (1000) lukas     (1000)      672 2021-07-30 16:34:49.000000 moldoc-0.0.3/setup.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2021-08-05 11:44:34.844851 moldoc-0.0.3/src/
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2021-08-05 11:44:34.844851 moldoc-0.0.3/src/moldoc/
--rw-r--r--   0 lukas     (1000) lukas     (1000)       70 2021-08-05 11:44:08.000000 moldoc-0.0.3/src/moldoc/__init__.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2021-08-05 11:44:34.844851 moldoc-0.0.3/src/moldoc/javascript/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      259 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/javascript/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1915 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/javascript/atoms.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      386 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/javascript/bonds.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)       88 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/javascript/bool.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      292 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/javascript/color.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4311 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/javascript/material.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2793 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/javascript/mesh_config.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      930 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/javascript/scene_config.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)   351667 2021-07-30 16:20:22.000000 moldoc-0.0.3/src/moldoc/molDraw.js
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3191 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/moldoc.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     5409 2021-08-05 11:42:04.000000 moldoc-0.0.3/src/moldoc/molecule.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)   551410 2021-07-30 16:20:22.000000 moldoc-0.0.3/src/moldoc/three.min.js
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2021-08-05 11:44:34.844851 moldoc-0.0.3/src/moldoc.egg-info/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      272 2021-08-05 11:44:34.000000 moldoc-0.0.3/src/moldoc.egg-info/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)      575 2021-08-05 11:44:34.000000 moldoc-0.0.3/src/moldoc.egg-info/SOURCES.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2021-08-05 11:44:34.000000 moldoc-0.0.3/src/moldoc.egg-info/dependency_links.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2021-08-05 11:44:34.000000 moldoc-0.0.3/src/moldoc.egg-info/requires.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2021-08-05 11:44:34.000000 moldoc-0.0.3/src/moldoc.egg-info/top_level.txt
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.774025 moldoc-0.0.4/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1053 2023-06-17 13:13:28.000000 moldoc-0.0.4/LICENSE
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      210 2023-06-17 13:36:11.774025 moldoc-0.0.4/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5615 2023-06-17 13:13:28.000000 moldoc-0.0.4/README.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-06-17 13:36:11.774025 moldoc-0.0.4/setup.cfg
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      672 2023-06-17 13:13:28.000000 moldoc-0.0.4/setup.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.770692 moldoc-0.0.4/src/
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.770692 moldoc-0.0.4/src/moldoc/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       70 2023-06-17 13:28:21.000000 moldoc-0.0.4/src/moldoc/__init__.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.774025 moldoc-0.0.4/src/moldoc/javascript/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      259 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1915 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/atoms.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      386 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/bonds.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       88 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/bool.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      292 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/color.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4311 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/material.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2793 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/mesh_config.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      930 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/javascript/scene_config.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   351667 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/molDraw.js
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3193 2023-06-17 13:14:12.000000 moldoc-0.0.4/src/moldoc/moldoc.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     5409 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/molecule.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   551410 2023-06-17 13:13:28.000000 moldoc-0.0.4/src/moldoc/three.min.js
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-17 13:36:11.774025 moldoc-0.0.4/src/moldoc.egg-info/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      210 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      575 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/requires.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2023-06-17 13:36:11.000000 moldoc-0.0.4/src/moldoc.egg-info/top_level.txt
```

### Comparing `moldoc-0.0.3/LICENSE` & `moldoc-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/README.rst` & `moldoc-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/setup.py` & `moldoc-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/src/moldoc/javascript/atoms.py` & `moldoc-0.0.4/src/moldoc/javascript/atoms.py`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/src/moldoc/javascript/material.py` & `moldoc-0.0.4/src/moldoc/javascript/material.py`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/src/moldoc/javascript/mesh_config.py` & `moldoc-0.0.4/src/moldoc/javascript/mesh_config.py`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/src/moldoc/javascript/scene_config.py` & `moldoc-0.0.4/src/moldoc/javascript/scene_config.py`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/src/moldoc/molDraw.js` & `moldoc-0.0.4/src/moldoc/molDraw.js`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/src/moldoc/moldoc.py` & `moldoc-0.0.4/src/moldoc/moldoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,16 @@
 
 def html_moldoc(self, node: MolDocNode):
     molecule = node.get_molecule()
     moldoc_node_id = node.get_moldoc_name()
 
     if not getattr(self, 'moldoc_scripts_added', False):
         self.body.append(
-            '<script src="_static/three.min.js"></script>'
-            '<script src="_static/molDraw.js"></script>'
+            '<script src="/_static/three.min.js"></script>'
+            '<script src="/_static/molDraw.js"></script>'
             '<script>const md=molDraw;'
             'let atoms=[];'
             'let bonds=[];'
             'let maybeMolecule=undefined;'
             '</script>'
         )
         self.moldoc_scripts_added = True
```

### Comparing `moldoc-0.0.3/src/moldoc/molecule.py` & `moldoc-0.0.4/src/moldoc/molecule.py`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/src/moldoc/three.min.js` & `moldoc-0.0.4/src/moldoc/three.min.js`

 * *Files identical despite different names*

### Comparing `moldoc-0.0.3/src/moldoc.egg-info/SOURCES.txt` & `moldoc-0.0.4/src/moldoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

