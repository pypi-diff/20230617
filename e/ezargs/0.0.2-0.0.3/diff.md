# Comparing `tmp/ezargs-0.0.2.tar.gz` & `tmp/ezargs-0.0.3.tar.gz`

## Comparing `ezargs-0.0.2.tar` & `ezargs-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 ezargs-0.0.2/ezargs/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ezargs-0.0.2/ezargs/main.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ezargs-0.0.2/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 ezargs-0.0.2/LICENSE
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ezargs-0.0.2/README.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 ezargs-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ezargs-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 ezargs-0.0.3/ezargs/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 ezargs-0.0.3/ezargs/main.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 ezargs-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 ezargs-0.0.3/LICENSE
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ezargs-0.0.3/README.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 ezargs-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 ezargs-0.0.3/PKG-INFO
```

### Comparing `ezargs-0.0.2/.gitignore` & `ezargs-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ezargs-0.0.2/LICENSE` & `ezargs-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ezargs-0.0.2/pyproject.toml` & `ezargs-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ezargs"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Michael", email="m12tbucket@gmail.com" },
 ]
 description = "zero-setup dynamic python command line argument parsing"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ezargs-0.0.2/PKG-INFO` & `ezargs-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezargs
-Version: 0.0.2
+Version: 0.0.3
 Summary: zero-setup dynamic python command line argument parsing
 Project-URL: Homepage, https://github.com/m12t/ezargs
 Project-URL: Bug Tracker, https://github.com/m12t/ezargs/issues
 Author-email: Michael <m12tbucket@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

