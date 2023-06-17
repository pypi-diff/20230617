# Comparing `tmp/kaya-module-sdk-1.2.tar.gz` & `tmp/kaya_module_sdk-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaya-module-sdk-1.2.tar", last modified: Sun Jun 11 23:31:26 2023, max compression
+gzip compressed data, was "kaya_module_sdk-1.3.tar", last modified: Sat Jun 17 03:45:04 2023, max compression
```

## Comparing `kaya-module-sdk-1.2.tar` & `kaya_module_sdk-1.3.tar`

### file list

```diff
@@ -1,77 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/kaya-module-sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/kaya-module-sdk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4209 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/_k_number.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/src/module/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/module/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/module/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/src/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/testing/kit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/src/testing/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/tst/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/tst/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/integration/test_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.279157 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-06-11 23:31:22.000000 kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:31:26.000000 kaya-module-sdk-1.2/kaya_module_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     4209 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/src/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/_k_number.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_int.py
--rw-r--r--   0 runner    (1001) docker     (123)     3590 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/data_types/k_time_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/src/module/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/module/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/module/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/src/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/testing/kit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/src/testing/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/tst/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/tst/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/integration/test_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 23:31:26.283157 kaya-module-sdk-1.2/tst/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/unit/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/unit/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10935 2023-06-11 23:30:09.000000 kaya-module-sdk-1.2/tst/unit/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.466796 kaya_module_sdk-1.3/
+-rw-r--r--   0 root         (0) root         (0)    11356 2023-06-12 21:13:44.000000 kaya_module_sdk-1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-06-16 23:11:50.000000 kaya_module_sdk-1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.442796 kaya_module_sdk-1.3/kaya_module_sdk/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      705 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/sdk.py
+-rwxr-xr-x   0 root         (0) root         (0)     4209 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.446796 kaya_module_sdk-1.3/kaya_module_sdk/src/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      541 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.450796 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/_k_number.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_float.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_int.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_list.py
+-rw-r--r--   0 root         (0) root         (0)      491 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_string.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_time_series.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.450796 kaya_module_sdk-1.3/kaya_module_sdk/src/module/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/module/run.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/module/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.450796 kaya_module_sdk-1.3/kaya_module_sdk/src/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/testing/kit.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/src/testing/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.450796 kaya_module_sdk-1.3/kaya_module_sdk/tst/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.454796 kaya_module_sdk-1.3/kaya_module_sdk/tst/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/integration/test_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.454796 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_module.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_sdk.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-06-17 03:45:02.000000 kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.446796 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3401 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-17 03:45:04.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 23:14:30.000000 kaya_module_sdk-1.3/kaya_module_sdk.egg-info/zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-17 03:45:04.466796 kaya_module_sdk-1.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     4209 2023-06-16 22:37:50.000000 kaya_module_sdk-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.454796 kaya_module_sdk-1.3/src/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 16:03:20.000000 kaya_module_sdk-1.3/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      541 2023-06-05 05:47:56.000000 kaya_module_sdk-1.3/src/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.458796 kaya_module_sdk-1.3/src/data_types/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 23:34:41.000000 kaya_module_sdk-1.3/src/data_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-04-06 00:33:46.000000 kaya_module_sdk-1.3/src/data_types/_k_number.py
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-03 20:31:53.000000 kaya_module_sdk-1.3/src/data_types/k_float.py
+-rw-r--r--   0 root         (0) root         (0)      151 2023-04-03 20:31:45.000000 kaya_module_sdk-1.3/src/data_types/k_int.py
+-rw-r--r--   0 root         (0) root         (0)     3590 2023-04-03 20:31:37.000000 kaya_module_sdk-1.3/src/data_types/k_list.py
+-rw-r--r--   0 root         (0) root         (0)      491 2023-03-18 03:32:53.000000 kaya_module_sdk-1.3/src/data_types/k_string.py
+-rw-r--r--   0 root         (0) root         (0)     1548 2023-03-18 03:13:25.000000 kaya_module_sdk-1.3/src/data_types/k_time_series.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.458796 kaya_module_sdk-1.3/src/module/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 23:34:52.000000 kaya_module_sdk-1.3/src/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-06-02 00:44:27.000000 kaya_module_sdk-1.3/src/module/run.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-09 16:25:01.000000 kaya_module_sdk-1.3/src/module/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/src/testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-09 16:58:36.000000 kaya_module_sdk-1.3/src/testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2023-06-17 03:30:24.000000 kaya_module_sdk-1.3/src/testing/kit.py
+-rw-r--r--   0 root         (0) root         (0)     1437 2023-06-17 03:30:31.000000 kaya_module_sdk-1.3/src/testing/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/tst/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-17 23:33:13.000000 kaya_module_sdk-1.3/tst/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/tst/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 23:31:50.000000 kaya_module_sdk-1.3/tst/integration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-16 23:12:35.000000 kaya_module_sdk-1.3/tst/integration/test_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 03:45:04.462796 kaya_module_sdk-1.3/tst/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 23:31:54.000000 kaya_module_sdk-1.3/tst/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-16 23:12:41.000000 kaya_module_sdk-1.3/tst/unit/test_module.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-06-16 23:12:55.000000 kaya_module_sdk-1.3/tst/unit/test_sdk.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-06-16 23:13:07.000000 kaya_module_sdk-1.3/tst/unit/test_types.py
```

### Comparing `kaya-module-sdk-1.2/LICENSE` & `kaya_module_sdk-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/PKG-INFO` & `kaya_module_sdk-1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kaya-module-sdk
-Version: 1.2
+Name: kaya_module_sdk
+Version: 1.3
 Summary: Provides the user a way to create custom strategy modules.
 Home-page: https://kaya.wanolabs.com
 Download-URL: http://pypi.python.org/pypi/kaya-module-sdk
 Author: Del:Tango
 Author-email: alvearesolutions@gmail.com
 License: BSD
 Project-URL: Documentation, https://kaya.wanolabs.com.readthedocs.io/en/latest
@@ -85,15 +85,15 @@
             self.dummy_time_series = KTimeSeries[float]
 
         def main(self, args: int, debug: bool = False) -> float:
             return float(sum(args))
 
 [ **Example** ]: Using the SDK to run a strategy module -
 
-    from kaya.sdk import run
+    from kaya_module_sdk.sdk import run
     from my_module import MyModule
 
     module_instance = MyModule()
     run(module_instance, args=(1,2,3,4,), kwargs={'debug': True})
```

### Comparing `kaya-module-sdk-1.2/README.md` & `kaya_module_sdk-1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             self.dummy_time_series = KTimeSeries[float]
 
         def main(self, args: int, debug: bool = False) -> float:
             return float(sum(args))
 
 [ **Example** ]: Using the SDK to run a strategy module -
 
-    from kaya.sdk import run
+    from kaya_module_sdk.sdk import run
     from my_module import MyModule
 
     module_instance = MyModule()
     run(module_instance, args=(1,2,3,4,), kwargs={'debug': True})
```

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/sdk.py` & `kaya_module_sdk-1.3/kaya_module_sdk/sdk.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from kaya.src.data_types.k_time_series import KTimeSeries
-from kaya.src.data_types.k_list import KList
-from kaya.src.data_types.k_string import KString
-from kaya.src.data_types.k_int import KInt
-from kaya.src.data_types.k_float import KFloat
-from kaya.src.module.template import Module
-from kaya.src.module.run import run as module_run
-from kaya.src.config import Config
-from kaya.src.testing.kit import KIT
-from kaya.src.testing.run import run as test_run
+from kaya_module_sdk.src.data_types.k_time_series import KTimeSeries
+from kaya_module_sdk.src.data_types.k_list import KList
+from kaya_module_sdk.src.data_types.k_string import KString
+from kaya_module_sdk.src.data_types.k_int import KInt
+from kaya_module_sdk.src.data_types.k_float import KFloat
+from kaya_module_sdk.src.module.template import Module
+from kaya_module_sdk.src.module.run import run as module_run
+from kaya_module_sdk.src.config import Config
+from kaya_module_sdk.src.testing.kit import KIT
+from kaya_module_sdk.src.testing.run import run as test_run
 
 '''
 [ DESCRIPTION ]: Interface for the Kaya Module SDK :)
 [ NOTE ]: Exposes only Kaya data types, module template and module runner.
 '''
```

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/setup.py` & `kaya_module_sdk-1.3/kaya_module_sdk/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 # MISCELLANEOUS
 
 # TODO - Check type hints used or break compilation
 #MyPyCommand().run()
 
 add_package_dir_to_path()
 setup_info = dict(
-    name='kaya-module-sdk',
-    version='1.2',
+    name='kaya_module_sdk',
+    version='1.3',
     author='Del:Tango',
     author_email='alvearesolutions@gmail.com',
     url='https://kaya.wanolabs.com',
     download_url='http://pypi.python.org/pypi/kaya-module-sdk',
     project_urls={
         'Documentation': 'https://kaya.wanolabs.com.readthedocs.io/en/latest',
         'Source': 'https://github.com/WanoLabs/KayaModuleSDK',
```

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/src/config.py` & `kaya_module_sdk-1.3/kaya_module_sdk/src/config.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/_k_number.py` & `kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/_k_number.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_list.py` & `kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_list.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/src/data_types/k_time_series.py` & `kaya_module_sdk-1.3/kaya_module_sdk/src/data_types/k_time_series.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/src/module/run.py` & `kaya_module_sdk-1.3/kaya_module_sdk/src/module/run.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/src/module/template.py` & `kaya_module_sdk-1.3/kaya_module_sdk/src/module/template.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/src/testing/kit.py` & `kaya_module_sdk-1.3/kaya_module_sdk/src/testing/kit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import pysnooper
 import docker
 import unittest
 import logging
+import json
+import re
 
 from abc import ABC, abstractmethod
 
 log = logging.getLogger('')
 
 
 class KIT(ABC, unittest.TestCase):
     '''
     [ KayaIntegrationTests ]: Morty puts his custom strategy module integration
         tests into subclasses of KIT.
     '''
     integration_tests = []
     docker_container_id = str()
     docker_container = None
-    runner_host = 'http://localhost:80'
+    runner_host = 'http://127.0.0.1:80'
 
 #   @pysnooper.snoop()
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.docker_container_id = kwargs.get('docker_container_id', str())
-        self.runer_host = kwargs.get('runner_host', 'http://localhost:80')
+        self.runer_host = kwargs.get('runner_host', 'http://127.0.0.1:80')
         self.docker_client = docker.from_env()
         self.integration_tests = [
             method for method in dir(self) if callable(getattr(self, method))
             and not method.startswith('__') and method.startswith('test_')
         ]
 
     @classmethod
@@ -35,31 +37,41 @@
         pass
 
     @classmethod
     @abstractmethod
     def teardown(cls):
         pass
 
+#   @pysnooper.snoop()
     def module(self, module_name, *args, request_type='GET', **kwargs):
         if request_type not in ['GET', 'POST']:
             print(f'[ ERROR ]: Invalid request type! ({request_type})')
             return False
+        # [ NOTE ]: Make sure request body uses double quotes!!
         return self.module_request(
-            request_type, module_name, {'args': list(args), 'kwargs': kwargs}
+            request_type, module_name, {"args": list(args), "kwargs": kwargs}
         )
 
 #   @pysnooper.snoop()
     def module_request(self, verb: str, module_name: str, body: dict):
         cmd = f'curl -X {verb} -H "Content-Type: application/json" -d \'{body}\' '\
             f'{self.runner_host}/{module_name}'
+        cmd = cmd.replace("'args'", '"args"').replace("'kwargs'", '"kwargs"')
         run = self.docker_container.exec_run(cmd)
-        return {
-            'response': run.output.decode('utf-8').strip(),
+        run_stdout = run.output.decode('utf-8').strip()
+        # Regular expression pattern to match everything between \n{ and $
+        pattern = r'\{.*?\{.*?\}.*?\}'
+        # Search for the JSON object using the pattern
+        match = re.search(pattern, run_stdout)
+        response = match.group() if match else '{}'
+        result = {
+            'response': json.loads(response),
             'exit': run.exit_code,
         }
+        return result
 
 #   @pysnooper.snoop()
     def run_test(self, method_name):
         try:
             test_run = getattr(self, method_name)()
         except Exception as e:
             return False
@@ -77,15 +89,15 @@
         self.docker_container_id = docker_container_id
         self.docker_container = self.docker_client.containers.get(
             docker_container_id
         )
         try:
             for method_name in self.integration_tests:
                 run = self.run_test(method_name)
-                if run and not run.get('failures'):
+                if run:
                     print(f'[ OK ]: Integration Test ({method_name})')
                     ok.append(method_name)
                 else:
                     print(f'[ NOK ]: Integration Test ({method_name})')
                     nok.append(method_name)
                 test_runs.update({method_name: run})
         finally:
@@ -95,13 +107,9 @@
             'test-runs': test_runs,
             'teardown': kit_teardown,
             'ok': ok,
             'nok': nok,
         }
 
 # CODE DUMP
-#       kit_setup = self.setup()
-#       kit_setup = self.run_test('setup')
 
-#           kit_teardown = self.teardown()
-#           kit_teardown = self.run_test('teardown')
```

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/src/testing/run.py` & `kaya_module_sdk-1.3/kaya_module_sdk/src/testing/run.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/tst/integration/test_module.py` & `kaya_module_sdk-1.3/kaya_module_sdk/tst/integration/test_module.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from kaya.sdk import KIT
+from kaya_module_sdk.sdk import KIT
 
 
 class KayaIntegrationTests(KIT):
 
     package_name = 'dummy'
 
     def __init__(self, *args, **kwargs):
@@ -14,20 +14,20 @@
 
     @classmethod
     def teardown(cls):
         print('\n[ DONE ]: Kaya Integration Test Suit (KITS)')
 
     def test_add_two(self):
         print('\n[ TEST ]: Good Weather - AddTwo')
-        response = self.module(f'{package_name}/AddTwo', *[13, 420])
+        response = self.module(f'{self.package_name}/AddTwo', *[13, 420])
         self.assertTrue(isinstance(response, dict))
-        self.assertTrue(response.get('result'))
-        self.assertEqual(response['result'], 433)
+        self.assertTrue(response.get('response'))
+        self.assertEqual(response['response'], 433)
 
     def test_subtract_two(self):
         print('\n[ TEST ]: Good Weather - SubtractTwo')
-        response = self.module(f'{package_name}/SubtractTwo', *[420, 13])
+        response = self.module(f'{self.package_name}/SubtractTwo', *[420, 13])
         self.assertTrue(isinstance(response, dict))
-        self.assertTrue(response.get('result'))
-        self.assertEqual(response['result'], 407)
+        self.assertTrue(response.get('response'))
+        self.assertEqual(response['response'], 407)
```

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_module.py` & `kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from kaya.sdk import Module, module_run
+from kaya_module_sdk.sdk import Module, module_run
 
 
 class DummyMortyModule(Module):
 
     def main(self, *args: int, debug='off', **kwargs) -> float:
         return float(sum(args))
```

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_sdk.py` & `kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_sdk.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,11 +12,11 @@
         print('\n[ DONE ]: Kaya SDK\n')
 
     # Test cases
 
     def test_sdk_imports(self):
         print('\n[ TEST ]: Test imports from Kaya SDK...\n')
         try:
-            from kaya.sdk import module_run, Module, KTimeSeries, KList
+            from kaya_module_sdk.sdk import module_run, Module, KTimeSeries, KList
         except Exception as e:
             print('\n[ NOK ]: Importing from SDK failed!\n')
             self.assertTrue(False)
```

### Comparing `kaya-module-sdk-1.2/kaya-module-sdk/tst/unit/test_types.py` & `kaya_module_sdk-1.3/kaya_module_sdk/tst/unit/test_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import time
 
-from kaya.sdk import KTimeSeries, KList, KString, KInt, KFloat
+from kaya_module_sdk.sdk import KTimeSeries, KList, KString, KInt, KFloat
 
 
 class TestDataTypeTimeSeries(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         print('\n[ TestSuit ]: Kaya Module SDK Data Types\n')
```

### Comparing `kaya-module-sdk-1.2/kaya_module_sdk.egg-info/PKG-INFO` & `kaya_module_sdk-1.3/kaya_module_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaya-module-sdk
-Version: 1.2
+Version: 1.3
 Summary: Provides the user a way to create custom strategy modules.
 Home-page: https://kaya.wanolabs.com
 Download-URL: http://pypi.python.org/pypi/kaya-module-sdk
 Author: Del:Tango
 Author-email: alvearesolutions@gmail.com
 License: BSD
 Project-URL: Documentation, https://kaya.wanolabs.com.readthedocs.io/en/latest
@@ -85,15 +85,15 @@
             self.dummy_time_series = KTimeSeries[float]
 
         def main(self, args: int, debug: bool = False) -> float:
             return float(sum(args))
 
 [ **Example** ]: Using the SDK to run a strategy module -
 
-    from kaya.sdk import run
+    from kaya_module_sdk.sdk import run
     from my_module import MyModule
 
     module_instance = MyModule()
     run(module_instance, args=(1,2,3,4,), kwargs={'debug': True})
```

### Comparing `kaya-module-sdk-1.2/kaya_module_sdk.egg-info/SOURCES.txt` & `kaya_module_sdk-1.3/kaya_module_sdk.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 LICENSE
 README.md
 setup.py
-kaya-module-sdk/__init__.py
-kaya-module-sdk/sdk.py
-kaya-module-sdk/setup.py
-kaya-module-sdk/kaya-module-sdk/__init__.py
-kaya-module-sdk/src/__init__.py
-kaya-module-sdk/src/config.py
-kaya-module-sdk/src/data_types/__init__.py
-kaya-module-sdk/src/data_types/_k_number.py
-kaya-module-sdk/src/data_types/k_float.py
-kaya-module-sdk/src/data_types/k_int.py
-kaya-module-sdk/src/data_types/k_list.py
-kaya-module-sdk/src/data_types/k_string.py
-kaya-module-sdk/src/data_types/k_time_series.py
-kaya-module-sdk/src/module/__init__.py
-kaya-module-sdk/src/module/run.py
-kaya-module-sdk/src/module/template.py
-kaya-module-sdk/src/testing/__init__.py
-kaya-module-sdk/src/testing/kit.py
-kaya-module-sdk/src/testing/run.py
-kaya-module-sdk/tst/__init__.py
-kaya-module-sdk/tst/integration/__init__.py
-kaya-module-sdk/tst/integration/test_module.py
-kaya-module-sdk/tst/unit/__init__.py
-kaya-module-sdk/tst/unit/test_module.py
-kaya-module-sdk/tst/unit/test_sdk.py
-kaya-module-sdk/tst/unit/test_types.py
+kaya_module_sdk/__init__.py
+kaya_module_sdk/sdk.py
+kaya_module_sdk/setup.py
 kaya_module_sdk.egg-info/PKG-INFO
 kaya_module_sdk.egg-info/SOURCES.txt
 kaya_module_sdk.egg-info/dependency_links.txt
 kaya_module_sdk.egg-info/requires.txt
 kaya_module_sdk.egg-info/top_level.txt
 kaya_module_sdk.egg-info/zip-safe
+kaya_module_sdk/src/__init__.py
+kaya_module_sdk/src/config.py
+kaya_module_sdk/src/data_types/__init__.py
+kaya_module_sdk/src/data_types/_k_number.py
+kaya_module_sdk/src/data_types/k_float.py
+kaya_module_sdk/src/data_types/k_int.py
+kaya_module_sdk/src/data_types/k_list.py
+kaya_module_sdk/src/data_types/k_string.py
+kaya_module_sdk/src/data_types/k_time_series.py
+kaya_module_sdk/src/module/__init__.py
+kaya_module_sdk/src/module/run.py
+kaya_module_sdk/src/module/template.py
+kaya_module_sdk/src/testing/__init__.py
+kaya_module_sdk/src/testing/kit.py
+kaya_module_sdk/src/testing/run.py
+kaya_module_sdk/tst/__init__.py
+kaya_module_sdk/tst/integration/__init__.py
+kaya_module_sdk/tst/integration/test_module.py
+kaya_module_sdk/tst/unit/__init__.py
+kaya_module_sdk/tst/unit/test_module.py
+kaya_module_sdk/tst/unit/test_sdk.py
+kaya_module_sdk/tst/unit/test_types.py
 src/__init__.py
 src/config.py
 src/data_types/__init__.py
 src/data_types/_k_number.py
 src/data_types/k_float.py
 src/data_types/k_int.py
 src/data_types/k_list.py
```

### Comparing `kaya-module-sdk-1.2/setup.py` & `kaya_module_sdk-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,16 @@
 # MISCELLANEOUS
 
 # TODO - Check type hints used or break compilation
 #MyPyCommand().run()
 
 add_package_dir_to_path()
 setup_info = dict(
-    name='kaya-module-sdk',
-    version='1.2',
+    name='kaya_module_sdk',
+    version='1.3',
     author='Del:Tango',
     author_email='alvearesolutions@gmail.com',
     url='https://kaya.wanolabs.com',
     download_url='http://pypi.python.org/pypi/kaya-module-sdk',
     project_urls={
         'Documentation': 'https://kaya.wanolabs.com.readthedocs.io/en/latest',
         'Source': 'https://github.com/WanoLabs/KayaModuleSDK',
```

### Comparing `kaya-module-sdk-1.2/src/config.py` & `kaya_module_sdk-1.3/src/config.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/src/data_types/_k_number.py` & `kaya_module_sdk-1.3/src/data_types/_k_number.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/src/data_types/k_list.py` & `kaya_module_sdk-1.3/src/data_types/k_list.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/src/data_types/k_time_series.py` & `kaya_module_sdk-1.3/src/data_types/k_time_series.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/src/module/run.py` & `kaya_module_sdk-1.3/src/module/run.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/src/module/template.py` & `kaya_module_sdk-1.3/src/module/template.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/src/testing/kit.py` & `kaya_module_sdk-1.3/src/testing/kit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import pysnooper
 import docker
 import unittest
 import logging
+import json
+import re
 
 from abc import ABC, abstractmethod
 
 log = logging.getLogger('')
 
 
 class KIT(ABC, unittest.TestCase):
     '''
     [ KayaIntegrationTests ]: Morty puts his custom strategy module integration
         tests into subclasses of KIT.
     '''
     integration_tests = []
     docker_container_id = str()
     docker_container = None
-    runner_host = 'http://localhost:80'
+    runner_host = 'http://127.0.0.1:80'
 
 #   @pysnooper.snoop()
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.docker_container_id = kwargs.get('docker_container_id', str())
-        self.runer_host = kwargs.get('runner_host', 'http://localhost:80')
+        self.runer_host = kwargs.get('runner_host', 'http://127.0.0.1:80')
         self.docker_client = docker.from_env()
         self.integration_tests = [
             method for method in dir(self) if callable(getattr(self, method))
             and not method.startswith('__') and method.startswith('test_')
         ]
 
     @classmethod
@@ -35,31 +37,41 @@
         pass
 
     @classmethod
     @abstractmethod
     def teardown(cls):
         pass
 
+#   @pysnooper.snoop()
     def module(self, module_name, *args, request_type='GET', **kwargs):
         if request_type not in ['GET', 'POST']:
             print(f'[ ERROR ]: Invalid request type! ({request_type})')
             return False
+        # [ NOTE ]: Make sure request body uses double quotes!!
         return self.module_request(
-            request_type, module_name, {'args': list(args), 'kwargs': kwargs}
+            request_type, module_name, {"args": list(args), "kwargs": kwargs}
         )
 
 #   @pysnooper.snoop()
     def module_request(self, verb: str, module_name: str, body: dict):
         cmd = f'curl -X {verb} -H "Content-Type: application/json" -d \'{body}\' '\
             f'{self.runner_host}/{module_name}'
+        cmd = cmd.replace("'args'", '"args"').replace("'kwargs'", '"kwargs"')
         run = self.docker_container.exec_run(cmd)
-        return {
-            'response': run.output.decode('utf-8').strip(),
+        run_stdout = run.output.decode('utf-8').strip()
+        # Regular expression pattern to match everything between \n{ and $
+        pattern = r'\{.*?\{.*?\}.*?\}'
+        # Search for the JSON object using the pattern
+        match = re.search(pattern, run_stdout)
+        response = match.group() if match else '{}'
+        result = {
+            'response': json.loads(response),
             'exit': run.exit_code,
         }
+        return result
 
 #   @pysnooper.snoop()
     def run_test(self, method_name):
         try:
             test_run = getattr(self, method_name)()
         except Exception as e:
             return False
@@ -77,15 +89,15 @@
         self.docker_container_id = docker_container_id
         self.docker_container = self.docker_client.containers.get(
             docker_container_id
         )
         try:
             for method_name in self.integration_tests:
                 run = self.run_test(method_name)
-                if run and not run.get('failures'):
+                if run:
                     print(f'[ OK ]: Integration Test ({method_name})')
                     ok.append(method_name)
                 else:
                     print(f'[ NOK ]: Integration Test ({method_name})')
                     nok.append(method_name)
                 test_runs.update({method_name: run})
         finally:
@@ -95,13 +107,9 @@
             'test-runs': test_runs,
             'teardown': kit_teardown,
             'ok': ok,
             'nok': nok,
         }
 
 # CODE DUMP
-#       kit_setup = self.setup()
-#       kit_setup = self.run_test('setup')
 
-#           kit_teardown = self.teardown()
-#           kit_teardown = self.run_test('teardown')
```

### Comparing `kaya-module-sdk-1.2/src/testing/run.py` & `kaya_module_sdk-1.3/src/testing/run.py`

 * *Files identical despite different names*

### Comparing `kaya-module-sdk-1.2/tst/integration/test_module.py` & `kaya_module_sdk-1.3/tst/integration/test_module.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from kaya.sdk import KIT
+from kaya_module_sdk.sdk import KIT
 
 
 class KayaIntegrationTests(KIT):
 
     package_name = 'dummy'
 
     def __init__(self, *args, **kwargs):
@@ -14,20 +14,20 @@
 
     @classmethod
     def teardown(cls):
         print('\n[ DONE ]: Kaya Integration Test Suit (KITS)')
 
     def test_add_two(self):
         print('\n[ TEST ]: Good Weather - AddTwo')
-        response = self.module(f'{package_name}/AddTwo', *[13, 420])
+        response = self.module(f'{self.package_name}/AddTwo', *[13, 420])
         self.assertTrue(isinstance(response, dict))
-        self.assertTrue(response.get('result'))
-        self.assertEqual(response['result'], 433)
+        self.assertTrue(response.get('response'))
+        self.assertEqual(response['response'], 433)
 
     def test_subtract_two(self):
         print('\n[ TEST ]: Good Weather - SubtractTwo')
-        response = self.module(f'{package_name}/SubtractTwo', *[420, 13])
+        response = self.module(f'{self.package_name}/SubtractTwo', *[420, 13])
         self.assertTrue(isinstance(response, dict))
-        self.assertTrue(response.get('result'))
-        self.assertEqual(response['result'], 407)
+        self.assertTrue(response.get('response'))
+        self.assertEqual(response['response'], 407)
```

### Comparing `kaya-module-sdk-1.2/tst/unit/test_module.py` & `kaya_module_sdk-1.3/tst/unit/test_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from kaya.sdk import Module, module_run
+from kaya_module_sdk.sdk import Module, module_run
 
 
 class DummyMortyModule(Module):
 
     def main(self, *args: int, debug='off', **kwargs) -> float:
         return float(sum(args))
```

### Comparing `kaya-module-sdk-1.2/tst/unit/test_sdk.py` & `kaya_module_sdk-1.3/tst/unit/test_sdk.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,11 +12,11 @@
         print('\n[ DONE ]: Kaya SDK\n')
 
     # Test cases
 
     def test_sdk_imports(self):
         print('\n[ TEST ]: Test imports from Kaya SDK...\n')
         try:
-            from kaya.sdk import module_run, Module, KTimeSeries, KList
+            from kaya_module_sdk.sdk import module_run, Module, KTimeSeries, KList
         except Exception as e:
             print('\n[ NOK ]: Importing from SDK failed!\n')
             self.assertTrue(False)
```

### Comparing `kaya-module-sdk-1.2/tst/unit/test_types.py` & `kaya_module_sdk-1.3/tst/unit/test_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 import time
 
-from kaya.sdk import KTimeSeries, KList, KString, KInt, KFloat
+from kaya_module_sdk.sdk import KTimeSeries, KList, KString, KInt, KFloat
 
 
 class TestDataTypeTimeSeries(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         print('\n[ TestSuit ]: Kaya Module SDK Data Types\n')
```

