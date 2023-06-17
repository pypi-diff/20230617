# Comparing `tmp/ezargs-0.0.3.tar.gz` & `tmp/ezargs-0.0.4.tar.gz`

## Comparing `ezargs-0.0.3.tar` & `ezargs-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ezargs-0.0.3/ezargs/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ezargs-0.0.3/ezargs/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ezargs-0.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 ezargs-0.0.3/LICENSE
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ezargs-0.0.3/README.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 ezargs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ezargs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ezargs-0.0.4/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 ezargs-0.0.4/ezargs/.DS_Store
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ezargs-0.0.4/ezargs/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ezargs-0.0.4/ezargs/main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ezargs-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 ezargs-0.0.4/LICENSE
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ezargs-0.0.4/README.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 ezargs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ezargs-0.0.4/PKG-INFO
```

### Comparing `ezargs-0.0.3/.gitignore` & `ezargs-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ezargs-0.0.3/LICENSE` & `ezargs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ezargs-0.0.3/pyproject.toml` & `ezargs-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ezargs"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Michael", email="m12tbucket@gmail.com" },
 ]
 description = "zero-setup dynamic python command line argument parsing"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ezargs-0.0.3/PKG-INFO` & `ezargs-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezargs
-Version: 0.0.3
+Version: 0.0.4
 Summary: zero-setup dynamic python command line argument parsing
 Project-URL: Homepage, https://github.com/m12t/ezargs
 Project-URL: Bug Tracker, https://github.com/m12t/ezargs/issues
 Author-email: Michael <m12tbucket@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

