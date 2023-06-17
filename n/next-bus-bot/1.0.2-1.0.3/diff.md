# Comparing `tmp/next-bus-bot-1.0.2.tar.gz` & `tmp/next-bus-bot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "next-bus-bot-1.0.2.tar", last modified: Tue Dec 13 08:48:00 2022, max compression
+gzip compressed data, was "next-bus-bot-1.0.3.tar", last modified: Tue Dec 13 08:52:18 2022, max compression
```

## Comparing `next-bus-bot-1.0.2.tar` & `next-bus-bot-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:48:00.046543 next-bus-bot-1.0.2/
--rw-r--r--   0 pac       (1000) pac       (1000)     2748 2022-12-13 08:48:00.046543 next-bus-bot-1.0.2/PKG-INFO
--rw-r--r--   0 pac       (1000) pac       (1000)     1990 2022-12-12 22:00:13.000000 next-bus-bot-1.0.2/README.rst
--rw-r--r--   0 pac       (1000) pac       (1000)     1618 2022-12-13 08:47:51.000000 next-bus-bot-1.0.2/pyproject.toml
--rw-r--r--   0 pac       (1000) pac       (1000)       38 2022-12-13 08:48:00.046543 next-bus-bot-1.0.2/setup.cfg
-drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:48:00.046543 next-bus-bot-1.0.2/src/
-drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:48:00.046543 next-bus-bot-1.0.2/src/nbb/
--rw-r--r--   0 pac       (1000) pac       (1000)        0 2022-12-03 11:17:27.000000 next-bus-bot-1.0.2/src/nbb/__init__.py
--rw-r--r--   0 pac       (1000) pac       (1000)     5364 2022-12-12 21:49:32.000000 next-bus-bot-1.0.2/src/nbb/backend.py
--rwxr-xr-x   0 pac       (1000) pac       (1000)     1864 2022-12-12 21:39:45.000000 next-bus-bot-1.0.2/src/nbb/cli.py
-drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:48:00.046543 next-bus-bot-1.0.2/src/next_bus_bot.egg-info/
--rw-r--r--   0 pac       (1000) pac       (1000)     2748 2022-12-13 08:48:00.000000 next-bus-bot-1.0.2/src/next_bus_bot.egg-info/PKG-INFO
--rw-r--r--   0 pac       (1000) pac       (1000)      321 2022-12-13 08:48:00.000000 next-bus-bot-1.0.2/src/next_bus_bot.egg-info/SOURCES.txt
--rw-r--r--   0 pac       (1000) pac       (1000)        1 2022-12-13 08:48:00.000000 next-bus-bot-1.0.2/src/next_bus_bot.egg-info/dependency_links.txt
--rw-r--r--   0 pac       (1000) pac       (1000)       37 2022-12-13 08:48:00.000000 next-bus-bot-1.0.2/src/next_bus_bot.egg-info/entry_points.txt
--rw-r--r--   0 pac       (1000) pac       (1000)      115 2022-12-13 08:48:00.000000 next-bus-bot-1.0.2/src/next_bus_bot.egg-info/requires.txt
--rw-r--r--   0 pac       (1000) pac       (1000)        4 2022-12-13 08:48:00.000000 next-bus-bot-1.0.2/src/next_bus_bot.egg-info/top_level.txt
+drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:52:18.809865 next-bus-bot-1.0.3/
+-rw-r--r--   0 pac       (1000) pac       (1000)     2748 2022-12-13 08:52:18.809865 next-bus-bot-1.0.3/PKG-INFO
+-rw-r--r--   0 pac       (1000) pac       (1000)     1990 2022-12-12 22:00:13.000000 next-bus-bot-1.0.3/README.rst
+-rw-r--r--   0 pac       (1000) pac       (1000)     1673 2022-12-13 08:51:44.000000 next-bus-bot-1.0.3/pyproject.toml
+-rw-r--r--   0 pac       (1000) pac       (1000)       38 2022-12-13 08:52:18.809865 next-bus-bot-1.0.3/setup.cfg
+drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:52:18.806532 next-bus-bot-1.0.3/src/
+drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:52:18.806532 next-bus-bot-1.0.3/src/nbb/
+-rw-r--r--   0 pac       (1000) pac       (1000)        0 2022-12-03 11:17:27.000000 next-bus-bot-1.0.3/src/nbb/__init__.py
+-rw-r--r--   0 pac       (1000) pac       (1000)     5364 2022-12-12 21:49:32.000000 next-bus-bot-1.0.3/src/nbb/backend.py
+-rwxr-xr-x   0 pac       (1000) pac       (1000)     1864 2022-12-12 21:39:45.000000 next-bus-bot-1.0.3/src/nbb/cli.py
+-rw-r--r--   0 pac       (1000) pac       (1000)     1503 2022-12-12 21:13:50.000000 next-bus-bot-1.0.3/src/nbb/nbb_conf.toml
+drwxr-xr-x   0 pac       (1000) pac       (1000)        0 2022-12-13 08:52:18.806532 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/
+-rw-r--r--   0 pac       (1000) pac       (1000)     2748 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/PKG-INFO
+-rw-r--r--   0 pac       (1000) pac       (1000)      343 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 pac       (1000) pac       (1000)        1 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 pac       (1000) pac       (1000)       37 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/entry_points.txt
+-rw-r--r--   0 pac       (1000) pac       (1000)      115 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/requires.txt
+-rw-r--r--   0 pac       (1000) pac       (1000)        4 2022-12-13 08:52:18.000000 next-bus-bot-1.0.3/src/next_bus_bot.egg-info/top_level.txt
```

### Comparing `next-bus-bot-1.0.2/PKG-INFO` & `next-bus-bot-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: next-bus-bot
-Version: 1.0.2
+Version: 1.0.3
 Summary: Get the next in coming buses at a Paris area Station.
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@crans.org>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `next-bus-bot-1.0.2/README.rst` & `next-bus-bot-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.0.2/pyproject.toml` & `next-bus-bot-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "next-bus-bot"
 description = "Get the next in coming buses at a Paris area Station."
 
-version = "1.0.2"
+version = "1.0.3"
 authors =[
 {name="Pierre-Antoine Comby", email="pierre-antoine.comby@crans.org"}
 ]
 
 dependencies = [
   "requests",
   "tomli; python_version <= '3.10'",
@@ -39,14 +39,17 @@
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "pytest-xdist", "pytest-sugar"]
 dev = ["black", "isort"]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 
+[tool.setuptools]
+
+package-data = {"nbb" = ["*.toml"]}
 
 [tool.coverage.run]
 omit = ["*tests*"]
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = ["pragma: no cover", "raise NotImplementedError"]
```

### Comparing `next-bus-bot-1.0.2/src/nbb/backend.py` & `next-bus-bot-1.0.3/src/nbb/backend.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.0.2/src/nbb/cli.py` & `next-bus-bot-1.0.3/src/nbb/cli.py`

 * *Files identical despite different names*

### Comparing `next-bus-bot-1.0.2/src/next_bus_bot.egg-info/PKG-INFO` & `next-bus-bot-1.0.3/src/next_bus_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: next-bus-bot
-Version: 1.0.2
+Version: 1.0.3
 Summary: Get the next in coming buses at a Paris area Station.
 Author-email: Pierre-Antoine Comby <pierre-antoine.comby@crans.org>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

