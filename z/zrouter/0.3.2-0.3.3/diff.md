# Comparing `tmp/zrouter-0.3.2.tar.gz` & `tmp/zrouter-0.3.3.tar.gz`

## Comparing `zrouter-0.3.2.tar` & `zrouter-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 zrouter-0.3.2/src/zrouter/__init__.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 zrouter-0.3.2/src/zrouter/decorator.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.3.2/src/zrouter/exception.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.3.2/LICENSE
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.3.2/README.md
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 zrouter-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 zrouter-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 zrouter-0.3.3/src/zrouter/__init__.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 zrouter-0.3.3/src/zrouter/decorator.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.3.3/src/zrouter/exception.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.3.3/LICENSE
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 zrouter-0.3.3/README.md
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 zrouter-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 zrouter-0.3.3/PKG-INFO
```

### Comparing `zrouter-0.3.2/src/zrouter/__init__.py` & `zrouter-0.3.3/src/zrouter/__init__.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.3.2/src/zrouter/decorator.py` & `zrouter-0.3.3/src/zrouter/decorator.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.3.2/LICENSE` & `zrouter-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.3.2/pyproject.toml` & `zrouter-0.3.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   "flask==2.2.2",
+  "jsonschema==4.17.3",
   "inspirare",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `zrouter-0.3.2/PKG-INFO` & `zrouter-0.3.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.3.2
+Version: 0.3.3
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: flask==2.2.2
 Requires-Dist: inspirare
+Requires-Dist: jsonschema==4.17.3
 Description-Content-Type: text/markdown
 
 # ztime
 
 Zen time library.
```

