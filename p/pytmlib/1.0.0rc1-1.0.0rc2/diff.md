# Comparing `tmp/pytmlib-1.0.0rc1.tar.gz` & `tmp/pytmlib-1.0.0rc2.tar.gz`

## Comparing `pytmlib-1.0.0rc1.tar` & `pytmlib-1.0.0rc2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/__init__.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/abstract_exercise.py
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/api.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/archiver.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/context.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/create_app.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/handle_error.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/latex.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/method_call_exception.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/serializer.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/abstract.py
--rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/builder.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/button.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/field.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/field_attribute.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/field_type_enum.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/figure.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/image.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/option.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/option_group.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/paragraph.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/table.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/src/pytmlib/output/table_cell.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/__init__.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/abstract_exercise.py
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/api.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/archiver.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/context.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/create_app.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/handle_error.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/latex.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/method_call_exception.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/serializer.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/abstract.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/builder.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/button.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/field.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/field_attribute.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/field_type_enum.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/figure.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/image.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/option.py
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/option_group.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/paragraph.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/table.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pytmlib/output/table_cell.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/README.md
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 pytmlib-1.0.0rc2/PKG-INFO
```

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/abstract_exercise.py` & `pytmlib-1.0.0rc2/pytmlib/abstract_exercise.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/api.py` & `pytmlib-1.0.0rc2/pytmlib/api.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/archiver.py` & `pytmlib-1.0.0rc2/pytmlib/archiver.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/context.py` & `pytmlib-1.0.0rc2/pytmlib/context.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/create_app.py` & `pytmlib-1.0.0rc2/pytmlib/create_app.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/handle_error.py` & `pytmlib-1.0.0rc2/pytmlib/handle_error.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/serializer.py` & `pytmlib-1.0.0rc2/pytmlib/serializer.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/abstract.py` & `pytmlib-1.0.0rc2/pytmlib/output/abstract.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/builder.py` & `pytmlib-1.0.0rc2/pytmlib/output/builder.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/button.py` & `pytmlib-1.0.0rc2/pytmlib/output/button.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/field.py` & `pytmlib-1.0.0rc2/pytmlib/output/field.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/figure.py` & `pytmlib-1.0.0rc2/pytmlib/output/figure.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/image.py` & `pytmlib-1.0.0rc2/pytmlib/output/image.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/option.py` & `pytmlib-1.0.0rc2/pytmlib/output/option.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/option_group.py` & `pytmlib-1.0.0rc2/pytmlib/output/option_group.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/paragraph.py` & `pytmlib-1.0.0rc2/pytmlib/output/paragraph.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/table.py` & `pytmlib-1.0.0rc2/pytmlib/output/table.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/src/pytmlib/output/table_cell.py` & `pytmlib-1.0.0rc2/pytmlib/output/table_cell.py`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/LICENSE` & `pytmlib-1.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytmlib-1.0.0rc1/pyproject.toml` & `pytmlib-1.0.0rc2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pytmlib"
-version = "1.0.0rc1"
+version = "1.0.0rc2"
 authors = [
     { name = "Oliver Fabel", email = "oliver.fabel@fhnw.ch" },
 ]
 description = "This is the base library for the Python Tool Manager."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
@@ -33,9 +33,8 @@
 [project.urls]
 "Homepage" = "https://github.com/ofabel/pytm-bootstrap"
 "Bug Tracker" = "https://github.com/ofabel/pytm-bootstrap/issues"
 "Changelog" = "https://github.com/ofabel/pytm-bootstrap/blob/main/CHANGELOG.md"
 
 [tool.hatch.build]
 ignore-vcs = true
-only-include = ["src"]
-exclude = [".gitignore"]
+packages = ["src/pytmlib"]
```

### Comparing `pytmlib-1.0.0rc1/PKG-INFO` & `pytmlib-1.0.0rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmlib
-Version: 1.0.0rc1
+Version: 1.0.0rc2
 Summary: This is the base library for the Python Tool Manager.
 Project-URL: Homepage, https://github.com/ofabel/pytm-bootstrap
 Project-URL: Bug Tracker, https://github.com/ofabel/pytm-bootstrap/issues
 Project-URL: Changelog, https://github.com/ofabel/pytm-bootstrap/blob/main/CHANGELOG.md
 Author-email: Oliver Fabel <oliver.fabel@fhnw.ch>
 License: MIT License
```

