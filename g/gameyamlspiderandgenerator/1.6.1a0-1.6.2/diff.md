# Comparing `tmp/gameyamlspiderandgenerator-1.6.1a0.tar.gz` & `tmp/gameyamlspiderandgenerator-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.6.1a0.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.6.2.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.6.1a0.tar` & `gameyamlspiderandgenerator-1.6.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.6.1a0/LICENSE
--rwxr-xr-x   0        0        0     1350 2023-06-11 10:23:19.902922 gameyamlspiderandgenerator-1.6.1a0/README.md
--rwxr-xr-x   0        0        0      568 2023-06-07 14:28:47.706873 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1924 2023-06-11 10:27:03.919708 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      675 2023-06-11 14:22:24.297547 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0      235 2023-06-17 06:19:48.870893 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0       56 2023-06-07 14:15:34.823402 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3177 2023-06-11 10:23:19.906828 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7088 2023-06-13 14:02:11.945879 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7919 2023-06-11 14:16:45.563698 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1848 2023-06-13 13:39:03.156896 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     2545 2023-06-17 06:37:16.080809 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2550 2023-06-11 10:23:19.910070 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      833 2023-06-17 06:37:55.131945 gameyamlspiderandgenerator-1.6.1a0/pyproject.toml
--rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.1a0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.6.2/LICENSE
+-rwxr-xr-x   0        0        0     1350 2023-06-11 10:23:19.902922 gameyamlspiderandgenerator-1.6.2/README.md
+-rwxr-xr-x   0        0        0      568 2023-06-07 14:28:47.706873 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1924 2023-06-11 10:27:03.919708 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      675 2023-06-11 14:22:24.297547 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0      235 2023-06-17 06:19:48.870893 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0       56 2023-06-07 14:15:34.823402 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3177 2023-06-11 10:23:19.906828 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7088 2023-06-13 14:02:11.945879 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7919 2023-06-11 14:16:45.563698 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1848 2023-06-13 13:39:03.156896 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     2545 2023-06-17 06:37:16.080809 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2550 2023-06-11 10:23:19.910070 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      832 2023-06-17 06:38:48.531151 gameyamlspiderandgenerator-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     2675 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.6.2/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.6.1a0/LICENSE` & `gameyamlspiderandgenerator-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/README.md` & `gameyamlspiderandgenerator-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/__main__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.6.2/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.6.1a0/pyproject.toml` & `gameyamlspiderandgenerator-1.6.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.6.1a"
+version = "1.6.2"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.6.1a0/PKG-INFO` & `gameyamlspiderandgenerator-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.6.1a0
+Version: 1.6.2
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

