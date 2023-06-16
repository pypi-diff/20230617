# Comparing `tmp/excel-models-0.2.1.tar.gz` & `tmp/excel-models-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-models-0.2.1.tar", last modified: Thu Jun  8 22:01:26 2023, max compression
+gzip compressed data, was "excel-models-0.3.tar", last modified: Fri Jun 16 23:57:25 2023, max compression
```

## Comparing `excel-models-0.2.1.tar` & `excel-models-0.3.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.118219 excel-models-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-08 22:01:18.000000 excel-models-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 22:01:26.118219 excel-models-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-08 22:01:18.000000 excel-models-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.110219 excel-models-0.2.1/excel_models/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/column_inst/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/column_inst/remainder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/columns/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/basic_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/collection_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/columns/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/models/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/models/_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/tables/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/tables/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/tables/_inst.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/tables/_std.py
--rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/assignable_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/class_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/utils/descriptors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/validators/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-08 22:01:12.000000 excel-models-0.2.1/excel_models/validators/comparisons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.114219 excel-models-0.2.1/excel_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:01:26.000000 excel-models-0.2.1/excel_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:01:26.118219 excel-models-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-08 22:01:12.000000 excel-models-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:01:26.118219 excel-models-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_cell_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_cell_access_many.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_cell_access_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_custom_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_custom_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_model_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-08 22:01:12.000000 excel-models-0.2.1/tests/test_open_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.929114 excel-models-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-16 23:57:19.000000 excel-models-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 23:57:25.929114 excel-models-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-16 23:57:19.000000 excel-models-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.925114 excel-models-0.3/excel_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.925114 excel-models-0.3/excel_models/column_inst/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/column_inst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/column_inst/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/column_inst/_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/column_inst/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/column_inst/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/column_inst/remainder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.925114 excel-models-0.3/excel_models/columns/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/columns/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/columns/_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/columns/_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/columns/basic_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/columns/collection_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/columns/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.925114 excel-models-0.3/excel_models/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/models/_std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.925114 excel-models-0.3/excel_models/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/tables/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/tables/_inst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/tables/_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.925114 excel-models-0.3/excel_models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/utils/assignable_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/utils/class_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/utils/descriptors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.929114 excel-models-0.3/excel_models/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/validators/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-16 23:57:16.000000 excel-models-0.3/excel_models/validators/comparisons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.925114 excel-models-0.3/excel_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-16 23:57:25.000000 excel-models-0.3/excel_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-16 23:57:25.000000 excel-models-0.3/excel_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 23:57:25.000000 excel-models-0.3/excel_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-16 23:57:25.000000 excel-models-0.3/excel_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 23:57:25.000000 excel-models-0.3/excel_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 23:57:25.929114 excel-models-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-16 23:57:16.000000 excel-models-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 23:57:25.929114 excel-models-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_accessor_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_cell_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_cell_access_many.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_cell_access_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_custom_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_custom_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_model_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-16 23:57:16.000000 excel-models-0.3/tests/test_open_modes.py
```

### Comparing `excel-models-0.2.1/LICENSE` & `excel-models-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/PKG-INFO` & `excel-models-0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-models
-Version: 0.2.1
+Version: 0.3
 Summary: Model-style Excel File Accessor
 Home-page: https://github.com/MichaelKim0407/excel-models
 Author: Zheng Jin
 Author-email: mkim0407@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `excel-models-0.2.1/README.md` & `excel-models-0.3/README.md`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/column_inst/_base.py` & `excel-models-0.3/excel_models/column_inst/_base.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/column_inst/_std.py` & `excel-models-0.3/excel_models/column_inst/_std.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/column_inst/array.py` & `excel-models-0.3/excel_models/column_inst/array.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/column_inst/map.py` & `excel-models-0.3/excel_models/column_inst/map.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/column_inst/remainder.py` & `excel-models-0.3/excel_models/column_inst/remainder.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/columns/_base.py` & `excel-models-0.3/excel_models/columns/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 
 from excel_models.typing import (
     AbstractColumnDefinition,
     TModel, TTable, TColumn,
-    CellValue, ColumnValue,
+    CellValue, ColumnValue, ColumnCell,
 )
 from excel_models.utils.descriptors import BasePropertyDescriptor
 
 
 class BaseColumnDefinition(
     BasePropertyDescriptor[TModel],
     AbstractColumnDefinition,
@@ -18,23 +18,26 @@
     def _add_to_class(self):
         super()._add_to_class()
         self.obj_type.column_defs.append(self)
 
     def get_column(self, table: TTable) -> TColumn:
         return getattr(table, self.attr)
 
-    def to_python(self, raw: CellValue) -> ColumnValue:
+    def cell(self, row: TModel) -> ColumnCell:
+        return self.get_column(row.table).cell(row.row_num)
+
+    def to_python(self, row: TModel, raw: CellValue) -> ColumnValue:
         return raw
 
     def get_raw(self, row: TModel) -> CellValue:
         return self.get_column(row.table).get_raw(row.row_num)
 
     def _get_default(self, row: TModel) -> ColumnValue:
         raw = self.get_raw(row)
-        return self.to_python(raw)
+        return self.to_python(row, raw)
 
     validators = ()
 
     def _validate(self, row: TModel, value: ColumnValue) -> None:
         for validator in self.validators:
             validator(row, value)
 
@@ -76,22 +79,22 @@
             if self.attr not in row.values_cache:
                 value = self._get_nocache(row)
                 row.values_cache[self.attr] = value
             return row.values_cache[self.attr]
         else:
             return self._get_nocache(row)
 
-    def from_python(self, value: ColumnValue) -> CellValue:
+    def from_python(self, row: TModel, value: ColumnValue) -> CellValue:
         return value
 
     def set_raw(self, row: TModel, raw: CellValue) -> None:
         self.get_column(row.table).set_raw(row.row_num, raw)
 
     def _set_default(self, row: TModel, value: ColumnValue) -> None:
-        raw = self.from_python(value)
+        raw = self.from_python(row, value)
         self.set_raw(row, raw)
 
     def _set(self, row: TModel, value: ColumnValue) -> None:
         self._validate(row, value)
         self._set_method(row, value)
         if self.cache:
             row.values_cache[self.attr] = value
@@ -103,7 +106,15 @@
         self.delete_raw(row)
 
     def _delete(self, row: TModel):
         self._delete_method(row)
         if self.cache:
             if self.attr in row.values_cache:
                 del row.values_cache[self.attr]
+
+    @property
+    def cell_accessor(self) -> property:
+        return property(self.cell)
+
+    @property
+    def raw_value_accessor(self) -> property:
+        return property(self.get_raw, self.set_raw, self.delete_raw)
```

### Comparing `excel-models-0.2.1/excel_models/columns/_std.py` & `excel-models-0.3/excel_models/columns/_std.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/columns/collection_types.py` & `excel-models-0.3/excel_models/columns/collection_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 import json
 import typing
 
 from returns import returns
 
+from excel_models.typing import TModel
 from ._container import BaseContainer
+from ._std import Column
 from .basic_types import BaseTypedColumn
 
 
-class ArrayColumn(BaseContainer, BaseTypedColumn):
+class ArrayColumn(BaseContainer, Column):
     delimiter: str = '\n'
     strip: bool = False
+    empty_as_none: bool = True
 
     def split(self, value: str) -> list[str]:
         return value.split(self.delimiter)
 
+    def to_python(self, row: TModel, raw):
+        if not raw:
+            if self.empty_as_none:
+                return None
+            else:
+                return ()
+        return self._to_python(row, raw)
+
     @returns(tuple)
-    def _convert_to_python(self, raw):
+    def _to_python(self, row: TModel, raw):
         if not isinstance(raw, str):
-            yield self.inner.to_python(raw)
+            yield self.inner.to_python(row, raw)
             return
 
         for item in self.split(raw):
             if self.strip:
                 item = item.strip()
-            yield self.inner.to_python(item)
+            yield self.inner.to_python(row, item)
 
     def join(self, value: typing.Iterable[str]) -> str:
         return self.delimiter.join(value)
 
-    def _convert_from_python(self, value):
+    def from_python(self, row: TModel, value):
+        if not value:
+            return None
+
         return self.join(
-            self.inner.from_python(item)
+            self.inner.from_python(row, item)
             for item in value
         )
 
 
 class JsonColumn(BaseTypedColumn):
     def _convert_to_python(self, raw):
         if not isinstance(raw, str):
```

### Comparing `excel-models-0.2.1/excel_models/columns/multi.py` & `excel-models-0.3/excel_models/columns/multi.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from returns import returns
 
 from excel_models.column_inst.array import ExcelColumnArray
 from excel_models.column_inst.map import ExcelColumnMap
 from excel_models.column_inst.remainder import ExcelColumnRemainder
 from excel_models.exceptions import DuplicateColumn
-from excel_models.typing import TTable, TColumn
+from excel_models.typing import TTable, TColumn, TModel
 from ._container import BaseContainer
 
 
 class Columns(BaseContainer):
     column_class = ExcelColumnArray
     width: int
 
@@ -22,22 +22,22 @@
         return self.column_class(table, self, col_num, self.width)
 
     def init_column(self, table: TTable, col_num: int) -> tuple[TColumn, int]:
         table.set_title(col_num, self.name)
         return self.column_class(table, self, col_num, self.width), self.width
 
     @returns(tuple)
-    def to_python(self, raw: typing.Sequence) -> typing.Sequence:
+    def to_python(self, row: TModel, raw: typing.Sequence) -> typing.Sequence:
         for v in raw:
-            yield self.inner.to_python(v)
+            yield self.inner.to_python(row, v)
 
     @returns(tuple)
-    def from_python(self, value: typing.Sequence) -> typing.Sequence:
+    def from_python(self, row: TModel, value: typing.Sequence) -> typing.Sequence:
         for v in value:
-            yield self.inner.from_python(v)
+            yield self.inner.from_python(row, v)
 
 
 class ColumnsStartWith(BaseContainer):
     column_class = ExcelColumnMap
     create_keys: typing.Collection[str]
 
     def match_column(self, table: TTable, col_num: int) -> TColumn | None:
@@ -61,22 +61,22 @@
             for c, k in enumerate(self.create_keys, start=col_num)
         }
         for k, c in col_map.items():
             table.set_title(c, f'{self.name}{k}')
         return self.column_class(table, self, col_map), len(col_map)
 
     @returns(dict)
-    def to_python(self, raw: typing.Mapping) -> typing.Mapping:
+    def to_python(self, row: TModel, raw: typing.Mapping) -> typing.Mapping:
         for k, v in raw.items():
-            yield k, self.inner.to_python(v)
+            yield k, self.inner.to_python(row, v)
 
     @returns(dict)
-    def from_python(self, value: typing.Mapping) -> typing.Mapping:
+    def from_python(self, row: TModel, value: typing.Mapping) -> typing.Mapping:
         for k, v in value.items():
-            yield k, self.inner.from_python(v)
+            yield k, self.inner.from_python(row, v)
 
 
 class Remainder(BaseContainer):
     column_class = ExcelColumnRemainder
 
     def match_column(self, table: TTable, col_num: int) -> TColumn | None:
         title = table.get_title(col_num)
@@ -86,15 +86,15 @@
         return self.column_class(table, self, col_num)
 
     def init_column(self, table: TTable, col_num: int) -> tuple[TColumn, int]:
         table.set_title(col_num, self.name)
         return self.column_class(table, self, col_num), 1  # use 1 here but this must be the last column
 
     @returns(tuple)
-    def to_python(self, raw: typing.Sequence) -> typing.Sequence:
+    def to_python(self, row: TModel, raw: typing.Sequence) -> typing.Sequence:
         for v in raw:
-            yield self.inner.to_python(v)
+            yield self.inner.to_python(row, v)
 
     @returns(tuple)
-    def from_python(self, value: typing.Sequence) -> typing.Sequence:
+    def from_python(self, row: TModel, value: typing.Sequence) -> typing.Sequence:
         for v in value:
-            yield self.inner.from_python(v)
+            yield self.inner.from_python(row, v)
```

### Comparing `excel-models-0.2.1/excel_models/db.py` & `excel-models-0.3/excel_models/db.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/models/_base.py` & `excel-models-0.3/excel_models/models/_base.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/tables/_base.py` & `excel-models-0.3/excel_models/tables/_base.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/tables/_inst.py` & `excel-models-0.3/excel_models/tables/_inst.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/typing.py` & `excel-models-0.3/excel_models/typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,38 +80,51 @@
 
     def init_column(self, table: 'TTable', col_num: int) -> tuple['TColumn', int]:
         raise NotImplementedError  # pragma: no cover
 
     def get_column(self, table: 'TTable') -> 'TColumn':
         raise NotImplementedError  # pragma: no cover
 
-    def to_python(self, raw: CellValue) -> ColumnValue:
+    def cell(self, row: TModel) -> ColumnCell:
+        raise NotImplementedError  # pragma: no cover
+
+    def to_python(self, row: TModel, raw: CellValue) -> ColumnValue:
         raise NotImplementedError  # pragma: no cover
 
     def get_raw(self, row: TModel) -> CellValue:
         raise NotImplementedError  # pragma: no cover
 
     def __get__(self, row: TModel, model: typing.Type[TModel] = None) -> ColumnValue:
         raise NotImplementedError  # pragma: no cover
 
-    def from_python(self, value: ColumnValue) -> CellValue:
+    def from_python(self, row: TModel, value: ColumnValue) -> CellValue:
         raise NotImplementedError  # pragma: no cover
 
     def set_raw(self, row: TModel, raw: CellValue) -> None:
         raise NotImplementedError  # pragma: no cover
 
     def __set__(self, row: TModel, value: ColumnValue) -> None:
         raise NotImplementedError  # pragma: no cover
 
     def delete_raw(self, row: TModel) -> None:
         raise NotImplementedError  # pragma: no cover
 
     def __delete__(self, row: TModel) -> None:
         raise NotImplementedError  # pragma: no cover
 
+    # --- accessor properties ---
+
+    @property
+    def cell_accessor(self) -> property:
+        raise NotImplementedError  # pragma: no cover
+
+    @property
+    def raw_value_accessor(self) -> property:
+        raise NotImplementedError  # pragma: no cover
+
 
 TColumnDef = typing.TypeVar('TColumnDef', bound=AbstractColumnDefinition)
 
 
 class AbstractTableDefinition(typing.Generic[TDB, TModel]):
     attr: str
     name: str
```

### Comparing `excel-models-0.2.1/excel_models/utils/class_collector.py` & `excel-models-0.3/excel_models/utils/class_collector.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/utils/descriptors.py` & `excel-models-0.3/excel_models/utils/descriptors.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/validators/_base.py` & `excel-models-0.3/excel_models/validators/_base.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models/validators/comparisons.py` & `excel-models-0.3/excel_models/validators/comparisons.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/excel_models.egg-info/PKG-INFO` & `excel-models-0.3/excel_models.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-models
-Version: 0.2.1
+Version: 0.3
 Summary: Model-style Excel File Accessor
 Home-page: https://github.com/MichaelKim0407/excel-models
 Author: Zheng Jin
 Author-email: mkim0407@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `excel-models-0.2.1/excel_models.egg-info/SOURCES.txt` & `excel-models-0.3/excel_models.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 excel_models/utils/assignable_property.py
 excel_models/utils/class_collector.py
 excel_models/utils/collections.py
 excel_models/utils/descriptors.py
 excel_models/validators/__init__.py
 excel_models/validators/_base.py
 excel_models/validators/comparisons.py
+tests/test_accessor_properties.py
 tests/test_alias.py
 tests/test_bool.py
 tests/test_caching.py
 tests/test_cell_access.py
 tests/test_cell_access_many.py
 tests/test_cell_access_raw.py
 tests/test_custom_column.py
```

### Comparing `excel-models-0.2.1/setup.py` & `excel-models-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_alias.py` & `excel-models-0.3/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_caching.py` & `excel-models-0.3/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_cell_access.py` & `excel-models-0.3/tests/test_cell_access.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_cell_access_many.py` & `excel-models-0.3/tests/test_cell_access_many.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_cell_access_raw.py` & `excel-models-0.3/tests/test_cell_access_raw.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_custom_column.py` & `excel-models-0.3/tests/test_custom_column.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,36 +9,35 @@
 def excel(lazy_init_excel):
     return lazy_init_excel('users', 'name', 'John\nDoe', None, 'Bob', 1.5)
 
 
 class User(ExcelModel):
     @Column()
     def name(self):
-        raw = self._get_name(self)
+        raw = self.raw_name
         if raw is None or raw == '':
             return []
         return raw.split('\n')
 
-    _get_name = name.get_raw
-    _set_name = name.set_raw
+    raw_name = name.raw_value_accessor
 
     @name.setter
     def name(self, value):
         if not value:
-            self._set_name(self, '')
+            self.raw_name = ''
             return
-        self._set_name(self, '\n'.join(value))
+        self.raw_name = '\n'.join(value)
 
     @name.deleter
     def name(self):
-        self._set_name(self, '')
+        self.raw_name = ''
 
-    @name.error_handler
+    @name.error_handler  # noqa: pycharm
     def name(self, ex: Exception):
-        return [str(self._get_name(self))]
+        return [str(self.raw_name)]
 
 
 class MyDB(ExcelDB):
     users = User.as_table()
 
 
 @pytest.fixture()
```

### Comparing `excel-models-0.2.1/tests/test_custom_table.py` & `excel-models-0.3/tests/test_custom_table.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_eq.py` & `excel-models-0.3/tests/test_eq.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_model_inheritance.py` & `excel-models-0.3/tests/test_model_inheritance.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_new.py` & `excel-models-0.3/tests/test_new.py`

 * *Files identical despite different names*

### Comparing `excel-models-0.2.1/tests/test_open_modes.py` & `excel-models-0.3/tests/test_open_modes.py`

 * *Files identical despite different names*

