# Comparing `tmp/pyvalueobjects-0.8.1.tar.gz` & `tmp/pyvalueobjects-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvalueobjects-0.8.1.tar", last modified: Fri Jan 20 09:30:08 2023, max compression
+gzip compressed data, was "pyvalueobjects-0.9.0.tar", last modified: Sun Jan 29 09:00:22 2023, max compression
```

## Comparing `pyvalueobjects-0.8.1.tar` & `pyvalueobjects-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:30:08.848305 pyvalueobjects-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-01-20 09:30:08.848305 pyvalueobjects-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:30:08.844304 pyvalueobjects-0.8.1/pyvalueobjects/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:30:08.844304 pyvalueobjects-0.8.1/pyvalueobjects/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/abstract/nullablevalueobject.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/abstract/valueobject.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:30:08.844304 pyvalueobjects-0.8.1/pyvalueobjects/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/errors/ValueObjectError.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:30:08.848305 pyvalueobjects-0.8.1/pyvalueobjects/numbers/
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/numbers/int.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/numbers/negative_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/numbers/negative_or_zero_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/numbers/nullable_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/numbers/nullable_negative_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/numbers/nullable_negative_or_zero_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/numbers/nullable_positive_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/numbers/positive_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-20 09:29:54.000000 pyvalueobjects-0.8.1/pyvalueobjects/numbers/positive_or_zero_int.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 09:30:08.844304 pyvalueobjects-0.8.1/pyvalueobjects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-01-20 09:30:08.000000 pyvalueobjects-0.8.1/pyvalueobjects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-01-20 09:30:08.000000 pyvalueobjects-0.8.1/pyvalueobjects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 09:30:08.000000 pyvalueobjects-0.8.1/pyvalueobjects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-20 09:30:08.000000 pyvalueobjects-0.8.1/pyvalueobjects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-20 09:30:08.848305 pyvalueobjects-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 09:00:22.169560 pyvalueobjects-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-01-29 09:00:22.169560 pyvalueobjects-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 09:00:22.169560 pyvalueobjects-0.9.0/pyvalueobjects/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 09:00:22.169560 pyvalueobjects-0.9.0/pyvalueobjects/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/abstract/nullablevalueobject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/abstract/valueobject.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 09:00:22.169560 pyvalueobjects-0.9.0/pyvalueobjects/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/errors/ValueObjectError.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 09:00:22.169560 pyvalueobjects-0.9.0/pyvalueobjects/numbers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/negative_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/negative_or_zero_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/nullable_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/nullable_negative_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/nullable_negative_or_zero_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/nullable_positive_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/nullable_positive_or_zero_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/positive_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-29 09:00:06.000000 pyvalueobjects-0.9.0/pyvalueobjects/numbers/positive_or_zero_int.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 09:00:22.169560 pyvalueobjects-0.9.0/pyvalueobjects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-01-29 09:00:22.000000 pyvalueobjects-0.9.0/pyvalueobjects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-01-29 09:00:22.000000 pyvalueobjects-0.9.0/pyvalueobjects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 09:00:22.000000 pyvalueobjects-0.9.0/pyvalueobjects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-29 09:00:22.000000 pyvalueobjects-0.9.0/pyvalueobjects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-01-29 09:00:22.169560 pyvalueobjects-0.9.0/setup.cfg
```

### Comparing `pyvalueobjects-0.8.1/LICENSE` & `pyvalueobjects-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvalueobjects-0.8.1/PKG-INFO` & `pyvalueobjects-0.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvalueobjects
-Version: 0.8.1
+Version: 0.9.0
 Summary: A collection of Value Objects to save time by generalizing data type and format validations.
 Home-page: https://github.com/jparadadev/python-value-objects
 Author: Javier Parada
 Author-email: javierparadadev@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jparadadev/python-value-objects/issues
 Keywords: valueobjects,values
```

### Comparing `pyvalueobjects-0.8.1/pyvalueobjects/__init__.py` & `pyvalueobjects-0.9.0/pyvalueobjects/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 
 from pyvalueobjects.numbers.int import Int
 from pyvalueobjects.numbers.nullable_int import NullableInt
 from pyvalueobjects.numbers.positive_int import PositiveInt
 from pyvalueobjects.numbers.negative_int import NegativeInt
 from pyvalueobjects.numbers.nullable_negative_int import NullableNegativeInt
 from pyvalueobjects.numbers.positive_or_zero_int import PositiveOrZeroInt
+from pyvalueobjects.numbers.nullable_positive_or_zero_int import NullablePositiveOrZeroInt
 from pyvalueobjects.numbers.negative_or_zero_int import NegativeOrZeroInt
 from pyvalueobjects.numbers.nullable_negative_or_zero_int import NullableNegativeOrZeroInt
```

### Comparing `pyvalueobjects-0.8.1/pyvalueobjects/numbers/int.py` & `pyvalueobjects-0.9.0/pyvalueobjects/numbers/int.py`

 * *Files identical despite different names*

### Comparing `pyvalueobjects-0.8.1/pyvalueobjects.egg-info/PKG-INFO` & `pyvalueobjects-0.9.0/pyvalueobjects.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvalueobjects
-Version: 0.8.1
+Version: 0.9.0
 Summary: A collection of Value Objects to save time by generalizing data type and format validations.
 Home-page: https://github.com/jparadadev/python-value-objects
 Author: Javier Parada
 Author-email: javierparadadev@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/jparadadev/python-value-objects/issues
 Keywords: valueobjects,values
```

### Comparing `pyvalueobjects-0.8.1/pyvalueobjects.egg-info/SOURCES.txt` & `pyvalueobjects-0.9.0/pyvalueobjects.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,9 +13,10 @@
 pyvalueobjects/numbers/int.py
 pyvalueobjects/numbers/negative_int.py
 pyvalueobjects/numbers/negative_or_zero_int.py
 pyvalueobjects/numbers/nullable_int.py
 pyvalueobjects/numbers/nullable_negative_int.py
 pyvalueobjects/numbers/nullable_negative_or_zero_int.py
 pyvalueobjects/numbers/nullable_positive_int.py
+pyvalueobjects/numbers/nullable_positive_or_zero_int.py
 pyvalueobjects/numbers/positive_int.py
 pyvalueobjects/numbers/positive_or_zero_int.py
```

### Comparing `pyvalueobjects-0.8.1/setup.cfg` & `pyvalueobjects-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyvalueobjects
-version = 0.8.1
+version = 0.9.0
 author = Javier Parada
 author_email = javierparadadev@gmail.com
 description = A collection of Value Objects to save time by generalizing data type and format validations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 platform = any
```

