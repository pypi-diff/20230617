# Comparing `tmp/skbase-0.4.5.tar.gz` & `tmp/skbase-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skbase-0.4.5.tar", last modified: Sun May 14 14:07:44 2023, max compression
+gzip compressed data, was "skbase-0.4.6.tar", last modified: Sat Jun 17 20:17:00 2023, max compression
```

## Comparing `skbase-0.4.5.tar` & `skbase-0.4.6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.401671 skbase-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-05-14 14:07:33.000000 skbase-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-14 14:07:44.401671 skbase-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-05-14 14:07:33.000000 skbase-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.385670 skbase-0.4.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.389670 skbase-0.4.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (122)     9845 2023-05-14 14:07:33.000000 skbase-0.4.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-14 14:07:33.000000 skbase-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-05-14 14:07:44.401671 skbase-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1077 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/_nopytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/base/
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43618 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_base.py
--rw-r--r--   0 runner    (1001) docker     (122)    35626 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/base/_pretty_printing/
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_pretty_printing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11539 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_pretty_printing/_object_html_repr.py
--rw-r--r--   0 runner    (1001) docker     (122)    15634 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_pretty_printing/_pprint.py
--rw-r--r--   0 runner    (1001) docker     (122)     7290 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/base/_tagmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/lookup/
--rw-r--r--   0 runner    (1001) docker     (122)     1089 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/lookup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    38936 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/lookup/_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/lookup/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/lookup/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36924 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/lookup/tests/test_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase/testing/
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36442 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/test_all_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/testing/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9890 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/_conditional_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)      335 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/deep_equals.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/inspect.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/testing/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2233 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/tests/test_check_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/testing/utils/tests/test_deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8398 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/tests/mock_package/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/mock_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/mock_package/test_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (122)    41827 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4730 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/test_baseestimator.py
--rw-r--r--   0 runner    (1001) docker     (122)      629 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     4436 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1395 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8037 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4566 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     3134 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    11299 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/deep_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.397671 skbase-0.4.5/skbase/utils/dependencies/
--rw-r--r--   0 runner    (1001) docker     (122)      352 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10359 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/dependencies/_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.401671 skbase-0.4.5/skbase/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     4918 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/test_nested_iter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1182 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/utils/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.401671 skbase-0.4.5/skbase/validate/
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14777 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    12121 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.401671 skbase-0.4.5/skbase/validate/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7438 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/tests/test_iterable_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-14 14:07:33.000000 skbase-0.4.5/skbase/validate/tests/test_type_validations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-14 14:07:44.393670 skbase-0.4.5/skbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6492 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-14 14:07:44.000000 skbase-0.4.5/skbase.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-17 20:17:00.169021 skbase-0.4.6/
+-rw-rw-rw-   0        0        0     1554 2022-09-08 21:53:10.000000 skbase-0.4.6/LICENSE
+-rw-rw-rw-   0        0        0     6806 2023-06-17 20:17:00.169021 skbase-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3506 2023-06-16 01:46:32.000000 skbase-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:58.725999 skbase-0.4.6/docs/
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.062209 skbase-0.4.6/docs/source/
+-rw-rw-rw-   0        0        0    10144 2023-04-18 19:57:18.000000 skbase-0.4.6/docs/source/conf.py
+-rw-rw-rw-   0        0        0     3426 2023-06-16 01:48:54.000000 skbase-0.4.6/pyproject.toml
+-rw-rw-rw-   0        0        0      368 2023-06-17 20:17:00.189021 skbase-0.4.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.123582 skbase-0.4.6/skbase/
+-rw-rw-rw-   0        0        0      468 2023-06-16 01:37:08.000000 skbase-0.4.6/skbase/__init__.py
+-rw-rw-rw-   0        0        0     1144 2022-12-28 00:03:43.000000 skbase-0.4.6/skbase/_exceptions.py
+-rw-rw-rw-   0        0        0     1112 2023-05-13 18:22:14.000000 skbase-0.4.6/skbase/_nopytest_tests.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.298519 skbase-0.4.6/skbase/base/
+-rw-rw-rw-   0        0        0      649 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/base/__init__.py
+-rw-rw-rw-   0        0        0    47999 2023-06-16 01:37:17.000000 skbase-0.4.6/skbase/base/_base.py
+-rw-rw-rw-   0        0        0    36497 2023-06-11 22:51:35.000000 skbase-0.4.6/skbase/base/_meta.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.330167 skbase-0.4.6/skbase/base/_pretty_printing/
+-rw-rw-rw-   0        0        0      503 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/base/_pretty_printing/__init__.py
+-rw-rw-rw-   0        0        0    11931 2023-04-26 13:58:57.000000 skbase-0.4.6/skbase/base/_pretty_printing/_object_html_repr.py
+-rw-rw-rw-   0        0        0    16046 2023-04-23 21:36:04.000000 skbase-0.4.6/skbase/base/_pretty_printing/_pprint.py
+-rw-rw-rw-   0        0        0     7507 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/base/_tagmanager.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.361416 skbase-0.4.6/skbase/lookup/
+-rw-rw-rw-   0        0        0     1120 2022-12-28 00:03:43.000000 skbase-0.4.6/skbase/lookup/__init__.py
+-rw-rw-rw-   0        0        0    40149 2023-06-16 01:37:08.000000 skbase-0.4.6/skbase/lookup/_lookup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.432999 skbase-0.4.6/skbase/lookup/tests/
+-rw-rw-rw-   0        0        0       70 2022-12-31 19:03:49.000000 skbase-0.4.6/skbase/lookup/tests/__init__.py
+-rw-rw-rw-   0        0        0    37915 2023-04-26 14:48:09.000000 skbase-0.4.6/skbase/lookup/tests/test_lookup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.476511 skbase-0.4.6/skbase/testing/
+-rw-rw-rw-   0        0        0      363 2022-12-28 00:00:00.000000 skbase-0.4.6/skbase/testing/__init__.py
+-rw-rw-rw-   0        0        0    37298 2023-05-13 18:22:13.000000 skbase-0.4.6/skbase/testing/test_all_objects.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.598080 skbase-0.4.6/skbase/testing/utils/
+-rw-rw-rw-   0        0        0      118 2022-12-31 19:03:49.000000 skbase-0.4.6/skbase/testing/utils/__init__.py
+-rw-rw-rw-   0        0        0    10099 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/testing/utils/_conditional_fixtures.py
+-rw-rw-rw-   0        0        0      484 2023-05-13 18:22:13.000000 skbase-0.4.6/skbase/testing/utils/_dependencies.py
+-rw-rw-rw-   0        0        0      350 2023-05-13 23:40:38.000000 skbase-0.4.6/skbase/testing/utils/deep_equals.py
+-rw-rw-rw-   0        0        0      771 2022-09-08 20:20:18.000000 skbase-0.4.6/skbase/testing/utils/inspect.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.647647 skbase-0.4.6/skbase/testing/utils/tests/
+-rw-rw-rw-   0        0        0       73 2022-09-08 20:20:18.000000 skbase-0.4.6/skbase/testing/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0     2282 2022-12-30 11:07:07.000000 skbase-0.4.6/skbase/testing/utils/tests/test_check_dependencies.py
+-rw-rw-rw-   0        0        0     1771 2023-05-13 18:22:13.000000 skbase-0.4.6/skbase/testing/utils/tests/test_deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.808273 skbase-0.4.6/skbase/tests/
+-rw-rw-rw-   0        0        0       39 2022-04-29 16:15:46.000000 skbase-0.4.6/skbase/tests/__init__.py
+-rw-rw-rw-   0        0        0     8671 2023-05-13 23:40:38.000000 skbase-0.4.6/skbase/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.842119 skbase-0.4.6/skbase/tests/mock_package/
+-rw-rw-rw-   0        0        0      140 2022-12-31 19:03:49.000000 skbase-0.4.6/skbase/tests/mock_package/__init__.py
+-rw-rw-rw-   0        0        0     2095 2022-12-31 19:03:49.000000 skbase-0.4.6/skbase/tests/mock_package/test_mock_package.py
+-rw-rw-rw-   0        0        0    43784 2023-06-16 01:37:17.000000 skbase-0.4.6/skbase/tests/test_base.py
+-rw-rw-rw-   0        0        0     4860 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/tests/test_baseestimator.py
+-rw-rw-rw-   0        0        0      652 2022-12-31 19:03:49.000000 skbase-0.4.6/skbase/tests/test_exceptions.py
+-rw-rw-rw-   0        0        0     4567 2023-05-11 20:27:18.000000 skbase-0.4.6/skbase/tests/test_meta.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.928718 skbase-0.4.6/skbase/utils/
+-rw-rw-rw-   0        0        0      654 2023-05-13 23:40:38.000000 skbase-0.4.6/skbase/utils/__init__.py
+-rw-rw-rw-   0        0        0     1448 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/utils/_check.py
+-rw-rw-rw-   0        0        0     8275 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/utils/_iter.py
+-rw-rw-rw-   0        0        0     4746 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/utils/_nested_iter.py
+-rw-rw-rw-   0        0        0     3225 2023-05-04 17:40:43.000000 skbase-0.4.6/skbase/utils/_utils.py
+-rw-rw-rw-   0        0        0    11657 2023-05-13 18:22:13.000000 skbase-0.4.6/skbase/utils/deep_equals.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.963128 skbase-0.4.6/skbase/utils/dependencies/
+-rw-rw-rw-   0        0        0      363 2023-05-13 18:22:13.000000 skbase-0.4.6/skbase/utils/dependencies/__init__.py
+-rw-rw-rw-   0        0        0    10612 2023-05-13 18:22:13.000000 skbase-0.4.6/skbase/utils/dependencies/_dependencies.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:17:00.075256 skbase-0.4.6/skbase/utils/tests/
+-rw-rw-rw-   0        0        0      169 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/utils/tests/__init__.py
+-rw-rw-rw-   0        0        0      774 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/utils/tests/test_check.py
+-rw-rw-rw-   0        0        0     5045 2023-05-04 17:40:43.000000 skbase-0.4.6/skbase/utils/tests/test_iter.py
+-rw-rw-rw-   0        0        0     2314 2023-05-04 17:40:43.000000 skbase-0.4.6/skbase/utils/tests/test_nested_iter.py
+-rw-rw-rw-   0        0        0     1219 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/utils/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:17:00.131232 skbase-0.4.6/skbase/validate/
+-rw-rw-rw-   0        0        0      698 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/validate/__init__.py
+-rw-rw-rw-   0        0        0    15180 2023-05-11 20:27:18.000000 skbase-0.4.6/skbase/validate/_named_objects.py
+-rw-rw-rw-   0        0        0    12466 2023-05-11 20:51:59.000000 skbase-0.4.6/skbase/validate/_types.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:17:00.167020 skbase-0.4.6/skbase/validate/tests/
+-rw-rw-rw-   0        0        0       72 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/validate/tests/__init__.py
+-rw-rw-rw-   0        0        0     7638 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/validate/tests/test_iterable_named_objects.py
+-rw-rw-rw-   0        0        0    14501 2023-04-18 19:57:18.000000 skbase-0.4.6/skbase/validate/tests/test_type_validations.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:16:59.235996 skbase-0.4.6/skbase.egg-info/
+-rw-rw-rw-   0        0        0     6806 2023-06-17 20:16:58.000000 skbase-0.4.6/skbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1907 2023-06-17 20:16:58.000000 skbase-0.4.6/skbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 20:16:58.000000 skbase-0.4.6/skbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      517 2023-06-17 20:16:58.000000 skbase-0.4.6/skbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2023-06-17 20:16:58.000000 skbase-0.4.6/skbase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-12-28 13:43:15.000000 skbase-0.4.6/skbase.egg-info/zip-safe
```

### Comparing `skbase-0.4.5/LICENSE` & `skbase-0.4.6/LICENSE`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2022, skbase Developers
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2022, skbase Developers
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `skbase-0.4.5/PKG-INFO` & `skbase-0.4.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,406 +1,426 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 736b 6261  : 2.1.Name: skba
-00000020: 7365 0a56 6572 7369 6f6e 3a20 302e 342e  se.Version: 0.4.
-00000030: 350a 5375 6d6d 6172 793a 2042 6173 6520  5.Summary: Base 
-00000040: 636c 6173 7365 7320 666f 7220 736b 6c65  classes for skle
-00000050: 6172 6e2d 6c69 6b65 2070 6172 616d 6574  arn-like paramet
-00000060: 7269 6320 6f62 6a65 6374 730a 4175 7468  ric objects.Auth
-00000070: 6f72 3a20 4672 616e 7a20 4b69 72c3 a16c  or: Franz Kir..l
-00000080: 792c 204d 6172 6b75 7320 4cc3 b66e 696e  y, Markus L..nin
-00000090: 672c 2052 7961 6e20 4b75 686e 730a 4d61  g, Ryan Kuhns.Ma
-000000a0: 696e 7461 696e 6572 2d65 6d61 696c 3a20  intainer-email: 
-000000b0: 4672 616e 7a20 4b69 7261 6c79 203c 662e  Franz Kiraly <f.
-000000c0: 6b69 7261 6c79 4075 636c 2e61 632e 756b  kiraly@ucl.ac.uk
-000000d0: 3e2c 2052 7961 6e20 4b75 686e 7320 3c72  >, Ryan Kuhns <r
-000000e0: 6b2e 736b 6261 7365 4067 6d61 696c 2e63  k.skbase@gmail.c
-000000f0: 6f6d 3e0a 4c69 6365 6e73 653a 2042 5344  om>.License: BSD
-00000100: 2033 2d43 6c61 7573 6520 4c69 6365 6e73   3-Clause Licens
-00000110: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
-00000120: 2020 2043 6f70 7972 6967 6874 2028 6329     Copyright (c)
-00000130: 2032 3032 322c 2073 6b62 6173 6520 4465   2022, skbase De
-00000140: 7665 6c6f 7065 7273 0a20 2020 2020 2020  velopers.       
-00000150: 2041 6c6c 2072 6967 6874 7320 7265 7365   All rights rese
-00000160: 7276 6564 2e0a 2020 2020 2020 2020 0a20  rved..        . 
-00000170: 2020 2020 2020 2052 6564 6973 7472 6962         Redistrib
-00000180: 7574 696f 6e20 616e 6420 7573 6520 696e  ution and use in
-00000190: 2073 6f75 7263 6520 616e 6420 6269 6e61   source and bina
-000001a0: 7279 2066 6f72 6d73 2c20 7769 7468 206f  ry forms, with o
-000001b0: 7220 7769 7468 6f75 740a 2020 2020 2020  r without.      
-000001c0: 2020 6d6f 6469 6669 6361 7469 6f6e 2c20    modification, 
-000001d0: 6172 6520 7065 726d 6974 7465 6420 7072  are permitted pr
-000001e0: 6f76 6964 6564 2074 6861 7420 7468 6520  ovided that the 
-000001f0: 666f 6c6c 6f77 696e 6720 636f 6e64 6974  following condit
-00000200: 696f 6e73 2061 7265 206d 6574 3a0a 2020  ions are met:.  
-00000210: 2020 2020 2020 0a20 2020 2020 2020 2031        .        1
-00000220: 2e20 5265 6469 7374 7269 6275 7469 6f6e  . Redistribution
-00000230: 7320 6f66 2073 6f75 7263 6520 636f 6465  s of source code
-00000240: 206d 7573 7420 7265 7461 696e 2074 6865   must retain the
-00000250: 2061 626f 7665 2063 6f70 7972 6967 6874   above copyright
-00000260: 206e 6f74 6963 652c 2074 6869 730a 2020   notice, this.  
-00000270: 2020 2020 2020 2020 206c 6973 7420 6f66           list of
-00000280: 2063 6f6e 6469 7469 6f6e 7320 616e 6420   conditions and 
-00000290: 7468 6520 666f 6c6c 6f77 696e 6720 6469  the following di
-000002a0: 7363 6c61 696d 6572 2e0a 2020 2020 2020  sclaimer..      
-000002b0: 2020 0a20 2020 2020 2020 2032 2e20 5265    .        2. Re
-000002c0: 6469 7374 7269 6275 7469 6f6e 7320 696e  distributions in
-000002d0: 2062 696e 6172 7920 666f 726d 206d 7573   binary form mus
-000002e0: 7420 7265 7072 6f64 7563 6520 7468 6520  t reproduce the 
-000002f0: 6162 6f76 6520 636f 7079 7269 6768 7420  above copyright 
-00000300: 6e6f 7469 6365 2c0a 2020 2020 2020 2020  notice,.        
-00000310: 2020 2074 6869 7320 6c69 7374 206f 6620     this list of 
-00000320: 636f 6e64 6974 696f 6e73 2061 6e64 2074  conditions and t
-00000330: 6865 2066 6f6c 6c6f 7769 6e67 2064 6973  he following dis
-00000340: 636c 6169 6d65 7220 696e 2074 6865 2064  claimer in the d
-00000350: 6f63 756d 656e 7461 7469 6f6e 0a20 2020  ocumentation.   
-00000360: 2020 2020 2020 2020 616e 642f 6f72 206f          and/or o
-00000370: 7468 6572 206d 6174 6572 6961 6c73 2070  ther materials p
-00000380: 726f 7669 6465 6420 7769 7468 2074 6865  rovided with the
-00000390: 2064 6973 7472 6962 7574 696f 6e2e 0a20   distribution.. 
-000003a0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000003b0: 332e 204e 6569 7468 6572 2074 6865 206e  3. Neither the n
-000003c0: 616d 6520 6f66 2074 6865 2063 6f70 7972  ame of the copyr
-000003d0: 6967 6874 2068 6f6c 6465 7220 6e6f 7220  ight holder nor 
-000003e0: 7468 6520 6e61 6d65 7320 6f66 2069 7473  the names of its
-000003f0: 0a20 2020 2020 2020 2020 2020 636f 6e74  .           cont
-00000400: 7269 6275 746f 7273 206d 6179 2062 6520  ributors may be 
-00000410: 7573 6564 2074 6f20 656e 646f 7273 6520  used to endorse 
-00000420: 6f72 2070 726f 6d6f 7465 2070 726f 6475  or promote produ
-00000430: 6374 7320 6465 7269 7665 6420 6672 6f6d  cts derived from
-00000440: 0a20 2020 2020 2020 2020 2020 7468 6973  .           this
-00000450: 2073 6f66 7477 6172 6520 7769 7468 6f75   software withou
-00000460: 7420 7370 6563 6966 6963 2070 7269 6f72  t specific prior
-00000470: 2077 7269 7474 656e 2070 6572 6d69 7373   written permiss
-00000480: 696f 6e2e 0a20 2020 2020 2020 200a 2020  ion..        .  
-00000490: 2020 2020 2020 5448 4953 2053 4f46 5457        THIS SOFTW
-000004a0: 4152 4520 4953 2050 524f 5649 4445 4420  ARE IS PROVIDED 
-000004b0: 4259 2054 4845 2043 4f50 5952 4947 4854  BY THE COPYRIGHT
-000004c0: 2048 4f4c 4445 5253 2041 4e44 2043 4f4e   HOLDERS AND CON
-000004d0: 5452 4942 5554 4f52 5320 2241 5320 4953  TRIBUTORS "AS IS
-000004e0: 220a 2020 2020 2020 2020 414e 4420 414e  ".        AND AN
-000004f0: 5920 4558 5052 4553 5320 4f52 2049 4d50  Y EXPRESS OR IMP
-00000500: 4c49 4544 2057 4152 5241 4e54 4945 532c  LIED WARRANTIES,
-00000510: 2049 4e43 4c55 4449 4e47 2c20 4255 5420   INCLUDING, BUT 
-00000520: 4e4f 5420 4c49 4d49 5445 4420 544f 2c20  NOT LIMITED TO, 
-00000530: 5448 450a 2020 2020 2020 2020 494d 504c  THE.        IMPL
-00000540: 4945 4420 5741 5252 414e 5449 4553 204f  IED WARRANTIES O
-00000550: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
-00000560: 5920 414e 4420 4649 544e 4553 5320 464f  Y AND FITNESS FO
-00000570: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
-00000580: 5552 504f 5345 2041 5245 0a20 2020 2020  URPOSE ARE.     
-00000590: 2020 2044 4953 434c 4149 4d45 442e 2049     DISCLAIMED. I
-000005a0: 4e20 4e4f 2045 5645 4e54 2053 4841 4c4c  N NO EVENT SHALL
-000005b0: 2054 4845 2043 4f50 5952 4947 4854 2048   THE COPYRIGHT H
-000005c0: 4f4c 4445 5220 4f52 2043 4f4e 5452 4942  OLDER OR CONTRIB
-000005d0: 5554 4f52 5320 4245 204c 4941 424c 450a  UTORS BE LIABLE.
-000005e0: 2020 2020 2020 2020 464f 5220 414e 5920          FOR ANY 
-000005f0: 4449 5245 4354 2c20 494e 4449 5245 4354  DIRECT, INDIRECT
-00000600: 2c20 494e 4349 4445 4e54 414c 2c20 5350  , INCIDENTAL, SP
-00000610: 4543 4941 4c2c 2045 5845 4d50 4c41 5259  ECIAL, EXEMPLARY
-00000620: 2c20 4f52 2043 4f4e 5345 5155 454e 5449  , OR CONSEQUENTI
-00000630: 414c 0a20 2020 2020 2020 2044 414d 4147  AL.        DAMAG
-00000640: 4553 2028 494e 434c 5544 494e 472c 2042  ES (INCLUDING, B
-00000650: 5554 204e 4f54 204c 494d 4954 4544 2054  UT NOT LIMITED T
-00000660: 4f2c 2050 524f 4355 5245 4d45 4e54 204f  O, PROCUREMENT O
-00000670: 4620 5355 4253 5449 5455 5445 2047 4f4f  F SUBSTITUTE GOO
-00000680: 4453 204f 520a 2020 2020 2020 2020 5345  DS OR.        SE
-00000690: 5256 4943 4553 3b20 4c4f 5353 204f 4620  RVICES; LOSS OF 
-000006a0: 5553 452c 2044 4154 412c 204f 5220 5052  USE, DATA, OR PR
-000006b0: 4f46 4954 533b 204f 5220 4255 5349 4e45  OFITS; OR BUSINE
-000006c0: 5353 2049 4e54 4552 5255 5054 494f 4e29  SS INTERRUPTION)
-000006d0: 2048 4f57 4556 4552 0a20 2020 2020 2020   HOWEVER.       
-000006e0: 2043 4155 5345 4420 414e 4420 4f4e 2041   CAUSED AND ON A
-000006f0: 4e59 2054 4845 4f52 5920 4f46 204c 4941  NY THEORY OF LIA
-00000700: 4249 4c49 5459 2c20 5748 4554 4845 5220  BILITY, WHETHER 
-00000710: 494e 2043 4f4e 5452 4143 542c 2053 5452  IN CONTRACT, STR
-00000720: 4943 5420 4c49 4142 494c 4954 592c 0a20  ICT LIABILITY,. 
-00000730: 2020 2020 2020 204f 5220 544f 5254 2028         OR TORT (
-00000740: 494e 434c 5544 494e 4720 4e45 474c 4947  INCLUDING NEGLIG
-00000750: 454e 4345 204f 5220 4f54 4845 5257 4953  ENCE OR OTHERWIS
-00000760: 4529 2041 5249 5349 4e47 2049 4e20 414e  E) ARISING IN AN
-00000770: 5920 5741 5920 4f55 5420 4f46 2054 4845  Y WAY OUT OF THE
-00000780: 2055 5345 0a20 2020 2020 2020 204f 4620   USE.        OF 
-00000790: 5448 4953 2053 4f46 5457 4152 452c 2045  THIS SOFTWARE, E
-000007a0: 5645 4e20 4946 2041 4456 4953 4544 204f  VEN IF ADVISED O
-000007b0: 4620 5448 4520 504f 5353 4942 494c 4954  F THE POSSIBILIT
-000007c0: 5920 4f46 2053 5543 4820 4441 4d41 4745  Y OF SUCH DAMAGE
-000007d0: 2e0a 2020 2020 2020 2020 0a50 726f 6a65  ..        .Proje
-000007e0: 6374 2d55 524c 3a20 686f 6d65 7061 6765  ct-URL: homepage
-000007f0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000800: 2e63 6f6d 2f73 6b74 696d 652f 736b 6261  .com/sktime/skba
-00000810: 7365 0a50 726f 6a65 6374 2d55 524c 3a20  se.Project-URL: 
-00000820: 7265 706f 7369 746f 7279 2c20 6874 7470  repository, http
-00000830: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000840: 6b74 696d 652f 736b 6261 7365 0a50 726f  ktime/skbase.Pro
-00000850: 6a65 6374 2d55 524c 3a20 646f 6375 6d65  ject-URL: docume
-00000860: 6e74 6174 696f 6e2c 2068 7474 7073 3a2f  ntation, https:/
-00000870: 2f67 6974 6875 622e 636f 6d2f 736b 7469  /github.com/skti
-00000880: 6d65 2f73 6b62 6173 650a 5072 6f6a 6563  me/skbase.Projec
-00000890: 742d 5552 4c3a 2064 6f77 6e6c 6f61 642c  t-URL: download,
-000008a0: 2068 7474 7073 3a2f 2f70 7970 692e 6f72   https://pypi.or
-000008b0: 672f 7072 6f6a 6563 742f 736b 6261 7365  g/project/skbase
-000008c0: 2f23 6669 6c65 730a 4b65 7977 6f72 6473  /#files.Keywords
-000008d0: 3a20 6461 7461 2d73 6369 656e 6365 2c6d  : data-science,m
-000008e0: 6163 6869 6e65 2d6c 6561 726e 696e 672c  achine-learning,
-000008f0: 7363 696b 6974 2d6c 6561 726e 0a43 6c61  scikit-learn.Cla
-00000900: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-00000910: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
-00000920: 6965 6e63 652f 5265 7365 6172 6368 0a43  ience/Research.C
-00000930: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
-00000940: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000950: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
-00000960: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00000970: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000980: 3a20 4253 4420 4c69 6365 6e73 650a 436c  : BSD License.Cl
-00000990: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000009a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000009b0: 3a20 5079 7468 6f6e 0a43 6c61 7373 6966  : Python.Classif
-000009c0: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
-000009d0: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
-000009e0: 6e74 0a43 6c61 7373 6966 6965 723a 2054  nt.Classifier: T
-000009f0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-00000a00: 6963 2f45 6e67 696e 6565 7269 6e67 0a43  ic/Engineering.C
-00000a10: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-00000a20: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
-00000a30: 6963 726f 736f 6674 203a 3a20 5769 6e64  icrosoft :: Wind
-00000a40: 6f77 730a 436c 6173 7369 6669 6572 3a20  ows.Classifier: 
-00000a50: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000a60: 203a 3a20 504f 5349 580a 436c 6173 7369   :: POSIX.Classi
-00000a70: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00000a80: 5379 7374 656d 203a 3a20 556e 6978 0a43  System :: Unix.C
-00000a90: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-00000aa0: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
-00000ab0: 6163 4f53 0a43 6c61 7373 6966 6965 723a  acOS.Classifier:
-00000ac0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000ad0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000ae0: 3a3a 2033 2e37 0a43 6c61 7373 6966 6965  :: 3.7.Classifie
-00000af0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000b00: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000b10: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
-00000b20: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000b30: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000b40: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
-00000b50: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000b60: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000b70: 7974 686f 6e20 3a3a 2033 2e31 300a 436c  ython :: 3.10.Cl
-00000b80: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000b90: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000ba0: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
-00000bb0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-00000bc0: 3a20 3c33 2e31 322c 3e3d 332e 370a 4465  : <3.12,>=3.7.De
-00000bd0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000be0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000bf0: 6b64 6f77 6e0a 5072 6f76 6964 6573 2d45  kdown.Provides-E
-00000c00: 7874 7261 3a20 616c 6c5f 6578 7472 6173  xtra: all_extras
-00000c10: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000c20: 2064 6576 0a50 726f 7669 6465 732d 4578   dev.Provides-Ex
-00000c30: 7472 613a 206c 696e 7465 7273 0a50 726f  tra: linters.Pro
-00000c40: 7669 6465 732d 4578 7472 613a 2062 696e  vides-Extra: bin
-00000c50: 6465 720a 5072 6f76 6964 6573 2d45 7874  der.Provides-Ext
-00000c60: 7261 3a20 646f 6373 0a50 726f 7669 6465  ra: docs.Provide
-00000c70: 732d 4578 7472 613a 2074 6573 740a 4c69  s-Extra: test.Li
-00000c80: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000c90: 4e53 450a 0a0a 2320 5765 6c63 6f6d 6520  NSE...# Welcome 
-00000ca0: 746f 2073 6b62 6173 650a 0a3e 2041 2062  to skbase..> A b
-00000cb0: 6173 6520 636c 6173 7320 666f 7220 7363  ase class for sc
-00000cc0: 696b 6974 2d6c 6561 726e 2d6c 696b 6520  ikit-learn-like 
-00000cd0: 616e 6420 736b 7469 6d65 2d6c 696b 6520  and sktime-like 
-00000ce0: 7061 7261 6d65 7472 6963 206f 626a 6563  parametric objec
-00000cf0: 7473 0a0a 6073 6b62 6173 6560 2070 726f  ts..`skbase` pro
-00000d00: 7669 6465 7320 6261 7365 2063 6c61 7373  vides base class
-00000d10: 6573 2066 6f72 2063 7265 6174 696e 6720  es for creating 
-00000d20: 7363 696b 6974 2d6c 6561 726e 2d6c 696b  scikit-learn-lik
-00000d30: 6520 7061 7261 6d65 7472 6963 206f 626a  e parametric obj
-00000d40: 6563 7473 2c0a 616c 6f6e 6720 7769 7468  ects,.along with
-00000d50: 2074 6f6f 6c73 2074 6f20 6d61 6b65 2069   tools to make i
-00000d60: 7420 6561 7369 6572 2074 6f20 6275 696c  t easier to buil
-00000d70: 6420 796f 7572 206f 776e 2070 6163 6b61  d your own packa
-00000d80: 6765 7320 7468 6174 2066 6f6c 6c6f 7720  ges that follow 
-00000d90: 7468 6573 650a 6465 7369 676e 2070 6174  these.design pat
-00000da0: 7465 726e 732e 0a0a 3a72 6f63 6b65 743a  terns...:rocket:
-00000db0: 2056 6572 7369 6f6e 2030 2e34 2e35 2069   Version 0.4.5 i
-00000dc0: 7320 6e6f 7720 6176 6169 6c61 626c 652e  s now available.
-00000dd0: 2043 6865 636b 6f75 7420 6f75 720a 5b72   Checkout our.[r
-00000de0: 656c 6561 7365 206e 6f74 6573 5d28 6874  elease notes](ht
-00000df0: 7470 733a 2f2f 736b 6261 7365 2e72 6561  tps://skbase.rea
-00000e00: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000e10: 6174 6573 742f 6368 616e 6765 6c6f 672e  atest/changelog.
-00000e20: 6874 6d6c 292e 0a0a 7c20 4f76 6572 7669  html)...| Overvi
-00000e30: 6577 207c 207c 0a7c 2d2d 2d7c 2d2d 2d7c  ew | |.|---|---|
-00000e40: 0a7c 202a 2a43 492f 4344 2a2a 207c 205b  .| **CI/CD** | [
-00000e50: 215b 5465 7374 735d 2868 7474 7073 3a2f  ![Tests](https:/
-00000e60: 2f67 6974 6875 622e 636f 6d2f 736b 7469  /github.com/skti
-00000e70: 6d65 2f73 6b62 6173 652f 6163 7469 6f6e  me/skbase/action
-00000e80: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
-00000e90: 2e79 6d6c 2f62 6164 6765 2e73 7667 3f62  .yml/badge.svg?b
-00000ea0: 7261 6e63 683d 6d61 696e 295d 2868 7474  ranch=main)](htt
-00000eb0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ec0: 736b 7469 6d65 2f73 6b62 6173 652f 6163  sktime/skbase/ac
-00000ed0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000ee0: 7465 7374 2e79 6d6c 2920 5b21 5b63 6f64  test.yml) [![cod
-00000ef0: 6563 6f76 5d28 6874 7470 733a 2f2f 636f  ecov](https://co
-00000f00: 6465 636f 762e 696f 2f67 682f 736b 7469  decov.io/gh/skti
-00000f10: 6d65 2f73 6b62 6173 652f 6272 616e 6368  me/skbase/branch
-00000f20: 2f6d 6169 6e2f 6772 6170 682f 6261 6467  /main/graph/badg
-00000f30: 652e 7376 673f 746f 6b65 6e3d 324a 3432  e.svg?token=2J42
-00000f40: 344e 4c4f 3832 295d 2868 7474 7073 3a2f  4NLO82)](https:/
-00000f50: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f73  /codecov.io/gh/s
-00000f60: 6b74 696d 652f 736b 6261 7365 2920 5b21  ktime/skbase) [!
-00000f70: 5b44 6f63 756d 656e 7461 7469 6f6e 2053  [Documentation S
-00000f80: 7461 7475 735d 2868 7474 7073 3a2f 2f72  tatus](https://r
-00000f90: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
-00000fa0: 726f 6a65 6374 732f 736b 6261 7365 2f62  rojects/skbase/b
-00000fb0: 6164 6765 2f3f 7665 7273 696f 6e3d 6c61  adge/?version=la
-00000fc0: 7465 7374 295d 2868 7474 7073 3a2f 2f73  test)](https://s
-00000fd0: 6b62 6173 652e 7265 6164 7468 6564 6f63  kbase.readthedoc
-00000fe0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f3f  s.io/en/latest/?
-00000ff0: 6261 6467 653d 6c61 7465 7374 2920 5b21  badge=latest) [!
-00001000: 5b70 7265 2d63 6f6d 6d69 742e 6369 2073  [pre-commit.ci s
-00001010: 7461 7475 735d 2868 7474 7073 3a2f 2f72  tatus](https://r
-00001020: 6573 756c 7473 2e70 7265 2d63 6f6d 6d69  esults.pre-commi
-00001030: 742e 6369 2f62 6164 6765 2f67 6974 6875  t.ci/badge/githu
-00001040: 622f 736b 7469 6d65 2f73 6b62 6173 652f  b/sktime/skbase/
-00001050: 6d61 696e 2e73 7667 295d 2868 7474 7073  main.svg)](https
-00001060: 3a2f 2f72 6573 756c 7473 2e70 7265 2d63  ://results.pre-c
-00001070: 6f6d 6d69 742e 6369 2f6c 6174 6573 742f  ommit.ci/latest/
-00001080: 6769 7468 7562 2f73 6b74 696d 652f 736b  github/sktime/sk
-00001090: 6261 7365 2f6d 6169 6e29 207c 0a7c 202a  base/main) |.| *
-000010a0: 2a43 6f64 652a 2a20 7c20 205b 215b 2170  *Code** |  [![!p
-000010b0: 7970 695d 2868 7474 7073 3a2f 2f69 6d67  ypi](https://img
-000010c0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000010d0: 2f76 2f73 6369 6b69 742d 6261 7365 3f63  /v/scikit-base?c
-000010e0: 6f6c 6f72 3d6f 7261 6e67 6529 5d28 6874  olor=orange)](ht
-000010f0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00001100: 726f 6a65 6374 2f73 6b62 6173 652f 2920  roject/skbase/) 
-00001110: 205b 215b 2170 7974 686f 6e2d 7665 7273   [![!python-vers
-00001120: 696f 6e73 5d28 6874 7470 733a 2f2f 696d  ions](https://im
-00001130: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00001140: 692f 7079 7665 7273 696f 6e73 2f73 6369  i/pyversions/sci
-00001150: 6b69 742d 6261 7365 295d 2868 7474 7073  kit-base)](https
-00001160: 3a2f 2f77 7777 2e70 7974 686f 6e2e 6f72  ://www.python.or
-00001170: 672f 2920 5b21 5b21 626c 6163 6b5d 2868  g/) [![!black](h
-00001180: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00001190: 6473 2e69 6f2f 6261 6467 652f 636f 6465  ds.io/badge/code
-000011a0: 2532 3073 7479 6c65 2d62 6c61 636b 2d30  %20style-black-0
-000011b0: 3030 3030 302e 7376 6729 5d28 6874 7470  00000.svg)](http
-000011c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-000011d0: 7366 2f62 6c61 636b 2920 5b21 5b73 6563  sf/black) [![sec
-000011e0: 7572 6974 793a 2062 616e 6469 745d 2868  urity: bandit](h
-000011f0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00001200: 6473 2e69 6f2f 6261 6467 652f 7365 6375  ds.io/badge/secu
-00001210: 7269 7479 2d62 616e 6469 742d 7965 6c6c  rity-bandit-yell
-00001220: 6f77 2e73 7667 295d 2868 7474 7073 3a2f  ow.svg)](https:/
-00001230: 2f67 6974 6875 622e 636f 6d2f 5079 4351  /github.com/PyCQ
-00001240: 412f 6261 6e64 6974 2920 7c0a 7c20 2a2a  A/bandit) |.| **
-00001250: 446f 776e 6c6f 6164 732a 2a7c 205b 215b  Downloads**| [![
-00001260: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
-00001270: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
-00001280: 6563 682f 7065 7273 6f6e 616c 697a 6564  ech/personalized
-00001290: 2d62 6164 6765 2f73 6369 6b69 742d 6261  -badge/scikit-ba
-000012a0: 7365 3f70 6572 696f 643d 7765 656b 2675  se?period=week&u
-000012b0: 6e69 7473 3d69 6e74 6572 6e61 7469 6f6e  nits=internation
-000012c0: 616c 5f73 7973 7465 6d26 6c65 6674 5f63  al_system&left_c
-000012d0: 6f6c 6f72 3d67 7265 7926 7269 6768 745f  olor=grey&right_
-000012e0: 636f 6c6f 723d 626c 7565 266c 6566 745f  color=blue&left_
-000012f0: 7465 7874 3d77 6565 6b6c 7925 3230 2870  text=weekly%20(p
-00001300: 7970 6929 295d 2868 7474 7073 3a2f 2f70  ypi))](https://p
-00001310: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
-00001320: 2f73 6369 6b69 742d 6261 7365 2920 5b21  /scikit-base) [!
-00001330: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
-00001340: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
-00001350: 7465 6368 2f70 6572 736f 6e61 6c69 7a65  tech/personalize
-00001360: 642d 6261 6467 652f 7363 696b 6974 2d62  d-badge/scikit-b
-00001370: 6173 653f 7065 7269 6f64 3d6d 6f6e 7468  ase?period=month
-00001380: 2675 6e69 7473 3d69 6e74 6572 6e61 7469  &units=internati
-00001390: 6f6e 616c 5f73 7973 7465 6d26 6c65 6674  onal_system&left
-000013a0: 5f63 6f6c 6f72 3d67 7265 7926 7269 6768  _color=grey&righ
-000013b0: 745f 636f 6c6f 723d 626c 7565 266c 6566  t_color=blue&lef
-000013c0: 745f 7465 7874 3d6d 6f6e 7468 6c79 2532  t_text=monthly%2
-000013d0: 3028 7079 7069 2929 5d28 6874 7470 733a  0(pypi))](https:
-000013e0: 2f2f 7065 7079 2e74 6563 682f 7072 6f6a  //pepy.tech/proj
-000013f0: 6563 742f 7363 696b 6974 2d62 6173 6529  ect/scikit-base)
-00001400: 205b 215b 446f 776e 6c6f 6164 735d 2868   [![Downloads](h
-00001410: 7474 7073 3a2f 2f73 7461 7469 632e 7065  ttps://static.pe
-00001420: 7079 2e74 6563 682f 7065 7273 6f6e 616c  py.tech/personal
-00001430: 697a 6564 2d62 6164 6765 2f73 6369 6b69  ized-badge/sciki
-00001440: 742d 6261 7365 3f70 6572 696f 643d 746f  t-base?period=to
-00001450: 7461 6c26 756e 6974 733d 696e 7465 726e  tal&units=intern
-00001460: 6174 696f 6e61 6c5f 7379 7374 656d 266c  ational_system&l
-00001470: 6566 745f 636f 6c6f 723d 6772 6579 2672  eft_color=grey&r
-00001480: 6967 6874 5f63 6f6c 6f72 3d62 6c75 6526  ight_color=blue&
-00001490: 6c65 6674 5f74 6578 743d 6375 6d75 6c61  left_text=cumula
-000014a0: 7469 7665 2532 3028 7079 7069 2929 5d28  tive%20(pypi))](
-000014b0: 6874 7470 733a 2f2f 7065 7079 2e74 6563  https://pepy.tec
-000014c0: 682f 7072 6f6a 6563 742f 7363 696b 6974  h/project/scikit
-000014d0: 2d62 6173 6529 207c 0a0a 3c21 2d2d 2041  -base) |..<!-- A
-000014e0: 4c4c 2d43 4f4e 5452 4942 5554 4f52 532d  LL-CONTRIBUTORS-
-000014f0: 4241 4447 453a 5354 4152 5420 2d20 446f  BADGE:START - Do
-00001500: 206e 6f74 2072 656d 6f76 6520 6f72 206d   not remove or m
-00001510: 6f64 6966 7920 7468 6973 2073 6563 7469  odify this secti
-00001520: 6f6e 202d 2d3e 0a5b 215b 416c 6c20 436f  on -->.[![All Co
-00001530: 6e74 7269 6275 746f 7273 5d28 6874 7470  ntributors](http
-00001540: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00001550: 696f 2f62 6164 6765 2f61 6c6c 5f63 6f6e  io/badge/all_con
-00001560: 7472 6962 7574 6f72 732d 3133 2d6f 7261  tributors-13-ora
-00001570: 6e67 652e 7376 673f 7374 796c 653d 666c  nge.svg?style=fl
-00001580: 6174 2d73 7175 6172 6529 5d28 2363 6f6e  at-square)](#con
-00001590: 7472 6962 7574 6f72 7329 0a3c 212d 2d20  tributors).<!-- 
-000015a0: 414c 4c2d 434f 4e54 5249 4255 544f 5253  ALL-CONTRIBUTORS
-000015b0: 2d42 4144 4745 3a45 4e44 202d 2d3e 0a0a  -BADGE:END -->..
-000015c0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-000015d0: 0a0a 546f 206c 6561 726e 206d 6f72 6520  ..To learn more 
-000015e0: 6162 6f75 7420 7468 6520 7061 636b 6167  about the packag
-000015f0: 6520 6368 6563 6b6f 7574 206f 7572 205b  e checkout our [
-00001600: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-00001610: 7474 7073 3a2f 2f73 6b62 6173 652e 7265  ttps://skbase.re
-00001620: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00001630: 6c61 7465 7374 2f29 2e0a 0a23 2320 3a68  latest/)...## :h
-00001640: 6f75 7267 6c61 7373 5f66 6c6f 7769 6e67  ourglass_flowing
-00001650: 5f73 616e 643a 2049 6e73 7461 6c6c 2073  _sand: Install s
-00001660: 6b62 6173 650a 466f 7220 7472 6f75 626c  kbase.For troubl
-00001670: 6520 7368 6f6f 7469 6e67 206f 7220 6d6f  e shooting or mo
-00001680: 7265 2069 6e66 6f72 6d61 7469 6f6e 2c20  re information, 
-00001690: 7365 6520 6f75 720a 5b64 6574 6169 6c65  see our.[detaile
-000016a0: 6420 696e 7374 616c 6c61 7469 6f6e 2069  d installation i
-000016b0: 6e73 7472 7563 7469 6f6e 735d 2868 7474  nstructions](htt
-000016c0: 7073 3a2f 2f73 6b62 6173 652e 7265 6164  ps://skbase.read
-000016d0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000016e0: 7465 7374 2f75 7365 725f 646f 6375 6d65  test/user_docume
-000016f0: 6e74 6174 696f 6e2f 696e 7374 616c 6c61  ntation/installa
-00001700: 7469 6f6e 2e68 746d 6c29 2e0a 0a2d 202a  tion.html)...- *
-00001710: 2a4f 7065 7261 7469 6e67 2073 7973 7465  *Operating syste
-00001720: 6d2a 2a3a 206d 6163 4f53 2058 20c2 b720  m**: macOS X .. 
-00001730: 4c69 6e75 7820 c2b7 2057 696e 646f 7773  Linux .. Windows
-00001740: 2038 2e31 206f 7220 6869 6768 6572 0a2d   8.1 or higher.-
-00001750: 202a 2a50 7974 686f 6e20 7665 7273 696f   **Python versio
-00001760: 6e2a 2a3a 2050 7974 686f 6e20 332e 372c  n**: Python 3.7,
-00001770: 2033 2e38 2c20 332e 392c 2033 2e31 3020   3.8, 3.9, 3.10 
-00001780: 616e 6420 332e 3131 0a2d 202a 2a50 6163  and 3.11.- **Pac
-00001790: 6b61 6765 206d 616e 6167 6572 732a 2a3a  kage managers**:
-000017a0: 205b 7069 705d 0a0a 5b70 6970 5d3a 2068   [pip]..[pip]: h
-000017b0: 7474 7073 3a2f 2f70 6970 2e70 7970 612e  ttps://pip.pypa.
-000017c0: 696f 2f65 6e2f 7374 6162 6c65 2f0a 0a23  io/en/stable/..#
-000017d0: 2323 2070 6970 0a73 6b62 6173 6520 7265  ## pip.skbase re
-000017e0: 6c65 6173 6573 2061 7265 2061 7661 696c  leases are avail
-000017f0: 6162 6c65 2061 7320 736f 7572 6365 2070  able as source p
-00001800: 6163 6b61 6765 7320 616e 6420 6269 6e61  ackages and bina
-00001810: 7279 2077 6865 656c 7320 7669 6120 5079  ry wheels via Py
-00001820: 5049 0a61 6e64 2063 616e 2062 6520 696e  PI.and can be in
-00001830: 7374 616c 6c65 6420 7573 696e 6720 7069  stalled using pi
-00001840: 702e 2043 6865 636b 6f75 7420 7468 6520  p. Checkout the 
-00001850: 6675 6c6c 206c 6973 7420 6f66 2070 7265  full list of pre
-00001860: 2d63 6f6d 7069 6c65 6420 5b77 6865 656c  -compiled [wheel
-00001870: 7320 6f6e 2050 7950 695d 2868 7474 7073  s on PyPi](https
-00001880: 3a2f 2f70 7970 692e 6f72 672f 7369 6d70  ://pypi.org/simp
-00001890: 6c65 2f73 6b62 6173 652f 292e 0a0a 546f  le/skbase/)...To
-000018a0: 2069 6e73 7461 6c6c 2074 6865 2063 6f72   install the cor
-000018b0: 6520 7061 636b 6167 6520 7573 653a 0a0a  e package use:..
-000018c0: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
-000018d0: 616c 6c20 7363 696b 6974 2d62 6173 650a  all scikit-base.
-000018e0: 6060 600a 0a6f 722c 2069 6620 796f 7520  ```..or, if you 
-000018f0: 7761 6e74 2074 6f20 696e 7374 616c 6c20  want to install 
-00001900: 7769 7468 2074 6865 206d 6178 696d 756d  with the maximum
-00001910: 2073 6574 206f 6620 6465 7065 6e64 656e   set of dependen
-00001920: 6369 6573 2c20 7573 653a 0a0a 6060 6062  cies, use:..```b
-00001930: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-00001940: 7363 696b 6974 2d62 6173 655b 616c 6c5f  scikit-base[all_
-00001950: 6578 7472 6173 5d0a 6060 600a            extras].```.
+00000010: 3a20 322e 310d 0a4e 616d 653a 2073 6b62  : 2.1..Name: skb
+00000020: 6173 650d 0a56 6572 7369 6f6e 3a20 302e  ase..Version: 0.
+00000030: 342e 360d 0a53 756d 6d61 7279 3a20 4261  4.6..Summary: Ba
+00000040: 7365 2063 6c61 7373 6573 2066 6f72 2073  se classes for s
+00000050: 6b6c 6561 726e 2d6c 696b 6520 7061 7261  klearn-like para
+00000060: 6d65 7472 6963 206f 626a 6563 7473 0d0a  metric objects..
+00000070: 4175 7468 6f72 2d65 6d61 696c 3a20 736b  Author-email: sk
+00000080: 7469 6d65 2064 6576 656c 6f70 6572 7320  time developers 
+00000090: 3c73 6b74 696d 652e 746f 6f6c 626f 7840  <sktime.toolbox@
+000000a0: 676d 6169 6c2e 636f 6d3e 0d0a 4d61 696e  gmail.com>..Main
+000000b0: 7461 696e 6572 3a20 4672 616e 7a20 4b69  tainer: Franz Ki
+000000c0: 72c3 a16c 790d 0a4d 6169 6e74 6169 6e65  r..ly..Maintaine
+000000d0: 722d 656d 6169 6c3a 2073 6b74 696d 6520  r-email: sktime 
+000000e0: 6465 7665 6c6f 7065 7273 203c 736b 7469  developers <skti
+000000f0: 6d65 2e74 6f6f 6c62 6f78 4067 6d61 696c  me.toolbox@gmail
+00000100: 2e63 6f6d 3e0d 0a4c 6963 656e 7365 3a20  .com>..License: 
+00000110: 4253 4420 332d 436c 6175 7365 204c 6963  BSD 3-Clause Lic
+00000120: 656e 7365 0d0a 2020 2020 2020 2020 0d0a  ense..        ..
+00000130: 2020 2020 2020 2020 436f 7079 7269 6768          Copyrigh
+00000140: 7420 2863 2920 3230 3232 2c20 736b 6261  t (c) 2022, skba
+00000150: 7365 2044 6576 656c 6f70 6572 730d 0a20  se Developers.. 
+00000160: 2020 2020 2020 2041 6c6c 2072 6967 6874         All right
+00000170: 7320 7265 7365 7276 6564 2e0d 0a20 2020  s reserved...   
+00000180: 2020 2020 200d 0a20 2020 2020 2020 2052       ..        R
+00000190: 6564 6973 7472 6962 7574 696f 6e20 616e  edistribution an
+000001a0: 6420 7573 6520 696e 2073 6f75 7263 6520  d use in source 
+000001b0: 616e 6420 6269 6e61 7279 2066 6f72 6d73  and binary forms
+000001c0: 2c20 7769 7468 206f 7220 7769 7468 6f75  , with or withou
+000001d0: 740d 0a20 2020 2020 2020 206d 6f64 6966  t..        modif
+000001e0: 6963 6174 696f 6e2c 2061 7265 2070 6572  ication, are per
+000001f0: 6d69 7474 6564 2070 726f 7669 6465 6420  mitted provided 
+00000200: 7468 6174 2074 6865 2066 6f6c 6c6f 7769  that the followi
+00000210: 6e67 2063 6f6e 6469 7469 6f6e 7320 6172  ng conditions ar
+00000220: 6520 6d65 743a 0d0a 2020 2020 2020 2020  e met:..        
+00000230: 0d0a 2020 2020 2020 2020 312e 2052 6564  ..        1. Red
+00000240: 6973 7472 6962 7574 696f 6e73 206f 6620  istributions of 
+00000250: 736f 7572 6365 2063 6f64 6520 6d75 7374  source code must
+00000260: 2072 6574 6169 6e20 7468 6520 6162 6f76   retain the abov
+00000270: 6520 636f 7079 7269 6768 7420 6e6f 7469  e copyright noti
+00000280: 6365 2c20 7468 6973 0d0a 2020 2020 2020  ce, this..      
+00000290: 2020 2020 206c 6973 7420 6f66 2063 6f6e       list of con
+000002a0: 6469 7469 6f6e 7320 616e 6420 7468 6520  ditions and the 
+000002b0: 666f 6c6c 6f77 696e 6720 6469 7363 6c61  following discla
+000002c0: 696d 6572 2e0d 0a20 2020 2020 2020 200d  imer...        .
+000002d0: 0a20 2020 2020 2020 2032 2e20 5265 6469  .        2. Redi
+000002e0: 7374 7269 6275 7469 6f6e 7320 696e 2062  stributions in b
+000002f0: 696e 6172 7920 666f 726d 206d 7573 7420  inary form must 
+00000300: 7265 7072 6f64 7563 6520 7468 6520 6162  reproduce the ab
+00000310: 6f76 6520 636f 7079 7269 6768 7420 6e6f  ove copyright no
+00000320: 7469 6365 2c0d 0a20 2020 2020 2020 2020  tice,..         
+00000330: 2020 7468 6973 206c 6973 7420 6f66 2063    this list of c
+00000340: 6f6e 6469 7469 6f6e 7320 616e 6420 7468  onditions and th
+00000350: 6520 666f 6c6c 6f77 696e 6720 6469 7363  e following disc
+00000360: 6c61 696d 6572 2069 6e20 7468 6520 646f  laimer in the do
+00000370: 6375 6d65 6e74 6174 696f 6e0d 0a20 2020  cumentation..   
+00000380: 2020 2020 2020 2020 616e 642f 6f72 206f          and/or o
+00000390: 7468 6572 206d 6174 6572 6961 6c73 2070  ther materials p
+000003a0: 726f 7669 6465 6420 7769 7468 2074 6865  rovided with the
+000003b0: 2064 6973 7472 6962 7574 696f 6e2e 0d0a   distribution...
+000003c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000003d0: 2020 332e 204e 6569 7468 6572 2074 6865    3. Neither the
+000003e0: 206e 616d 6520 6f66 2074 6865 2063 6f70   name of the cop
+000003f0: 7972 6967 6874 2068 6f6c 6465 7220 6e6f  yright holder no
+00000400: 7220 7468 6520 6e61 6d65 7320 6f66 2069  r the names of i
+00000410: 7473 0d0a 2020 2020 2020 2020 2020 2063  ts..           c
+00000420: 6f6e 7472 6962 7574 6f72 7320 6d61 7920  ontributors may 
+00000430: 6265 2075 7365 6420 746f 2065 6e64 6f72  be used to endor
+00000440: 7365 206f 7220 7072 6f6d 6f74 6520 7072  se or promote pr
+00000450: 6f64 7563 7473 2064 6572 6976 6564 2066  oducts derived f
+00000460: 726f 6d0d 0a20 2020 2020 2020 2020 2020  rom..           
+00000470: 7468 6973 2073 6f66 7477 6172 6520 7769  this software wi
+00000480: 7468 6f75 7420 7370 6563 6966 6963 2070  thout specific p
+00000490: 7269 6f72 2077 7269 7474 656e 2070 6572  rior written per
+000004a0: 6d69 7373 696f 6e2e 0d0a 2020 2020 2020  mission...      
+000004b0: 2020 0d0a 2020 2020 2020 2020 5448 4953    ..        THIS
+000004c0: 2053 4f46 5457 4152 4520 4953 2050 524f   SOFTWARE IS PRO
+000004d0: 5649 4445 4420 4259 2054 4845 2043 4f50  VIDED BY THE COP
+000004e0: 5952 4947 4854 2048 4f4c 4445 5253 2041  YRIGHT HOLDERS A
+000004f0: 4e44 2043 4f4e 5452 4942 5554 4f52 5320  ND CONTRIBUTORS 
+00000500: 2241 5320 4953 220d 0a20 2020 2020 2020  "AS IS"..       
+00000510: 2041 4e44 2041 4e59 2045 5850 5245 5353   AND ANY EXPRESS
+00000520: 204f 5220 494d 504c 4945 4420 5741 5252   OR IMPLIED WARR
+00000530: 414e 5449 4553 2c20 494e 434c 5544 494e  ANTIES, INCLUDIN
+00000540: 472c 2042 5554 204e 4f54 204c 494d 4954  G, BUT NOT LIMIT
+00000550: 4544 2054 4f2c 2054 4845 0d0a 2020 2020  ED TO, THE..    
+00000560: 2020 2020 494d 504c 4945 4420 5741 5252      IMPLIED WARR
+00000570: 414e 5449 4553 204f 4620 4d45 5243 4841  ANTIES OF MERCHA
+00000580: 4e54 4142 494c 4954 5920 414e 4420 4649  NTABILITY AND FI
+00000590: 544e 4553 5320 464f 5220 4120 5041 5254  TNESS FOR A PART
+000005a0: 4943 554c 4152 2050 5552 504f 5345 2041  ICULAR PURPOSE A
+000005b0: 5245 0d0a 2020 2020 2020 2020 4449 5343  RE..        DISC
+000005c0: 4c41 494d 4544 2e20 494e 204e 4f20 4556  LAIMED. IN NO EV
+000005d0: 454e 5420 5348 414c 4c20 5448 4520 434f  ENT SHALL THE CO
+000005e0: 5059 5249 4748 5420 484f 4c44 4552 204f  PYRIGHT HOLDER O
+000005f0: 5220 434f 4e54 5249 4255 544f 5253 2042  R CONTRIBUTORS B
+00000600: 4520 4c49 4142 4c45 0d0a 2020 2020 2020  E LIABLE..      
+00000610: 2020 464f 5220 414e 5920 4449 5245 4354    FOR ANY DIRECT
+00000620: 2c20 494e 4449 5245 4354 2c20 494e 4349  , INDIRECT, INCI
+00000630: 4445 4e54 414c 2c20 5350 4543 4941 4c2c  DENTAL, SPECIAL,
+00000640: 2045 5845 4d50 4c41 5259 2c20 4f52 2043   EXEMPLARY, OR C
+00000650: 4f4e 5345 5155 454e 5449 414c 0d0a 2020  ONSEQUENTIAL..  
+00000660: 2020 2020 2020 4441 4d41 4745 5320 2849        DAMAGES (I
+00000670: 4e43 4c55 4449 4e47 2c20 4255 5420 4e4f  NCLUDING, BUT NO
+00000680: 5420 4c49 4d49 5445 4420 544f 2c20 5052  T LIMITED TO, PR
+00000690: 4f43 5552 454d 454e 5420 4f46 2053 5542  OCUREMENT OF SUB
+000006a0: 5354 4954 5554 4520 474f 4f44 5320 4f52  STITUTE GOODS OR
+000006b0: 0d0a 2020 2020 2020 2020 5345 5256 4943  ..        SERVIC
+000006c0: 4553 3b20 4c4f 5353 204f 4620 5553 452c  ES; LOSS OF USE,
+000006d0: 2044 4154 412c 204f 5220 5052 4f46 4954   DATA, OR PROFIT
+000006e0: 533b 204f 5220 4255 5349 4e45 5353 2049  S; OR BUSINESS I
+000006f0: 4e54 4552 5255 5054 494f 4e29 2048 4f57  NTERRUPTION) HOW
+00000700: 4556 4552 0d0a 2020 2020 2020 2020 4341  EVER..        CA
+00000710: 5553 4544 2041 4e44 204f 4e20 414e 5920  USED AND ON ANY 
+00000720: 5448 454f 5259 204f 4620 4c49 4142 494c  THEORY OF LIABIL
+00000730: 4954 592c 2057 4845 5448 4552 2049 4e20  ITY, WHETHER IN 
+00000740: 434f 4e54 5241 4354 2c20 5354 5249 4354  CONTRACT, STRICT
+00000750: 204c 4941 4249 4c49 5459 2c0d 0a20 2020   LIABILITY,..   
+00000760: 2020 2020 204f 5220 544f 5254 2028 494e       OR TORT (IN
+00000770: 434c 5544 494e 4720 4e45 474c 4947 454e  CLUDING NEGLIGEN
+00000780: 4345 204f 5220 4f54 4845 5257 4953 4529  CE OR OTHERWISE)
+00000790: 2041 5249 5349 4e47 2049 4e20 414e 5920   ARISING IN ANY 
+000007a0: 5741 5920 4f55 5420 4f46 2054 4845 2055  WAY OUT OF THE U
+000007b0: 5345 0d0a 2020 2020 2020 2020 4f46 2054  SE..        OF T
+000007c0: 4849 5320 534f 4654 5741 5245 2c20 4556  HIS SOFTWARE, EV
+000007d0: 454e 2049 4620 4144 5649 5345 4420 4f46  EN IF ADVISED OF
+000007e0: 2054 4845 2050 4f53 5349 4249 4c49 5459   THE POSSIBILITY
+000007f0: 204f 4620 5355 4348 2044 414d 4147 452e   OF SUCH DAMAGE.
+00000800: 0d0a 2020 2020 2020 2020 0d0a 5072 6f6a  ..        ..Proj
+00000810: 6563 742d 5552 4c3a 2068 6f6d 6570 6167  ect-URL: homepag
+00000820: 652c 2068 7474 7073 3a2f 2f67 6974 6875  e, https://githu
+00000830: 622e 636f 6d2f 736b 7469 6d65 2f73 6b62  b.com/sktime/skb
+00000840: 6173 650d 0a50 726f 6a65 6374 2d55 524c  ase..Project-URL
+00000850: 3a20 7265 706f 7369 746f 7279 2c20 6874  : repository, ht
+00000860: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000870: 2f73 6b74 696d 652f 736b 6261 7365 0d0a  /sktime/skbase..
+00000880: 5072 6f6a 6563 742d 5552 4c3a 2064 6f63  Project-URL: doc
+00000890: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
+000008a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+000008b0: 6b74 696d 652f 736b 6261 7365 0d0a 5072  ktime/skbase..Pr
+000008c0: 6f6a 6563 742d 5552 4c3a 2064 6f77 6e6c  oject-URL: downl
+000008d0: 6f61 642c 2068 7474 7073 3a2f 2f70 7970  oad, https://pyp
+000008e0: 692e 6f72 672f 7072 6f6a 6563 742f 736b  i.org/project/sk
+000008f0: 6261 7365 2f23 6669 6c65 730d 0a4b 6579  base/#files..Key
+00000900: 776f 7264 733a 2064 6174 612d 7363 6965  words: data-scie
+00000910: 6e63 652c 6d61 6368 696e 652d 6c65 6172  nce,machine-lear
+00000920: 6e69 6e67 2c73 6369 6b69 742d 6c65 6172  ning,scikit-lear
+00000930: 6e0d 0a43 6c61 7373 6966 6965 723a 2049  n..Classifier: I
+00000940: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000950: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
+00000960: 6172 6368 0d0a 436c 6173 7369 6669 6572  arch..Classifier
+00000970: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
+00000980: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+00000990: 730d 0a43 6c61 7373 6966 6965 723a 204c  s..Classifier: L
+000009a0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000009b0: 7072 6f76 6564 203a 3a20 4253 4420 4c69  proved :: BSD Li
+000009c0: 6365 6e73 650d 0a43 6c61 7373 6966 6965  cense..Classifie
+000009d0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000009e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000009f0: 6e0d 0a43 6c61 7373 6966 6965 723a 2054  n..Classifier: T
+00000a00: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000a10: 2044 6576 656c 6f70 6d65 6e74 0d0a 436c   Development..Cl
+00000a20: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+00000a30: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+00000a40: 6769 6e65 6572 696e 670d 0a43 6c61 7373  gineering..Class
+00000a50: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+00000a60: 2053 7973 7465 6d20 3a3a 204d 6963 726f   System :: Micro
+00000a70: 736f 6674 203a 3a20 5769 6e64 6f77 730d  soft :: Windows.
+00000a80: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000a90: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000aa0: 2050 4f53 4958 0d0a 436c 6173 7369 6669   POSIX..Classifi
+00000ab0: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+00000ac0: 7374 656d 203a 3a20 556e 6978 0d0a 436c  stem :: Unix..Cl
+00000ad0: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+00000ae0: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
+00000af0: 634f 530d 0a43 6c61 7373 6966 6965 723a  cOS..Classifier:
+00000b00: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000b10: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000b20: 3a3a 2033 2e37 0d0a 436c 6173 7369 6669  :: 3.7..Classifi
+00000b30: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000b40: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000b50: 6f6e 203a 3a20 332e 380d 0a43 6c61 7373  on :: 3.8..Class
+00000b60: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000b70: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000b80: 7974 686f 6e20 3a3a 2033 2e39 0d0a 436c  ython :: 3.9..Cl
+00000b90: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000ba0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000bb0: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000bc0: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
+00000bd0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000be0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000bf0: 332e 3131 0d0a 5265 7175 6972 6573 2d50  3.11..Requires-P
+00000c00: 7974 686f 6e3a 203c 332e 3132 2c3e 3d33  ython: <3.12,>=3
+00000c10: 2e37 0d0a 4465 7363 7269 7074 696f 6e2d  .7..Description-
+00000c20: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+00000c30: 7874 2f6d 6172 6b64 6f77 6e0d 0a50 726f  xt/markdown..Pro
+00000c40: 7669 6465 732d 4578 7472 613a 2061 6c6c  vides-Extra: all
+00000c50: 5f65 7874 7261 730d 0a50 726f 7669 6465  _extras..Provide
+00000c60: 732d 4578 7472 613a 2064 6576 0d0a 5072  s-Extra: dev..Pr
+00000c70: 6f76 6964 6573 2d45 7874 7261 3a20 6c69  ovides-Extra: li
+00000c80: 6e74 6572 730d 0a50 726f 7669 6465 732d  nters..Provides-
+00000c90: 4578 7472 613a 2062 696e 6465 720d 0a50  Extra: binder..P
+00000ca0: 726f 7669 6465 732d 4578 7472 613a 2064  rovides-Extra: d
+00000cb0: 6f63 730d 0a50 726f 7669 6465 732d 4578  ocs..Provides-Ex
+00000cc0: 7472 613a 2074 6573 740d 0a4c 6963 656e  tra: test..Licen
+00000cd0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+00000ce0: 0d0a 0d0a 3c61 2068 7265 663d 2268 7474  ....<a href="htt
+00000cf0: 7073 3a2f 2f73 6b62 6173 652e 7265 6164  ps://skbase.read
+00000d00: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000d10: 7465 7374 2f22 3e3c 696d 6720 7372 633d  test/"><img src=
+00000d20: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000d30: 636f 6d2f 736b 7469 6d65 2f73 6b62 6173  com/sktime/skbas
+00000d40: 652f 626c 6f62 2f6d 6169 6e2f 646f 6373  e/blob/main/docs
+00000d50: 2f73 6f75 7263 652f 696d 6167 6573 2f73  /source/images/s
+00000d60: 6b62 6173 652d 6c6f 676f 2d77 6974 682d  kbase-logo-with-
+00000d70: 6e61 6d65 2e70 6e67 2220 7769 6474 683d  name.png" width=
+00000d80: 2231 3735 2220 616c 6967 6e3d 2272 6967  "175" align="rig
+00000d90: 6874 2220 2f3e 3c2f 613e 0d0a 0d0a 2320  ht" /></a>....# 
+00000da0: 5765 6c63 6f6d 6520 746f 2073 6b62 6173  Welcome to skbas
+00000db0: 650d 0a0d 0a3e 2041 2062 6173 6520 636c  e....> A base cl
+00000dc0: 6173 7320 666f 7220 7363 696b 6974 2d6c  ass for scikit-l
+00000dd0: 6561 726e 2d6c 696b 6520 616e 6420 736b  earn-like and sk
+00000de0: 7469 6d65 2d6c 696b 6520 7061 7261 6d65  time-like parame
+00000df0: 7472 6963 206f 626a 6563 7473 0d0a 0d0a  tric objects....
+00000e00: 6073 6b62 6173 6560 2070 726f 7669 6465  `skbase` provide
+00000e10: 7320 6261 7365 2063 6c61 7373 6573 2066  s base classes f
+00000e20: 6f72 2063 7265 6174 696e 6720 7363 696b  or creating scik
+00000e30: 6974 2d6c 6561 726e 2d6c 696b 6520 7061  it-learn-like pa
+00000e40: 7261 6d65 7472 6963 206f 626a 6563 7473  rametric objects
+00000e50: 2c0d 0a61 6c6f 6e67 2077 6974 6820 746f  ,..along with to
+00000e60: 6f6c 7320 746f 206d 616b 6520 6974 2065  ols to make it e
+00000e70: 6173 6965 7220 746f 2062 7569 6c64 2079  asier to build y
+00000e80: 6f75 7220 6f77 6e20 7061 636b 6167 6573  our own packages
+00000e90: 2074 6861 7420 666f 6c6c 6f77 2074 6865   that follow the
+00000ea0: 7365 0d0a 6465 7369 676e 2070 6174 7465  se..design patte
+00000eb0: 726e 732e 0d0a 0d0a 3a72 6f63 6b65 743a  rns.....:rocket:
+00000ec0: 2056 6572 7369 6f6e 2030 2e34 2e36 2069   Version 0.4.6 i
+00000ed0: 7320 6e6f 7720 6176 6169 6c61 626c 652e  s now available.
+00000ee0: 2043 6865 636b 6f75 7420 6f75 720d 0a5b   Checkout our..[
+00000ef0: 7265 6c65 6173 6520 6e6f 7465 735d 2868  release notes](h
+00000f00: 7474 7073 3a2f 2f73 6b62 6173 652e 7265  ttps://skbase.re
+00000f10: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000f20: 6c61 7465 7374 2f63 6861 6e67 656c 6f67  latest/changelog
+00000f30: 2e68 746d 6c29 2e0d 0a0d 0a7c 204f 7665  .html).....| Ove
+00000f40: 7276 6965 7720 7c20 7c0d 0a7c 2d2d 2d7c  rview | |..|---|
+00000f50: 2d2d 2d7c 0d0a 7c20 2a2a 4349 2f43 442a  ---|..| **CI/CD*
+00000f60: 2a20 7c20 5b21 5b54 6573 7473 5d28 6874  * | [![Tests](ht
+00000f70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000f80: 2f73 6b74 696d 652f 736b 6261 7365 2f61  /sktime/skbase/a
+00000f90: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000fa0: 2f74 6573 742e 796d 6c2f 6261 6467 652e  /test.yml/badge.
+00000fb0: 7376 673f 6272 616e 6368 3d6d 6169 6e29  svg?branch=main)
+00000fc0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000fd0: 2e63 6f6d 2f73 6b74 696d 652f 736b 6261  .com/sktime/skba
+00000fe0: 7365 2f61 6374 696f 6e73 2f77 6f72 6b66  se/actions/workf
+00000ff0: 6c6f 7773 2f74 6573 742e 796d 6c29 205b  lows/test.yml) [
+00001000: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
+00001010: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00001020: 2f73 6b74 696d 652f 736b 6261 7365 2f62  /sktime/skbase/b
+00001030: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
+00001040: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+00001050: 3d32 4a34 3234 4e4c 4f38 3229 5d28 6874  =2J424NLO82)](ht
+00001060: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00001070: 2f67 682f 736b 7469 6d65 2f73 6b62 6173  /gh/sktime/skbas
+00001080: 6529 205b 215b 446f 6375 6d65 6e74 6174  e) [![Documentat
+00001090: 696f 6e20 5374 6174 7573 5d28 6874 7470  ion Status](http
+000010a0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
+000010b0: 6f72 672f 7072 6f6a 6563 7473 2f73 6b62  org/projects/skb
+000010c0: 6173 652f 6261 6467 652f 3f76 6572 7369  ase/badge/?versi
+000010d0: 6f6e 3d6c 6174 6573 7429 5d28 6874 7470  on=latest)](http
+000010e0: 733a 2f2f 736b 6261 7365 2e72 6561 6474  s://skbase.readt
+000010f0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001100: 6573 742f 3f62 6164 6765 3d6c 6174 6573  est/?badge=lates
+00001110: 7429 205b 215b 7072 652d 636f 6d6d 6974  t) [![pre-commit
+00001120: 2e63 6920 7374 6174 7573 5d28 6874 7470  .ci status](http
+00001130: 733a 2f2f 7265 7375 6c74 732e 7072 652d  s://results.pre-
+00001140: 636f 6d6d 6974 2e63 692f 6261 6467 652f  commit.ci/badge/
+00001150: 6769 7468 7562 2f73 6b74 696d 652f 736b  github/sktime/sk
+00001160: 6261 7365 2f6d 6169 6e2e 7376 6729 5d28  base/main.svg)](
+00001170: 6874 7470 733a 2f2f 7265 7375 6c74 732e  https://results.
+00001180: 7072 652d 636f 6d6d 6974 2e63 692f 6c61  pre-commit.ci/la
+00001190: 7465 7374 2f67 6974 6875 622f 736b 7469  test/github/skti
+000011a0: 6d65 2f73 6b62 6173 652f 6d61 696e 2920  me/skbase/main) 
+000011b0: 7c0d 0a7c 202a 2a43 6f64 652a 2a20 7c20  |..| **Code** | 
+000011c0: 205b 215b 2170 7970 695d 2868 7474 7073   [![!pypi](https
+000011d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000011e0: 6f2f 7079 7069 2f76 2f73 6369 6b69 742d  o/pypi/v/scikit-
+000011f0: 6261 7365 3f63 6f6c 6f72 3d6f 7261 6e67  base?color=orang
+00001200: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
+00001210: 2e6f 7267 2f70 726f 6a65 6374 2f73 6b62  .org/project/skb
+00001220: 6173 652f 2920 205b 215b 2170 7974 686f  ase/)  [![!pytho
+00001230: 6e2d 7665 7273 696f 6e73 5d28 6874 7470  n-versions](http
+00001240: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00001250: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
+00001260: 6e73 2f73 6369 6b69 742d 6261 7365 295d  ns/scikit-base)]
+00001270: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
+00001280: 686f 6e2e 6f72 672f 2920 5b21 5b21 626c  hon.org/) [![!bl
+00001290: 6163 6b5d 2868 7474 7073 3a2f 2f69 6d67  ack](https://img
+000012a0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000012b0: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
+000012c0: 6c61 636b 2d30 3030 3030 302e 7376 6729  lack-000000.svg)
+000012d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000012e0: 2e63 6f6d 2f70 7366 2f62 6c61 636b 2920  .com/psf/black) 
+000012f0: 5b21 5b73 6563 7572 6974 793a 2062 616e  [![security: ban
+00001300: 6469 745d 2868 7474 7073 3a2f 2f69 6d67  dit](https://img
+00001310: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00001320: 652f 7365 6375 7269 7479 2d62 616e 6469  e/security-bandi
+00001330: 742d 7965 6c6c 6f77 2e73 7667 295d 2868  t-yellow.svg)](h
+00001340: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001350: 6d2f 5079 4351 412f 6261 6e64 6974 2920  m/PyCQA/bandit) 
+00001360: 7c0d 0a7c 202a 2a44 6f77 6e6c 6f61 6473  |..| **Downloads
+00001370: 2a2a 7c20 5b21 5b44 6f77 6e6c 6f61 6473  **| [![Downloads
+00001380: 5d28 6874 7470 733a 2f2f 7374 6174 6963  ](https://static
+00001390: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
+000013a0: 6e61 6c69 7a65 642d 6261 6467 652f 7363  nalized-badge/sc
+000013b0: 696b 6974 2d62 6173 653f 7065 7269 6f64  ikit-base?period
+000013c0: 3d77 6565 6b26 756e 6974 733d 696e 7465  =week&units=inte
+000013d0: 726e 6174 696f 6e61 6c5f 7379 7374 656d  rnational_system
+000013e0: 266c 6566 745f 636f 6c6f 723d 6772 6579  &left_color=grey
+000013f0: 2672 6967 6874 5f63 6f6c 6f72 3d62 6c75  &right_color=blu
+00001400: 6526 6c65 6674 5f74 6578 743d 7765 656b  e&left_text=week
+00001410: 6c79 2532 3028 7079 7069 2929 5d28 6874  ly%20(pypi))](ht
+00001420: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
+00001430: 7072 6f6a 6563 742f 7363 696b 6974 2d62  project/scikit-b
+00001440: 6173 6529 205b 215b 446f 776e 6c6f 6164  ase) [![Download
+00001450: 735d 2868 7474 7073 3a2f 2f73 7461 7469  s](https://stati
+00001460: 632e 7065 7079 2e74 6563 682f 7065 7273  c.pepy.tech/pers
+00001470: 6f6e 616c 697a 6564 2d62 6164 6765 2f73  onalized-badge/s
+00001480: 6369 6b69 742d 6261 7365 3f70 6572 696f  cikit-base?perio
+00001490: 643d 6d6f 6e74 6826 756e 6974 733d 696e  d=month&units=in
+000014a0: 7465 726e 6174 696f 6e61 6c5f 7379 7374  ternational_syst
+000014b0: 656d 266c 6566 745f 636f 6c6f 723d 6772  em&left_color=gr
+000014c0: 6579 2672 6967 6874 5f63 6f6c 6f72 3d62  ey&right_color=b
+000014d0: 6c75 6526 6c65 6674 5f74 6578 743d 6d6f  lue&left_text=mo
+000014e0: 6e74 686c 7925 3230 2870 7970 6929 295d  nthly%20(pypi))]
+000014f0: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
+00001500: 6368 2f70 726f 6a65 6374 2f73 6369 6b69  ch/project/sciki
+00001510: 742d 6261 7365 2920 5b21 5b44 6f77 6e6c  t-base) [![Downl
+00001520: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
+00001530: 6174 6963 2e70 6570 792e 7465 6368 2f70  atic.pepy.tech/p
+00001540: 6572 736f 6e61 6c69 7a65 642d 6261 6467  ersonalized-badg
+00001550: 652f 7363 696b 6974 2d62 6173 653f 7065  e/scikit-base?pe
+00001560: 7269 6f64 3d74 6f74 616c 2675 6e69 7473  riod=total&units
+00001570: 3d69 6e74 6572 6e61 7469 6f6e 616c 5f73  =international_s
+00001580: 7973 7465 6d26 6c65 6674 5f63 6f6c 6f72  ystem&left_color
+00001590: 3d67 7265 7926 7269 6768 745f 636f 6c6f  =grey&right_colo
+000015a0: 723d 626c 7565 266c 6566 745f 7465 7874  r=blue&left_text
+000015b0: 3d63 756d 756c 6174 6976 6525 3230 2870  =cumulative%20(p
+000015c0: 7970 6929 295d 2868 7474 7073 3a2f 2f70  ypi))](https://p
+000015d0: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+000015e0: 2f73 6369 6b69 742d 6261 7365 2920 7c0d  /scikit-base) |.
+000015f0: 0a0d 0a3c 212d 2d20 414c 4c2d 434f 4e54  ...<!-- ALL-CONT
+00001600: 5249 4255 544f 5253 2d42 4144 4745 3a53  RIBUTORS-BADGE:S
+00001610: 5441 5254 202d 2044 6f20 6e6f 7420 7265  TART - Do not re
+00001620: 6d6f 7665 206f 7220 6d6f 6469 6679 2074  move or modify t
+00001630: 6869 7320 7365 6374 696f 6e20 2d2d 3e0d  his section -->.
+00001640: 0a5b 215b 416c 6c20 436f 6e74 7269 6275  .[![All Contribu
+00001650: 746f 7273 5d28 6874 7470 733a 2f2f 696d  tors](https://im
+00001660: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00001670: 6765 2f61 6c6c 5f63 6f6e 7472 6962 7574  ge/all_contribut
+00001680: 6f72 732d 3133 2d6f 7261 6e67 652e 7376  ors-13-orange.sv
+00001690: 673f 7374 796c 653d 666c 6174 2d73 7175  g?style=flat-squ
+000016a0: 6172 6529 5d28 2363 6f6e 7472 6962 7574  are)](#contribut
+000016b0: 6f72 7329 0d0a 3c21 2d2d 2041 4c4c 2d43  ors)..<!-- ALL-C
+000016c0: 4f4e 5452 4942 5554 4f52 532d 4241 4447  ONTRIBUTORS-BADG
+000016d0: 453a 454e 4420 2d2d 3e0d 0a0d 0a23 2320  E:END -->....## 
+000016e0: 446f 6375 6d65 6e74 6174 696f 6e0d 0a0d  Documentation...
+000016f0: 0a54 6f20 6c65 6172 6e20 6d6f 7265 2061  .To learn more a
+00001700: 626f 7574 2074 6865 2070 6163 6b61 6765  bout the package
+00001710: 2063 6865 636b 6f75 7420 6f75 7220 5b64   checkout our [d
+00001720: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00001730: 7470 733a 2f2f 736b 6261 7365 2e72 6561  tps://skbase.rea
+00001740: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00001750: 6174 6573 742f 292e 0d0a 0d0a 2323 203a  atest/).....## :
+00001760: 686f 7572 676c 6173 735f 666c 6f77 696e  hourglass_flowin
+00001770: 675f 7361 6e64 3a20 496e 7374 616c 6c20  g_sand: Install 
+00001780: 736b 6261 7365 0d0a 466f 7220 7472 6f75  skbase..For trou
+00001790: 626c 6520 7368 6f6f 7469 6e67 206f 7220  ble shooting or 
+000017a0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+000017b0: 2c20 7365 6520 6f75 720d 0a5b 6465 7461  , see our..[deta
+000017c0: 696c 6564 2069 6e73 7461 6c6c 6174 696f  iled installatio
+000017d0: 6e20 696e 7374 7275 6374 696f 6e73 5d28  n instructions](
+000017e0: 6874 7470 733a 2f2f 736b 6261 7365 2e72  https://skbase.r
+000017f0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00001800: 2f6c 6174 6573 742f 7573 6572 5f64 6f63  /latest/user_doc
+00001810: 756d 656e 7461 7469 6f6e 2f69 6e73 7461  umentation/insta
+00001820: 6c6c 6174 696f 6e2e 6874 6d6c 292e 0d0a  llation.html)...
+00001830: 0d0a 2d20 2a2a 4f70 6572 6174 696e 6720  ..- **Operating 
+00001840: 7379 7374 656d 2a2a 3a20 6d61 634f 5320  system**: macOS 
+00001850: 5820 c2b7 204c 696e 7578 20c2 b720 5769  X .. Linux .. Wi
+00001860: 6e64 6f77 7320 382e 3120 6f72 2068 6967  ndows 8.1 or hig
+00001870: 6865 720d 0a2d 202a 2a50 7974 686f 6e20  her..- **Python 
+00001880: 7665 7273 696f 6e2a 2a3a 2050 7974 686f  version**: Pytho
+00001890: 6e20 332e 372c 2033 2e38 2c20 332e 392c  n 3.7, 3.8, 3.9,
+000018a0: 2033 2e31 3020 616e 6420 332e 3131 0d0a   3.10 and 3.11..
+000018b0: 2d20 2a2a 5061 636b 6167 6520 6d61 6e61  - **Package mana
+000018c0: 6765 7273 2a2a 3a20 5b70 6970 5d0d 0a0d  gers**: [pip]...
+000018d0: 0a5b 7069 705d 3a20 6874 7470 733a 2f2f  .[pip]: https://
+000018e0: 7069 702e 7079 7061 2e69 6f2f 656e 2f73  pip.pypa.io/en/s
+000018f0: 7461 626c 652f 0d0a 0d0a 2323 2320 7069  table/....### pi
+00001900: 700d 0a73 6b62 6173 6520 7265 6c65 6173  p..skbase releas
+00001910: 6573 2061 7265 2061 7661 696c 6162 6c65  es are available
+00001920: 2061 7320 736f 7572 6365 2070 6163 6b61   as source packa
+00001930: 6765 7320 616e 6420 6269 6e61 7279 2077  ges and binary w
+00001940: 6865 656c 7320 7669 6120 5079 5049 0d0a  heels via PyPI..
+00001950: 616e 6420 6361 6e20 6265 2069 6e73 7461  and can be insta
+00001960: 6c6c 6564 2075 7369 6e67 2070 6970 2e20  lled using pip. 
+00001970: 4368 6563 6b6f 7574 2074 6865 2066 756c  Checkout the ful
+00001980: 6c20 6c69 7374 206f 6620 7072 652d 636f  l list of pre-co
+00001990: 6d70 696c 6564 205b 7768 6565 6c73 206f  mpiled [wheels o
+000019a0: 6e20 5079 5069 5d28 6874 7470 733a 2f2f  n PyPi](https://
+000019b0: 7079 7069 2e6f 7267 2f73 696d 706c 652f  pypi.org/simple/
+000019c0: 736b 6261 7365 2f29 2e0d 0a0d 0a54 6f20  skbase/).....To 
+000019d0: 696e 7374 616c 6c20 7468 6520 636f 7265  install the core
+000019e0: 2070 6163 6b61 6765 2075 7365 3a0d 0a0d   package use:...
+000019f0: 0a60 6060 6261 7368 0d0a 7069 7020 696e  .```bash..pip in
+00001a00: 7374 616c 6c20 7363 696b 6974 2d62 6173  stall scikit-bas
+00001a10: 650d 0a60 6060 0d0a 0d0a 6f72 2c20 6966  e..```....or, if
+00001a20: 2079 6f75 2077 616e 7420 746f 2069 6e73   you want to ins
+00001a30: 7461 6c6c 2077 6974 6820 7468 6520 6d61  tall with the ma
+00001a40: 7869 6d75 6d20 7365 7420 6f66 2064 6570  ximum set of dep
+00001a50: 656e 6465 6e63 6965 732c 2075 7365 3a0d  endencies, use:.
+00001a60: 0a0d 0a60 6060 6261 7368 0d0a 7069 7020  ...```bash..pip 
+00001a70: 696e 7374 616c 6c20 7363 696b 6974 2d62  install scikit-b
+00001a80: 6173 655b 616c 6c5f 6578 7472 6173 5d0d  ase[all_extras].
+00001a90: 0a60 6060 0d0a                           .```..
```

### Comparing `skbase-0.4.5/README.md` & `skbase-0.4.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,205 +1,220 @@
-00000000: 0a23 2057 656c 636f 6d65 2074 6f20 736b  .# Welcome to sk
-00000010: 6261 7365 0a0a 3e20 4120 6261 7365 2063  base..> A base c
-00000020: 6c61 7373 2066 6f72 2073 6369 6b69 742d  lass for scikit-
-00000030: 6c65 6172 6e2d 6c69 6b65 2061 6e64 2073  learn-like and s
-00000040: 6b74 696d 652d 6c69 6b65 2070 6172 616d  ktime-like param
-00000050: 6574 7269 6320 6f62 6a65 6374 730a 0a60  etric objects..`
-00000060: 736b 6261 7365 6020 7072 6f76 6964 6573  skbase` provides
-00000070: 2062 6173 6520 636c 6173 7365 7320 666f   base classes fo
-00000080: 7220 6372 6561 7469 6e67 2073 6369 6b69  r creating sciki
-00000090: 742d 6c65 6172 6e2d 6c69 6b65 2070 6172  t-learn-like par
-000000a0: 616d 6574 7269 6320 6f62 6a65 6374 732c  ametric objects,
-000000b0: 0a61 6c6f 6e67 2077 6974 6820 746f 6f6c  .along with tool
-000000c0: 7320 746f 206d 616b 6520 6974 2065 6173  s to make it eas
-000000d0: 6965 7220 746f 2062 7569 6c64 2079 6f75  ier to build you
-000000e0: 7220 6f77 6e20 7061 636b 6167 6573 2074  r own packages t
-000000f0: 6861 7420 666f 6c6c 6f77 2074 6865 7365  hat follow these
-00000100: 0a64 6573 6967 6e20 7061 7474 6572 6e73  .design patterns
-00000110: 2e0a 0a3a 726f 636b 6574 3a20 5665 7273  ...:rocket: Vers
-00000120: 696f 6e20 302e 342e 3520 6973 206e 6f77  ion 0.4.5 is now
-00000130: 2061 7661 696c 6162 6c65 2e20 4368 6563   available. Chec
-00000140: 6b6f 7574 206f 7572 0a5b 7265 6c65 6173  kout our.[releas
-00000150: 6520 6e6f 7465 735d 2868 7474 7073 3a2f  e notes](https:/
-00000160: 2f73 6b62 6173 652e 7265 6164 7468 6564  /skbase.readthed
-00000170: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
-00000180: 2f63 6861 6e67 656c 6f67 2e68 746d 6c29  /changelog.html)
-00000190: 2e0a 0a7c 204f 7665 7276 6965 7720 7c20  ...| Overview | 
-000001a0: 7c0a 7c2d 2d2d 7c2d 2d2d 7c0a 7c20 2a2a  |.|---|---|.| **
-000001b0: 4349 2f43 442a 2a20 7c20 5b21 5b54 6573  CI/CD** | [![Tes
-000001c0: 7473 5d28 6874 7470 733a 2f2f 6769 7468  ts](https://gith
-000001d0: 7562 2e63 6f6d 2f73 6b74 696d 652f 736b  ub.com/sktime/sk
-000001e0: 6261 7365 2f61 6374 696f 6e73 2f77 6f72  base/actions/wor
-000001f0: 6b66 6c6f 7773 2f74 6573 742e 796d 6c2f  kflows/test.yml/
-00000200: 6261 6467 652e 7376 673f 6272 616e 6368  badge.svg?branch
-00000210: 3d6d 6169 6e29 5d28 6874 7470 733a 2f2f  =main)](https://
-00000220: 6769 7468 7562 2e63 6f6d 2f73 6b74 696d  github.com/sktim
-00000230: 652f 736b 6261 7365 2f61 6374 696f 6e73  e/skbase/actions
-00000240: 2f77 6f72 6b66 6c6f 7773 2f74 6573 742e  /workflows/test.
-00000250: 796d 6c29 205b 215b 636f 6465 636f 765d  yml) [![codecov]
-00000260: 2868 7474 7073 3a2f 2f63 6f64 6563 6f76  (https://codecov
-00000270: 2e69 6f2f 6768 2f73 6b74 696d 652f 736b  .io/gh/sktime/sk
-00000280: 6261 7365 2f62 7261 6e63 682f 6d61 696e  base/branch/main
-00000290: 2f67 7261 7068 2f62 6164 6765 2e73 7667  /graph/badge.svg
-000002a0: 3f74 6f6b 656e 3d32 4a34 3234 4e4c 4f38  ?token=2J424NLO8
-000002b0: 3229 5d28 6874 7470 733a 2f2f 636f 6465  2)](https://code
-000002c0: 636f 762e 696f 2f67 682f 736b 7469 6d65  cov.io/gh/sktime
-000002d0: 2f73 6b62 6173 6529 205b 215b 446f 6375  /skbase) [![Docu
-000002e0: 6d65 6e74 6174 696f 6e20 5374 6174 7573  mentation Status
-000002f0: 5d28 6874 7470 733a 2f2f 7265 6164 7468  ](https://readth
-00000300: 6564 6f63 732e 6f72 672f 7072 6f6a 6563  edocs.org/projec
-00000310: 7473 2f73 6b62 6173 652f 6261 6467 652f  ts/skbase/badge/
-00000320: 3f76 6572 7369 6f6e 3d6c 6174 6573 7429  ?version=latest)
-00000330: 5d28 6874 7470 733a 2f2f 736b 6261 7365  ](https://skbase
-00000340: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
-00000350: 656e 2f6c 6174 6573 742f 3f62 6164 6765  en/latest/?badge
-00000360: 3d6c 6174 6573 7429 205b 215b 7072 652d  =latest) [![pre-
-00000370: 636f 6d6d 6974 2e63 6920 7374 6174 7573  commit.ci status
-00000380: 5d28 6874 7470 733a 2f2f 7265 7375 6c74  ](https://result
-00000390: 732e 7072 652d 636f 6d6d 6974 2e63 692f  s.pre-commit.ci/
-000003a0: 6261 6467 652f 6769 7468 7562 2f73 6b74  badge/github/skt
-000003b0: 696d 652f 736b 6261 7365 2f6d 6169 6e2e  ime/skbase/main.
-000003c0: 7376 6729 5d28 6874 7470 733a 2f2f 7265  svg)](https://re
-000003d0: 7375 6c74 732e 7072 652d 636f 6d6d 6974  sults.pre-commit
-000003e0: 2e63 692f 6c61 7465 7374 2f67 6974 6875  .ci/latest/githu
-000003f0: 622f 736b 7469 6d65 2f73 6b62 6173 652f  b/sktime/skbase/
-00000400: 6d61 696e 2920 7c0a 7c20 2a2a 436f 6465  main) |.| **Code
-00000410: 2a2a 207c 2020 5b21 5b21 7079 7069 5d28  ** |  [![!pypi](
-00000420: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000430: 6c64 732e 696f 2f70 7970 692f 762f 7363  lds.io/pypi/v/sc
-00000440: 696b 6974 2d62 6173 653f 636f 6c6f 723d  ikit-base?color=
-00000450: 6f72 616e 6765 295d 2868 7474 7073 3a2f  orange)](https:/
-00000460: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000470: 742f 736b 6261 7365 2f29 2020 5b21 5b21  t/skbase/)  [![!
-00000480: 7079 7468 6f6e 2d76 6572 7369 6f6e 735d  python-versions]
-00000490: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000004a0: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
-000004b0: 6572 7369 6f6e 732f 7363 696b 6974 2d62  ersions/scikit-b
-000004c0: 6173 6529 5d28 6874 7470 733a 2f2f 7777  ase)](https://ww
-000004d0: 772e 7079 7468 6f6e 2e6f 7267 2f29 205b  w.python.org/) [
-000004e0: 215b 2162 6c61 636b 5d28 6874 7470 733a  ![!black](https:
-000004f0: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000500: 2f62 6164 6765 2f63 6f64 6525 3230 7374  /badge/code%20st
-00000510: 796c 652d 626c 6163 6b2d 3030 3030 3030  yle-black-000000
-00000520: 2e73 7667 295d 2868 7474 7073 3a2f 2f67  .svg)](https://g
-00000530: 6974 6875 622e 636f 6d2f 7073 662f 626c  ithub.com/psf/bl
-00000540: 6163 6b29 205b 215b 7365 6375 7269 7479  ack) [![security
-00000550: 3a20 6261 6e64 6974 5d28 6874 7470 733a  : bandit](https:
-00000560: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000570: 2f62 6164 6765 2f73 6563 7572 6974 792d  /badge/security-
-00000580: 6261 6e64 6974 2d79 656c 6c6f 772e 7376  bandit-yellow.sv
-00000590: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
-000005a0: 7562 2e63 6f6d 2f50 7943 5141 2f62 616e  ub.com/PyCQA/ban
-000005b0: 6469 7429 207c 0a7c 202a 2a44 6f77 6e6c  dit) |.| **Downl
-000005c0: 6f61 6473 2a2a 7c20 5b21 5b44 6f77 6e6c  oads**| [![Downl
-000005d0: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
-000005e0: 6174 6963 2e70 6570 792e 7465 6368 2f70  atic.pepy.tech/p
-000005f0: 6572 736f 6e61 6c69 7a65 642d 6261 6467  ersonalized-badg
-00000600: 652f 7363 696b 6974 2d62 6173 653f 7065  e/scikit-base?pe
-00000610: 7269 6f64 3d77 6565 6b26 756e 6974 733d  riod=week&units=
-00000620: 696e 7465 726e 6174 696f 6e61 6c5f 7379  international_sy
-00000630: 7374 656d 266c 6566 745f 636f 6c6f 723d  stem&left_color=
-00000640: 6772 6579 2672 6967 6874 5f63 6f6c 6f72  grey&right_color
-00000650: 3d62 6c75 6526 6c65 6674 5f74 6578 743d  =blue&left_text=
-00000660: 7765 656b 6c79 2532 3028 7079 7069 2929  weekly%20(pypi))
-00000670: 5d28 6874 7470 733a 2f2f 7065 7079 2e74  ](https://pepy.t
-00000680: 6563 682f 7072 6f6a 6563 742f 7363 696b  ech/project/scik
-00000690: 6974 2d62 6173 6529 205b 215b 446f 776e  it-base) [![Down
-000006a0: 6c6f 6164 735d 2868 7474 7073 3a2f 2f73  loads](https://s
-000006b0: 7461 7469 632e 7065 7079 2e74 6563 682f  tatic.pepy.tech/
-000006c0: 7065 7273 6f6e 616c 697a 6564 2d62 6164  personalized-bad
-000006d0: 6765 2f73 6369 6b69 742d 6261 7365 3f70  ge/scikit-base?p
-000006e0: 6572 696f 643d 6d6f 6e74 6826 756e 6974  eriod=month&unit
-000006f0: 733d 696e 7465 726e 6174 696f 6e61 6c5f  s=international_
-00000700: 7379 7374 656d 266c 6566 745f 636f 6c6f  system&left_colo
-00000710: 723d 6772 6579 2672 6967 6874 5f63 6f6c  r=grey&right_col
-00000720: 6f72 3d62 6c75 6526 6c65 6674 5f74 6578  or=blue&left_tex
-00000730: 743d 6d6f 6e74 686c 7925 3230 2870 7970  t=monthly%20(pyp
-00000740: 6929 295d 2868 7474 7073 3a2f 2f70 6570  i))](https://pep
-00000750: 792e 7465 6368 2f70 726f 6a65 6374 2f73  y.tech/project/s
-00000760: 6369 6b69 742d 6261 7365 2920 5b21 5b44  cikit-base) [![D
-00000770: 6f77 6e6c 6f61 6473 5d28 6874 7470 733a  ownloads](https:
-00000780: 2f2f 7374 6174 6963 2e70 6570 792e 7465  //static.pepy.te
-00000790: 6368 2f70 6572 736f 6e61 6c69 7a65 642d  ch/personalized-
-000007a0: 6261 6467 652f 7363 696b 6974 2d62 6173  badge/scikit-bas
-000007b0: 653f 7065 7269 6f64 3d74 6f74 616c 2675  e?period=total&u
-000007c0: 6e69 7473 3d69 6e74 6572 6e61 7469 6f6e  nits=internation
-000007d0: 616c 5f73 7973 7465 6d26 6c65 6674 5f63  al_system&left_c
-000007e0: 6f6c 6f72 3d67 7265 7926 7269 6768 745f  olor=grey&right_
-000007f0: 636f 6c6f 723d 626c 7565 266c 6566 745f  color=blue&left_
-00000800: 7465 7874 3d63 756d 756c 6174 6976 6525  text=cumulative%
-00000810: 3230 2870 7970 6929 295d 2868 7474 7073  20(pypi))](https
-00000820: 3a2f 2f70 6570 792e 7465 6368 2f70 726f  ://pepy.tech/pro
-00000830: 6a65 6374 2f73 6369 6b69 742d 6261 7365  ject/scikit-base
-00000840: 2920 7c0a 0a3c 212d 2d20 414c 4c2d 434f  ) |..<!-- ALL-CO
-00000850: 4e54 5249 4255 544f 5253 2d42 4144 4745  NTRIBUTORS-BADGE
-00000860: 3a53 5441 5254 202d 2044 6f20 6e6f 7420  :START - Do not 
-00000870: 7265 6d6f 7665 206f 7220 6d6f 6469 6679  remove or modify
-00000880: 2074 6869 7320 7365 6374 696f 6e20 2d2d   this section --
-00000890: 3e0a 5b21 5b41 6c6c 2043 6f6e 7472 6962  >.[![All Contrib
-000008a0: 7574 6f72 735d 2868 7474 7073 3a2f 2f69  utors](https://i
-000008b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-000008c0: 6467 652f 616c 6c5f 636f 6e74 7269 6275  dge/all_contribu
-000008d0: 746f 7273 2d31 332d 6f72 616e 6765 2e73  tors-13-orange.s
-000008e0: 7667 3f73 7479 6c65 3d66 6c61 742d 7371  vg?style=flat-sq
-000008f0: 7561 7265 295d 2823 636f 6e74 7269 6275  uare)](#contribu
-00000900: 746f 7273 290a 3c21 2d2d 2041 4c4c 2d43  tors).<!-- ALL-C
-00000910: 4f4e 5452 4942 5554 4f52 532d 4241 4447  ONTRIBUTORS-BADG
-00000920: 453a 454e 4420 2d2d 3e0a 0a23 2320 446f  E:END -->..## Do
-00000930: 6375 6d65 6e74 6174 696f 6e0a 0a54 6f20  cumentation..To 
-00000940: 6c65 6172 6e20 6d6f 7265 2061 626f 7574  learn more about
-00000950: 2074 6865 2070 6163 6b61 6765 2063 6865   the package che
-00000960: 636b 6f75 7420 6f75 7220 5b64 6f63 756d  ckout our [docum
-00000970: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
-00000980: 2f2f 736b 6261 7365 2e72 6561 6474 6865  //skbase.readthe
-00000990: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
-000009a0: 742f 292e 0a0a 2323 203a 686f 7572 676c  t/)...## :hourgl
-000009b0: 6173 735f 666c 6f77 696e 675f 7361 6e64  ass_flowing_sand
-000009c0: 3a20 496e 7374 616c 6c20 736b 6261 7365  : Install skbase
-000009d0: 0a46 6f72 2074 726f 7562 6c65 2073 686f  .For trouble sho
-000009e0: 6f74 696e 6720 6f72 206d 6f72 6520 696e  oting or more in
-000009f0: 666f 726d 6174 696f 6e2c 2073 6565 206f  formation, see o
-00000a00: 7572 0a5b 6465 7461 696c 6564 2069 6e73  ur.[detailed ins
-00000a10: 7461 6c6c 6174 696f 6e20 696e 7374 7275  tallation instru
-00000a20: 6374 696f 6e73 5d28 6874 7470 733a 2f2f  ctions](https://
-00000a30: 736b 6261 7365 2e72 6561 6474 6865 646f  skbase.readthedo
-00000a40: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00000a50: 7573 6572 5f64 6f63 756d 656e 7461 7469  user_documentati
-00000a60: 6f6e 2f69 6e73 7461 6c6c 6174 696f 6e2e  on/installation.
-00000a70: 6874 6d6c 292e 0a0a 2d20 2a2a 4f70 6572  html)...- **Oper
-00000a80: 6174 696e 6720 7379 7374 656d 2a2a 3a20  ating system**: 
-00000a90: 6d61 634f 5320 5820 c2b7 204c 696e 7578  macOS X .. Linux
-00000aa0: 20c2 b720 5769 6e64 6f77 7320 382e 3120   .. Windows 8.1 
-00000ab0: 6f72 2068 6967 6865 720a 2d20 2a2a 5079  or higher.- **Py
-00000ac0: 7468 6f6e 2076 6572 7369 6f6e 2a2a 3a20  thon version**: 
-00000ad0: 5079 7468 6f6e 2033 2e37 2c20 332e 382c  Python 3.7, 3.8,
-00000ae0: 2033 2e39 2c20 332e 3130 2061 6e64 2033   3.9, 3.10 and 3
-00000af0: 2e31 310a 2d20 2a2a 5061 636b 6167 6520  .11.- **Package 
-00000b00: 6d61 6e61 6765 7273 2a2a 3a20 5b70 6970  managers**: [pip
-00000b10: 5d0a 0a5b 7069 705d 3a20 6874 7470 733a  ]..[pip]: https:
-00000b20: 2f2f 7069 702e 7079 7061 2e69 6f2f 656e  //pip.pypa.io/en
-00000b30: 2f73 7461 626c 652f 0a0a 2323 2320 7069  /stable/..### pi
-00000b40: 700a 736b 6261 7365 2072 656c 6561 7365  p.skbase release
-00000b50: 7320 6172 6520 6176 6169 6c61 626c 6520  s are available 
-00000b60: 6173 2073 6f75 7263 6520 7061 636b 6167  as source packag
-00000b70: 6573 2061 6e64 2062 696e 6172 7920 7768  es and binary wh
-00000b80: 6565 6c73 2076 6961 2050 7950 490a 616e  eels via PyPI.an
-00000b90: 6420 6361 6e20 6265 2069 6e73 7461 6c6c  d can be install
-00000ba0: 6564 2075 7369 6e67 2070 6970 2e20 4368  ed using pip. Ch
-00000bb0: 6563 6b6f 7574 2074 6865 2066 756c 6c20  eckout the full 
-00000bc0: 6c69 7374 206f 6620 7072 652d 636f 6d70  list of pre-comp
-00000bd0: 696c 6564 205b 7768 6565 6c73 206f 6e20  iled [wheels on 
-00000be0: 5079 5069 5d28 6874 7470 733a 2f2f 7079  PyPi](https://py
-00000bf0: 7069 2e6f 7267 2f73 696d 706c 652f 736b  pi.org/simple/sk
-00000c00: 6261 7365 2f29 2e0a 0a54 6f20 696e 7374  base/)...To inst
-00000c10: 616c 6c20 7468 6520 636f 7265 2070 6163  all the core pac
-00000c20: 6b61 6765 2075 7365 3a0a 0a60 6060 6261  kage use:..```ba
-00000c30: 7368 0a70 6970 2069 6e73 7461 6c6c 2073  sh.pip install s
-00000c40: 6369 6b69 742d 6261 7365 0a60 6060 0a0a  cikit-base.```..
-00000c50: 6f72 2c20 6966 2079 6f75 2077 616e 7420  or, if you want 
-00000c60: 746f 2069 6e73 7461 6c6c 2077 6974 6820  to install with 
-00000c70: 7468 6520 6d61 7869 6d75 6d20 7365 7420  the maximum set 
-00000c80: 6f66 2064 6570 656e 6465 6e63 6965 732c  of dependencies,
-00000c90: 2075 7365 3a0a 0a60 6060 6261 7368 0a70   use:..```bash.p
-00000ca0: 6970 2069 6e73 7461 6c6c 2073 6369 6b69  ip install sciki
-00000cb0: 742d 6261 7365 5b61 6c6c 5f65 7874 7261  t-base[all_extra
-00000cc0: 735d 0a60 6060 0a                        s].```.
+00000000: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00000010: 2f73 6b62 6173 652e 7265 6164 7468 6564  /skbase.readthed
+00000020: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00000030: 2f22 3e3c 696d 6720 7372 633d 2268 7474  /"><img src="htt
+00000040: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000050: 736b 7469 6d65 2f73 6b62 6173 652f 626c  sktime/skbase/bl
+00000060: 6f62 2f6d 6169 6e2f 646f 6373 2f73 6f75  ob/main/docs/sou
+00000070: 7263 652f 696d 6167 6573 2f73 6b62 6173  rce/images/skbas
+00000080: 652d 6c6f 676f 2d77 6974 682d 6e61 6d65  e-logo-with-name
+00000090: 2e70 6e67 2220 7769 6474 683d 2231 3735  .png" width="175
+000000a0: 2220 616c 6967 6e3d 2272 6967 6874 2220  " align="right" 
+000000b0: 2f3e 3c2f 613e 0d0a 0d0a 2320 5765 6c63  /></a>....# Welc
+000000c0: 6f6d 6520 746f 2073 6b62 6173 650d 0a0d  ome to skbase...
+000000d0: 0a3e 2041 2062 6173 6520 636c 6173 7320  .> A base class 
+000000e0: 666f 7220 7363 696b 6974 2d6c 6561 726e  for scikit-learn
+000000f0: 2d6c 696b 6520 616e 6420 736b 7469 6d65  -like and sktime
+00000100: 2d6c 696b 6520 7061 7261 6d65 7472 6963  -like parametric
+00000110: 206f 626a 6563 7473 0d0a 0d0a 6073 6b62   objects....`skb
+00000120: 6173 6560 2070 726f 7669 6465 7320 6261  ase` provides ba
+00000130: 7365 2063 6c61 7373 6573 2066 6f72 2063  se classes for c
+00000140: 7265 6174 696e 6720 7363 696b 6974 2d6c  reating scikit-l
+00000150: 6561 726e 2d6c 696b 6520 7061 7261 6d65  earn-like parame
+00000160: 7472 6963 206f 626a 6563 7473 2c0d 0a61  tric objects,..a
+00000170: 6c6f 6e67 2077 6974 6820 746f 6f6c 7320  long with tools 
+00000180: 746f 206d 616b 6520 6974 2065 6173 6965  to make it easie
+00000190: 7220 746f 2062 7569 6c64 2079 6f75 7220  r to build your 
+000001a0: 6f77 6e20 7061 636b 6167 6573 2074 6861  own packages tha
+000001b0: 7420 666f 6c6c 6f77 2074 6865 7365 0d0a  t follow these..
+000001c0: 6465 7369 676e 2070 6174 7465 726e 732e  design patterns.
+000001d0: 0d0a 0d0a 3a72 6f63 6b65 743a 2056 6572  ....:rocket: Ver
+000001e0: 7369 6f6e 2030 2e34 2e36 2069 7320 6e6f  sion 0.4.6 is no
+000001f0: 7720 6176 6169 6c61 626c 652e 2043 6865  w available. Che
+00000200: 636b 6f75 7420 6f75 720d 0a5b 7265 6c65  ckout our..[rele
+00000210: 6173 6520 6e6f 7465 735d 2868 7474 7073  ase notes](https
+00000220: 3a2f 2f73 6b62 6173 652e 7265 6164 7468  ://skbase.readth
+00000230: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00000240: 7374 2f63 6861 6e67 656c 6f67 2e68 746d  st/changelog.htm
+00000250: 6c29 2e0d 0a0d 0a7c 204f 7665 7276 6965  l).....| Overvie
+00000260: 7720 7c20 7c0d 0a7c 2d2d 2d7c 2d2d 2d7c  w | |..|---|---|
+00000270: 0d0a 7c20 2a2a 4349 2f43 442a 2a20 7c20  ..| **CI/CD** | 
+00000280: 5b21 5b54 6573 7473 5d28 6874 7470 733a  [![Tests](https:
+00000290: 2f2f 6769 7468 7562 2e63 6f6d 2f73 6b74  //github.com/skt
+000002a0: 696d 652f 736b 6261 7365 2f61 6374 696f  ime/skbase/actio
+000002b0: 6e73 2f77 6f72 6b66 6c6f 7773 2f74 6573  ns/workflows/tes
+000002c0: 742e 796d 6c2f 6261 6467 652e 7376 673f  t.yml/badge.svg?
+000002d0: 6272 616e 6368 3d6d 6169 6e29 5d28 6874  branch=main)](ht
+000002e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000002f0: 2f73 6b74 696d 652f 736b 6261 7365 2f61  /sktime/skbase/a
+00000300: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000310: 2f74 6573 742e 796d 6c29 205b 215b 636f  /test.yml) [![co
+00000320: 6465 636f 765d 2868 7474 7073 3a2f 2f63  decov](https://c
+00000330: 6f64 6563 6f76 2e69 6f2f 6768 2f73 6b74  odecov.io/gh/skt
+00000340: 696d 652f 736b 6261 7365 2f62 7261 6e63  ime/skbase/branc
+00000350: 682f 6d61 696e 2f67 7261 7068 2f62 6164  h/main/graph/bad
+00000360: 6765 2e73 7667 3f74 6f6b 656e 3d32 4a34  ge.svg?token=2J4
+00000370: 3234 4e4c 4f38 3229 5d28 6874 7470 733a  24NLO82)](https:
+00000380: 2f2f 636f 6465 636f 762e 696f 2f67 682f  //codecov.io/gh/
+00000390: 736b 7469 6d65 2f73 6b62 6173 6529 205b  sktime/skbase) [
+000003a0: 215b 446f 6375 6d65 6e74 6174 696f 6e20  ![Documentation 
+000003b0: 5374 6174 7573 5d28 6874 7470 733a 2f2f  Status](https://
+000003c0: 7265 6164 7468 6564 6f63 732e 6f72 672f  readthedocs.org/
+000003d0: 7072 6f6a 6563 7473 2f73 6b62 6173 652f  projects/skbase/
+000003e0: 6261 6467 652f 3f76 6572 7369 6f6e 3d6c  badge/?version=l
+000003f0: 6174 6573 7429 5d28 6874 7470 733a 2f2f  atest)](https://
+00000400: 736b 6261 7365 2e72 6561 6474 6865 646f  skbase.readthedo
+00000410: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
+00000420: 3f62 6164 6765 3d6c 6174 6573 7429 205b  ?badge=latest) [
+00000430: 215b 7072 652d 636f 6d6d 6974 2e63 6920  ![pre-commit.ci 
+00000440: 7374 6174 7573 5d28 6874 7470 733a 2f2f  status](https://
+00000450: 7265 7375 6c74 732e 7072 652d 636f 6d6d  results.pre-comm
+00000460: 6974 2e63 692f 6261 6467 652f 6769 7468  it.ci/badge/gith
+00000470: 7562 2f73 6b74 696d 652f 736b 6261 7365  ub/sktime/skbase
+00000480: 2f6d 6169 6e2e 7376 6729 5d28 6874 7470  /main.svg)](http
+00000490: 733a 2f2f 7265 7375 6c74 732e 7072 652d  s://results.pre-
+000004a0: 636f 6d6d 6974 2e63 692f 6c61 7465 7374  commit.ci/latest
+000004b0: 2f67 6974 6875 622f 736b 7469 6d65 2f73  /github/sktime/s
+000004c0: 6b62 6173 652f 6d61 696e 2920 7c0d 0a7c  kbase/main) |..|
+000004d0: 202a 2a43 6f64 652a 2a20 7c20 205b 215b   **Code** |  [![
+000004e0: 2170 7970 695d 2868 7474 7073 3a2f 2f69  !pypi](https://i
+000004f0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000500: 7069 2f76 2f73 6369 6b69 742d 6261 7365  pi/v/scikit-base
+00000510: 3f63 6f6c 6f72 3d6f 7261 6e67 6529 5d28  ?color=orange)](
+00000520: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00000530: 2f70 726f 6a65 6374 2f73 6b62 6173 652f  /project/skbase/
+00000540: 2920 205b 215b 2170 7974 686f 6e2d 7665  )  [![!python-ve
+00000550: 7273 696f 6e73 5d28 6874 7470 733a 2f2f  rsions](https://
+00000560: 696d 672e 7368 6965 6c64 732e 696f 2f70  img.shields.io/p
+00000570: 7970 692f 7079 7665 7273 696f 6e73 2f73  ypi/pyversions/s
+00000580: 6369 6b69 742d 6261 7365 295d 2868 7474  cikit-base)](htt
+00000590: 7073 3a2f 2f77 7777 2e70 7974 686f 6e2e  ps://www.python.
+000005a0: 6f72 672f 2920 5b21 5b21 626c 6163 6b5d  org/) [![!black]
+000005b0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+000005c0: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
+000005d0: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
+000005e0: 2d30 3030 3030 302e 7376 6729 5d28 6874  -000000.svg)](ht
+000005f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000600: 2f70 7366 2f62 6c61 636b 2920 5b21 5b73  /psf/black) [![s
+00000610: 6563 7572 6974 793a 2062 616e 6469 745d  ecurity: bandit]
+00000620: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000630: 656c 6473 2e69 6f2f 6261 6467 652f 7365  elds.io/badge/se
+00000640: 6375 7269 7479 2d62 616e 6469 742d 7965  curity-bandit-ye
+00000650: 6c6c 6f77 2e73 7667 295d 2868 7474 7073  llow.svg)](https
+00000660: 3a2f 2f67 6974 6875 622e 636f 6d2f 5079  ://github.com/Py
+00000670: 4351 412f 6261 6e64 6974 2920 7c0d 0a7c  CQA/bandit) |..|
+00000680: 202a 2a44 6f77 6e6c 6f61 6473 2a2a 7c20   **Downloads**| 
+00000690: 5b21 5b44 6f77 6e6c 6f61 6473 5d28 6874  [![Downloads](ht
+000006a0: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
+000006b0: 792e 7465 6368 2f70 6572 736f 6e61 6c69  y.tech/personali
+000006c0: 7a65 642d 6261 6467 652f 7363 696b 6974  zed-badge/scikit
+000006d0: 2d62 6173 653f 7065 7269 6f64 3d77 6565  -base?period=wee
+000006e0: 6b26 756e 6974 733d 696e 7465 726e 6174  k&units=internat
+000006f0: 696f 6e61 6c5f 7379 7374 656d 266c 6566  ional_system&lef
+00000700: 745f 636f 6c6f 723d 6772 6579 2672 6967  t_color=grey&rig
+00000710: 6874 5f63 6f6c 6f72 3d62 6c75 6526 6c65  ht_color=blue&le
+00000720: 6674 5f74 6578 743d 7765 656b 6c79 2532  ft_text=weekly%2
+00000730: 3028 7079 7069 2929 5d28 6874 7470 733a  0(pypi))](https:
+00000740: 2f2f 7065 7079 2e74 6563 682f 7072 6f6a  //pepy.tech/proj
+00000750: 6563 742f 7363 696b 6974 2d62 6173 6529  ect/scikit-base)
+00000760: 205b 215b 446f 776e 6c6f 6164 735d 2868   [![Downloads](h
+00000770: 7474 7073 3a2f 2f73 7461 7469 632e 7065  ttps://static.pe
+00000780: 7079 2e74 6563 682f 7065 7273 6f6e 616c  py.tech/personal
+00000790: 697a 6564 2d62 6164 6765 2f73 6369 6b69  ized-badge/sciki
+000007a0: 742d 6261 7365 3f70 6572 696f 643d 6d6f  t-base?period=mo
+000007b0: 6e74 6826 756e 6974 733d 696e 7465 726e  nth&units=intern
+000007c0: 6174 696f 6e61 6c5f 7379 7374 656d 266c  ational_system&l
+000007d0: 6566 745f 636f 6c6f 723d 6772 6579 2672  eft_color=grey&r
+000007e0: 6967 6874 5f63 6f6c 6f72 3d62 6c75 6526  ight_color=blue&
+000007f0: 6c65 6674 5f74 6578 743d 6d6f 6e74 686c  left_text=monthl
+00000800: 7925 3230 2870 7970 6929 295d 2868 7474  y%20(pypi))](htt
+00000810: 7073 3a2f 2f70 6570 792e 7465 6368 2f70  ps://pepy.tech/p
+00000820: 726f 6a65 6374 2f73 6369 6b69 742d 6261  roject/scikit-ba
+00000830: 7365 2920 5b21 5b44 6f77 6e6c 6f61 6473  se) [![Downloads
+00000840: 5d28 6874 7470 733a 2f2f 7374 6174 6963  ](https://static
+00000850: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
+00000860: 6e61 6c69 7a65 642d 6261 6467 652f 7363  nalized-badge/sc
+00000870: 696b 6974 2d62 6173 653f 7065 7269 6f64  ikit-base?period
+00000880: 3d74 6f74 616c 2675 6e69 7473 3d69 6e74  =total&units=int
+00000890: 6572 6e61 7469 6f6e 616c 5f73 7973 7465  ernational_syste
+000008a0: 6d26 6c65 6674 5f63 6f6c 6f72 3d67 7265  m&left_color=gre
+000008b0: 7926 7269 6768 745f 636f 6c6f 723d 626c  y&right_color=bl
+000008c0: 7565 266c 6566 745f 7465 7874 3d63 756d  ue&left_text=cum
+000008d0: 756c 6174 6976 6525 3230 2870 7970 6929  ulative%20(pypi)
+000008e0: 295d 2868 7474 7073 3a2f 2f70 6570 792e  )](https://pepy.
+000008f0: 7465 6368 2f70 726f 6a65 6374 2f73 6369  tech/project/sci
+00000900: 6b69 742d 6261 7365 2920 7c0d 0a0d 0a3c  kit-base) |....<
+00000910: 212d 2d20 414c 4c2d 434f 4e54 5249 4255  !-- ALL-CONTRIBU
+00000920: 544f 5253 2d42 4144 4745 3a53 5441 5254  TORS-BADGE:START
+00000930: 202d 2044 6f20 6e6f 7420 7265 6d6f 7665   - Do not remove
+00000940: 206f 7220 6d6f 6469 6679 2074 6869 7320   or modify this 
+00000950: 7365 6374 696f 6e20 2d2d 3e0d 0a5b 215b  section -->..[![
+00000960: 416c 6c20 436f 6e74 7269 6275 746f 7273  All Contributors
+00000970: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000980: 6965 6c64 732e 696f 2f62 6164 6765 2f61  ields.io/badge/a
+00000990: 6c6c 5f63 6f6e 7472 6962 7574 6f72 732d  ll_contributors-
+000009a0: 3133 2d6f 7261 6e67 652e 7376 673f 7374  13-orange.svg?st
+000009b0: 796c 653d 666c 6174 2d73 7175 6172 6529  yle=flat-square)
+000009c0: 5d28 2363 6f6e 7472 6962 7574 6f72 7329  ](#contributors)
+000009d0: 0d0a 3c21 2d2d 2041 4c4c 2d43 4f4e 5452  ..<!-- ALL-CONTR
+000009e0: 4942 5554 4f52 532d 4241 4447 453a 454e  IBUTORS-BADGE:EN
+000009f0: 4420 2d2d 3e0d 0a0d 0a23 2320 446f 6375  D -->....## Docu
+00000a00: 6d65 6e74 6174 696f 6e0d 0a0d 0a54 6f20  mentation....To 
+00000a10: 6c65 6172 6e20 6d6f 7265 2061 626f 7574  learn more about
+00000a20: 2074 6865 2070 6163 6b61 6765 2063 6865   the package che
+00000a30: 636b 6f75 7420 6f75 7220 5b64 6f63 756d  ckout our [docum
+00000a40: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+00000a50: 2f2f 736b 6261 7365 2e72 6561 6474 6865  //skbase.readthe
+00000a60: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00000a70: 742f 292e 0d0a 0d0a 2323 203a 686f 7572  t/).....## :hour
+00000a80: 676c 6173 735f 666c 6f77 696e 675f 7361  glass_flowing_sa
+00000a90: 6e64 3a20 496e 7374 616c 6c20 736b 6261  nd: Install skba
+00000aa0: 7365 0d0a 466f 7220 7472 6f75 626c 6520  se..For trouble 
+00000ab0: 7368 6f6f 7469 6e67 206f 7220 6d6f 7265  shooting or more
+00000ac0: 2069 6e66 6f72 6d61 7469 6f6e 2c20 7365   information, se
+00000ad0: 6520 6f75 720d 0a5b 6465 7461 696c 6564  e our..[detailed
+00000ae0: 2069 6e73 7461 6c6c 6174 696f 6e20 696e   installation in
+00000af0: 7374 7275 6374 696f 6e73 5d28 6874 7470  structions](http
+00000b00: 733a 2f2f 736b 6261 7365 2e72 6561 6474  s://skbase.readt
+00000b10: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00000b20: 6573 742f 7573 6572 5f64 6f63 756d 656e  est/user_documen
+00000b30: 7461 7469 6f6e 2f69 6e73 7461 6c6c 6174  tation/installat
+00000b40: 696f 6e2e 6874 6d6c 292e 0d0a 0d0a 2d20  ion.html).....- 
+00000b50: 2a2a 4f70 6572 6174 696e 6720 7379 7374  **Operating syst
+00000b60: 656d 2a2a 3a20 6d61 634f 5320 5820 c2b7  em**: macOS X ..
+00000b70: 204c 696e 7578 20c2 b720 5769 6e64 6f77   Linux .. Window
+00000b80: 7320 382e 3120 6f72 2068 6967 6865 720d  s 8.1 or higher.
+00000b90: 0a2d 202a 2a50 7974 686f 6e20 7665 7273  .- **Python vers
+00000ba0: 696f 6e2a 2a3a 2050 7974 686f 6e20 332e  ion**: Python 3.
+00000bb0: 372c 2033 2e38 2c20 332e 392c 2033 2e31  7, 3.8, 3.9, 3.1
+00000bc0: 3020 616e 6420 332e 3131 0d0a 2d20 2a2a  0 and 3.11..- **
+00000bd0: 5061 636b 6167 6520 6d61 6e61 6765 7273  Package managers
+00000be0: 2a2a 3a20 5b70 6970 5d0d 0a0d 0a5b 7069  **: [pip]....[pi
+00000bf0: 705d 3a20 6874 7470 733a 2f2f 7069 702e  p]: https://pip.
+00000c00: 7079 7061 2e69 6f2f 656e 2f73 7461 626c  pypa.io/en/stabl
+00000c10: 652f 0d0a 0d0a 2323 2320 7069 700d 0a73  e/....### pip..s
+00000c20: 6b62 6173 6520 7265 6c65 6173 6573 2061  kbase releases a
+00000c30: 7265 2061 7661 696c 6162 6c65 2061 7320  re available as 
+00000c40: 736f 7572 6365 2070 6163 6b61 6765 7320  source packages 
+00000c50: 616e 6420 6269 6e61 7279 2077 6865 656c  and binary wheel
+00000c60: 7320 7669 6120 5079 5049 0d0a 616e 6420  s via PyPI..and 
+00000c70: 6361 6e20 6265 2069 6e73 7461 6c6c 6564  can be installed
+00000c80: 2075 7369 6e67 2070 6970 2e20 4368 6563   using pip. Chec
+00000c90: 6b6f 7574 2074 6865 2066 756c 6c20 6c69  kout the full li
+00000ca0: 7374 206f 6620 7072 652d 636f 6d70 696c  st of pre-compil
+00000cb0: 6564 205b 7768 6565 6c73 206f 6e20 5079  ed [wheels on Py
+00000cc0: 5069 5d28 6874 7470 733a 2f2f 7079 7069  Pi](https://pypi
+00000cd0: 2e6f 7267 2f73 696d 706c 652f 736b 6261  .org/simple/skba
+00000ce0: 7365 2f29 2e0d 0a0d 0a54 6f20 696e 7374  se/).....To inst
+00000cf0: 616c 6c20 7468 6520 636f 7265 2070 6163  all the core pac
+00000d00: 6b61 6765 2075 7365 3a0d 0a0d 0a60 6060  kage use:....```
+00000d10: 6261 7368 0d0a 7069 7020 696e 7374 616c  bash..pip instal
+00000d20: 6c20 7363 696b 6974 2d62 6173 650d 0a60  l scikit-base..`
+00000d30: 6060 0d0a 0d0a 6f72 2c20 6966 2079 6f75  ``....or, if you
+00000d40: 2077 616e 7420 746f 2069 6e73 7461 6c6c   want to install
+00000d50: 2077 6974 6820 7468 6520 6d61 7869 6d75   with the maximu
+00000d60: 6d20 7365 7420 6f66 2064 6570 656e 6465  m set of depende
+00000d70: 6e63 6965 732c 2075 7365 3a0d 0a0d 0a60  ncies, use:....`
+00000d80: 6060 6261 7368 0d0a 7069 7020 696e 7374  ``bash..pip inst
+00000d90: 616c 6c20 7363 696b 6974 2d62 6173 655b  all scikit-base[
+00000da0: 616c 6c5f 6578 7472 6173 5d0d 0a60 6060  all_extras]..```
+00000db0: 0d0a                                     ..
```

### Comparing `skbase-0.4.5/docs/source/conf.py` & `skbase-0.4.6/docs/source/conf.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,299 +1,299 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Configure skbase Sphinx documentation."""
-
-# -- Path setup --------------------------------------------------------------
-
-# If extensions (or modules to document with autodoc) are in another directory,
-# add these directories to sys.path here. If the directory is relative to the
-# documentation root, use os.path.abspath to make it absolute, like shown here.
-
-import datetime
-import inspect
-import os
-import sys
-
-import skbase
-
-# -- Path setup --------------------------------------------------------------
-
-# When we build the docs on readthedocs, we build the package and want to
-# use the built files in order for sphinx to be able to properly read the
-# Cython files. Hence, we do not add the source code path to the system path.
-env_rtd = os.environ.get("READTHEDOCS")
-# Check if on Read the docs
-if not env_rtd == "True":
-    print("Not on ReadTheDocs")
-    sys.path.insert(0, os.path.abspath("../.."))
-
-# -- Project information -----------------------------------------------------
-
-current_year = datetime.datetime.now().year
-project = "skbase"
-copyright = f"{current_year} (BSD-3-Clause License)"
-author = "skbase Developers"
-
-
-# The full version, including alpha/beta/rc tags
-release = skbase.__version__
-
-# -- General configuration ---------------------------------------------------
-
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
-# ones.
-extensions = [
-    "sphinx.ext.autodoc",
-    "sphinx.ext.autosummary",
-    "numpydoc",
-    "sphinx.ext.intersphinx",
-    "sphinx.ext.linkcode",  # link to GitHub source code via linkcode_resolve()
-    "nbsphinx",  # integrates example notebooks
-    "sphinx_gallery.load_style",
-    "myst_parser",
-    "sphinx_panels",
-    "sphinx_issues",
-    "sphinx_design",
-]
-
-myst_enable_extensions = ["colon_fence"]
-
-# -- Internationalization ------------------------------------------------
-# specifying the natural language populates some key tags
-language = "en"
-
-# Use bootstrap CSS from theme.
-panels_add_bootstrap_css = False
-
-# Add any paths that contain templates here, relative to this directory.
-templates_path = ["_templates"]
-
-# The suffix(es) of source filenames.
-# You can specify multiple suffix as a list of string:
-source_suffix = {
-    ".rst": "restructuredtext",
-    ".md": "markdown",
-}
-
-# The main toctree document.
-master_doc = "index"
-
-# List of patterns, relative to source directory, that match files and
-# directories to ignore when looking for source files.
-# This pattern also affects html_static_path and html_extra_path.
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "**.ipynb_checkpoints"]
-
-# add_module_names = False
-
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
-
-# Members and inherited-members default to showing methods and attributes from
-# a class or those inherited.
-# Member-order orders the documentation in the order of how the members are
-# defined in the source code.
-autodoc_default_options = {
-    "members": True,
-    "inherited-members": True,
-    "member-order": "bysource",
-}
-
-# If true, '()' will be appended to :func: etc. cross-reference text.
-add_function_parentheses = False
-
-# Link to GitHub repo for github_issues extension
-issues_github_path = "sktime/skbase"
-
-
-def linkcode_resolve(domain, info):
-    """Return URL to source code corresponding.
-
-    Parameters
-    ----------
-    domain : str
-    info : dict
-
-    Returns
-    -------
-    url : str
-    """
-
-    def find_source():
-        # try to find the file and line number, based on code from numpy:
-        # https://github.com/numpy/numpy/blob/main/doc/source/conf.py#L286
-        obj = sys.modules[info["module"]]
-        for part in info["fullname"].split("."):
-            obj = getattr(obj, part)
-
-        fn = inspect.getsourcefile(obj)
-        fn = os.path.relpath(fn, start=os.path.dirname(skbase.__file__))
-        source, lineno = inspect.getsourcelines(obj)
-        return fn, lineno, lineno + len(source) - 1
-
-    if domain != "py" or not info["module"]:
-        return None
-    try:
-        filename = "skbase/%s#L%d-L%d" % find_source()
-    except Exception:
-        filename = info["module"].replace(".", "/") + ".py"
-    return f"https://github.com/sktime/skbase/blob/{version_match}/{filename}"
-
-
-# -- Options for HTML output -------------------------------------------------
-
-# The theme to use for HTML and HTML Help pages.  See the documentation for
-# a list of builtin themes.
-
-html_theme = "pydata_sphinx_theme"
-
-# Define the json_url for our version switcher.
-json_url = "https://skbase.readthedocs.io/en/latest/_static/switcher.json"
-
-# This uses code from the py-data-sphinx theme's own conf.py
-# Define the version we use for matching in the version switcher.
-version_match = os.environ.get("READTHEDOCS_VERSION")
-
-# If READTHEDOCS_VERSION doesn't exist, we're not on RTD
-# If it is an integer, we're in a PR build and the version isn't correct.
-if not version_match or version_match.isdigit():
-    # For local development, infer the version to match from the package.
-    if "dev" in release or "rc" in release:
-        version_match = "latest"
-        # We want to keep the relative reference if we are in dev mode
-        # but we want the whole url if we are effectively in a released version
-        json_url = "_static/switcher.json"
-    else:
-        version_match = "v" + release
-
-html_theme_options = {
-    "logo": {
-        "text": "skbase",
-        "alt_text": "skbase",
-    },
-    "icon_links": [
-        {
-            "name": "GitHub",
-            "url": "https://github.com/sktime/skbase",
-            "icon": "fab fa-github",
-        },
-        {
-            "name": "Slack",
-            "url": "https://join.slack.com/t/skbase/shared_invite/zt-1qke3vzl2-fADjZBZadBlXsLUym5NlhA",  # noqa: E501
-            "icon": "fab fa-slack",
-        },
-        {
-            "name": "PyPI",
-            "url": "https://pypi.org/project/skbase",
-            "icon": "fa-solid fa-box",
-        },
-    ],
-    "icon_links_label": "Quick Links",
-    "show_nav_level": 1,
-    "show_prev_next": False,
-    "use_edit_page_button": False,
-    "navbar_start": ["navbar-logo", "version-switcher"],
-    "navbar_center": ["navbar-nav"],
-    "switcher": {
-        "json_url": json_url,
-        "version_match": version_match,
-    },
-    "header_links_before_dropdown": 6,
-}
-
-html_context = {
-    "github_user": "sktime",
-    "github_repo": "skbase",
-    "github_version": "main",
-    "doc_path": "docs/source/",
-    "default_mode": "light",
-}
-html_sidebars = {"**": ["sidebar-nav-bs.html", "sidebar-ethical-ads.html"]}
-
-# Add any paths that contain custom static files (such as style sheets) here,
-# relative to this directory. They are copied after the builtin static files,
-# so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ["_static"]
-
-# -- Options for HTMLHelp output ---------------------------------------------
-# Output file base name for HTML help builder.
-htmlhelp_basename = "skbasedoc"
-
-
-# -- Options for LaTeX output ------------------------------------------------
-# latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-# 'papersize': 'letterpaper',
-# The font size ('10pt', '11pt' or '12pt').
-# 'pointsize': '10pt',
-# Additional stuff for the LaTeX preamble.
-# 'preamble': '',
-# Latex figure (float) alignment
-# 'figure_align': 'htbp',
-# }
-
-# Grouping the document tree into LaTeX files. List of tuples
-# (source start file, target name, title,
-#  author, documentclass [howto, manual, or own class]).
-latex_documents = [
-    (
-        master_doc,
-        "skbase.tex",
-        "skbase Documentation",
-        "skbase developers",
-        "manual",
-    ),
-]
-
-# -- Extension configuration -------------------------------------------------
-
-# -- Options for numpydoc extension ------------------------------------------
-# see http://stackoverflow.com/q/12206334/562769
-numpydoc_show_class_members = True
-# this is needed for some reason...
-# see https://github.com/numpy/numpydoc/issues/69
-numpydoc_class_members_toctree = False
-
-numpydoc_validation_checks = {"all", "GL01", "SA01", "EX01"}
-
-# -- Options for sphinx-copybutton extension----------------------------------
-copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
-copybutton_prompt_is_regexp = True
-
-# -- Options for nbsphinx extension ------------------------------------------
-nbsphinx_execute = "never"  # always  # whether to run notebooks
-nbsphinx_allow_errors = False  # False
-nbsphinx_timeout = 600  # seconds, set to -1 to disable timeout
-
-# add Binder launch buttom at the top
-current_file = "{{ env.doc2path( env.docname, base=None) }}"
-
-# make sure Binder points to latest stable release, not main
-binder_base = "https://mybinder.org/v2/gh//skbase/"
-binder_url = binder_base + f"{version_match}?filepath={current_file}"
-nbsphinx_prolog = f"""
-.. |binder| image:: https://mybinder.org/badge_logo.svg
-.. _Binder: {binder_url}
-
-|Binder|_
-"""
-
-# add link to original notebook at the bottom
-notebook_url = f"https://github.com/sktime/skbase/tree/{version_match}/{current_file}"
-nbsphinx_epilog = f"""
-----
-
-Generated using nbsphinx_. The Jupyter notebook can be found here_.
-
-.. _here: {notebook_url}
-.. _nbsphinx: https://nbsphinx.readthedocs.io/
-"""
-
-# -- Options for intersphinx extension ---------------------------------------
-
-# Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {
-    "python": ("https://docs.python.org/{.major}".format(sys.version_info), None),
-    "scikit-learn": ("https://scikit-learn.org/stable/", None),
-    "sktime": ("https://www.sktime.org/en/stable/", None),
-}
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Configure skbase Sphinx documentation."""
+
+# -- Path setup --------------------------------------------------------------
+
+# If extensions (or modules to document with autodoc) are in another directory,
+# add these directories to sys.path here. If the directory is relative to the
+# documentation root, use os.path.abspath to make it absolute, like shown here.
+
+import datetime
+import inspect
+import os
+import sys
+
+import skbase
+
+# -- Path setup --------------------------------------------------------------
+
+# When we build the docs on readthedocs, we build the package and want to
+# use the built files in order for sphinx to be able to properly read the
+# Cython files. Hence, we do not add the source code path to the system path.
+env_rtd = os.environ.get("READTHEDOCS")
+# Check if on Read the docs
+if not env_rtd == "True":
+    print("Not on ReadTheDocs")
+    sys.path.insert(0, os.path.abspath("../.."))
+
+# -- Project information -----------------------------------------------------
+
+current_year = datetime.datetime.now().year
+project = "skbase"
+copyright = f"{current_year} (BSD-3-Clause License)"
+author = "skbase Developers"
+
+
+# The full version, including alpha/beta/rc tags
+release = skbase.__version__
+
+# -- General configuration ---------------------------------------------------
+
+# Add any Sphinx extension module names here, as strings. They can be
+# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
+# ones.
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.autosummary",
+    "numpydoc",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.linkcode",  # link to GitHub source code via linkcode_resolve()
+    "nbsphinx",  # integrates example notebooks
+    "sphinx_gallery.load_style",
+    "myst_parser",
+    "sphinx_panels",
+    "sphinx_issues",
+    "sphinx_design",
+]
+
+myst_enable_extensions = ["colon_fence"]
+
+# -- Internationalization ------------------------------------------------
+# specifying the natural language populates some key tags
+language = "en"
+
+# Use bootstrap CSS from theme.
+panels_add_bootstrap_css = False
+
+# Add any paths that contain templates here, relative to this directory.
+templates_path = ["_templates"]
+
+# The suffix(es) of source filenames.
+# You can specify multiple suffix as a list of string:
+source_suffix = {
+    ".rst": "restructuredtext",
+    ".md": "markdown",
+}
+
+# The main toctree document.
+master_doc = "index"
+
+# List of patterns, relative to source directory, that match files and
+# directories to ignore when looking for source files.
+# This pattern also affects html_static_path and html_extra_path.
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "**.ipynb_checkpoints"]
+
+# add_module_names = False
+
+# The name of the Pygments (syntax highlighting) style to use.
+pygments_style = "sphinx"
+
+# Members and inherited-members default to showing methods and attributes from
+# a class or those inherited.
+# Member-order orders the documentation in the order of how the members are
+# defined in the source code.
+autodoc_default_options = {
+    "members": True,
+    "inherited-members": True,
+    "member-order": "bysource",
+}
+
+# If true, '()' will be appended to :func: etc. cross-reference text.
+add_function_parentheses = False
+
+# Link to GitHub repo for github_issues extension
+issues_github_path = "sktime/skbase"
+
+
+def linkcode_resolve(domain, info):
+    """Return URL to source code corresponding.
+
+    Parameters
+    ----------
+    domain : str
+    info : dict
+
+    Returns
+    -------
+    url : str
+    """
+
+    def find_source():
+        # try to find the file and line number, based on code from numpy:
+        # https://github.com/numpy/numpy/blob/main/doc/source/conf.py#L286
+        obj = sys.modules[info["module"]]
+        for part in info["fullname"].split("."):
+            obj = getattr(obj, part)
+
+        fn = inspect.getsourcefile(obj)
+        fn = os.path.relpath(fn, start=os.path.dirname(skbase.__file__))
+        source, lineno = inspect.getsourcelines(obj)
+        return fn, lineno, lineno + len(source) - 1
+
+    if domain != "py" or not info["module"]:
+        return None
+    try:
+        filename = "skbase/%s#L%d-L%d" % find_source()
+    except Exception:
+        filename = info["module"].replace(".", "/") + ".py"
+    return f"https://github.com/sktime/skbase/blob/{version_match}/{filename}"
+
+
+# -- Options for HTML output -------------------------------------------------
+
+# The theme to use for HTML and HTML Help pages.  See the documentation for
+# a list of builtin themes.
+
+html_theme = "pydata_sphinx_theme"
+
+# Define the json_url for our version switcher.
+json_url = "https://skbase.readthedocs.io/en/latest/_static/switcher.json"
+
+# This uses code from the py-data-sphinx theme's own conf.py
+# Define the version we use for matching in the version switcher.
+version_match = os.environ.get("READTHEDOCS_VERSION")
+
+# If READTHEDOCS_VERSION doesn't exist, we're not on RTD
+# If it is an integer, we're in a PR build and the version isn't correct.
+if not version_match or version_match.isdigit():
+    # For local development, infer the version to match from the package.
+    if "dev" in release or "rc" in release:
+        version_match = "latest"
+        # We want to keep the relative reference if we are in dev mode
+        # but we want the whole url if we are effectively in a released version
+        json_url = "_static/switcher.json"
+    else:
+        version_match = "v" + release
+
+html_theme_options = {
+    "logo": {
+        "text": "skbase",
+        "alt_text": "skbase",
+    },
+    "icon_links": [
+        {
+            "name": "GitHub",
+            "url": "https://github.com/sktime/skbase",
+            "icon": "fab fa-github",
+        },
+        {
+            "name": "Slack",
+            "url": "https://join.slack.com/t/skbase/shared_invite/zt-1qke3vzl2-fADjZBZadBlXsLUym5NlhA",  # noqa: E501
+            "icon": "fab fa-slack",
+        },
+        {
+            "name": "PyPI",
+            "url": "https://pypi.org/project/skbase",
+            "icon": "fa-solid fa-box",
+        },
+    ],
+    "icon_links_label": "Quick Links",
+    "show_nav_level": 1,
+    "show_prev_next": False,
+    "use_edit_page_button": False,
+    "navbar_start": ["navbar-logo", "version-switcher"],
+    "navbar_center": ["navbar-nav"],
+    "switcher": {
+        "json_url": json_url,
+        "version_match": version_match,
+    },
+    "header_links_before_dropdown": 6,
+}
+
+html_context = {
+    "github_user": "sktime",
+    "github_repo": "skbase",
+    "github_version": "main",
+    "doc_path": "docs/source/",
+    "default_mode": "light",
+}
+html_sidebars = {"**": ["sidebar-nav-bs.html", "sidebar-ethical-ads.html"]}
+
+# Add any paths that contain custom static files (such as style sheets) here,
+# relative to this directory. They are copied after the builtin static files,
+# so a file named "default.css" will overwrite the builtin "default.css".
+html_static_path = ["_static"]
+
+# -- Options for HTMLHelp output ---------------------------------------------
+# Output file base name for HTML help builder.
+htmlhelp_basename = "skbasedoc"
+
+
+# -- Options for LaTeX output ------------------------------------------------
+# latex_elements = {
+# The paper size ('letterpaper' or 'a4paper').
+# 'papersize': 'letterpaper',
+# The font size ('10pt', '11pt' or '12pt').
+# 'pointsize': '10pt',
+# Additional stuff for the LaTeX preamble.
+# 'preamble': '',
+# Latex figure (float) alignment
+# 'figure_align': 'htbp',
+# }
+
+# Grouping the document tree into LaTeX files. List of tuples
+# (source start file, target name, title,
+#  author, documentclass [howto, manual, or own class]).
+latex_documents = [
+    (
+        master_doc,
+        "skbase.tex",
+        "skbase Documentation",
+        "skbase developers",
+        "manual",
+    ),
+]
+
+# -- Extension configuration -------------------------------------------------
+
+# -- Options for numpydoc extension ------------------------------------------
+# see http://stackoverflow.com/q/12206334/562769
+numpydoc_show_class_members = True
+# this is needed for some reason...
+# see https://github.com/numpy/numpydoc/issues/69
+numpydoc_class_members_toctree = False
+
+numpydoc_validation_checks = {"all", "GL01", "SA01", "EX01"}
+
+# -- Options for sphinx-copybutton extension----------------------------------
+copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
+copybutton_prompt_is_regexp = True
+
+# -- Options for nbsphinx extension ------------------------------------------
+nbsphinx_execute = "never"  # always  # whether to run notebooks
+nbsphinx_allow_errors = False  # False
+nbsphinx_timeout = 600  # seconds, set to -1 to disable timeout
+
+# add Binder launch buttom at the top
+current_file = "{{ env.doc2path( env.docname, base=None) }}"
+
+# make sure Binder points to latest stable release, not main
+binder_base = "https://mybinder.org/v2/gh//skbase/"
+binder_url = binder_base + f"{version_match}?filepath={current_file}"
+nbsphinx_prolog = f"""
+.. |binder| image:: https://mybinder.org/badge_logo.svg
+.. _Binder: {binder_url}
+
+|Binder|_
+"""
+
+# add link to original notebook at the bottom
+notebook_url = f"https://github.com/sktime/skbase/tree/{version_match}/{current_file}"
+nbsphinx_epilog = f"""
+----
+
+Generated using nbsphinx_. The Jupyter notebook can be found here_.
+
+.. _here: {notebook_url}
+.. _nbsphinx: https://nbsphinx.readthedocs.io/
+"""
+
+# -- Options for intersphinx extension ---------------------------------------
+
+# Example configuration for intersphinx: refer to the Python standard library.
+intersphinx_mapping = {
+    "python": ("https://docs.python.org/{.major}".format(sys.version_info), None),
+    "scikit-learn": ("https://scikit-learn.org/stable/", None),
+    "sktime": ("https://www.sktime.org/en/stable/", None),
+}
```

### Comparing `skbase-0.4.5/skbase/_nopytest_tests.py` & `skbase-0.4.6/skbase/_nopytest_tests.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# -*- coding: utf-8 -*-
-"""Tests to run without pytest, to check pytest isolation."""
-# copyright: sktime developers, BSD-3-Clause License (see LICENSE file)
-
-from skbase.base import BaseObject
-from skbase.lookup import all_objects
-
-MODULES_TO_IGNORE = ("tests", "testing", "dependencies", "all")
-
-# all_objectscrawls all modules excepting pytest test files
-# if it encounters an unisolated import, it will throw an exception
-results = all_objects(modules_to_ignore=MODULES_TO_IGNORE)
-
-# try to run all methods of BaseObject without arguments
-# very basic test, but needs to run without pytest
-METHODS = {
-    "clone": {},
-    "get_params": {},
-    "reset": {},
-    "get_param_names": {},
-    "get_param_defaults": {},
-    "get_class_tags": {},
-    "get_tags": {},
-    "get_config": {},
-    "get_test_params": {},
-    "create_test_instance": {},
-    "create_test_instances_and_names": {},
-    "is_composite": {},
-    "set_tags": {"foo": "bar"},
-    "set_config": {"bar": "foo"},
-}
-
-mybo = BaseObject()
-for method, params in METHODS.items():
-    getattr(mybo, method)(**params)
+# -*- coding: utf-8 -*-
+"""Tests to run without pytest, to check pytest isolation."""
+# copyright: sktime developers, BSD-3-Clause License (see LICENSE file)
+
+from skbase.base import BaseObject
+from skbase.lookup import all_objects
+
+MODULES_TO_IGNORE = ("tests", "testing", "dependencies", "all")
+
+# all_objectscrawls all modules excepting pytest test files
+# if it encounters an unisolated import, it will throw an exception
+results = all_objects(modules_to_ignore=MODULES_TO_IGNORE)
+
+# try to run all methods of BaseObject without arguments
+# very basic test, but needs to run without pytest
+METHODS = {
+    "clone": {},
+    "get_params": {},
+    "reset": {},
+    "get_param_names": {},
+    "get_param_defaults": {},
+    "get_class_tags": {},
+    "get_tags": {},
+    "get_config": {},
+    "get_test_params": {},
+    "create_test_instance": {},
+    "create_test_instances_and_names": {},
+    "is_composite": {},
+    "set_tags": {"foo": "bar"},
+    "set_config": {"bar": "foo"},
+}
+
+mybo = BaseObject()
+for method, params in METHODS.items():
+    getattr(mybo, method)(**params)
```

### Comparing `skbase-0.4.5/skbase/base/_base.py` & `skbase-0.4.6/skbase/base/_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1178 +1,1249 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-# Elements of BaseObject re-use code developed in scikit-learn. These elements
-# are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
-# conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
-"""Base class template for objects and fittable objects.
-
-templates in this module:
-
-    BaseObject - object with parameters and tags
-    BaseEstimator - BaseObject that can be fitted
-
-Interface specifications below.
-
----
-
-    class name: BaseObject
-
-Parameter inspection and setter methods
-    inspect parameter values      - get_params()
-    setting parameter values      - set_params(**params)
-    list of parameter names       - get_param_names()
-    dict of parameter defaults    - get_param_defaults()
-
-Tag inspection and setter methods
-    inspect tags (all)            - get_tags()
-    inspect tags (one tag)        - get_tag(tag_name: str, tag_value_default=None)
-    inspect tags (class method)   - get_class_tags()
-    inspect tags (one tag, class) - get_class_tag(tag_name:str, tag_value_default=None)
-    setting dynamic tags          - set_tag(**tag_dict: dict)
-    set/clone dynamic tags        - clone_tags(estimator, tag_names=None)
-
-Blueprinting: resetting and cloning, post-init state with same hyper-parameters
-    reset estimator to post-init  - reset()
-    cloneestimator (copy&reset)   - clone()
-
-Testing with default parameters methods
-    getting default parameters (all sets)         - get_test_params()
-    get one test instance with default parameters - create_test_instance()
-    get list of all test instances plus name list - create_test_instances_and_names()
----
-
-    class name: BaseEstimator
-
-Provides all interface points of BaseObject, plus:
-
-Parameter inspection:
-    fitted parameter inspection - get_fitted_params()
-
-State:
-    fitted model/strategy   - by convention, any attributes ending in "_"
-    fitted state flag       - is_fitted (property)
-    fitted state check      - check_is_fitted (raises error if not is_fitted)
-"""
-import inspect
-import re
-import warnings
-from collections import defaultdict
-from copy import deepcopy
-from typing import List
-
-from skbase._exceptions import NotFittedError
-from skbase.base._pretty_printing._object_html_repr import _object_html_repr
-from skbase.base._tagmanager import _FlagManager
-
-__author__: List[str] = ["mloning", "RNKuhns", "fkiraly"]
-__all__: List[str] = ["BaseEstimator", "BaseObject"]
-
-
-class BaseObject(_FlagManager):
-    """Base class for parametric objects with sktime style tag interface.
-
-    Extends scikit-learn's BaseEstimator to include sktime style interface for tags.
-    """
-
-    _config = {
-        "display": "diagram",
-        "print_changed_only": True,
-        "check_clone": False,  # whether to execute validity checks in clone
-    }
-
-    def __init__(self):
-        """Construct BaseObject."""
-        self._init_flags(flag_attr_name="_tags")
-        self._init_flags(flag_attr_name="_config")
-        super(BaseObject, self).__init__()
-
-    def __eq__(self, other):
-        """Equality dunder. Checks equal class and parameters.
-
-        Returns True iff result of get_params(deep=False)
-        results in equal parameter sets.
-
-        Nested BaseObject descendants from get_params are compared via __eq__ as well.
-        """
-        from skbase.utils.deep_equals import deep_equals
-
-        if not isinstance(other, BaseObject):
-            return False
-
-        self_params = self.get_params(deep=False)
-        other_params = other.get_params(deep=False)
-
-        return deep_equals(self_params, other_params)
-
-    def reset(self):
-        """Reset the object to a clean post-init state.
-
-        Using reset, runs __init__ with current values of hyper-parameters
-        (result of get_params). This Removes any object attributes, except:
-
-            - hyper-parameters = arguments of __init__
-            - object attributes containing double-underscores, i.e., the string "__"
-
-        Class and object methods, and class attributes are also unaffected.
-
-        Returns
-        -------
-        self
-            Instance of class reset to a clean post-init state but retaining
-            the current hyper-parameter values.
-
-        Notes
-        -----
-        Equivalent to sklearn.clone but overwrites self. After self.reset()
-        call, self is equal in value to `type(self)(**self.get_params(deep=False))`
-        """
-        # retrieve parameters to copy them later
-        params = self.get_params(deep=False)
-
-        # delete all object attributes in self
-        attrs = [attr for attr in dir(self) if "__" not in attr]
-        cls_attrs = list(dir(type(self)))
-        self_attrs = set(attrs).difference(cls_attrs)
-        for attr in self_attrs:
-            delattr(self, attr)
-
-        # run init with a copy of parameters self had at the start
-        self.__init__(**params)
-
-        return self
-
-    def clone(self):
-        """Obtain a clone of the object with same hyper-parameters.
-
-        A clone is a different object without shared references, in post-init state.
-        This function is equivalent to returning sklearn.clone of self.
-
-        Raises
-        ------
-        RuntimeError if the clone is non-conforming, due to faulty ``__init__``.
-
-        Notes
-        -----
-        If successful, equal in value to ``type(self)(**self.get_params(deep=False))``.
-        """
-        self_params = self.get_params(deep=False)
-        self_clone = type(self)(**self_params)
-
-        # if checking the clone is turned off, return now
-        if not self.get_config()["check_clone"]:
-            return self_clone
-
-        from skbase.utils.deep_equals import deep_equals
-
-        # check that all attributes are written to the clone
-        for attrname in self_params.keys():
-            if not hasattr(self_clone, attrname):
-                raise RuntimeError(
-                    f"error in {self}.clone, __init__ must write all arguments "
-                    f"to self and not mutate them, but {attrname} was not found. "
-                    f"Please check __init__ of {self}."
-                )
-
-        clone_attrs = {attr: getattr(self_clone, attr) for attr in self_params.keys()}
-
-        # check equality of parameters post-clone and pre-clone
-        clone_attrs_valid, msg = deep_equals(self_params, clone_attrs, return_msg=True)
-        if not clone_attrs_valid:
-            raise RuntimeError(
-                f"error in {self}.clone, __init__ must write all arguments "
-                f"to self and not mutate them, but this is not the case. "
-                f"Error on equality check of arguments (x) vs parameters (y): {msg}"
-            )
-
-        return self_clone
-
-    @classmethod
-    def _get_init_signature(cls):
-        """Get class init sigature.
-
-        Useful in parameter inspection.
-
-        Returns
-        -------
-        List
-            The inspected parameter objects (including defaults).
-
-        Raises
-        ------
-        RuntimeError if cls has varargs in __init__.
-        """
-        # fetch the constructor or the original constructor before
-        # deprecation wrapping if any
-        init = getattr(cls.__init__, "deprecated_original", cls.__init__)
-        if init is object.__init__:
-            # No explicit constructor to introspect
-            return []
-
-        # introspect the constructor arguments to find the model parameters
-        # to represent
-        init_signature = inspect.signature(init)
-
-        # Consider the constructor parameters excluding 'self'
-        parameters = [
-            p
-            for p in init_signature.parameters.values()
-            if p.name != "self" and p.kind != p.VAR_KEYWORD
-        ]
-        for p in parameters:
-            if p.kind == p.VAR_POSITIONAL:
-                raise RuntimeError(
-                    "scikit-learn compatible estimators should always "
-                    "specify their parameters in the signature"
-                    " of their __init__ (no varargs)."
-                    " %s with constructor %s doesn't "
-                    " follow this convention." % (cls, init_signature)
-                )
-        return parameters
-
-    @classmethod
-    def get_param_names(cls):
-        """Get object's parameter names.
-
-        Returns
-        -------
-        param_names: list[str]
-            Alphabetically sorted list of parameter names of cls.
-        """
-        parameters = cls._get_init_signature()
-        param_names = sorted([p.name for p in parameters])
-        return param_names
-
-    @classmethod
-    def get_param_defaults(cls):
-        """Get object's parameter defaults.
-
-        Returns
-        -------
-        default_dict: dict[str, Any]
-            Keys are all parameters of cls that have a default defined in __init__
-            values are the defaults, as defined in __init__.
-        """
-        parameters = cls._get_init_signature()
-        default_dict = {
-            x.name: x.default for x in parameters if x.default != inspect._empty
-        }
-        return default_dict
-
-    def get_params(self, deep=True):
-        """Get a dict of parameters values for this object.
-
-        Parameters
-        ----------
-        deep : bool, default=True
-            Whether to return parameters of components.
-
-            * If True, will return a dict of parameter name : value for this object,
-              including parameters of components (= BaseObject-valued parameters).
-            * If False, will return a dict of parameter name : value for this object,
-              but not include parameters of components.
-
-        Returns
-        -------
-        params : dict with str-valued keys
-            Dictionary of parameters, paramname : paramvalue
-            keys-value pairs include:
-
-            * always: all parameters of this object, as via `get_param_names`
-              values are parameter value for that key, of this object
-              values are always identical to values passed at construction
-            * if `deep=True`, also contains keys/value pairs of component parameters
-              parameters of components are indexed as `[componentname]__[paramname]`
-              all parameters of `componentname` appear as `paramname` with its value
-            * if `deep=True`, also contains arbitrary levels of component recursion,
-              e.g., `[componentname]__[componentcomponentname]__[paramname]`, etc
-        """
-        params = {key: getattr(self, key) for key in self.get_param_names()}
-
-        if deep:
-            deep_params = {}
-            for key, value in params.items():
-                if hasattr(value, "get_params"):
-                    deep_items = value.get_params().items()
-                    deep_params.update({f"{key}__{k}": val for k, val in deep_items})
-            params.update(deep_params)
-
-        return params
-
-    def set_params(self, **params):
-        """Set the parameters of this object.
-
-        The method works on simple estimators as well as on nested objects.
-        The latter have parameters of the form ``<component>__<parameter>`` so
-        that it's possible to update each component of a nested object.
-
-        Parameters
-        ----------
-        **params : dict
-            BaseObject parameters.
-
-        Returns
-        -------
-        self
-            Reference to self (after parameters have been set).
-        """
-        if not params:
-            # Simple optimization to gain speed (inspect is slow)
-            return self
-        valid_params = self.get_params(deep=True)
-
-        nested_params = defaultdict(dict)  # grouped by prefix
-        for key, value in params.items():
-            key, delim, sub_key = key.partition("__")
-            if key not in valid_params:
-                raise ValueError(
-                    "Invalid parameter %s for object %s. "
-                    "Check the list of available parameters "
-                    "with `object.get_params().keys()`." % (key, self)
-                )
-
-            if delim:
-                nested_params[key][sub_key] = value
-            else:
-                setattr(self, key, value)
-                valid_params[key] = value
-
-        self.reset()
-
-        # recurse in components
-        for key, sub_params in nested_params.items():
-            valid_params[key].set_params(**sub_params)
-
-        return self
-
-    @classmethod
-    def get_class_tags(cls):
-        """Get class tags from the class and all its parent classes.
-
-        Retrieves tag: value pairs from _tags class attribute. Does not return
-        information from dynamic tags (set via set_tags or clone_tags)
-        that are defined on instances.
-
-        Returns
-        -------
-        collected_tags : dict
-            Dictionary of class tag name: tag value pairs. Collected from _tags
-            class attribute via nested inheritance.
-        """
-        return cls._get_class_flags(flag_attr_name="_tags")
-
-    @classmethod
-    def get_class_tag(cls, tag_name, tag_value_default=None):
-        """Get a class tag's value.
-
-        Does not return information from dynamic tags (set via set_tags or clone_tags)
-        that are defined on instances.
-
-        Parameters
-        ----------
-        tag_name : str
-            Name of tag value.
-        tag_value_default : any
-            Default/fallback value if tag is not found.
-
-        Returns
-        -------
-        tag_value :
-            Value of the `tag_name` tag in self. If not found, returns
-            `tag_value_default`.
-        """
-        return cls._get_class_flag(
-            flag_name=tag_name,
-            flag_value_default=tag_value_default,
-            flag_attr_name="_tags",
-        )
-
-    def get_tags(self):
-        """Get tags from estimator class and dynamic tag overrides.
-
-        Returns
-        -------
-        collected_tags : dict
-            Dictionary of tag name : tag value pairs. Collected from _tags
-            class attribute via nested inheritance and then any overrides
-            and new tags from _tags_dynamic object attribute.
-        """
-        return self._get_flags(flag_attr_name="_tags")
-
-    def get_tag(self, tag_name, tag_value_default=None, raise_error=True):
-        """Get tag value from estimator class and dynamic tag overrides.
-
-        Parameters
-        ----------
-        tag_name : str
-            Name of tag to be retrieved
-        tag_value_default : any type, optional; default=None
-            Default/fallback value if tag is not found
-        raise_error : bool
-            whether a ValueError is raised when the tag is not found
-
-        Returns
-        -------
-        tag_value : Any
-            Value of the `tag_name` tag in self. If not found, returns an error if
-            `raise_error` is True, otherwise it returns `tag_value_default`.
-
-        Raises
-        ------
-        ValueError if raise_error is True i.e. if `tag_name` is not in
-        self.get_tags().keys()
-        """
-        return self._get_flag(
-            flag_name=tag_name,
-            flag_value_default=tag_value_default,
-            raise_error=raise_error,
-            flag_attr_name="_tags",
-        )
-
-    def set_tags(self, **tag_dict):
-        """Set dynamic tags to given values.
-
-        Parameters
-        ----------
-        **tag_dict : dict
-            Dictionary of tag name: tag value pairs.
-
-        Returns
-        -------
-        Self
-            Reference to self.
-
-        Notes
-        -----
-        Changes object state by settting tag values in tag_dict as dynamic tags in self.
-        """
-        self._set_flags(flag_attr_name="_tags", **tag_dict)
-
-        return self
-
-    def clone_tags(self, estimator, tag_names=None):
-        """Clone tags from another estimator as dynamic override.
-
-        Parameters
-        ----------
-        estimator : estimator inheriting from :class:BaseEstimator
-        tag_names : str or list of str, default = None
-            Names of tags to clone. If None then all tags in estimator are used
-            as `tag_names`.
-
-        Returns
-        -------
-        Self :
-            Reference to self.
-
-        Notes
-        -----
-        Changes object state by setting tag values in tag_set from estimator as
-        dynamic tags in self.
-        """
-        self._clone_flags(
-            estimator=estimator, flag_names=tag_names, flag_attr_name="_tags"
-        )
-
-        return self
-
-    def get_config(self):
-        """Get config flags for self.
-
-        Returns
-        -------
-        config_dict : dict
-            Dictionary of config name : config value pairs. Collected from _config
-            class attribute via nested inheritance and then any overrides
-            and new tags from _onfig_dynamic object attribute.
-        """
-        return self._get_flags(flag_attr_name="_config")
-
-    def set_config(self, **config_dict):
-        """Set config flags to given values.
-
-        Parameters
-        ----------
-        config_dict : dict
-            Dictionary of config name : config value pairs.
-
-        Returns
-        -------
-        self : reference to self.
-
-        Notes
-        -----
-        Changes object state, copies configs in config_dict to self._config_dynamic.
-        """
-        self._set_flags(flag_attr_name="_config", **config_dict)
-
-        return self
-
-    @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
-
-        Parameters
-        ----------
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
-
-        Returns
-        -------
-        params : dict or list of dict, default = {}
-            Parameters to create testing instances of the class
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`
-        """
-        # if non-default parameters are required, but none have been found, raise error
-        if hasattr(cls, "_required_parameters"):
-            required_parameters = getattr(cls, "_required_parameters", [])
-            if len(required_parameters) > 0:
-                raise ValueError(
-                    f"Estimator: {cls} requires "
-                    f"non-default parameters for construction, "
-                    f"but none were given. Please set them "
-                    f"as given in the extension template"
-                )
-
-        # construct with parameter configuration for testing, otherwise construct with
-        # default parameters (empty dict)
-        params = {}
-        return params
-
-    @classmethod
-    def create_test_instance(cls, parameter_set="default"):
-        """Construct Estimator instance if possible.
-
-        Parameters
-        ----------
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
-
-        Returns
-        -------
-        instance : instance of the class with default parameters
-
-        Notes
-        -----
-        `get_test_params` can return dict or list of dict.
-        This function takes first or single dict that get_test_params returns, and
-        constructs the object with that.
-        """
-        if "parameter_set" in inspect.getfullargspec(cls.get_test_params).args:
-            params = cls.get_test_params(parameter_set=parameter_set)
-        else:
-            params = cls.get_test_params()
-
-        if isinstance(params, list) and isinstance(params[0], dict):
-            params = params[0]
-        elif isinstance(params, dict):
-            pass
-        else:
-            raise TypeError(
-                "get_test_params should either return a dict or list of dict."
-            )
-
-        return cls(**params)
-
-    @classmethod
-    def create_test_instances_and_names(cls, parameter_set="default"):
-        """Create list of all test instances and a list of names for them.
-
-        Parameters
-        ----------
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
-
-        Returns
-        -------
-        objs : list of instances of cls
-            i-th instance is cls(**cls.get_test_params()[i])
-        names : list of str, same length as objs
-            i-th element is name of i-th instance of obj in tests
-            convention is {cls.__name__}-{i} if more than one instance
-            otherwise {cls.__name__}
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
-        """
-        if "parameter_set" in inspect.getfullargspec(cls.get_test_params).args:
-            param_list = cls.get_test_params(parameter_set=parameter_set)
-        else:
-            param_list = cls.get_test_params()
-
-        objs = []
-        if not isinstance(param_list, (dict, list)):
-            raise RuntimeError(
-                f"Error in {cls.__name__}.get_test_params, "
-                "return must be param dict for class, or list thereof"
-            )
-        if isinstance(param_list, dict):
-            param_list = [param_list]
-        for params in param_list:
-            if not isinstance(params, dict):
-                raise RuntimeError(
-                    f"Error in {cls.__name__}.get_test_params, "
-                    "return must be param dict for class, or list thereof"
-                )
-            objs += [cls(**params)]
-
-        num_instances = len(param_list)
-        if num_instances > 1:
-            names = [cls.__name__ + "-" + str(i) for i in range(num_instances)]
-        else:
-            names = [cls.__name__]
-
-        return objs, names
-
-    @classmethod
-    def _has_implementation_of(cls, method):
-        """Check if method has a concrete implementation in this class.
-
-        This assumes that having an implementation is equivalent to
-            one or more overrides of `method` in the method resolution order.
-
-        Parameters
-        ----------
-        method : str, name of method to check implementation of
-
-        Returns
-        -------
-        bool, whether method has implementation in cls
-            True if cls.method has been overridden at least once in
-                the inheritance tree (according to method resolution order)
-        """
-        # walk through method resolution order and inspect methods
-        #   of classes and direct parents, "adjacent" classes in mro
-        mro = inspect.getmro(cls)
-        # collect all methods that are not none
-        methods = [getattr(c, method, None) for c in mro]
-        methods = [m for m in methods if m is not None]
-
-        for i in range(len(methods) - 1):
-            # the method has been overridden once iff
-            #  at least two of the methods collected are not equal
-            #  equivalently: some two adjacent methods are not equal
-            overridden = methods[i] != methods[i + 1]
-            if overridden:
-                return True
-
-        return False
-
-    def is_composite(self):
-        """Check if the object is composed of other BaseObjects.
-
-        A composite object is an object which contains objects, as parameters.
-        Called on an instance, since this may differ by instance.
-
-        Returns
-        -------
-        composite: bool
-            Whether an object has any parameters whose values
-            are BaseObjects.
-        """
-        # walk through method resolution order and inspect methods
-        #   of classes and direct parents, "adjacent" classes in mro
-        params = self.get_params(deep=False)
-        composite = any(isinstance(x, BaseObject) for x in params.values())
-
-        return composite
-
-    def _components(self, base_class=None):
-        """Return references to all state changing BaseObject type attributes.
-
-        This *excludes* the blue-print-like components passed in the __init__.
-
-        Caution: this method returns *references* and not *copies*.
-            Writing to the reference will change the respective attribute of self.
-
-        Parameters
-        ----------
-        base_class : class, optional, default=None, must be subclass of BaseObject
-            if not None, sub-sets return dict to only descendants of base_class
-
-        Returns
-        -------
-        dict with key = attribute name, value = reference to that BaseObject attribute
-        dict contains all attributes of self that inherit from BaseObjects, and:
-            whose names do not contain the string "__", e.g., hidden attributes
-            are not class attributes, and are not hyper-parameters (__init__ args)
-        """
-        if base_class is None:
-            base_class = BaseObject
-        if base_class is not None and not inspect.isclass(base_class):
-            raise TypeError(f"base_class must be a class, but found {type(base_class)}")
-        if base_class is not None and not issubclass(base_class, BaseObject):
-            raise TypeError("base_class must be a subclass of BaseObject")
-
-        # retrieve parameter names to exclude them later
-        param_names = self.get_params(deep=False).keys()
-
-        # retrieve all attributes that are BaseObject descendants
-        attrs = [attr for attr in dir(self) if "__" not in attr]
-        cls_attrs = list(dir(type(self)))
-        self_attrs = set(attrs).difference(cls_attrs).difference(param_names)
-
-        comp_dict = {x: getattr(self, x) for x in self_attrs}
-        comp_dict = {x: y for (x, y) in comp_dict.items() if isinstance(y, base_class)}
-
-        return comp_dict
-
-    def __repr__(self, n_char_max: int = 700):
-        """Represent class as string.
-
-        This follows the scikit-learn implementation for the string representation
-        of parameterized objects.
-
-        Parameters
-        ----------
-        n_char_max : int
-            Maximum (approximate) number of non-blank characters to render. This
-            can be useful in testing.
-        """
-        from skbase.base._pretty_printing._pprint import _BaseObjectPrettyPrinter
-
-        n_max_elements_to_show = 30  # number of elements to show in sequences
-        # use ellipsis for sequences with a lot of elements
-        pp = _BaseObjectPrettyPrinter(
-            compact=True,
-            indent=1,
-            indent_at_name=True,
-            n_max_elements_to_show=n_max_elements_to_show,
-            changed_only=self.get_config()["print_changed_only"],
-        )
-
-        repr_ = pp.pformat(self)
-
-        # Use bruteforce ellipsis when there are a lot of non-blank characters
-        n_nonblank = len("".join(repr_.split()))
-        if n_nonblank > n_char_max:
-            lim = n_char_max // 2  # apprx number of chars to keep on both ends
-            regex = r"^(\s*\S){%d}" % lim
-            # The regex '^(\s*\S){%d}' matches from the start of the string
-            # until the nth non-blank character:
-            # - ^ matches the start of string
-            # - (pattern){n} matches n repetitions of pattern
-            # - \s*\S matches a non-blank char following zero or more blanks
-            left_match = re.match(regex, repr_)
-            right_match = re.match(regex, repr_[::-1])
-            left_lim = left_match.end() if left_match is not None else 0
-            right_lim = right_match.end() if right_match is not None else 0
-
-            if "\n" in repr_[left_lim:-right_lim]:
-                # The left side and right side aren't on the same line.
-                # To avoid weird cuts, e.g.:
-                # categoric...ore',
-                # we need to start the right side with an appropriate newline
-                # character so that it renders properly as:
-                # categoric...
-                # handle_unknown='ignore',
-                # so we add [^\n]*\n which matches until the next \n
-                regex += r"[^\n]*\n"
-                right_match = re.match(regex, repr_[::-1])
-                right_lim = right_match.end() if right_match is not None else 0
-
-            ellipsis = "..."
-            if left_lim + len(ellipsis) < len(repr_) - right_lim:
-                # Only add ellipsis if it results in a shorter repr
-                repr_ = repr_[:left_lim] + "..." + repr_[-right_lim:]
-
-        return repr_
-
-    @property
-    def _repr_html_(self):
-        """HTML representation of BaseObject.
-
-        This is redundant with the logic of `_repr_mimebundle_`. The latter
-        should be favorted in the long term, `_repr_html_` is only
-        implemented for consumers who do not interpret `_repr_mimbundle_`.
-        """
-        if self.get_config()["display"] != "diagram":
-            raise AttributeError(
-                "_repr_html_ is only defined when the "
-                "`display` configuration option is set to 'diagram'."
-            )
-        return self._repr_html_inner
-
-    def _repr_html_inner(self):
-        """Return HTML representation of class.
-
-        This function is returned by the @property `_repr_html_` to make
-        `hasattr(BaseObject, "_repr_html_") return `True` or `False` depending
-        on `self.get_config()["display"]`.
-        """
-        return _object_html_repr(self)
-
-    def _repr_mimebundle_(self, **kwargs):
-        """Mime bundle used by jupyter kernels to display instances of BaseObject."""
-        output = {"text/plain": repr(self)}
-        if self.get_config()["display"] == "diagram":
-            output["text/html"] = _object_html_repr(self)
-        return output
-
-
-class TagAliaserMixin:
-    """Mixin class for tag aliasing and deprecation of old tags.
-
-    To deprecate tags, add the TagAliaserMixin to BaseObject or BaseEstimator.
-    alias_dict contains the deprecated tags, and supports removal and renaming.
-        For removal, add an entry "old_tag_name": ""
-        For renaming, add an entry "old_tag_name": "new_tag_name"
-    deprecate_dict contains the version number of renaming or removal.
-        the keys in deprecate_dict should be the same as in alias_dict.
-        values in deprecate_dict should be strings, the version of removal/renaming.
-
-    The class will ensure that new tags alias old tags and vice versa, during
-    the deprecation period. Informative warnings will be raised whenever the
-    deprecated tags are being accessed.
-
-    When removing tags, ensure to remove the removed tags from this class.
-    If no tags are deprecated anymore (e.g., all deprecated tags are removed/renamed),
-    ensure toremove this class as a parent of BaseObject or BaseEstimator.
-    """
-
-    # dictionary of aliases
-    # key = old tag; value = new tag, aliased by old tag
-    # override this in a child class
-    alias_dict = {"old_tag": "new_tag", "tag_to_remove": ""}
-
-    # dictionary of removal version
-    # key = old tag; value = version in which tag will be removed, as string
-    deprecate_dict = {"old_tag": "0.12.0", "tag_to_remove": "99.99.99"}
-
-    def __init__(self):
-        """Construct TagAliaserMixin."""
-        super(TagAliaserMixin, self).__init__()
-
-    @classmethod
-    def get_class_tags(cls):
-        """Get class tags from estimator class and all its parent classes.
-
-        Returns
-        -------
-        collected_tags : dict
-            Dictionary of tag name : tag value pairs. Collected from _tags
-            class attribute via nested inheritance. NOT overridden by dynamic
-            tags set by set_tags or mirror_tags.
-        """
-        collected_tags = super(TagAliaserMixin, cls).get_class_tags()
-        collected_tags = cls._complete_dict(collected_tags)
-        return collected_tags
-
-    @classmethod
-    def get_class_tag(cls, tag_name, tag_value_default=None):
-        """Get tag value from estimator class (only class tags).
-
-        Parameters
-        ----------
-        tag_name : str
-            Name of tag value.
-        tag_value_default : any type
-            Default/fallback value if tag is not found.
-
-        Returns
-        -------
-        tag_value :
-            Value of the `tag_name` tag in self. If not found, returns
-            `tag_value_default`.
-        """
-        cls._deprecate_tag_warn([tag_name])
-        return super(TagAliaserMixin, cls).get_class_tag(
-            tag_name=tag_name, tag_value_default=tag_value_default
-        )
-
-    def get_tags(self):
-        """Get tags from estimator class and dynamic tag overrides.
-
-        Returns
-        -------
-        collected_tags : dict
-            Dictionary of tag name : tag value pairs. Collected from _tags
-            class attribute via nested inheritance and then any overrides
-            and new tags from _tags_dynamic object attribute.
-        """
-        collected_tags = super(TagAliaserMixin, self).get_tags()
-        collected_tags = self._complete_dict(collected_tags)
-        return collected_tags
-
-    def get_tag(self, tag_name, tag_value_default=None, raise_error=True):
-        """Get tag value from estimator class and dynamic tag overrides.
-
-        Parameters
-        ----------
-        tag_name : str
-            Name of tag to be retrieved
-        tag_value_default : any type, optional; default=None
-            Default/fallback value if tag is not found
-        raise_error : bool
-            whether a ValueError is raised when the tag is not found
-
-        Returns
-        -------
-        tag_value :
-            Value of the `tag_name` tag in self. If not found, returns an error if
-            raise_error is True, otherwise it returns `tag_value_default`.
-
-        Raises
-        ------
-        ValueError if raise_error is True i.e. if tag_name is not in self.get_tags(
-        ).keys()
-        """
-        self._deprecate_tag_warn([tag_name])
-        return super(TagAliaserMixin, self).get_tag(
-            tag_name=tag_name,
-            tag_value_default=tag_value_default,
-            raise_error=raise_error,
-        )
-
-    def set_tags(self, **tag_dict):
-        """Set dynamic tags to given values.
-
-        Parameters
-        ----------
-        tag_dict : dict
-            Dictionary of tag name : tag value pairs.
-
-        Returns
-        -------
-        Self :
-            Reference to self.
-
-        Notes
-        -----
-        Changes object state by settting tag values in tag_dict as dynamic tags
-        in self.
-        """
-        self._deprecate_tag_warn(tag_dict.keys())
-
-        tag_dict = self._complete_dict(tag_dict)
-        super(TagAliaserMixin, self).set_tags(**tag_dict)
-        return self
-
-    @classmethod
-    def _complete_dict(cls, tag_dict):
-        """Add all aliased and aliasing tags to the dictionary."""
-        alias_dict = cls.alias_dict
-        deprecated_tags = set(tag_dict.keys()).intersection(alias_dict.keys())
-        new_tags = set(tag_dict.keys()).intersection(alias_dict.values())
-
-        if len(deprecated_tags) > 0 or len(new_tags) > 0:
-            new_tag_dict = deepcopy(tag_dict)
-            # for all tag strings being set, write the value
-            #   to all tags that could *be aliased by* the string
-            #   and all tags that could be *aliasing* the string
-            # this way we ensure upwards and downwards compatibility
-            for old_tag, new_tag in alias_dict.items():
-                for tag in tag_dict:
-                    if tag == old_tag and new_tag != "":
-                        new_tag_dict[new_tag] = tag_dict[tag]
-                    if tag == new_tag:
-                        new_tag_dict[old_tag] = tag_dict[tag]
-            return new_tag_dict
-        else:
-            return tag_dict
-
-    @classmethod
-    def _deprecate_tag_warn(cls, tags):
-        """Print warning message for tag deprecation.
-
-        Parameters
-        ----------
-        tags : list of str
-
-        Raises
-        ------
-        DeprecationWarning for each tag in tags that is aliased by cls.alias_dict
-        """
-        for tag_name in tags:
-            if tag_name in cls.alias_dict.keys():
-                version = cls.deprecate_dict[tag_name]
-                new_tag = cls.alias_dict[tag_name]
-                msg = f"tag {tag_name!r} will be removed in sktime version {version}"
-                if new_tag != "":
-                    msg += (
-                        f" and replaced by {new_tag!r}, please use {new_tag!r} instead"
-                    )
-                else:
-                    msg += ", please remove code that access or sets {tag_name!r}"
-                warnings.warn(msg, category=DeprecationWarning, stacklevel=2)
-
-
-class BaseEstimator(BaseObject):
-    """Base class for estimators with scikit-learn and sktime design patterns.
-
-    Extends BaseObject to include basic functionality for fittable estimators.
-    """
-
-    # tuple of non-BaseObject classes that count as nested objects
-    # get_fitted_params will retrieve parameters from these, too
-    # override in descendant class - common choice: BaseEstimator from sklearn
-    GET_FITTED_PARAMS_NESTING = ()
-
-    def __init__(self):
-        """Construct BaseEstimator."""
-        self._is_fitted = False
-        super(BaseEstimator, self).__init__()
-
-    @property
-    def is_fitted(self):
-        """Whether `fit` has been called.
-
-        Inspects object's `_is_fitted` attribute that should initialize to False
-        during object construction, and be set to True in calls to an object's
-        `fit` method.
-
-        Returns
-        -------
-        bool
-            Whether the estimator has been `fit`.
-        """
-        return self._is_fitted
-
-    def check_is_fitted(self):
-        """Check if the estimator has been fitted.
-
-        Inspects object's `_is_fitted` attribute that should initialize to False
-        during object construction, and be set to True in calls to an object's
-        `fit` method.
-
-        Raises
-        ------
-        NotFittedError
-            If the estimator has not been fitted yet.
-        """
-        if not self.is_fitted:
-            raise NotFittedError(
-                f"This instance of {self.__class__.__name__} has not been fitted yet. "
-                f"Please call `fit` first."
-            )
-
-    def get_fitted_params(self, deep=True):
-        """Get fitted parameters.
-
-        State required:
-            Requires state to be "fitted".
-
-        Parameters
-        ----------
-        deep : bool, default=True
-            Whether to return fitted parameters of components.
-
-            * If True, will return a dict of parameter name : value for this object,
-              including fitted parameters of fittable components
-              (= BaseEstimator-valued parameters).
-            * If False, will return a dict of parameter name : value for this object,
-              but not include fitted parameters of components.
-
-        Returns
-        -------
-        fitted_params : dict with str-valued keys
-            Dictionary of fitted parameters, paramname : paramvalue
-            keys-value pairs include:
-
-            * always: all fitted parameters of this object, as via `get_param_names`
-              values are fitted parameter value for that key, of this object
-            * if `deep=True`, also contains keys/value pairs of component parameters
-              parameters of components are indexed as `[componentname]__[paramname]`
-              all parameters of `componentname` appear as `paramname` with its value
-            * if `deep=True`, also contains arbitrary levels of component recursion,
-              e.g., `[componentname]__[componentcomponentname]__[paramname]`, etc
-        """
-        if not self.is_fitted:
-            raise NotFittedError(
-                f"estimator of type {type(self).__name__} has not been "
-                "fitted yet, please call fit on data before get_fitted_params"
-            )
-
-        # collect non-nested fitted params of self
-        fitted_params = self._get_fitted_params()
-
-        # the rest is only for nested parameters
-        # so, if deep=False, we simply return here
-        if not deep:
-            return fitted_params
-
-        def sh(x):
-            """Shorthand to remove all underscores at end of a string."""
-            if x.endswith("_"):
-                return sh(x[:-1])
-            else:
-                return x
-
-        # add all nested parameters from components that are skbase BaseEstimator
-        c_dict = self._components()
-        for c, comp in c_dict.items():
-            if isinstance(comp, BaseEstimator) and comp._is_fitted:
-                c_f_params = comp.get_fitted_params(deep=deep)
-                c_f_params = {f"{sh(c)}__{k}": v for k, v in c_f_params.items()}
-                fitted_params.update(c_f_params)
-
-        # add all nested parameters from components that are sklearn estimators
-        # we do this recursively as we have to reach into nested sklearn estimators
-        any_components_left_to_process = True
-        old_new_params = fitted_params
-        # this loop recursively and iteratively processes components inside components
-        while any_components_left_to_process:
-            new_params = {}
-            for c, comp in old_new_params.items():
-                if isinstance(comp, self.GET_FITTED_PARAMS_NESTING):
-                    c_f_params = self._get_fitted_params_default(comp)
-                    c_f_params = {f"{sh(c)}__{k}": v for k, v in c_f_params.items()}
-                    new_params.update(c_f_params)
-            fitted_params.update(new_params)
-            old_new_params = new_params.copy()
-            n_new_params = len(new_params)
-            any_components_left_to_process = n_new_params > 0
-
-        return fitted_params
-
-    def _get_fitted_params_default(self, obj=None):
-        """Obtain fitted params of object, per sklearn convention.
-
-        Extracts a dict with {paramstr : paramvalue} contents,
-        where paramstr are all string names of "fitted parameters".
-
-        A "fitted attribute" of obj is one that ends in "_" but does not start with "_".
-        "fitted parameters" are names of fitted attributes, minus the "_" at the end.
-
-        Parameters
-        ----------
-        obj : any object, optional, default=self
-
-        Returns
-        -------
-        fitted_params : dict with str keys
-            fitted parameters, keyed by names of fitted parameter
-        """
-        obj = obj if obj else self
-
-        # default retrieves all self attributes ending in "_"
-        # and returns them with keys that have the "_" removed
-        #
-        # get all attributes ending in "_", exclude any that start with "_" (private)
-        fitted_params = [
-            attr for attr in dir(obj) if attr.endswith("_") and not attr.startswith("_")
-        ]
-        # remove the "_" at the end
-        fitted_param_dict = {
-            p[:-1]: getattr(obj, p) for p in fitted_params if hasattr(obj, p)
-        }
-
-        return fitted_param_dict
-
-    def _get_fitted_params(self):
-        """Get fitted parameters.
-
-        private _get_fitted_params, called from get_fitted_params
-
-        State required:
-            Requires state to be "fitted".
-
-        Returns
-        -------
-        fitted_params : dict with str keys
-            fitted parameters, keyed by names of fitted parameter
-        """
-        return self._get_fitted_params_default()
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+# Elements of BaseObject re-use code developed in scikit-learn. These elements
+# are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
+# conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
+"""Base class template for objects and fittable objects.
+
+templates in this module:
+
+    BaseObject - object with parameters and tags
+    BaseEstimator - BaseObject that can be fitted
+
+Interface specifications below.
+
+---
+
+    class name: BaseObject
+
+Parameter inspection and setter methods
+    inspect parameter values      - get_params()
+    setting parameter values      - set_params(**params)
+    list of parameter names       - get_param_names()
+    dict of parameter defaults    - get_param_defaults()
+
+Tag inspection and setter methods
+    inspect tags (all)            - get_tags()
+    inspect tags (one tag)        - get_tag(tag_name: str, tag_value_default=None)
+    inspect tags (class method)   - get_class_tags()
+    inspect tags (one tag, class) - get_class_tag(tag_name:str, tag_value_default=None)
+    setting dynamic tags          - set_tag(**tag_dict: dict)
+    set/clone dynamic tags        - clone_tags(estimator, tag_names=None)
+
+Blueprinting: resetting and cloning, post-init state with same hyper-parameters
+    reset estimator to post-init  - reset()
+    cloneestimator (copy&reset)   - clone()
+
+Testing with default parameters methods
+    getting default parameters (all sets)         - get_test_params()
+    get one test instance with default parameters - create_test_instance()
+    get list of all test instances plus name list - create_test_instances_and_names()
+---
+
+    class name: BaseEstimator
+
+Provides all interface points of BaseObject, plus:
+
+Parameter inspection:
+    fitted parameter inspection - get_fitted_params()
+
+State:
+    fitted model/strategy   - by convention, any attributes ending in "_"
+    fitted state flag       - is_fitted (property)
+    fitted state check      - check_is_fitted (raises error if not is_fitted)
+"""
+import inspect
+import re
+import warnings
+from collections import defaultdict
+from copy import deepcopy
+from typing import List
+
+from skbase._exceptions import NotFittedError
+from skbase.base._pretty_printing._object_html_repr import _object_html_repr
+from skbase.base._tagmanager import _FlagManager
+
+__author__: List[str] = ["mloning", "RNKuhns", "fkiraly"]
+__all__: List[str] = ["BaseEstimator", "BaseObject"]
+
+
+class BaseObject(_FlagManager):
+    """Base class for parametric objects with sktime style tag interface.
+
+    Extends scikit-learn's BaseEstimator to include sktime style interface for tags.
+    """
+
+    _config = {
+        "display": "diagram",
+        "print_changed_only": True,
+        "check_clone": False,  # whether to execute validity checks in clone
+    }
+
+    def __init__(self):
+        """Construct BaseObject."""
+        self._init_flags(flag_attr_name="_tags")
+        self._init_flags(flag_attr_name="_config")
+        super(BaseObject, self).__init__()
+
+    def __eq__(self, other):
+        """Equality dunder. Checks equal class and parameters.
+
+        Returns True iff result of get_params(deep=False)
+        results in equal parameter sets.
+
+        Nested BaseObject descendants from get_params are compared via __eq__ as well.
+        """
+        from skbase.utils.deep_equals import deep_equals
+
+        if not isinstance(other, BaseObject):
+            return False
+
+        self_params = self.get_params(deep=False)
+        other_params = other.get_params(deep=False)
+
+        return deep_equals(self_params, other_params)
+
+    def reset(self):
+        """Reset the object to a clean post-init state.
+
+        Using reset, runs __init__ with current values of hyper-parameters
+        (result of get_params). This Removes any object attributes, except:
+
+            - hyper-parameters = arguments of __init__
+            - object attributes containing double-underscores, i.e., the string "__"
+
+        Class and object methods, and class attributes are also unaffected.
+
+        Returns
+        -------
+        self
+            Instance of class reset to a clean post-init state but retaining
+            the current hyper-parameter values.
+
+        Notes
+        -----
+        Equivalent to sklearn.clone but overwrites self. After self.reset()
+        call, self is equal in value to `type(self)(**self.get_params(deep=False))`
+        """
+        # retrieve parameters to copy them later
+        params = self.get_params(deep=False)
+
+        # delete all object attributes in self
+        attrs = [attr for attr in dir(self) if "__" not in attr]
+        cls_attrs = list(dir(type(self)))
+        self_attrs = set(attrs).difference(cls_attrs)
+        for attr in self_attrs:
+            delattr(self, attr)
+
+        # run init with a copy of parameters self had at the start
+        self.__init__(**params)
+
+        return self
+
+    def clone(self):
+        """Obtain a clone of the object with same hyper-parameters.
+
+        A clone is a different object without shared references, in post-init state.
+        This function is equivalent to returning sklearn.clone of self.
+
+        Raises
+        ------
+        RuntimeError if the clone is non-conforming, due to faulty ``__init__``.
+
+        Notes
+        -----
+        If successful, equal in value to ``type(self)(**self.get_params(deep=False))``.
+        """
+        self_params = self.get_params(deep=False)
+        self_clone = self._clone(self)
+
+        # if checking the clone is turned off, return now
+        if not self.get_config()["check_clone"]:
+            return self_clone
+
+        from skbase.utils.deep_equals import deep_equals
+
+        # check that all attributes are written to the clone
+        for attrname in self_params.keys():
+            if not hasattr(self_clone, attrname):
+                raise RuntimeError(
+                    f"error in {self}.clone, __init__ must write all arguments "
+                    f"to self and not mutate them, but {attrname} was not found. "
+                    f"Please check __init__ of {self}."
+                )
+
+        clone_attrs = {attr: getattr(self_clone, attr) for attr in self_params.keys()}
+
+        # check equality of parameters post-clone and pre-clone
+        clone_attrs_valid, msg = deep_equals(self_params, clone_attrs, return_msg=True)
+        if not clone_attrs_valid:
+            raise RuntimeError(
+                f"error in {self}.clone, __init__ must write all arguments "
+                f"to self and not mutate them, but this is not the case. "
+                f"Error on equality check of arguments (x) vs parameters (y): {msg}"
+            )
+
+        return self_clone
+
+    # copied from sklearn
+    def _clone(self, estimator, *, safe=True):
+        """Construct a new unfitted estimator with the same parameters.
+
+        Clone does a deep copy of the model in an estimator
+        without actually copying attached data. It returns a new estimator
+        with the same parameters that has not been fitted on any data.
+
+        Parameters
+        ----------
+        estimator : {list, tuple, set} of estimator instance or a single \
+                estimator instance
+            The estimator or group of estimators to be cloned.
+        safe : bool, default=True
+            If safe is False, clone will fall back to a deep copy on objects
+            that are not estimators.
+
+        Returns
+        -------
+        estimator : object
+            The deep copy of the input, an estimator if input is an estimator.
+
+        Notes
+        -----
+        If the estimator's `random_state` parameter is an integer (or if the
+        estimator doesn't have a `random_state` parameter), an *exact clone* is
+        returned: the clone and the original estimator will give the exact same
+        results. Otherwise, *statistical clone* is returned: the clone might
+        return different results from the original estimator. More details can be
+        found in :ref:`randomness`.
+        """
+        estimator_type = type(estimator)
+        # XXX: not handling dictionaries
+        if estimator_type in (list, tuple, set, frozenset):
+            return estimator_type([self._clone(e, safe=safe) for e in estimator])
+        elif not hasattr(estimator, "get_params") or isinstance(estimator, type):
+            if not safe:
+                return deepcopy(estimator)
+            else:
+                if isinstance(estimator, type):
+                    raise TypeError(
+                        "Cannot clone object. "
+                        + "You should provide an instance of "
+                        + "scikit-learn estimator instead of a class."
+                    )
+                else:
+                    raise TypeError(
+                        "Cannot clone object '%s' (type %s): "
+                        "it does not seem to be a scikit-learn "
+                        "estimator as it does not implement a "
+                        "'get_params' method." % (repr(estimator), type(estimator))
+                    )
+
+        klass = estimator.__class__
+        new_object_params = estimator.get_params(deep=False)
+        for name, param in new_object_params.items():
+            new_object_params[name] = self._clone(param, safe=False)
+        new_object = klass(**new_object_params)
+        params_set = new_object.get_params(deep=False)
+
+        # quick sanity check of the parameters of the clone
+        for name in new_object_params:
+            param1 = new_object_params[name]
+            param2 = params_set[name]
+            if param1 is not param2:
+                raise RuntimeError(
+                    "Cannot clone object %s, as the constructor "
+                    "either does not set or modifies parameter %s" % (estimator, name)
+                )
+        return new_object
+
+    @classmethod
+    def _get_init_signature(cls):
+        """Get class init sigature.
+
+        Useful in parameter inspection.
+
+        Returns
+        -------
+        List
+            The inspected parameter objects (including defaults).
+
+        Raises
+        ------
+        RuntimeError if cls has varargs in __init__.
+        """
+        # fetch the constructor or the original constructor before
+        # deprecation wrapping if any
+        init = getattr(cls.__init__, "deprecated_original", cls.__init__)
+        if init is object.__init__:
+            # No explicit constructor to introspect
+            return []
+
+        # introspect the constructor arguments to find the model parameters
+        # to represent
+        init_signature = inspect.signature(init)
+
+        # Consider the constructor parameters excluding 'self'
+        parameters = [
+            p
+            for p in init_signature.parameters.values()
+            if p.name != "self" and p.kind != p.VAR_KEYWORD
+        ]
+        for p in parameters:
+            if p.kind == p.VAR_POSITIONAL:
+                raise RuntimeError(
+                    "scikit-learn compatible estimators should always "
+                    "specify their parameters in the signature"
+                    " of their __init__ (no varargs)."
+                    " %s with constructor %s doesn't "
+                    " follow this convention." % (cls, init_signature)
+                )
+        return parameters
+
+    @classmethod
+    def get_param_names(cls):
+        """Get object's parameter names.
+
+        Returns
+        -------
+        param_names: list[str]
+            Alphabetically sorted list of parameter names of cls.
+        """
+        parameters = cls._get_init_signature()
+        param_names = sorted([p.name for p in parameters])
+        return param_names
+
+    @classmethod
+    def get_param_defaults(cls):
+        """Get object's parameter defaults.
+
+        Returns
+        -------
+        default_dict: dict[str, Any]
+            Keys are all parameters of cls that have a default defined in __init__
+            values are the defaults, as defined in __init__.
+        """
+        parameters = cls._get_init_signature()
+        default_dict = {
+            x.name: x.default for x in parameters if x.default != inspect._empty
+        }
+        return default_dict
+
+    def get_params(self, deep=True):
+        """Get a dict of parameters values for this object.
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            Whether to return parameters of components.
+
+            * If True, will return a dict of parameter name : value for this object,
+              including parameters of components (= BaseObject-valued parameters).
+            * If False, will return a dict of parameter name : value for this object,
+              but not include parameters of components.
+
+        Returns
+        -------
+        params : dict with str-valued keys
+            Dictionary of parameters, paramname : paramvalue
+            keys-value pairs include:
+
+            * always: all parameters of this object, as via `get_param_names`
+              values are parameter value for that key, of this object
+              values are always identical to values passed at construction
+            * if `deep=True`, also contains keys/value pairs of component parameters
+              parameters of components are indexed as `[componentname]__[paramname]`
+              all parameters of `componentname` appear as `paramname` with its value
+            * if `deep=True`, also contains arbitrary levels of component recursion,
+              e.g., `[componentname]__[componentcomponentname]__[paramname]`, etc
+        """
+        params = {key: getattr(self, key) for key in self.get_param_names()}
+
+        if deep:
+            deep_params = {}
+            for key, value in params.items():
+                if hasattr(value, "get_params"):
+                    deep_items = value.get_params().items()
+                    deep_params.update({f"{key}__{k}": val for k, val in deep_items})
+            params.update(deep_params)
+
+        return params
+
+    def set_params(self, **params):
+        """Set the parameters of this object.
+
+        The method works on simple estimators as well as on nested objects.
+        The latter have parameters of the form ``<component>__<parameter>`` so
+        that it's possible to update each component of a nested object.
+
+        Parameters
+        ----------
+        **params : dict
+            BaseObject parameters.
+
+        Returns
+        -------
+        self
+            Reference to self (after parameters have been set).
+        """
+        if not params:
+            # Simple optimization to gain speed (inspect is slow)
+            return self
+        valid_params = self.get_params(deep=True)
+
+        nested_params = defaultdict(dict)  # grouped by prefix
+        for key, value in params.items():
+            key, delim, sub_key = key.partition("__")
+            if key not in valid_params:
+                raise ValueError(
+                    "Invalid parameter %s for object %s. "
+                    "Check the list of available parameters "
+                    "with `object.get_params().keys()`." % (key, self)
+                )
+
+            if delim:
+                nested_params[key][sub_key] = value
+            else:
+                setattr(self, key, value)
+                valid_params[key] = value
+
+        self.reset()
+
+        # recurse in components
+        for key, sub_params in nested_params.items():
+            valid_params[key].set_params(**sub_params)
+
+        return self
+
+    @classmethod
+    def get_class_tags(cls):
+        """Get class tags from the class and all its parent classes.
+
+        Retrieves tag: value pairs from _tags class attribute. Does not return
+        information from dynamic tags (set via set_tags or clone_tags)
+        that are defined on instances.
+
+        Returns
+        -------
+        collected_tags : dict
+            Dictionary of class tag name: tag value pairs. Collected from _tags
+            class attribute via nested inheritance.
+        """
+        return cls._get_class_flags(flag_attr_name="_tags")
+
+    @classmethod
+    def get_class_tag(cls, tag_name, tag_value_default=None):
+        """Get a class tag's value.
+
+        Does not return information from dynamic tags (set via set_tags or clone_tags)
+        that are defined on instances.
+
+        Parameters
+        ----------
+        tag_name : str
+            Name of tag value.
+        tag_value_default : any
+            Default/fallback value if tag is not found.
+
+        Returns
+        -------
+        tag_value :
+            Value of the `tag_name` tag in self. If not found, returns
+            `tag_value_default`.
+        """
+        return cls._get_class_flag(
+            flag_name=tag_name,
+            flag_value_default=tag_value_default,
+            flag_attr_name="_tags",
+        )
+
+    def get_tags(self):
+        """Get tags from estimator class and dynamic tag overrides.
+
+        Returns
+        -------
+        collected_tags : dict
+            Dictionary of tag name : tag value pairs. Collected from _tags
+            class attribute via nested inheritance and then any overrides
+            and new tags from _tags_dynamic object attribute.
+        """
+        return self._get_flags(flag_attr_name="_tags")
+
+    def get_tag(self, tag_name, tag_value_default=None, raise_error=True):
+        """Get tag value from estimator class and dynamic tag overrides.
+
+        Parameters
+        ----------
+        tag_name : str
+            Name of tag to be retrieved
+        tag_value_default : any type, optional; default=None
+            Default/fallback value if tag is not found
+        raise_error : bool
+            whether a ValueError is raised when the tag is not found
+
+        Returns
+        -------
+        tag_value : Any
+            Value of the `tag_name` tag in self. If not found, returns an error if
+            `raise_error` is True, otherwise it returns `tag_value_default`.
+
+        Raises
+        ------
+        ValueError if raise_error is True i.e. if `tag_name` is not in
+        self.get_tags().keys()
+        """
+        return self._get_flag(
+            flag_name=tag_name,
+            flag_value_default=tag_value_default,
+            raise_error=raise_error,
+            flag_attr_name="_tags",
+        )
+
+    def set_tags(self, **tag_dict):
+        """Set dynamic tags to given values.
+
+        Parameters
+        ----------
+        **tag_dict : dict
+            Dictionary of tag name: tag value pairs.
+
+        Returns
+        -------
+        Self
+            Reference to self.
+
+        Notes
+        -----
+        Changes object state by settting tag values in tag_dict as dynamic tags in self.
+        """
+        self._set_flags(flag_attr_name="_tags", **tag_dict)
+
+        return self
+
+    def clone_tags(self, estimator, tag_names=None):
+        """Clone tags from another estimator as dynamic override.
+
+        Parameters
+        ----------
+        estimator : estimator inheriting from :class:BaseEstimator
+        tag_names : str or list of str, default = None
+            Names of tags to clone. If None then all tags in estimator are used
+            as `tag_names`.
+
+        Returns
+        -------
+        Self :
+            Reference to self.
+
+        Notes
+        -----
+        Changes object state by setting tag values in tag_set from estimator as
+        dynamic tags in self.
+        """
+        self._clone_flags(
+            estimator=estimator, flag_names=tag_names, flag_attr_name="_tags"
+        )
+
+        return self
+
+    def get_config(self):
+        """Get config flags for self.
+
+        Returns
+        -------
+        config_dict : dict
+            Dictionary of config name : config value pairs. Collected from _config
+            class attribute via nested inheritance and then any overrides
+            and new tags from _onfig_dynamic object attribute.
+        """
+        return self._get_flags(flag_attr_name="_config")
+
+    def set_config(self, **config_dict):
+        """Set config flags to given values.
+
+        Parameters
+        ----------
+        config_dict : dict
+            Dictionary of config name : config value pairs.
+
+        Returns
+        -------
+        self : reference to self.
+
+        Notes
+        -----
+        Changes object state, copies configs in config_dict to self._config_dynamic.
+        """
+        self._set_flags(flag_attr_name="_config", **config_dict)
+
+        return self
+
+    @classmethod
+    def get_test_params(cls, parameter_set="default"):
+        """Return testing parameter settings for the estimator.
+
+        Parameters
+        ----------
+        parameter_set : str, default="default"
+            Name of the set of test parameters to return, for use in tests. If no
+            special parameters are defined for a value, will return `"default"` set.
+
+        Returns
+        -------
+        params : dict or list of dict, default = {}
+            Parameters to create testing instances of the class
+            Each dict are parameters to construct an "interesting" test instance, i.e.,
+            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
+            `create_test_instance` uses the first (or only) dictionary in `params`
+        """
+        # if non-default parameters are required, but none have been found, raise error
+        if hasattr(cls, "_required_parameters"):
+            required_parameters = getattr(cls, "_required_parameters", [])
+            if len(required_parameters) > 0:
+                raise ValueError(
+                    f"Estimator: {cls} requires "
+                    f"non-default parameters for construction, "
+                    f"but none were given. Please set them "
+                    f"as given in the extension template"
+                )
+
+        # construct with parameter configuration for testing, otherwise construct with
+        # default parameters (empty dict)
+        params = {}
+        return params
+
+    @classmethod
+    def create_test_instance(cls, parameter_set="default"):
+        """Construct Estimator instance if possible.
+
+        Parameters
+        ----------
+        parameter_set : str, default="default"
+            Name of the set of test parameters to return, for use in tests. If no
+            special parameters are defined for a value, will return `"default"` set.
+
+        Returns
+        -------
+        instance : instance of the class with default parameters
+
+        Notes
+        -----
+        `get_test_params` can return dict or list of dict.
+        This function takes first or single dict that get_test_params returns, and
+        constructs the object with that.
+        """
+        if "parameter_set" in inspect.getfullargspec(cls.get_test_params).args:
+            params = cls.get_test_params(parameter_set=parameter_set)
+        else:
+            params = cls.get_test_params()
+
+        if isinstance(params, list) and isinstance(params[0], dict):
+            params = params[0]
+        elif isinstance(params, dict):
+            pass
+        else:
+            raise TypeError(
+                "get_test_params should either return a dict or list of dict."
+            )
+
+        return cls(**params)
+
+    @classmethod
+    def create_test_instances_and_names(cls, parameter_set="default"):
+        """Create list of all test instances and a list of names for them.
+
+        Parameters
+        ----------
+        parameter_set : str, default="default"
+            Name of the set of test parameters to return, for use in tests. If no
+            special parameters are defined for a value, will return `"default"` set.
+
+        Returns
+        -------
+        objs : list of instances of cls
+            i-th instance is cls(**cls.get_test_params()[i])
+        names : list of str, same length as objs
+            i-th element is name of i-th instance of obj in tests
+            convention is {cls.__name__}-{i} if more than one instance
+            otherwise {cls.__name__}
+        parameter_set : str, default="default"
+            Name of the set of test parameters to return, for use in tests. If no
+            special parameters are defined for a value, will return `"default"` set.
+        """
+        if "parameter_set" in inspect.getfullargspec(cls.get_test_params).args:
+            param_list = cls.get_test_params(parameter_set=parameter_set)
+        else:
+            param_list = cls.get_test_params()
+
+        objs = []
+        if not isinstance(param_list, (dict, list)):
+            raise RuntimeError(
+                f"Error in {cls.__name__}.get_test_params, "
+                "return must be param dict for class, or list thereof"
+            )
+        if isinstance(param_list, dict):
+            param_list = [param_list]
+        for params in param_list:
+            if not isinstance(params, dict):
+                raise RuntimeError(
+                    f"Error in {cls.__name__}.get_test_params, "
+                    "return must be param dict for class, or list thereof"
+                )
+            objs += [cls(**params)]
+
+        num_instances = len(param_list)
+        if num_instances > 1:
+            names = [cls.__name__ + "-" + str(i) for i in range(num_instances)]
+        else:
+            names = [cls.__name__]
+
+        return objs, names
+
+    @classmethod
+    def _has_implementation_of(cls, method):
+        """Check if method has a concrete implementation in this class.
+
+        This assumes that having an implementation is equivalent to
+            one or more overrides of `method` in the method resolution order.
+
+        Parameters
+        ----------
+        method : str, name of method to check implementation of
+
+        Returns
+        -------
+        bool, whether method has implementation in cls
+            True if cls.method has been overridden at least once in
+                the inheritance tree (according to method resolution order)
+        """
+        # walk through method resolution order and inspect methods
+        #   of classes and direct parents, "adjacent" classes in mro
+        mro = inspect.getmro(cls)
+        # collect all methods that are not none
+        methods = [getattr(c, method, None) for c in mro]
+        methods = [m for m in methods if m is not None]
+
+        for i in range(len(methods) - 1):
+            # the method has been overridden once iff
+            #  at least two of the methods collected are not equal
+            #  equivalently: some two adjacent methods are not equal
+            overridden = methods[i] != methods[i + 1]
+            if overridden:
+                return True
+
+        return False
+
+    def is_composite(self):
+        """Check if the object is composed of other BaseObjects.
+
+        A composite object is an object which contains objects, as parameters.
+        Called on an instance, since this may differ by instance.
+
+        Returns
+        -------
+        composite: bool
+            Whether an object has any parameters whose values
+            are BaseObjects.
+        """
+        # walk through method resolution order and inspect methods
+        #   of classes and direct parents, "adjacent" classes in mro
+        params = self.get_params(deep=False)
+        composite = any(isinstance(x, BaseObject) for x in params.values())
+
+        return composite
+
+    def _components(self, base_class=None):
+        """Return references to all state changing BaseObject type attributes.
+
+        This *excludes* the blue-print-like components passed in the __init__.
+
+        Caution: this method returns *references* and not *copies*.
+            Writing to the reference will change the respective attribute of self.
+
+        Parameters
+        ----------
+        base_class : class, optional, default=None, must be subclass of BaseObject
+            if not None, sub-sets return dict to only descendants of base_class
+
+        Returns
+        -------
+        dict with key = attribute name, value = reference to that BaseObject attribute
+        dict contains all attributes of self that inherit from BaseObjects, and:
+            whose names do not contain the string "__", e.g., hidden attributes
+            are not class attributes, and are not hyper-parameters (__init__ args)
+        """
+        if base_class is None:
+            base_class = BaseObject
+        if base_class is not None and not inspect.isclass(base_class):
+            raise TypeError(f"base_class must be a class, but found {type(base_class)}")
+        if base_class is not None and not issubclass(base_class, BaseObject):
+            raise TypeError("base_class must be a subclass of BaseObject")
+
+        # retrieve parameter names to exclude them later
+        param_names = self.get_params(deep=False).keys()
+
+        # retrieve all attributes that are BaseObject descendants
+        attrs = [attr for attr in dir(self) if "__" not in attr]
+        cls_attrs = list(dir(type(self)))
+        self_attrs = set(attrs).difference(cls_attrs).difference(param_names)
+
+        comp_dict = {x: getattr(self, x) for x in self_attrs}
+        comp_dict = {x: y for (x, y) in comp_dict.items() if isinstance(y, base_class)}
+
+        return comp_dict
+
+    def __repr__(self, n_char_max: int = 700):
+        """Represent class as string.
+
+        This follows the scikit-learn implementation for the string representation
+        of parameterized objects.
+
+        Parameters
+        ----------
+        n_char_max : int
+            Maximum (approximate) number of non-blank characters to render. This
+            can be useful in testing.
+        """
+        from skbase.base._pretty_printing._pprint import _BaseObjectPrettyPrinter
+
+        n_max_elements_to_show = 30  # number of elements to show in sequences
+        # use ellipsis for sequences with a lot of elements
+        pp = _BaseObjectPrettyPrinter(
+            compact=True,
+            indent=1,
+            indent_at_name=True,
+            n_max_elements_to_show=n_max_elements_to_show,
+            changed_only=self.get_config()["print_changed_only"],
+        )
+
+        repr_ = pp.pformat(self)
+
+        # Use bruteforce ellipsis when there are a lot of non-blank characters
+        n_nonblank = len("".join(repr_.split()))
+        if n_nonblank > n_char_max:
+            lim = n_char_max // 2  # apprx number of chars to keep on both ends
+            regex = r"^(\s*\S){%d}" % lim
+            # The regex '^(\s*\S){%d}' matches from the start of the string
+            # until the nth non-blank character:
+            # - ^ matches the start of string
+            # - (pattern){n} matches n repetitions of pattern
+            # - \s*\S matches a non-blank char following zero or more blanks
+            left_match = re.match(regex, repr_)
+            right_match = re.match(regex, repr_[::-1])
+            left_lim = left_match.end() if left_match is not None else 0
+            right_lim = right_match.end() if right_match is not None else 0
+
+            if "\n" in repr_[left_lim:-right_lim]:
+                # The left side and right side aren't on the same line.
+                # To avoid weird cuts, e.g.:
+                # categoric...ore',
+                # we need to start the right side with an appropriate newline
+                # character so that it renders properly as:
+                # categoric...
+                # handle_unknown='ignore',
+                # so we add [^\n]*\n which matches until the next \n
+                regex += r"[^\n]*\n"
+                right_match = re.match(regex, repr_[::-1])
+                right_lim = right_match.end() if right_match is not None else 0
+
+            ellipsis = "..."
+            if left_lim + len(ellipsis) < len(repr_) - right_lim:
+                # Only add ellipsis if it results in a shorter repr
+                repr_ = repr_[:left_lim] + "..." + repr_[-right_lim:]
+
+        return repr_
+
+    @property
+    def _repr_html_(self):
+        """HTML representation of BaseObject.
+
+        This is redundant with the logic of `_repr_mimebundle_`. The latter
+        should be favorted in the long term, `_repr_html_` is only
+        implemented for consumers who do not interpret `_repr_mimbundle_`.
+        """
+        if self.get_config()["display"] != "diagram":
+            raise AttributeError(
+                "_repr_html_ is only defined when the "
+                "`display` configuration option is set to 'diagram'."
+            )
+        return self._repr_html_inner
+
+    def _repr_html_inner(self):
+        """Return HTML representation of class.
+
+        This function is returned by the @property `_repr_html_` to make
+        `hasattr(BaseObject, "_repr_html_") return `True` or `False` depending
+        on `self.get_config()["display"]`.
+        """
+        return _object_html_repr(self)
+
+    def _repr_mimebundle_(self, **kwargs):
+        """Mime bundle used by jupyter kernels to display instances of BaseObject."""
+        output = {"text/plain": repr(self)}
+        if self.get_config()["display"] == "diagram":
+            output["text/html"] = _object_html_repr(self)
+        return output
+
+
+class TagAliaserMixin:
+    """Mixin class for tag aliasing and deprecation of old tags.
+
+    To deprecate tags, add the TagAliaserMixin to BaseObject or BaseEstimator.
+    alias_dict contains the deprecated tags, and supports removal and renaming.
+        For removal, add an entry "old_tag_name": ""
+        For renaming, add an entry "old_tag_name": "new_tag_name"
+    deprecate_dict contains the version number of renaming or removal.
+        the keys in deprecate_dict should be the same as in alias_dict.
+        values in deprecate_dict should be strings, the version of removal/renaming.
+
+    The class will ensure that new tags alias old tags and vice versa, during
+    the deprecation period. Informative warnings will be raised whenever the
+    deprecated tags are being accessed.
+
+    When removing tags, ensure to remove the removed tags from this class.
+    If no tags are deprecated anymore (e.g., all deprecated tags are removed/renamed),
+    ensure toremove this class as a parent of BaseObject or BaseEstimator.
+    """
+
+    # dictionary of aliases
+    # key = old tag; value = new tag, aliased by old tag
+    # override this in a child class
+    alias_dict = {"old_tag": "new_tag", "tag_to_remove": ""}
+
+    # dictionary of removal version
+    # key = old tag; value = version in which tag will be removed, as string
+    deprecate_dict = {"old_tag": "0.12.0", "tag_to_remove": "99.99.99"}
+
+    def __init__(self):
+        """Construct TagAliaserMixin."""
+        super(TagAliaserMixin, self).__init__()
+
+    @classmethod
+    def get_class_tags(cls):
+        """Get class tags from estimator class and all its parent classes.
+
+        Returns
+        -------
+        collected_tags : dict
+            Dictionary of tag name : tag value pairs. Collected from _tags
+            class attribute via nested inheritance. NOT overridden by dynamic
+            tags set by set_tags or mirror_tags.
+        """
+        collected_tags = super(TagAliaserMixin, cls).get_class_tags()
+        collected_tags = cls._complete_dict(collected_tags)
+        return collected_tags
+
+    @classmethod
+    def get_class_tag(cls, tag_name, tag_value_default=None):
+        """Get tag value from estimator class (only class tags).
+
+        Parameters
+        ----------
+        tag_name : str
+            Name of tag value.
+        tag_value_default : any type
+            Default/fallback value if tag is not found.
+
+        Returns
+        -------
+        tag_value :
+            Value of the `tag_name` tag in self. If not found, returns
+            `tag_value_default`.
+        """
+        cls._deprecate_tag_warn([tag_name])
+        return super(TagAliaserMixin, cls).get_class_tag(
+            tag_name=tag_name, tag_value_default=tag_value_default
+        )
+
+    def get_tags(self):
+        """Get tags from estimator class and dynamic tag overrides.
+
+        Returns
+        -------
+        collected_tags : dict
+            Dictionary of tag name : tag value pairs. Collected from _tags
+            class attribute via nested inheritance and then any overrides
+            and new tags from _tags_dynamic object attribute.
+        """
+        collected_tags = super(TagAliaserMixin, self).get_tags()
+        collected_tags = self._complete_dict(collected_tags)
+        return collected_tags
+
+    def get_tag(self, tag_name, tag_value_default=None, raise_error=True):
+        """Get tag value from estimator class and dynamic tag overrides.
+
+        Parameters
+        ----------
+        tag_name : str
+            Name of tag to be retrieved
+        tag_value_default : any type, optional; default=None
+            Default/fallback value if tag is not found
+        raise_error : bool
+            whether a ValueError is raised when the tag is not found
+
+        Returns
+        -------
+        tag_value :
+            Value of the `tag_name` tag in self. If not found, returns an error if
+            raise_error is True, otherwise it returns `tag_value_default`.
+
+        Raises
+        ------
+        ValueError if raise_error is True i.e. if tag_name is not in self.get_tags(
+        ).keys()
+        """
+        self._deprecate_tag_warn([tag_name])
+        return super(TagAliaserMixin, self).get_tag(
+            tag_name=tag_name,
+            tag_value_default=tag_value_default,
+            raise_error=raise_error,
+        )
+
+    def set_tags(self, **tag_dict):
+        """Set dynamic tags to given values.
+
+        Parameters
+        ----------
+        tag_dict : dict
+            Dictionary of tag name : tag value pairs.
+
+        Returns
+        -------
+        Self :
+            Reference to self.
+
+        Notes
+        -----
+        Changes object state by settting tag values in tag_dict as dynamic tags
+        in self.
+        """
+        self._deprecate_tag_warn(tag_dict.keys())
+
+        tag_dict = self._complete_dict(tag_dict)
+        super(TagAliaserMixin, self).set_tags(**tag_dict)
+        return self
+
+    @classmethod
+    def _complete_dict(cls, tag_dict):
+        """Add all aliased and aliasing tags to the dictionary."""
+        alias_dict = cls.alias_dict
+        deprecated_tags = set(tag_dict.keys()).intersection(alias_dict.keys())
+        new_tags = set(tag_dict.keys()).intersection(alias_dict.values())
+
+        if len(deprecated_tags) > 0 or len(new_tags) > 0:
+            new_tag_dict = deepcopy(tag_dict)
+            # for all tag strings being set, write the value
+            #   to all tags that could *be aliased by* the string
+            #   and all tags that could be *aliasing* the string
+            # this way we ensure upwards and downwards compatibility
+            for old_tag, new_tag in alias_dict.items():
+                for tag in tag_dict:
+                    if tag == old_tag and new_tag != "":
+                        new_tag_dict[new_tag] = tag_dict[tag]
+                    if tag == new_tag:
+                        new_tag_dict[old_tag] = tag_dict[tag]
+            return new_tag_dict
+        else:
+            return tag_dict
+
+    @classmethod
+    def _deprecate_tag_warn(cls, tags):
+        """Print warning message for tag deprecation.
+
+        Parameters
+        ----------
+        tags : list of str
+
+        Raises
+        ------
+        DeprecationWarning for each tag in tags that is aliased by cls.alias_dict
+        """
+        for tag_name in tags:
+            if tag_name in cls.alias_dict.keys():
+                version = cls.deprecate_dict[tag_name]
+                new_tag = cls.alias_dict[tag_name]
+                msg = f"tag {tag_name!r} will be removed in sktime version {version}"
+                if new_tag != "":
+                    msg += (
+                        f" and replaced by {new_tag!r}, please use {new_tag!r} instead"
+                    )
+                else:
+                    msg += ", please remove code that access or sets {tag_name!r}"
+                warnings.warn(msg, category=DeprecationWarning, stacklevel=2)
+
+
+class BaseEstimator(BaseObject):
+    """Base class for estimators with scikit-learn and sktime design patterns.
+
+    Extends BaseObject to include basic functionality for fittable estimators.
+    """
+
+    # tuple of non-BaseObject classes that count as nested objects
+    # get_fitted_params will retrieve parameters from these, too
+    # override in descendant class - common choice: BaseEstimator from sklearn
+    GET_FITTED_PARAMS_NESTING = ()
+
+    def __init__(self):
+        """Construct BaseEstimator."""
+        self._is_fitted = False
+        super(BaseEstimator, self).__init__()
+
+    @property
+    def is_fitted(self):
+        """Whether `fit` has been called.
+
+        Inspects object's `_is_fitted` attribute that should initialize to False
+        during object construction, and be set to True in calls to an object's
+        `fit` method.
+
+        Returns
+        -------
+        bool
+            Whether the estimator has been `fit`.
+        """
+        return self._is_fitted
+
+    def check_is_fitted(self):
+        """Check if the estimator has been fitted.
+
+        Inspects object's `_is_fitted` attribute that should initialize to False
+        during object construction, and be set to True in calls to an object's
+        `fit` method.
+
+        Raises
+        ------
+        NotFittedError
+            If the estimator has not been fitted yet.
+        """
+        if not self.is_fitted:
+            raise NotFittedError(
+                f"This instance of {self.__class__.__name__} has not been fitted yet. "
+                f"Please call `fit` first."
+            )
+
+    def get_fitted_params(self, deep=True):
+        """Get fitted parameters.
+
+        State required:
+            Requires state to be "fitted".
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            Whether to return fitted parameters of components.
+
+            * If True, will return a dict of parameter name : value for this object,
+              including fitted parameters of fittable components
+              (= BaseEstimator-valued parameters).
+            * If False, will return a dict of parameter name : value for this object,
+              but not include fitted parameters of components.
+
+        Returns
+        -------
+        fitted_params : dict with str-valued keys
+            Dictionary of fitted parameters, paramname : paramvalue
+            keys-value pairs include:
+
+            * always: all fitted parameters of this object, as via `get_param_names`
+              values are fitted parameter value for that key, of this object
+            * if `deep=True`, also contains keys/value pairs of component parameters
+              parameters of components are indexed as `[componentname]__[paramname]`
+              all parameters of `componentname` appear as `paramname` with its value
+            * if `deep=True`, also contains arbitrary levels of component recursion,
+              e.g., `[componentname]__[componentcomponentname]__[paramname]`, etc
+        """
+        if not self.is_fitted:
+            raise NotFittedError(
+                f"estimator of type {type(self).__name__} has not been "
+                "fitted yet, please call fit on data before get_fitted_params"
+            )
+
+        # collect non-nested fitted params of self
+        fitted_params = self._get_fitted_params()
+
+        # the rest is only for nested parameters
+        # so, if deep=False, we simply return here
+        if not deep:
+            return fitted_params
+
+        def sh(x):
+            """Shorthand to remove all underscores at end of a string."""
+            if x.endswith("_"):
+                return sh(x[:-1])
+            else:
+                return x
+
+        # add all nested parameters from components that are skbase BaseEstimator
+        c_dict = self._components()
+        for c, comp in c_dict.items():
+            if isinstance(comp, BaseEstimator) and comp._is_fitted:
+                c_f_params = comp.get_fitted_params(deep=deep)
+                c_f_params = {f"{sh(c)}__{k}": v for k, v in c_f_params.items()}
+                fitted_params.update(c_f_params)
+
+        # add all nested parameters from components that are sklearn estimators
+        # we do this recursively as we have to reach into nested sklearn estimators
+        any_components_left_to_process = True
+        old_new_params = fitted_params
+        # this loop recursively and iteratively processes components inside components
+        while any_components_left_to_process:
+            new_params = {}
+            for c, comp in old_new_params.items():
+                if isinstance(comp, self.GET_FITTED_PARAMS_NESTING):
+                    c_f_params = self._get_fitted_params_default(comp)
+                    c_f_params = {f"{sh(c)}__{k}": v for k, v in c_f_params.items()}
+                    new_params.update(c_f_params)
+            fitted_params.update(new_params)
+            old_new_params = new_params.copy()
+            n_new_params = len(new_params)
+            any_components_left_to_process = n_new_params > 0
+
+        return fitted_params
+
+    def _get_fitted_params_default(self, obj=None):
+        """Obtain fitted params of object, per sklearn convention.
+
+        Extracts a dict with {paramstr : paramvalue} contents,
+        where paramstr are all string names of "fitted parameters".
+
+        A "fitted attribute" of obj is one that ends in "_" but does not start with "_".
+        "fitted parameters" are names of fitted attributes, minus the "_" at the end.
+
+        Parameters
+        ----------
+        obj : any object, optional, default=self
+
+        Returns
+        -------
+        fitted_params : dict with str keys
+            fitted parameters, keyed by names of fitted parameter
+        """
+        obj = obj if obj else self
+
+        # default retrieves all self attributes ending in "_"
+        # and returns them with keys that have the "_" removed
+        #
+        # get all attributes ending in "_", exclude any that start with "_" (private)
+        fitted_params = [
+            attr for attr in dir(obj) if attr.endswith("_") and not attr.startswith("_")
+        ]
+        # remove the "_" at the end
+        fitted_param_dict = {
+            p[:-1]: getattr(obj, p) for p in fitted_params if hasattr(obj, p)
+        }
+
+        return fitted_param_dict
+
+    def _get_fitted_params(self):
+        """Get fitted parameters.
+
+        private _get_fitted_params, called from get_fitted_params
+
+        State required:
+            Requires state to be "fitted".
+
+        Returns
+        -------
+        fitted_params : dict with str keys
+            fitted parameters, keyed by names of fitted parameter
+        """
+        return self._get_fitted_params_default()
```

### Comparing `skbase-0.4.5/skbase/base/_meta.py` & `skbase-0.4.6/skbase/base/_meta.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,871 +1,871 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-# BaseMetaObject and BaseMetaEstimator re-use code developed in scikit-learn and sktime.
-# These elements are copyrighted by the respective
-# scikit-learn developers (BSD-3-Clause License) and sktime (BSD-3-Clause) developers.
-# For conditions see licensing:
-# scikit-learn: https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
-# sktime:  https://github.com/sktime/sktime/blob/main/LICENSE
-"""Implements functionality for meta objects composed of other objects."""
-from inspect import isclass
-from typing import TYPE_CHECKING, Any, Dict, List, Sequence, Tuple, Union, overload
-
-from skbase.base._base import BaseEstimator, BaseObject
-from skbase.base._pretty_printing._object_html_repr import _VisualBlock
-from skbase.utils._iter import _format_seq_to_str, make_strings_unique
-from skbase.validate import is_named_object_tuple
-
-__author__: List[str] = ["mloning", "fkiraly", "RNKuhns"]
-__all__: List[str] = ["BaseMetaEstimator", "BaseMetaObject"]
-
-
-class _MetaObjectMixin:
-    """Parameter and tag management for objects composed of named objects.
-
-    Allows objects to get and set nested parameters when a parameter of the the
-    class has values that follow the named object specification. For example,
-    in a pipeline class with the the "step" parameter accepting named objects,
-    this would allow `get_params` and `set_params` to retrieve and update the
-    parameters of the objects in each step.
-
-    Notes
-    -----
-    Partly adapted from sklearn utils.metaestimator.py and sktime's
-    _HeterogenousMetaEstimator.
-    """
-
-    # for default get_params/set_params from _HeterogenousMetaEstimator
-    # _steps_attr points to the attribute of self
-    # which contains the heterogeneous set of estimators
-    # this must be an iterable of (name: str, estimator) pairs for the default
-    _tags = {"named_object_parameters": "steps"}
-
-    def is_composite(self) -> bool:
-        """Check if the object is composite.
-
-        A composite object is an object which contains objects as parameter values.
-
-        Returns
-        -------
-        bool
-            Whether self contains a parameter whose value is a BaseObject,
-            list of (str, BaseObject) tuples or dict[str, BaseObject].
-        """
-        # children of this class are always composite
-        return True
-
-    def get_params(self, deep: bool = True) -> Dict[str, Any]:
-        """Get a dict of parameters values for this object.
-
-        This expands on `get_params` of standard `BaseObject` by also retrieving
-        components parameters when ``deep=True`` a component's follows the named
-        object API (either sequence of str, BaseObject tuples or dict[str, BaseObject]).
-
-        Parameters
-        ----------
-        deep : bool, default=True
-            Whether to return parameters of components.
-
-            - If True, will return a dict of parameter name : value for this object,
-              including parameters of components.
-            - If False, will return a dict of parameter name : value for this object,
-              but not include parameters of components.
-
-        Returns
-        -------
-        dict[str, Any]
-            Dictionary of parameter name and value pairs. Includes direct parameters
-            and indirect parameters whose values implement `get_params` or follow
-            the named object API (either sequence of str, BaseObject tuples or
-            dict[str, BaseObject]).
-
-            - If ``deep=False`` the name-value pairs for this object's direct
-              parameters (you can see these via `get_param_names`) are returned.
-            - If ``deep=True`` then the parameter name-value pairs are returned
-              for direct and component (indirect) parameters.
-
-              - When a BaseObject's direct parameter value implements `get_params`
-                the component parameters are returned as
-                `[direct_param_name]__[component_param_name]` for 1st level components.
-                Arbitrary levels of component recursion are supported (if the
-                component has parameter's whose values are objects that implement
-                `get_params`). In this case, return parameters follow
-                `[direct_param_name]__[component_param_name]__[param_name]` format.
-              - When a BaseObject's direct parameter value is a sequence of
-                (name, BaseObject) tuples or dict[str, BaseObject] the parameters name
-                and value pairs of all component objects are returned. The
-                parameter naming follows ``scikit-learn`` convention of treating
-                named component objects like they are direct parameters; therefore,
-                the names are assigned as `[component_param_name]__[param_name]`.
-        """
-        # Use tag interface that will be available when mixin is used
-        named_object_attr = self.get_tag("named_object_parameters")  # type: ignore
-        return self._get_params(named_object_attr, deep=deep)
-
-    def set_params(self, **kwargs):
-        """Set the object's direct parameters and the parameters of components.
-
-        Valid parameter keys can be listed with ``get_params()``.
-
-        Like `BaseObject` implementation it allows values of indirect parameters
-        of a component to be set when a parameter's value is an object that
-        implements `set_params`. This also also expands the functionality to
-        allow parameter to allow the indirect parameters of components to be set
-        when a parameter's values follow the named object API (either sequence
-        of str, BaseObject tuples or dict[str, BaseObject]).
-
-        Returns
-        -------
-        Self
-            Instance of self.
-        """
-        # Use tag interface that will be available when mixin is used
-        named_object_attr = self.get_tag("named_object_parameters")  # type: ignore
-        return self._set_params(named_object_attr, **kwargs)
-
-    def _get_fitted_params(self):
-        """Get fitted parameters.
-
-        Method implements logic to retrieve fitted parameters. It is called from
-        get_fitted_params.
-
-        Returns
-        -------
-        dict[str, Any]
-            Fitted parameters where keys represent the parameters name (with
-            trailing "_" removed) and the corresponding value is the value of
-            the parameter learned during fit.
-        """
-        fitted_params = self._get_fitted_params_default()
-
-        fitted_named_object_attr = self.get_tag(
-            "fitted_named_object_parameters"
-        )  # type: ignore
-
-        named_objects_fitted_params = self._get_params(
-            fitted_named_object_attr, fitted=True
-        )
-
-        fitted_params.update(named_objects_fitted_params)
-
-        return fitted_params
-
-    def _get_params(
-        self, attr: str, deep: bool = True, fitted: bool = False
-    ) -> Dict[str, Any]:
-        """Logic for getting parameters on meta objects/estimators.
-
-        Separates out logic for parameter getting on meta objects from public API point.
-
-        Parameters
-        ----------
-        attr : str
-            Name of parameter whose values should contain named objects.
-        deep : bool, default=True
-            Whether to return parameters of components.
-
-            - If True, will return a dict of parameter name : value for this object,
-              including parameters of components.
-            - If False, will return a dict of parameter name : value for this object,
-              but not include parameters of components.
-
-        fitted : bool, default=False
-            Whether to retrieve the fitted params learned when `fit` is called on
-            ``estimator`` instead of the instances parameters.
-
-            - If False, then retrieve instance parameters like typical.
-            - If True, the retrieves the parameters learned during "fitting" and
-              stored in attributes ending in "_" (private attributes excluded).
-
-        Returns
-        -------
-        dict[str, Any]
-            Dictionary of parameter name and value pairs. Includes direct parameters
-            and indirect parameters whose values implement `get_params` or follow
-            the named object API (either sequence of str, BaseObject tuples or
-            dict[str, BaseObject]).
-        """
-        # Set variables that let us use same code for retrieving params or fitted params
-        if fitted:
-            method = "_get_fitted_params"
-            deepkw = {}
-        else:
-            method = "get_params"
-            deepkw = {"deep": deep}
-
-        # Get the direct params/fitted params
-        out = getattr(super(), method)(**deepkw)
-
-        if deep and hasattr(self, attr):
-            named_objects = getattr(self, attr)
-            named_objects_ = [
-                (x[0], x[1])
-                for x in self._coerce_to_named_object_tuples(
-                    named_objects, make_unique=False
-                )
-            ]
-            out.update(named_objects_)
-            for name, obj in named_objects_:
-                if hasattr(obj, method):
-                    for key, value in getattr(obj, method)(**deepkw).items():
-                        out["%s__%s" % (name, key)] = value
-        return out
-
-    def _set_params(self, attr: str, **params):
-        """Logic for setting parameters on meta objects/estimators.
-
-        Separates out logic for parameter setting on meta objects from public API point.
-
-        Parameters
-        ----------
-        attr : str
-            Name of parameter whose values should contain named objects.
-
-        Returns
-        -------
-        Self
-            Instance of self.
-        """
-        # Ensure strict ordering of parameter setting:
-        # 1. All steps
-        if attr in params:
-            setattr(self, attr, params.pop(attr))
-        # 2. Step replacement
-        items = getattr(self, attr)
-        names = []
-        if items:
-            names, _ = zip(*items)
-        for name in list(params.keys()):
-            if "__" not in name and name in names:
-                self._replace_object(attr, name, params.pop(name))
-        # 3. Step parameters and other initialisation arguments
-        super().set_params(**params)  # type: ignore
-        return self
-
-    def _replace_object(self, attr: str, name: str, new_val: Any) -> None:
-        """Replace an object in attribute that contains named objects."""
-        # assumes `name` is a valid object name
-        new_objects = list(getattr(self, attr))
-        for i, (object_name, _) in enumerate(new_objects):
-            if object_name == name:
-                new_objects[i] = (name, new_val)
-                break
-        setattr(self, attr, new_objects)
-
-    @overload
-    def _check_names(self, names: List[str], make_unique: bool = True) -> List[str]:
-        ...  # pragma: no cover
-
-    @overload
-    def _check_names(
-        self, names: Tuple[str, ...], make_unique: bool = True
-    ) -> Tuple[str, ...]:
-        ...  # pragma: no cover
-
-    def _check_names(
-        self, names: Union[List[str], Tuple[str, ...]], make_unique: bool = True
-    ) -> Union[List[str], Tuple[str, ...]]:
-        """Validate that names of named objects follow API rules.
-
-        The names for named objects should:
-
-        - Be unique,
-        - Not be the name of one of the object's direct parameters,
-        - Not contain "__" (which is reserved to denote components in get/set params).
-
-        Parameters
-        ----------
-        names : list[str] | tuple[str]
-            The sequence of names from named objects.
-        make_unique : bool, default=True
-            Whether to coerce names to unique strings if they are not.
-
-        Returns
-        -------
-        list[str] | tuple[str]
-            A sequence of unique string names that follow named object API rules.
-        """
-        if len(set(names)) != len(names):
-            raise ValueError("Names provided are not unique: {0!r}".format(list(names)))
-        # Get names that match direct parameter
-        invalid_names = set(names).intersection(self.get_params(deep=False))
-        invalid_names = invalid_names.union({name for name in names if "__" in name})
-        if invalid_names:
-            raise ValueError(
-                "Object names conflict with constructor argument or "
-                "contain '__': {0!r}".format(sorted(invalid_names))
-            )
-        if make_unique:
-            names = make_strings_unique(names)
-
-        return names
-
-    def _coerce_object_tuple(
-        self,
-        obj: Union[BaseObject, Tuple[str, BaseObject]],
-        clone: bool = False,
-    ) -> Tuple[str, BaseObject]:
-        """Coerce object or (str, BaseObject) tuple to (str, BaseObject) tuple.
-
-        Used to make sure input will work with expected named object tuple API format.
-
-        Parameters
-        ----------
-        objs : BaseObject or (str, BaseObject) tuple
-            Assumes that this has been checked, no checks are performed.
-        clone : bool, default = False.
-            Whether to return clone of estimator in obj (True) or a reference (False).
-
-        Returns
-        -------
-        tuple[str, BaseObject]
-            Named object tuple.
-
-            - If `obj` was an object then returns (obj.__class__.__name__, obj).
-            - If `obj` was aleady a (name, object) tuple it is returned (a copy
-              is returned if ``clone=True``).
-        """
-        if isinstance(obj, tuple) and len(obj) >= 2:
-            _obj = obj[1]
-            name = obj[0]
-
-        else:
-            if isinstance(obj, tuple) and len(obj) == 1:
-                _obj = obj[0]
-            else:
-                _obj = obj
-            name = type(_obj).__name__
-
-        if clone:
-            _obj = _obj.clone()
-        return (name, _obj)
-
-    def _check_objects(
-        self,
-        objs: Any,
-        attr_name: str = "steps",
-        cls_type: Union[type, Tuple[type, ...]] = None,
-        allow_dict: bool = False,
-        allow_mix: bool = True,
-        clone: bool = True,
-    ) -> List[Tuple[str, BaseObject]]:
-        """Check that objects is a list of objects or sequence of named objects.
-
-        Parameters
-        ----------
-        objs : Any
-            Should be list of objects, a list of (str, object) tuples or a
-            dict[str, objects]. Any objects should `cls_type` class.
-        attr_name : str, default="steps"
-            Name of checked attribute in error messages.
-        cls_type : class or tuple of classes, default=BaseEstimator.
-            class(es) that all objects are checked to be an instance of.
-        allow_mix : bool, default=True
-            Whether mix of objects and (str, objects) is allowed in `objs.`
-        clone : bool, default=True
-            Whether objects or named objects in `objs` are returned as clones
-            (True) or references (False).
-
-        Returns
-        -------
-        list[tuple[str, BaseObject]]
-            List of tuples following named object API.
-
-            - If `objs` was already a list of (str, object) tuples then either the
-              same named objects (as with other cases cloned versions are
-              returned if ``clone=True``).
-            - If `objs` was a dict[str, object] then the named objects are unpacked
-              into a list of (str, object) tuples.
-            - If `objs` was a list of objects then string names were generated based
-               on the object's class names (with coercion to unique strings if
-               necessary).
-
-        Raises
-        ------
-        TypeError
-            If `objs` is not a list of (str, object) tuples or a dict[str, objects].
-            Also raised if objects in `objs` are not instances of `cls_type`
-            or `cls_type is not None, a class or tuple of classes.
-        """
-        msg = (
-            f"Invalid {attr_name!r} attribute, {attr_name!r} should be a list "
-            "of objects, or a list of (string, object) tuples. "
-        )
-
-        if cls_type is None:
-            cls_type = BaseObject
-            _class_name = "BaseObject"
-        elif isclass(cls_type):
-            _class_name = cls_type.__name__  # type: ignore
-        elif isinstance(cls_type, tuple) and all(isclass(c) for c in cls_type):
-            _class_name = _format_seq_to_str(
-                [c.__name__ for c in cls_type], last_sep="or"
-            )
-        else:
-            raise TypeError("`cls_type` must be a class or tuple of classes.")
-
-        msg += f"All objects in {attr_name!r} must be of type {_class_name}"
-
-        if (
-            objs is None
-            or len(objs) == 0
-            or not (isinstance(objs, list) or (allow_dict and isinstance(objs, dict)))
-        ):
-            raise TypeError(msg)
-
-        def is_obj_is_tuple(obj):
-            """Check whether obj is estimator of right type, or (str, est) tuple."""
-            is_est = isinstance(obj, cls_type)
-            is_tuple = is_named_object_tuple(obj, object_type=cls_type)
-
-            return is_est, is_tuple
-
-        # We've already guarded against objs being dict when allow_dict is False
-        # So here we can just check dictionary elements
-        if isinstance(objs, dict) and not all(
-            isinstance(name, str) and isinstance(obj, cls_type)
-            for name, obj in objs.items()
-        ):
-            raise TypeError(msg)
-
-        elif not all(any(is_obj_is_tuple(x)) for x in objs):
-            raise TypeError(msg)
-
-        msg_no_mix = (
-            f"Elements of {attr_name} must either all be objects, "
-            f"or all (str, objects) tuples. A mix of the two is not allowed."
-        )
-        if not allow_mix and not all(is_obj_is_tuple(x)[0] for x in objs):
-            if not all(is_obj_is_tuple(x)[1] for x in objs):
-                raise TypeError(msg_no_mix)
-
-        return self._coerce_to_named_object_tuples(objs, clone=clone, make_unique=True)
-
-    def _get_names_and_objects(
-        self,
-        named_objects: Union[
-            Sequence[Union[BaseObject, Tuple[str, BaseObject]]], Dict[str, BaseObject]
-        ],
-        make_unique: bool = False,
-    ) -> Tuple[List[str], List[BaseObject]]:
-        """Return lists of names and object from input that follows named object API.
-
-        Handles input that is dictionary mapping str names of object instances or
-        input that is a list of (str, object) tuples.
-
-        Parameters
-        ----------
-        named_objects : list[tuple[str, object], ...], list[object], dict[str, object]
-            The objects whose names should be returned.
-        make_unique : bool, default=False
-            Whether names should be made unique.
-
-        Returns
-        -------
-        names : list[str]
-            Lists of the names and objects that were input.
-        objs : list[BaseObject]
-            The
-        """
-        names: Tuple[str, ...]
-        objs: Tuple[BaseObject, ...]
-        if isinstance(named_objects, dict):
-            names, objs = zip(*named_objects.items())
-        else:
-            names, objs = zip(*[self._coerce_object_tuple(x) for x in named_objects])
-
-        # Optionally make names unique
-        if make_unique:
-            names = make_strings_unique(names)
-        return list(names), list(objs)
-
-    def _coerce_to_named_object_tuples(
-        self,
-        objs: Union[
-            Sequence[Union[BaseObject, Tuple[str, BaseObject]]], Dict[str, BaseObject]
-        ],
-        clone: bool = False,
-        make_unique: bool = True,
-    ) -> List[Tuple[str, BaseObject]]:
-        """Coerce sequence of objects or named objects to list of (str, obj) tuples.
-
-        Input that is sequence of objects, list of (str, obj) tuples or
-        dict[str, object] will be coerced to list of (str, obj) tuples on return.
-
-        Parameters
-        ----------
-        objs : list of objects, list of (str, object tuples) or dict[str, object]
-            The input should be coerced to list of (str, object) tuples. Should
-            be a sequence of objects, or follow named object API.
-        clone : bool, default=False.
-            Whether objects in the returned list of (str, object) tuples are
-            cloned (True) or references (False).
-        make_unique : bool, default=True
-            Whether the str names in the returned list of (str, object) tuples
-            should be coerced to unique str values (if str names in input
-            are already unique they will not be changed).
-
-        Returns
-        -------
-        list[tuple[str, BaseObject]]
-            List of tuples following named object API.
-
-            - If `objs` was already a list of (str, object) tuples then either the
-              same named objects (as with other cases cloned versions are
-              returned if ``clone=True``).
-            - If `objs` was a dict[str, object] then the named objects are unpacked
-              into a list of (str, object) tuples.
-            - If `objs` was a list of objects then string names were generated based
-               on the object's class names (with coercion to unique strings if
-               necessary).
-        """
-        if isinstance(objs, dict):
-            named_objects = [(k, v) for k, v in objs.items()]
-        else:
-            # Otherwise get named object format
-            if TYPE_CHECKING:
-                assert not isinstance(objs, dict)  # nosec: B1010
-            named_objects = [
-                self._coerce_object_tuple(obj, clone=clone) for obj in objs
-            ]
-        if make_unique:
-            # Unpack names and objects while making names unique
-            names, objs = self._get_names_and_objects(
-                named_objects, make_unique=make_unique
-            )
-            # Repack the objects
-            named_objects = list(zip(names, objs))
-        return named_objects
-
-    def _dunder_concat(
-        self,
-        other,
-        base_class,
-        composite_class,
-        attr_name="steps",
-        concat_order="left",
-        composite_params=None,
-    ):
-        """Logic to concatenate pipelines for dunder parsing.
-
-        This is useful in concrete heterogeneous meta-objects that implement
-        dunders for easy concatenation of pipeline-like composites.
-
-        Parameters
-        ----------
-        other : BaseObject subclass
-            An object inheritting from `composite_class` or `base_class`, otherwise
-            `NotImplemented` is returned.
-        base_class : BaseObject subclass
-            Class assumed as base class for self and `other`. ,
-            and estimator components of composite_class, in case of concatenation
-        composite_class : BaseMetaObject or BaseMetaEstimator subclass
-            Class that has parameter `attr_name` stored in attribute of same name
-            that contains list of base_class objects, list of (str, base_class)
-            tuples, or a mixture thereof.
-        attr_name : str, default="steps"
-            Name of the attribute that contains base_class objects,
-            list of (str, base_class) tuples. Concatenation is done for this attribute.
-        concat_order : {"left", "right"}, default="left"
-            Specifies ordering for concatenation.
-
-            - If "left", resulting attr_name will be like
-              self.attr_name + other.attr_name.
-            - If "right", resulting attr_name will be like
-              other.attr_name + self.attr_name.
-
-        composite_params : dict, default=None
-            Parameters of the composite are always set accordingly
-            i.e., contains key-value pairs, and composite_class has key set to value.
-
-        Returns
-        -------
-        BaseMetaObject or BaseMetaEstimator
-            Instance of `composite_class`, where `attr_name` is set so that self and
-            other are "concatenated".
-
-            - If other is instance of `composite_class` then instance of
-              `composite_class`, where `attr_name` is a concatenation of
-              ``self.attr_name`` and ``other.attr_name``.
-            - If `other` is instance of `base_class`, then instance of `composite_class`
-              is returned where `attr_name` is set so that so that
-              composite_class(attr_name=other) is returned.
-            - If str are all the class names of est, list of est only is used instead
-        """
-        # Validate input
-        if concat_order not in ["left", "right"]:
-            raise ValueError(
-                f"`concat_order` must be 'left' or 'right', but found {concat_order!r}."
-            )
-        if not isinstance(attr_name, str):
-            raise TypeError(f"`attr_name` must be str, but found {type(attr_name)}.")
-        if not isclass(composite_class):
-            raise TypeError("`composite_class` must be a class.")
-        if not isclass(base_class):
-            raise TypeError("`base_class` must be a class.")
-        if not issubclass(composite_class, base_class):
-            raise ValueError("`composite_class` must be a subclass of base_class.")
-        if not isinstance(self, composite_class):
-            raise TypeError("self must be an instance of `composite_class`.")
-
-        def concat(x, y):
-            if concat_order == "left":
-                return x + y
-            else:
-                return y + x
-
-        # get attr_name from self and other
-        # can be list of ests, list of (str, est) tuples, or list of mixture of these
-        self_attr = getattr(self, attr_name)
-
-        # from that, obtain ests, and original names (may be non-unique)
-        # we avoid _make_strings_unique call too early to avoid blow-up of string
-        self_names, self_objs = self._get_names_and_objects(self_attr)
-        if isinstance(other, composite_class):
-            other_attr = getattr(other, attr_name)
-            other_names, other_objs = other._get_names_and_objects(other_attr)
-        elif isinstance(other, base_class):
-            other_names = [type(other).__name__]
-            other_objs = [other]
-        elif is_named_object_tuple(other, object_type=base_class):
-            other_names = [other[0]]
-            other_objs = [other[1]]
-        else:
-            return NotImplemented
-
-        new_names = concat(self_names, other_names)
-        new_objs = concat(self_objs, other_objs)
-        # create the "steps" param for the composite
-        # if all the names are equal to class names, we eat them away
-        if all(type(x[1]).__name__ == x[0] for x in zip(new_names, new_objs)):
-            step_param = {attr_name: list(new_objs)}
-        else:
-            step_param = {attr_name: list(zip(new_names, new_objs))}
-
-        # retrieve other parameters, from composite_params attribute
-        if composite_params is None:
-            composite_params = {}
-        else:
-            composite_params = composite_params.copy()
-
-        # construct the composite with both step and additional params
-        composite_params.update(step_param)
-        return composite_class(**composite_params)
-
-    def _sk_visual_block_(self):
-        """Logic to help render meta estimator as visual HTML block."""
-        # Use tag interface that will be available when mixin is used
-        named_object_attr_name = self.get_tag("named_object_parameters")  # type: ignore
-        named_object_attr = getattr(self, named_object_attr_name)
-        named_objects = self._coerce_to_named_object_tuples(named_object_attr)
-        _, objs = self._get_names_and_objects(named_objects)
-
-        def _get_name(name, obj):
-            if obj is None or obj == "passthrough":
-                return f"{name}: passthrough"
-            # Is an estimator
-            return f"{name}: {obj.__class__.__name__}"
-
-        names = [_get_name(name, est) for name, est in named_objects]
-        name_details = [str(obj) for obj in objs]
-        return _VisualBlock(
-            "serial",
-            objs,
-            names=names,
-            name_details=name_details,
-            dash_wrapped=False,
-        )
-
-
-class _MetaTagLogicMixin:
-    """Mixin for tag conjunction, disjunction, chain operations for meta-objects.
-
-    Contains methods to set tags of a meta-object dependent on component objects.
-    """
-
-    def _anytagis(self, tag_name, value, estimators):
-        """Return whether any estimator in list has tag `tag_name` of value `value`.
-
-        Parameters
-        ----------
-        tag_name : str, name of the tag to check
-        value : value of the tag to check for
-        estimators : list of (str, estimator) pairs to query for the tag/value
-
-        Return
-        ------
-        bool : True iff at least one estimator in the list has value in tag tag_name
-        """
-        tagis = [est.get_tag(tag_name, value) == value for _, est in estimators]
-        return any(tagis)
-
-    def _anytagis_then_set(self, tag_name, value, value_if_not, estimators):
-        """Set self's `tag_name` tag to `value` if any estimator on the list has it.
-
-        Writes to self:
-        sets the tag `tag_name` to `value` if `_anytagis(tag_name, value)` is True
-            otherwise sets the tag `tag_name` to `value_if_not`
-
-        Parameters
-        ----------
-        tag_name : str, name of the tag
-        value : value to check and to set tag to if one of the tag values is `value`
-        value_if_not : value to set in self if none of the tag values is `value`
-        estimators : list of (str, estimator) pairs to query for the tag/value
-        """
-        if self._anytagis(tag_name=tag_name, value=value, estimators=estimators):
-            self.set_tags(**{tag_name: value})
-        else:
-            self.set_tags(**{tag_name: value_if_not})
-
-    def _anytag_notnone_val(self, tag_name, estimators):
-        """Return first non-'None' value of tag `tag_name` in estimator list.
-
-        Parameters
-        ----------
-        tag_name : str, name of the tag
-        estimators : list of (str, estimator) pairs to query for the tag/value
-
-        Return
-        ------
-        tag_val : first non-'None' value of tag `tag_name` in estimator list.
-        """
-        for _, est in estimators:
-            tag_val = est.get_tag(tag_name)
-            if tag_val != "None":
-                return tag_val
-        return tag_val
-
-    def _anytag_notnone_set(self, tag_name, estimators):
-        """Set self's `tag_name` tag to first non-'None' value in estimator list.
-
-        Writes to self:
-        tag with name tag_name, sets to _anytag_notnone_val(tag_name, estimators)
-
-        Parameters
-        ----------
-        tag_name : str, name of the tag
-        estimators : list of (str, estimator) pairs to query for the tag/value
-        """
-        tag_val = self._anytag_notnone_val(tag_name=tag_name, estimators=estimators)
-        if tag_val != "None":
-            self.set_tags(**{tag_name: tag_val})
-
-    def _tagchain_is_linked(
-        self,
-        left_tag_name,
-        mid_tag_name,
-        estimators,
-        left_tag_val=True,
-        mid_tag_val=True,
-    ):
-        """Check whether all tags left of the first mid_tag/val are left_tag/val.
-
-        Useful to check, for instance, whether all instances of estimators
-            left of the first missing value imputer can deal with missing values.
-
-        Parameters
-        ----------
-        left_tag_name : str, name of the left tag
-        mid_tag_name : str, name of the middle tag
-        estimators : list of (str, estimator) pairs to query for the tag/value
-        left_tag_val : value of the left tag, optional, default=True
-        mid_tag_val : value of the middle tag, optional, default=True
-
-        Returns
-        -------
-        chain_is_linked : bool,
-            True iff all "left" tag instances `left_tag_name` have value `left_tag_val`
-            a "left" tag instance is an instance in estimators which is earlier
-            than the first occurrence of `mid_tag_name` with value `mid_tag_val`
-        chain_is_complete : bool,
-            True iff chain_is_linked is True, and
-                there is an occurrence of `mid_tag_name` with value `mid_tag_val`
-        """
-        for _, est in estimators:
-            if est.get_tag(mid_tag_name) == mid_tag_val:
-                return True, True
-            if not est.get_tag(left_tag_name) == left_tag_val:
-                return False, False
-        return True, False
-
-    def _tagchain_is_linked_set(
-        self,
-        left_tag_name,
-        mid_tag_name,
-        estimators,
-        left_tag_val=True,
-        mid_tag_val=True,
-        left_tag_val_not=False,
-        mid_tag_val_not=False,
-    ):
-        """Check if _tagchain_is_linked, then set self left_tag_name and mid_tag_name.
-
-        Writes to self:
-        tag with name left_tag_name, sets to left_tag_val if _tag_chain_is_linked[0]
-            otherwise sets to left_tag_val_not
-        tag with name mid_tag_name, sets to mid_tag_val if _tag_chain_is_linked[1]
-            otherwise sets to mid_tag_val_not
-
-        Parameters
-        ----------
-        left_tag_name : str, name of the left tag
-        mid_tag_name : str, name of the middle tag
-        estimators : list of (str, estimator) pairs to query for the tag/value
-        left_tag_val : value of the left tag, optional, default=True
-        mid_tag_val : value of the middle tag, optional, default=True
-        left_tag_val_not : value to set if not linked, optional, default=False
-        mid_tag_val_not : value to set if not linked, optional, default=False
-        """
-        linked, complete = self._tagchain_is_linked(
-            left_tag_name=left_tag_name,
-            mid_tag_name=mid_tag_name,
-            estimators=estimators,
-            left_tag_val=left_tag_val,
-            mid_tag_val=mid_tag_val,
-        )
-        if linked:
-            self.set_tags(**{left_tag_name: left_tag_val})
-        else:
-            self.set_tags(**{left_tag_name: left_tag_val_not})
-        if complete:
-            self.set_tags(**{mid_tag_name: mid_tag_val})
-        else:
-            self.set_tags(**{mid_tag_name: mid_tag_val_not})
-
-
-class BaseMetaObject(_MetaObjectMixin, _MetaTagLogicMixin, BaseObject):
-    """Parameter and tag management for objects composed of named objects.
-
-    Allows objects to get and set nested parameters when a parameter of the the
-    class has values that follow the named object specification. For example,
-    in a pipeline class with the the "step" parameter accepting named objects,
-    this would allow `get_params` and `set_params` to retrieve and update the
-    parameters of the objects in each step.
-
-    See Also
-    --------
-    BaseMetaEstimator :
-        Expands on `BaseMetaObject` by adding functionality for getting fitted
-        parameters from a class's component estimators. `BaseEstimator` should
-        be used when you want to create a meta estimator.
-    """
-
-
-class BaseMetaEstimator(_MetaObjectMixin, _MetaTagLogicMixin, BaseEstimator):
-    """Parameter and tag management for estimators composed of named objects.
-
-    Allows estimators to get and set nested parameters when a parameter of the the
-    class has values that follow the named object specification. For example,
-    in a pipeline class with the the "step" parameter accepting named objects,
-    this would allow `get_params` and `set_params` to retrieve and update the
-    parameters of the objects in each step.
-
-    See Also
-    --------
-    BaseMetaObject :
-        Provides similar functionality to  `BaseMetaEstimator` for getting
-        parameters from a class's component objects, but does not have the
-        estimator interface.
-    """
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+# BaseMetaObject and BaseMetaEstimator re-use code developed in scikit-learn and sktime.
+# These elements are copyrighted by the respective
+# scikit-learn developers (BSD-3-Clause License) and sktime (BSD-3-Clause) developers.
+# For conditions see licensing:
+# scikit-learn: https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
+# sktime:  https://github.com/sktime/sktime/blob/main/LICENSE
+"""Implements functionality for meta objects composed of other objects."""
+from inspect import isclass
+from typing import TYPE_CHECKING, Any, Dict, List, Sequence, Tuple, Union, overload
+
+from skbase.base._base import BaseEstimator, BaseObject
+from skbase.base._pretty_printing._object_html_repr import _VisualBlock
+from skbase.utils._iter import _format_seq_to_str, make_strings_unique
+from skbase.validate import is_named_object_tuple
+
+__author__: List[str] = ["mloning", "fkiraly", "RNKuhns"]
+__all__: List[str] = ["BaseMetaEstimator", "BaseMetaObject"]
+
+
+class _MetaObjectMixin:
+    """Parameter and tag management for objects composed of named objects.
+
+    Allows objects to get and set nested parameters when a parameter of the the
+    class has values that follow the named object specification. For example,
+    in a pipeline class with the the "step" parameter accepting named objects,
+    this would allow `get_params` and `set_params` to retrieve and update the
+    parameters of the objects in each step.
+
+    Notes
+    -----
+    Partly adapted from sklearn utils.metaestimator.py and sktime's
+    _HeterogenousMetaEstimator.
+    """
+
+    # for default get_params/set_params from _HeterogenousMetaEstimator
+    # _steps_attr points to the attribute of self
+    # which contains the heterogeneous set of estimators
+    # this must be an iterable of (name: str, estimator) pairs for the default
+    _tags = {"named_object_parameters": "steps"}
+
+    def is_composite(self) -> bool:
+        """Check if the object is composite.
+
+        A composite object is an object which contains objects as parameter values.
+
+        Returns
+        -------
+        bool
+            Whether self contains a parameter whose value is a BaseObject,
+            list of (str, BaseObject) tuples or dict[str, BaseObject].
+        """
+        # children of this class are always composite
+        return True
+
+    def get_params(self, deep: bool = True) -> Dict[str, Any]:
+        """Get a dict of parameters values for this object.
+
+        This expands on `get_params` of standard `BaseObject` by also retrieving
+        components parameters when ``deep=True`` a component's follows the named
+        object API (either sequence of str, BaseObject tuples or dict[str, BaseObject]).
+
+        Parameters
+        ----------
+        deep : bool, default=True
+            Whether to return parameters of components.
+
+            - If True, will return a dict of parameter name : value for this object,
+              including parameters of components.
+            - If False, will return a dict of parameter name : value for this object,
+              but not include parameters of components.
+
+        Returns
+        -------
+        dict[str, Any]
+            Dictionary of parameter name and value pairs. Includes direct parameters
+            and indirect parameters whose values implement `get_params` or follow
+            the named object API (either sequence of str, BaseObject tuples or
+            dict[str, BaseObject]).
+
+            - If ``deep=False`` the name-value pairs for this object's direct
+              parameters (you can see these via `get_param_names`) are returned.
+            - If ``deep=True`` then the parameter name-value pairs are returned
+              for direct and component (indirect) parameters.
+
+              - When a BaseObject's direct parameter value implements `get_params`
+                the component parameters are returned as
+                `[direct_param_name]__[component_param_name]` for 1st level components.
+                Arbitrary levels of component recursion are supported (if the
+                component has parameter's whose values are objects that implement
+                `get_params`). In this case, return parameters follow
+                `[direct_param_name]__[component_param_name]__[param_name]` format.
+              - When a BaseObject's direct parameter value is a sequence of
+                (name, BaseObject) tuples or dict[str, BaseObject] the parameters name
+                and value pairs of all component objects are returned. The
+                parameter naming follows ``scikit-learn`` convention of treating
+                named component objects like they are direct parameters; therefore,
+                the names are assigned as `[component_param_name]__[param_name]`.
+        """
+        # Use tag interface that will be available when mixin is used
+        named_object_attr = self.get_tag("named_object_parameters")  # type: ignore
+        return self._get_params(named_object_attr, deep=deep)
+
+    def set_params(self, **kwargs):
+        """Set the object's direct parameters and the parameters of components.
+
+        Valid parameter keys can be listed with ``get_params()``.
+
+        Like `BaseObject` implementation it allows values of indirect parameters
+        of a component to be set when a parameter's value is an object that
+        implements `set_params`. This also also expands the functionality to
+        allow parameter to allow the indirect parameters of components to be set
+        when a parameter's values follow the named object API (either sequence
+        of str, BaseObject tuples or dict[str, BaseObject]).
+
+        Returns
+        -------
+        Self
+            Instance of self.
+        """
+        # Use tag interface that will be available when mixin is used
+        named_object_attr = self.get_tag("named_object_parameters")  # type: ignore
+        return self._set_params(named_object_attr, **kwargs)
+
+    def _get_fitted_params(self):
+        """Get fitted parameters.
+
+        Method implements logic to retrieve fitted parameters. It is called from
+        get_fitted_params.
+
+        Returns
+        -------
+        dict[str, Any]
+            Fitted parameters where keys represent the parameters name (with
+            trailing "_" removed) and the corresponding value is the value of
+            the parameter learned during fit.
+        """
+        fitted_params = self._get_fitted_params_default()
+
+        fitted_named_object_attr = self.get_tag(
+            "fitted_named_object_parameters"
+        )  # type: ignore
+
+        named_objects_fitted_params = self._get_params(
+            fitted_named_object_attr, fitted=True
+        )
+
+        fitted_params.update(named_objects_fitted_params)
+
+        return fitted_params
+
+    def _get_params(
+        self, attr: str, deep: bool = True, fitted: bool = False
+    ) -> Dict[str, Any]:
+        """Logic for getting parameters on meta objects/estimators.
+
+        Separates out logic for parameter getting on meta objects from public API point.
+
+        Parameters
+        ----------
+        attr : str
+            Name of parameter whose values should contain named objects.
+        deep : bool, default=True
+            Whether to return parameters of components.
+
+            - If True, will return a dict of parameter name : value for this object,
+              including parameters of components.
+            - If False, will return a dict of parameter name : value for this object,
+              but not include parameters of components.
+
+        fitted : bool, default=False
+            Whether to retrieve the fitted params learned when `fit` is called on
+            ``estimator`` instead of the instances parameters.
+
+            - If False, then retrieve instance parameters like typical.
+            - If True, the retrieves the parameters learned during "fitting" and
+              stored in attributes ending in "_" (private attributes excluded).
+
+        Returns
+        -------
+        dict[str, Any]
+            Dictionary of parameter name and value pairs. Includes direct parameters
+            and indirect parameters whose values implement `get_params` or follow
+            the named object API (either sequence of str, BaseObject tuples or
+            dict[str, BaseObject]).
+        """
+        # Set variables that let us use same code for retrieving params or fitted params
+        if fitted:
+            method = "_get_fitted_params"
+            deepkw = {}
+        else:
+            method = "get_params"
+            deepkw = {"deep": deep}
+
+        # Get the direct params/fitted params
+        out = getattr(super(), method)(**deepkw)
+
+        if deep and hasattr(self, attr):
+            named_objects = getattr(self, attr)
+            named_objects_ = [
+                (x[0], x[1])
+                for x in self._coerce_to_named_object_tuples(
+                    named_objects, make_unique=False
+                )
+            ]
+            out.update(named_objects_)
+            for name, obj in named_objects_:
+                if hasattr(obj, method):
+                    for key, value in getattr(obj, method)(**deepkw).items():
+                        out["%s__%s" % (name, key)] = value
+        return out
+
+    def _set_params(self, attr: str, **params):
+        """Logic for setting parameters on meta objects/estimators.
+
+        Separates out logic for parameter setting on meta objects from public API point.
+
+        Parameters
+        ----------
+        attr : str
+            Name of parameter whose values should contain named objects.
+
+        Returns
+        -------
+        Self
+            Instance of self.
+        """
+        # Ensure strict ordering of parameter setting:
+        # 1. All steps
+        if attr in params:
+            setattr(self, attr, params.pop(attr))
+        # 2. Step replacement
+        items = getattr(self, attr)
+        names = []
+        if items:
+            names, _ = zip(*items)
+        for name in list(params.keys()):
+            if "__" not in name and name in names:
+                self._replace_object(attr, name, params.pop(name))
+        # 3. Step parameters and other initialisation arguments
+        super().set_params(**params)  # type: ignore
+        return self
+
+    def _replace_object(self, attr: str, name: str, new_val: Any) -> None:
+        """Replace an object in attribute that contains named objects."""
+        # assumes `name` is a valid object name
+        new_objects = list(getattr(self, attr))
+        for i, (object_name, _) in enumerate(new_objects):
+            if object_name == name:
+                new_objects[i] = (name, new_val)
+                break
+        setattr(self, attr, new_objects)
+
+    @overload
+    def _check_names(self, names: List[str], make_unique: bool = True) -> List[str]:
+        ...  # pragma: no cover
+
+    @overload
+    def _check_names(
+        self, names: Tuple[str, ...], make_unique: bool = True
+    ) -> Tuple[str, ...]:
+        ...  # pragma: no cover
+
+    def _check_names(
+        self, names: Union[List[str], Tuple[str, ...]], make_unique: bool = True
+    ) -> Union[List[str], Tuple[str, ...]]:
+        """Validate that names of named objects follow API rules.
+
+        The names for named objects should:
+
+        - Be unique,
+        - Not be the name of one of the object's direct parameters,
+        - Not contain "__" (which is reserved to denote components in get/set params).
+
+        Parameters
+        ----------
+        names : list[str] | tuple[str]
+            The sequence of names from named objects.
+        make_unique : bool, default=True
+            Whether to coerce names to unique strings if they are not.
+
+        Returns
+        -------
+        list[str] | tuple[str]
+            A sequence of unique string names that follow named object API rules.
+        """
+        if len(set(names)) != len(names):
+            raise ValueError("Names provided are not unique: {0!r}".format(list(names)))
+        # Get names that match direct parameter
+        invalid_names = set(names).intersection(self.get_params(deep=False))
+        invalid_names = invalid_names.union({name for name in names if "__" in name})
+        if invalid_names:
+            raise ValueError(
+                "Object names conflict with constructor argument or "
+                "contain '__': {0!r}".format(sorted(invalid_names))
+            )
+        if make_unique:
+            names = make_strings_unique(names)
+
+        return names
+
+    def _coerce_object_tuple(
+        self,
+        obj: Union[BaseObject, Tuple[str, BaseObject]],
+        clone: bool = False,
+    ) -> Tuple[str, BaseObject]:
+        """Coerce object or (str, BaseObject) tuple to (str, BaseObject) tuple.
+
+        Used to make sure input will work with expected named object tuple API format.
+
+        Parameters
+        ----------
+        objs : BaseObject or (str, BaseObject) tuple
+            Assumes that this has been checked, no checks are performed.
+        clone : bool, default = False.
+            Whether to return clone of estimator in obj (True) or a reference (False).
+
+        Returns
+        -------
+        tuple[str, BaseObject]
+            Named object tuple.
+
+            - If `obj` was an object then returns (obj.__class__.__name__, obj).
+            - If `obj` was aleady a (name, object) tuple it is returned (a copy
+              is returned if ``clone=True``).
+        """
+        if isinstance(obj, tuple) and len(obj) >= 2:
+            _obj = obj[1]
+            name = obj[0]
+
+        else:
+            if isinstance(obj, tuple) and len(obj) == 1:
+                _obj = obj[0]
+            else:
+                _obj = obj
+            name = type(_obj).__name__
+
+        if clone:
+            _obj = _obj.clone()
+        return (name, _obj)
+
+    def _check_objects(
+        self,
+        objs: Any,
+        attr_name: str = "steps",
+        cls_type: Union[type, Tuple[type, ...]] = None,
+        allow_dict: bool = False,
+        allow_mix: bool = True,
+        clone: bool = True,
+    ) -> List[Tuple[str, BaseObject]]:
+        """Check that objects is a list of objects or sequence of named objects.
+
+        Parameters
+        ----------
+        objs : Any
+            Should be list of objects, a list of (str, object) tuples or a
+            dict[str, objects]. Any objects should `cls_type` class.
+        attr_name : str, default="steps"
+            Name of checked attribute in error messages.
+        cls_type : class or tuple of classes, default=BaseEstimator.
+            class(es) that all objects are checked to be an instance of.
+        allow_mix : bool, default=True
+            Whether mix of objects and (str, objects) is allowed in `objs.`
+        clone : bool, default=True
+            Whether objects or named objects in `objs` are returned as clones
+            (True) or references (False).
+
+        Returns
+        -------
+        list[tuple[str, BaseObject]]
+            List of tuples following named object API.
+
+            - If `objs` was already a list of (str, object) tuples then either the
+              same named objects (as with other cases cloned versions are
+              returned if ``clone=True``).
+            - If `objs` was a dict[str, object] then the named objects are unpacked
+              into a list of (str, object) tuples.
+            - If `objs` was a list of objects then string names were generated based
+               on the object's class names (with coercion to unique strings if
+               necessary).
+
+        Raises
+        ------
+        TypeError
+            If `objs` is not a list of (str, object) tuples or a dict[str, objects].
+            Also raised if objects in `objs` are not instances of `cls_type`
+            or `cls_type is not None, a class or tuple of classes.
+        """
+        msg = (
+            f"Invalid {attr_name!r} attribute, {attr_name!r} should be a list "
+            "of objects, or a list of (string, object) tuples. "
+        )
+
+        if cls_type is None:
+            cls_type = BaseObject
+            _class_name = "BaseObject"
+        elif isclass(cls_type):
+            _class_name = cls_type.__name__  # type: ignore
+        elif isinstance(cls_type, tuple) and all(isclass(c) for c in cls_type):
+            _class_name = _format_seq_to_str(
+                [c.__name__ for c in cls_type], last_sep="or"
+            )
+        else:
+            raise TypeError("`cls_type` must be a class or tuple of classes.")
+
+        msg += f"All objects in {attr_name!r} must be of type {_class_name}"
+
+        if (
+            objs is None
+            or len(objs) == 0
+            or not (isinstance(objs, list) or (allow_dict and isinstance(objs, dict)))
+        ):
+            raise TypeError(msg)
+
+        def is_obj_is_tuple(obj):
+            """Check whether obj is estimator of right type, or (str, est) tuple."""
+            is_est = isinstance(obj, cls_type)
+            is_tuple = is_named_object_tuple(obj, object_type=cls_type)
+
+            return is_est, is_tuple
+
+        # We've already guarded against objs being dict when allow_dict is False
+        # So here we can just check dictionary elements
+        if isinstance(objs, dict) and not all(
+            isinstance(name, str) and isinstance(obj, cls_type)
+            for name, obj in objs.items()
+        ):
+            raise TypeError(msg)
+
+        elif not all(any(is_obj_is_tuple(x)) for x in objs):
+            raise TypeError(msg)
+
+        msg_no_mix = (
+            f"Elements of {attr_name} must either all be objects, "
+            f"or all (str, objects) tuples. A mix of the two is not allowed."
+        )
+        if not allow_mix and not all(is_obj_is_tuple(x)[0] for x in objs):
+            if not all(is_obj_is_tuple(x)[1] for x in objs):
+                raise TypeError(msg_no_mix)
+
+        return self._coerce_to_named_object_tuples(objs, clone=clone, make_unique=True)
+
+    def _get_names_and_objects(
+        self,
+        named_objects: Union[
+            Sequence[Union[BaseObject, Tuple[str, BaseObject]]], Dict[str, BaseObject]
+        ],
+        make_unique: bool = False,
+    ) -> Tuple[List[str], List[BaseObject]]:
+        """Return lists of names and object from input that follows named object API.
+
+        Handles input that is dictionary mapping str names of object instances or
+        input that is a list of (str, object) tuples.
+
+        Parameters
+        ----------
+        named_objects : list[tuple[str, object], ...], list[object], dict[str, object]
+            The objects whose names should be returned.
+        make_unique : bool, default=False
+            Whether names should be made unique.
+
+        Returns
+        -------
+        names : list[str]
+            Lists of the names and objects that were input.
+        objs : list[BaseObject]
+            The
+        """
+        names: Tuple[str, ...]
+        objs: Tuple[BaseObject, ...]
+        if isinstance(named_objects, dict):
+            names, objs = zip(*named_objects.items())
+        else:
+            names, objs = zip(*[self._coerce_object_tuple(x) for x in named_objects])
+
+        # Optionally make names unique
+        if make_unique:
+            names = make_strings_unique(names)
+        return list(names), list(objs)
+
+    def _coerce_to_named_object_tuples(
+        self,
+        objs: Union[
+            Sequence[Union[BaseObject, Tuple[str, BaseObject]]], Dict[str, BaseObject]
+        ],
+        clone: bool = False,
+        make_unique: bool = True,
+    ) -> List[Tuple[str, BaseObject]]:
+        """Coerce sequence of objects or named objects to list of (str, obj) tuples.
+
+        Input that is sequence of objects, list of (str, obj) tuples or
+        dict[str, object] will be coerced to list of (str, obj) tuples on return.
+
+        Parameters
+        ----------
+        objs : list of objects, list of (str, object tuples) or dict[str, object]
+            The input should be coerced to list of (str, object) tuples. Should
+            be a sequence of objects, or follow named object API.
+        clone : bool, default=False.
+            Whether objects in the returned list of (str, object) tuples are
+            cloned (True) or references (False).
+        make_unique : bool, default=True
+            Whether the str names in the returned list of (str, object) tuples
+            should be coerced to unique str values (if str names in input
+            are already unique they will not be changed).
+
+        Returns
+        -------
+        list[tuple[str, BaseObject]]
+            List of tuples following named object API.
+
+            - If `objs` was already a list of (str, object) tuples then either the
+              same named objects (as with other cases cloned versions are
+              returned if ``clone=True``).
+            - If `objs` was a dict[str, object] then the named objects are unpacked
+              into a list of (str, object) tuples.
+            - If `objs` was a list of objects then string names were generated based
+               on the object's class names (with coercion to unique strings if
+               necessary).
+        """
+        if isinstance(objs, dict):
+            named_objects = [(k, v) for k, v in objs.items()]
+        else:
+            # Otherwise get named object format
+            if TYPE_CHECKING:
+                assert not isinstance(objs, dict)  # nosec: B1010
+            named_objects = [
+                self._coerce_object_tuple(obj, clone=clone) for obj in objs
+            ]
+        if make_unique:
+            # Unpack names and objects while making names unique
+            names, objs = self._get_names_and_objects(
+                named_objects, make_unique=make_unique
+            )
+            # Repack the objects
+            named_objects = list(zip(names, objs))
+        return named_objects
+
+    def _dunder_concat(
+        self,
+        other,
+        base_class,
+        composite_class,
+        attr_name="steps",
+        concat_order="left",
+        composite_params=None,
+    ):
+        """Logic to concatenate pipelines for dunder parsing.
+
+        This is useful in concrete heterogeneous meta-objects that implement
+        dunders for easy concatenation of pipeline-like composites.
+
+        Parameters
+        ----------
+        other : BaseObject subclass
+            An object inheritting from `composite_class` or `base_class`, otherwise
+            `NotImplemented` is returned.
+        base_class : BaseObject subclass
+            Class assumed as base class for self and `other`. ,
+            and estimator components of composite_class, in case of concatenation
+        composite_class : BaseMetaObject or BaseMetaEstimator subclass
+            Class that has parameter `attr_name` stored in attribute of same name
+            that contains list of base_class objects, list of (str, base_class)
+            tuples, or a mixture thereof.
+        attr_name : str, default="steps"
+            Name of the attribute that contains base_class objects,
+            list of (str, base_class) tuples. Concatenation is done for this attribute.
+        concat_order : {"left", "right"}, default="left"
+            Specifies ordering for concatenation.
+
+            - If "left", resulting attr_name will be like
+              self.attr_name + other.attr_name.
+            - If "right", resulting attr_name will be like
+              other.attr_name + self.attr_name.
+
+        composite_params : dict, default=None
+            Parameters of the composite are always set accordingly
+            i.e., contains key-value pairs, and composite_class has key set to value.
+
+        Returns
+        -------
+        BaseMetaObject or BaseMetaEstimator
+            Instance of `composite_class`, where `attr_name` is set so that self and
+            other are "concatenated".
+
+            - If other is instance of `composite_class` then instance of
+              `composite_class`, where `attr_name` is a concatenation of
+              ``self.attr_name`` and ``other.attr_name``.
+            - If `other` is instance of `base_class`, then instance of `composite_class`
+              is returned where `attr_name` is set so that so that
+              composite_class(attr_name=other) is returned.
+            - If str are all the class names of est, list of est only is used instead
+        """
+        # Validate input
+        if concat_order not in ["left", "right"]:
+            raise ValueError(
+                f"`concat_order` must be 'left' or 'right', but found {concat_order!r}."
+            )
+        if not isinstance(attr_name, str):
+            raise TypeError(f"`attr_name` must be str, but found {type(attr_name)}.")
+        if not isclass(composite_class):
+            raise TypeError("`composite_class` must be a class.")
+        if not isclass(base_class):
+            raise TypeError("`base_class` must be a class.")
+        if not issubclass(composite_class, base_class):
+            raise ValueError("`composite_class` must be a subclass of base_class.")
+        if not isinstance(self, composite_class):
+            raise TypeError("self must be an instance of `composite_class`.")
+
+        def concat(x, y):
+            if concat_order == "left":
+                return x + y
+            else:
+                return y + x
+
+        # get attr_name from self and other
+        # can be list of ests, list of (str, est) tuples, or list of mixture of these
+        self_attr = getattr(self, attr_name)
+
+        # from that, obtain ests, and original names (may be non-unique)
+        # we avoid _make_strings_unique call too early to avoid blow-up of string
+        self_names, self_objs = self._get_names_and_objects(self_attr)
+        if isinstance(other, composite_class):
+            other_attr = getattr(other, attr_name)
+            other_names, other_objs = other._get_names_and_objects(other_attr)
+        elif isinstance(other, base_class):
+            other_names = [type(other).__name__]
+            other_objs = [other]
+        elif is_named_object_tuple(other, object_type=base_class):
+            other_names = [other[0]]
+            other_objs = [other[1]]
+        else:
+            return NotImplemented
+
+        new_names = concat(self_names, other_names)
+        new_objs = concat(self_objs, other_objs)
+        # create the "steps" param for the composite
+        # if all the names are equal to class names, we eat them away
+        if all(type(x[1]).__name__ == x[0] for x in zip(new_names, new_objs)):
+            step_param = {attr_name: list(new_objs)}
+        else:
+            step_param = {attr_name: list(zip(new_names, new_objs))}
+
+        # retrieve other parameters, from composite_params attribute
+        if composite_params is None:
+            composite_params = {}
+        else:
+            composite_params = composite_params.copy()
+
+        # construct the composite with both step and additional params
+        composite_params.update(step_param)
+        return composite_class(**composite_params)
+
+    def _sk_visual_block_(self):
+        """Logic to help render meta estimator as visual HTML block."""
+        # Use tag interface that will be available when mixin is used
+        named_object_attr_name = self.get_tag("named_object_parameters")  # type: ignore
+        named_object_attr = getattr(self, named_object_attr_name)
+        named_objects = self._coerce_to_named_object_tuples(named_object_attr)
+        _, objs = self._get_names_and_objects(named_objects)
+
+        def _get_name(name, obj):
+            if obj is None or obj == "passthrough":
+                return f"{name}: passthrough"
+            # Is an estimator
+            return f"{name}: {obj.__class__.__name__}"
+
+        names = [_get_name(name, est) for name, est in named_objects]
+        name_details = [str(obj) for obj in objs]
+        return _VisualBlock(
+            "serial",
+            objs,
+            names=names,
+            name_details=name_details,
+            dash_wrapped=False,
+        )
+
+
+class _MetaTagLogicMixin:
+    """Mixin for tag conjunction, disjunction, chain operations for meta-objects.
+
+    Contains methods to set tags of a meta-object dependent on component objects.
+    """
+
+    def _anytagis(self, tag_name, value, estimators):
+        """Return whether any estimator in list has tag `tag_name` of value `value`.
+
+        Parameters
+        ----------
+        tag_name : str, name of the tag to check
+        value : value of the tag to check for
+        estimators : list of (str, estimator) pairs to query for the tag/value
+
+        Return
+        ------
+        bool : True iff at least one estimator in the list has value in tag tag_name
+        """
+        tagis = [est.get_tag(tag_name, value) == value for _, est in estimators]
+        return any(tagis)
+
+    def _anytagis_then_set(self, tag_name, value, value_if_not, estimators):
+        """Set self's `tag_name` tag to `value` if any estimator on the list has it.
+
+        Writes to self:
+        sets the tag `tag_name` to `value` if `_anytagis(tag_name, value)` is True
+            otherwise sets the tag `tag_name` to `value_if_not`
+
+        Parameters
+        ----------
+        tag_name : str, name of the tag
+        value : value to check and to set tag to if one of the tag values is `value`
+        value_if_not : value to set in self if none of the tag values is `value`
+        estimators : list of (str, estimator) pairs to query for the tag/value
+        """
+        if self._anytagis(tag_name=tag_name, value=value, estimators=estimators):
+            self.set_tags(**{tag_name: value})
+        else:
+            self.set_tags(**{tag_name: value_if_not})
+
+    def _anytag_notnone_val(self, tag_name, estimators):
+        """Return first non-'None' value of tag `tag_name` in estimator list.
+
+        Parameters
+        ----------
+        tag_name : str, name of the tag
+        estimators : list of (str, estimator) pairs to query for the tag/value
+
+        Return
+        ------
+        tag_val : first non-'None' value of tag `tag_name` in estimator list.
+        """
+        for _, est in estimators:
+            tag_val = est.get_tag(tag_name)
+            if tag_val != "None":
+                return tag_val
+        return tag_val
+
+    def _anytag_notnone_set(self, tag_name, estimators):
+        """Set self's `tag_name` tag to first non-'None' value in estimator list.
+
+        Writes to self:
+        tag with name tag_name, sets to _anytag_notnone_val(tag_name, estimators)
+
+        Parameters
+        ----------
+        tag_name : str, name of the tag
+        estimators : list of (str, estimator) pairs to query for the tag/value
+        """
+        tag_val = self._anytag_notnone_val(tag_name=tag_name, estimators=estimators)
+        if tag_val != "None":
+            self.set_tags(**{tag_name: tag_val})
+
+    def _tagchain_is_linked(
+        self,
+        left_tag_name,
+        mid_tag_name,
+        estimators,
+        left_tag_val=True,
+        mid_tag_val=True,
+    ):
+        """Check whether all tags left of the first mid_tag/val are left_tag/val.
+
+        Useful to check, for instance, whether all instances of estimators
+            left of the first missing value imputer can deal with missing values.
+
+        Parameters
+        ----------
+        left_tag_name : str, name of the left tag
+        mid_tag_name : str, name of the middle tag
+        estimators : list of (str, estimator) pairs to query for the tag/value
+        left_tag_val : value of the left tag, optional, default=True
+        mid_tag_val : value of the middle tag, optional, default=True
+
+        Returns
+        -------
+        chain_is_linked : bool,
+            True iff all "left" tag instances `left_tag_name` have value `left_tag_val`
+            a "left" tag instance is an instance in estimators which is earlier
+            than the first occurrence of `mid_tag_name` with value `mid_tag_val`
+        chain_is_complete : bool,
+            True iff chain_is_linked is True, and
+                there is an occurrence of `mid_tag_name` with value `mid_tag_val`
+        """
+        for _, est in estimators:
+            if est.get_tag(mid_tag_name) == mid_tag_val:
+                return True, True
+            if not est.get_tag(left_tag_name) == left_tag_val:
+                return False, False
+        return True, False
+
+    def _tagchain_is_linked_set(
+        self,
+        left_tag_name,
+        mid_tag_name,
+        estimators,
+        left_tag_val=True,
+        mid_tag_val=True,
+        left_tag_val_not=False,
+        mid_tag_val_not=False,
+    ):
+        """Check if _tagchain_is_linked, then set self left_tag_name and mid_tag_name.
+
+        Writes to self:
+        tag with name left_tag_name, sets to left_tag_val if _tag_chain_is_linked[0]
+            otherwise sets to left_tag_val_not
+        tag with name mid_tag_name, sets to mid_tag_val if _tag_chain_is_linked[1]
+            otherwise sets to mid_tag_val_not
+
+        Parameters
+        ----------
+        left_tag_name : str, name of the left tag
+        mid_tag_name : str, name of the middle tag
+        estimators : list of (str, estimator) pairs to query for the tag/value
+        left_tag_val : value of the left tag, optional, default=True
+        mid_tag_val : value of the middle tag, optional, default=True
+        left_tag_val_not : value to set if not linked, optional, default=False
+        mid_tag_val_not : value to set if not linked, optional, default=False
+        """
+        linked, complete = self._tagchain_is_linked(
+            left_tag_name=left_tag_name,
+            mid_tag_name=mid_tag_name,
+            estimators=estimators,
+            left_tag_val=left_tag_val,
+            mid_tag_val=mid_tag_val,
+        )
+        if linked:
+            self.set_tags(**{left_tag_name: left_tag_val})
+        else:
+            self.set_tags(**{left_tag_name: left_tag_val_not})
+        if complete:
+            self.set_tags(**{mid_tag_name: mid_tag_val})
+        else:
+            self.set_tags(**{mid_tag_name: mid_tag_val_not})
+
+
+class BaseMetaObject(_MetaObjectMixin, _MetaTagLogicMixin, BaseObject):
+    """Parameter and tag management for objects composed of named objects.
+
+    Allows objects to get and set nested parameters when a parameter of the the
+    class has values that follow the named object specification. For example,
+    in a pipeline class with the the "step" parameter accepting named objects,
+    this would allow `get_params` and `set_params` to retrieve and update the
+    parameters of the objects in each step.
+
+    See Also
+    --------
+    BaseMetaEstimator :
+        Expands on `BaseMetaObject` by adding functionality for getting fitted
+        parameters from a class's component estimators. `BaseEstimator` should
+        be used when you want to create a meta estimator.
+    """
+
+
+class BaseMetaEstimator(_MetaObjectMixin, _MetaTagLogicMixin, BaseEstimator):
+    """Parameter and tag management for estimators composed of named objects.
+
+    Allows estimators to get and set nested parameters when a parameter of the the
+    class has values that follow the named object specification. For example,
+    in a pipeline class with the the "step" parameter accepting named objects,
+    this would allow `get_params` and `set_params` to retrieve and update the
+    parameters of the objects in each step.
+
+    See Also
+    --------
+    BaseMetaObject :
+        Provides similar functionality to  `BaseMetaEstimator` for getting
+        parameters from a class's component objects, but does not have the
+        estimator interface.
+    """
```

### Comparing `skbase-0.4.5/skbase/base/_pretty_printing/_pprint.py` & `skbase-0.4.6/skbase/base/_pretty_printing/_pprint.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,412 +1,412 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-# Many elements of this code were developed in scikit-learn. These elements
-# are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
-# conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
-"""Utility functionality for pretty-printing objects used in BaseObject.__repr__."""
-import inspect
-import pprint
-from collections import OrderedDict
-
-from skbase.base import BaseObject
-
-# from skbase.config import get_config
-from skbase.utils._check import _is_scalar_nan
-
-
-class KeyValTuple(tuple):
-    """Dummy class for correctly rendering key-value tuples from dicts."""
-
-    def __repr__(self):
-        """Represent as string."""
-        # needed for _dispatch[tuple.__repr__] not to be overridden
-        return super().__repr__()
-
-
-class KeyValTupleParam(KeyValTuple):
-    """Dummy class for correctly rendering key-value tuples from parameters."""
-
-    pass
-
-
-def _changed_params(base_object):
-    """Return dict (param_name: value) of parameters with non-default values."""
-    params = base_object.get_params(deep=False)
-    init_func = getattr(
-        base_object.__init__, "deprecated_original", base_object.__init__
-    )
-    init_params = inspect.signature(init_func).parameters
-    init_params = {name: param.default for name, param in init_params.items()}
-
-    def has_changed(k, v):
-        if k not in init_params:  # happens if k is part of a **kwargs
-            return True
-        if init_params[k] == inspect._empty:  # k has no default value
-            return True
-        # try to avoid calling repr on nested BaseObjects
-        if isinstance(v, BaseObject) and v.__class__ != init_params[k].__class__:
-            return True
-        # Use repr as a last resort. It may be expensive.
-        if repr(v) != repr(init_params[k]) and not (
-            _is_scalar_nan(init_params[k]) and _is_scalar_nan(v)
-        ):
-            return True
-        return False
-
-    return {k: v for k, v in params.items() if has_changed(k, v)}
-
-
-class _BaseObjectPrettyPrinter(pprint.PrettyPrinter):
-    """Pretty Printer class for BaseObjects.
-
-    This extends the pprint.PrettyPrinter class similar to scikit-learn's
-    implementation, so that:
-
-    - BaseObjects are printed with their parameters, e.g.
-      BaseObject(param1=value1, ...) which is not supported by default.
-    - the 'compact' parameter of PrettyPrinter is ignored for dicts, which
-      may lead to very long representations that we want to avoid.
-
-    Quick overview of pprint.PrettyPrinter (see also
-    https://stackoverflow.com/questions/49565047/pprint-with-hex-numbers):
-
-    - the entry point is the _format() method which calls format() (overridden
-      here)
-    - format() directly calls _safe_repr() for a first try at rendering the
-      object
-    - _safe_repr formats the whole object recursively, only calling itself,
-      not caring about line length or anything
-    - back to _format(), if the output string is too long, _format() then calls
-      the appropriate _pprint_TYPE() method (e.g. _pprint_list()) depending on
-      the type of the object. This where the line length and the compact
-      parameters are taken into account.
-    - those _pprint_TYPE() methods will internally use the format() method for
-      rendering the nested objects of an object (e.g. the elements of a list)
-
-    In the end, everything has to be implemented twice: in _safe_repr and in
-    the custom _pprint_TYPE methods. Unfortunately PrettyPrinter is really not
-    straightforward to extend (especially when we want a compact output), so
-    the code is a bit convoluted.
-
-    This class overrides:
-    - format() to support the changed_only parameter
-    - _safe_repr to support printing of BaseObjects that fit on a single line
-    - _format_dict_items so that dict are correctly 'compacted'
-    - _format_items so that ellipsis is used on long lists and tuples
-
-    When BaseObjects cannot be printed on a single line, the builtin _format()
-    will call _pprint_object() because it was registered to do so (see
-    _dispatch[BaseObject.__repr__] = _pprint_object).
-
-    both _format_dict_items() and _pprint_Object() use the
-    _format_params_or_dict_items() method that will format parameters and
-    key-value pairs respecting the compact parameter. This method needs another
-    subroutine _pprint_key_val_tuple() used when a parameter or a key-value
-    pair is too long to fit on a single line. This subroutine is called in
-    _format() and is registered as well in the _dispatch dict (just like
-    _pprint_object). We had to create the two classes KeyValTuple and
-    KeyValTupleParam for this.
-    """
-
-    def __init__(
-        self,
-        indent=1,
-        width=80,
-        depth=None,
-        stream=None,
-        *,
-        compact=False,
-        indent_at_name=True,
-        n_max_elements_to_show=None,
-        changed_only=True,
-    ):
-        super().__init__(indent, width, depth, stream, compact=compact)
-        self._indent_at_name = indent_at_name
-        if self._indent_at_name:
-            self._indent_per_level = 1  # ignore indent param
-        self.changed_only = changed_only
-        # Max number of elements in a list, dict, tuple until we start using
-        # ellipsis. This also affects the number of arguments of a BaseObject
-        # (they are treated as dicts)
-        self.n_max_elements_to_show = n_max_elements_to_show
-
-    def format(self, obj, context, maxlevels, level):  # noqa
-        return _safe_repr(
-            obj, context, maxlevels, level, changed_only=self.changed_only
-        )
-
-    def _pprint_object(self, obj, stream, indent, allowance, context, level):
-        stream.write(obj.__class__.__name__ + "(")
-        if self._indent_at_name:
-            indent += len(obj.__class__.__name__)
-
-        if self.changed_only:
-            params = _changed_params(obj)
-        else:
-            params = obj.get_params(deep=False)
-
-        params = OrderedDict((name, val) for (name, val) in sorted(params.items()))
-
-        self._format_params(
-            params.items(), stream, indent, allowance + 1, context, level
-        )
-        stream.write(")")
-
-    def _format_dict_items(self, items, stream, indent, allowance, context, level):
-        return self._format_params_or_dict_items(
-            items, stream, indent, allowance, context, level, is_dict=True
-        )
-
-    def _format_params(self, items, stream, indent, allowance, context, level):
-        return self._format_params_or_dict_items(
-            items, stream, indent, allowance, context, level, is_dict=False
-        )
-
-    def _format_params_or_dict_items(
-        self, obj, stream, indent, allowance, context, level, is_dict
-    ):
-        """Format dict items or parameters respecting the compact=True parameter.
-
-        For some reason, the builtin rendering of dict items doesn't
-        respect compact=True and will use one line per key-value if all cannot
-        fit in a single line.
-        Dict items will be rendered as <'key': value> while params will be
-        rendered as <key=value>. The implementation is mostly copy/pasting from
-        the builtin _format_items().
-        This also adds ellipsis if the number of items is greater than
-        self.n_max_elements_to_show.
-        """
-        write = stream.write
-        indent += self._indent_per_level
-        delimnl = ",\n" + " " * indent
-        delim = ""
-        width = max_width = self._width - indent + 1
-        it = iter(obj)
-        try:
-            next_ent = next(it)
-        except StopIteration:
-            return
-        last = False
-        n_items = 0
-        while not last:
-            if n_items == self.n_max_elements_to_show:
-                write(", ...")
-                break
-            n_items += 1
-            ent = next_ent
-            try:
-                next_ent = next(it)
-            except StopIteration:
-                last = True
-                max_width -= allowance
-                width -= allowance
-            if self._compact:
-                k, v = ent
-                krepr = self._repr(k, context, level)
-                vrepr = self._repr(v, context, level)
-                if not is_dict:
-                    krepr = krepr.strip("'")
-                middle = ": " if is_dict else "="
-                rep = krepr + middle + vrepr
-                w = len(rep) + 2
-                if width < w:
-                    width = max_width
-                    if delim:
-                        delim = delimnl
-                if width >= w:
-                    width -= w
-                    write(delim)
-                    delim = ", "
-                    write(rep)
-                    continue
-            write(delim)
-            delim = delimnl
-            class_ = KeyValTuple if is_dict else KeyValTupleParam
-            self._format(
-                class_(ent), stream, indent, allowance if last else 1, context, level
-            )
-
-    def _format_items(self, items, stream, indent, allowance, context, level):
-        """Format the items of an iterable (list, tuple...).
-
-        Same as the built-in _format_items, with support for ellipsis if the
-        number of elements is greater than self.n_max_elements_to_show.
-        """
-        write = stream.write
-        indent += self._indent_per_level
-        if self._indent_per_level > 1:
-            write((self._indent_per_level - 1) * " ")
-        delimnl = ",\n" + " " * indent
-        delim = ""
-        width = max_width = self._width - indent + 1
-        it = iter(items)
-        try:
-            next_ent = next(it)
-        except StopIteration:
-            return
-        last = False
-        n_items = 0
-        while not last:
-            if n_items == self.n_max_elements_to_show:
-                write(", ...")
-                break
-            n_items += 1
-            ent = next_ent
-            try:
-                next_ent = next(it)
-            except StopIteration:
-                last = True
-                max_width -= allowance
-                width -= allowance
-            if self._compact:
-                rep = self._repr(ent, context, level)
-                w = len(rep) + 2
-                if width < w:
-                    width = max_width
-                    if delim:
-                        delim = delimnl
-                if width >= w:
-                    width -= w
-                    write(delim)
-                    delim = ", "
-                    write(rep)
-                    continue
-            write(delim)
-            delim = delimnl
-            self._format(ent, stream, indent, allowance if last else 1, context, level)
-
-    def _pprint_key_val_tuple(self, obj, stream, indent, allowance, context, level):
-        """Pretty printing for key-value tuples from dict or parameters."""
-        k, v = obj
-        rep = self._repr(k, context, level)
-        if isinstance(obj, KeyValTupleParam):
-            rep = rep.strip("'")
-            middle = "="
-        else:
-            middle = ": "
-        stream.write(rep)
-        stream.write(middle)
-        self._format(
-            v, stream, indent + len(rep) + len(middle), allowance, context, level
-        )
-
-    # Follow what scikit-learn did here and copy _dispatch to prevent instances
-    # of the builtin PrettyPrinter class to call methods of
-    # _BaseObjectPrettyPrinter (see scikit-learn Github issue 12906)
-    # mypy error: "Type[PrettyPrinter]" has no attribute "_dispatch"
-    _dispatch = pprint.PrettyPrinter._dispatch.copy()  # type: ignore
-    _dispatch[BaseObject.__repr__] = _pprint_object
-    _dispatch[KeyValTuple.__repr__] = _pprint_key_val_tuple
-
-
-def _safe_repr(obj, context, maxlevels, level, changed_only=False):
-    """Safe string representation logic.
-
-    Same as the builtin _safe_repr, with added support for BaseObjects.
-    """
-    typ = type(obj)
-
-    if typ in pprint._builtin_scalars:
-        return repr(obj), True, False
-
-    r = getattr(typ, "__repr__", None)
-    if issubclass(typ, dict) and r is dict.__repr__:
-        if not obj:
-            return "{}", True, False
-        objid = id(obj)
-        if maxlevels and level >= maxlevels:
-            return "{...}", False, objid in context
-        if objid in context:
-            return pprint._recursion(obj), False, True
-        context[objid] = 1
-        readable = True
-        recursive = False
-        components = []
-        append = components.append
-        level += 1
-        saferepr = _safe_repr
-        items = sorted(obj.items(), key=pprint._safe_tuple)
-        for k, v in items:
-            krepr, kreadable, krecur = saferepr(
-                k, context, maxlevels, level, changed_only=changed_only
-            )
-            vrepr, vreadable, vrecur = saferepr(
-                v, context, maxlevels, level, changed_only=changed_only
-            )
-            append("%s: %s" % (krepr, vrepr))
-            readable = readable and kreadable and vreadable
-            if krecur or vrecur:
-                recursive = True
-        del context[objid]
-        return "{%s}" % ", ".join(components), readable, recursive
-
-    if (issubclass(typ, list) and r is list.__repr__) or (
-        issubclass(typ, tuple) and r is tuple.__repr__
-    ):
-        if issubclass(typ, list):
-            if not obj:
-                return "[]", True, False
-            format_ = "[%s]"
-        elif len(obj) == 1:
-            format_ = "(%s,)"
-        else:
-            if not obj:
-                return "()", True, False
-            format_ = "(%s)"
-        objid = id(obj)
-        if maxlevels and level >= maxlevels:
-            return format_ % "...", False, objid in context
-        if objid in context:
-            return pprint._recursion(obj), False, True
-        context[objid] = 1
-        readable = True
-        recursive = False
-        components = []
-        append = components.append
-        level += 1
-        for o in obj:
-            orepr, oreadable, orecur = _safe_repr(
-                o, context, maxlevels, level, changed_only=changed_only
-            )
-            append(orepr)
-            if not oreadable:
-                readable = False
-            if orecur:
-                recursive = True
-        del context[objid]
-        return format_ % ", ".join(components), readable, recursive
-
-    if issubclass(typ, BaseObject):
-        objid = id(obj)
-        if maxlevels and level >= maxlevels:
-            return "{...}", False, objid in context
-        if objid in context:
-            return pprint._recursion(obj), False, True
-        context[objid] = 1
-        readable = True
-        recursive = False
-        if changed_only:
-            params = _changed_params(obj)
-        else:
-            params = obj.get_params(deep=False)
-        components = []
-        append = components.append
-        level += 1
-        saferepr = _safe_repr
-        items = sorted(params.items(), key=pprint._safe_tuple)
-        for k, v in items:
-            krepr, kreadable, krecur = saferepr(
-                k, context, maxlevels, level, changed_only=changed_only
-            )
-            vrepr, vreadable, vrecur = saferepr(
-                v, context, maxlevels, level, changed_only=changed_only
-            )
-            append("%s=%s" % (krepr.strip("'"), vrepr))
-            readable = readable and kreadable and vreadable
-            if krecur or vrecur:
-                recursive = True
-        del context[objid]
-        return ("%s(%s)" % (typ.__name__, ", ".join(components)), readable, recursive)
-
-    rep = repr(obj)
-    return rep, (rep and not rep.startswith("<")), False
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+# Many elements of this code were developed in scikit-learn. These elements
+# are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
+# conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
+"""Utility functionality for pretty-printing objects used in BaseObject.__repr__."""
+import inspect
+import pprint
+from collections import OrderedDict
+
+from skbase.base import BaseObject
+
+# from skbase.config import get_config
+from skbase.utils._check import _is_scalar_nan
+
+
+class KeyValTuple(tuple):
+    """Dummy class for correctly rendering key-value tuples from dicts."""
+
+    def __repr__(self):
+        """Represent as string."""
+        # needed for _dispatch[tuple.__repr__] not to be overridden
+        return super().__repr__()
+
+
+class KeyValTupleParam(KeyValTuple):
+    """Dummy class for correctly rendering key-value tuples from parameters."""
+
+    pass
+
+
+def _changed_params(base_object):
+    """Return dict (param_name: value) of parameters with non-default values."""
+    params = base_object.get_params(deep=False)
+    init_func = getattr(
+        base_object.__init__, "deprecated_original", base_object.__init__
+    )
+    init_params = inspect.signature(init_func).parameters
+    init_params = {name: param.default for name, param in init_params.items()}
+
+    def has_changed(k, v):
+        if k not in init_params:  # happens if k is part of a **kwargs
+            return True
+        if init_params[k] == inspect._empty:  # k has no default value
+            return True
+        # try to avoid calling repr on nested BaseObjects
+        if isinstance(v, BaseObject) and v.__class__ != init_params[k].__class__:
+            return True
+        # Use repr as a last resort. It may be expensive.
+        if repr(v) != repr(init_params[k]) and not (
+            _is_scalar_nan(init_params[k]) and _is_scalar_nan(v)
+        ):
+            return True
+        return False
+
+    return {k: v for k, v in params.items() if has_changed(k, v)}
+
+
+class _BaseObjectPrettyPrinter(pprint.PrettyPrinter):
+    """Pretty Printer class for BaseObjects.
+
+    This extends the pprint.PrettyPrinter class similar to scikit-learn's
+    implementation, so that:
+
+    - BaseObjects are printed with their parameters, e.g.
+      BaseObject(param1=value1, ...) which is not supported by default.
+    - the 'compact' parameter of PrettyPrinter is ignored for dicts, which
+      may lead to very long representations that we want to avoid.
+
+    Quick overview of pprint.PrettyPrinter (see also
+    https://stackoverflow.com/questions/49565047/pprint-with-hex-numbers):
+
+    - the entry point is the _format() method which calls format() (overridden
+      here)
+    - format() directly calls _safe_repr() for a first try at rendering the
+      object
+    - _safe_repr formats the whole object recursively, only calling itself,
+      not caring about line length or anything
+    - back to _format(), if the output string is too long, _format() then calls
+      the appropriate _pprint_TYPE() method (e.g. _pprint_list()) depending on
+      the type of the object. This where the line length and the compact
+      parameters are taken into account.
+    - those _pprint_TYPE() methods will internally use the format() method for
+      rendering the nested objects of an object (e.g. the elements of a list)
+
+    In the end, everything has to be implemented twice: in _safe_repr and in
+    the custom _pprint_TYPE methods. Unfortunately PrettyPrinter is really not
+    straightforward to extend (especially when we want a compact output), so
+    the code is a bit convoluted.
+
+    This class overrides:
+    - format() to support the changed_only parameter
+    - _safe_repr to support printing of BaseObjects that fit on a single line
+    - _format_dict_items so that dict are correctly 'compacted'
+    - _format_items so that ellipsis is used on long lists and tuples
+
+    When BaseObjects cannot be printed on a single line, the builtin _format()
+    will call _pprint_object() because it was registered to do so (see
+    _dispatch[BaseObject.__repr__] = _pprint_object).
+
+    both _format_dict_items() and _pprint_Object() use the
+    _format_params_or_dict_items() method that will format parameters and
+    key-value pairs respecting the compact parameter. This method needs another
+    subroutine _pprint_key_val_tuple() used when a parameter or a key-value
+    pair is too long to fit on a single line. This subroutine is called in
+    _format() and is registered as well in the _dispatch dict (just like
+    _pprint_object). We had to create the two classes KeyValTuple and
+    KeyValTupleParam for this.
+    """
+
+    def __init__(
+        self,
+        indent=1,
+        width=80,
+        depth=None,
+        stream=None,
+        *,
+        compact=False,
+        indent_at_name=True,
+        n_max_elements_to_show=None,
+        changed_only=True,
+    ):
+        super().__init__(indent, width, depth, stream, compact=compact)
+        self._indent_at_name = indent_at_name
+        if self._indent_at_name:
+            self._indent_per_level = 1  # ignore indent param
+        self.changed_only = changed_only
+        # Max number of elements in a list, dict, tuple until we start using
+        # ellipsis. This also affects the number of arguments of a BaseObject
+        # (they are treated as dicts)
+        self.n_max_elements_to_show = n_max_elements_to_show
+
+    def format(self, obj, context, maxlevels, level):  # noqa
+        return _safe_repr(
+            obj, context, maxlevels, level, changed_only=self.changed_only
+        )
+
+    def _pprint_object(self, obj, stream, indent, allowance, context, level):
+        stream.write(obj.__class__.__name__ + "(")
+        if self._indent_at_name:
+            indent += len(obj.__class__.__name__)
+
+        if self.changed_only:
+            params = _changed_params(obj)
+        else:
+            params = obj.get_params(deep=False)
+
+        params = OrderedDict((name, val) for (name, val) in sorted(params.items()))
+
+        self._format_params(
+            params.items(), stream, indent, allowance + 1, context, level
+        )
+        stream.write(")")
+
+    def _format_dict_items(self, items, stream, indent, allowance, context, level):
+        return self._format_params_or_dict_items(
+            items, stream, indent, allowance, context, level, is_dict=True
+        )
+
+    def _format_params(self, items, stream, indent, allowance, context, level):
+        return self._format_params_or_dict_items(
+            items, stream, indent, allowance, context, level, is_dict=False
+        )
+
+    def _format_params_or_dict_items(
+        self, obj, stream, indent, allowance, context, level, is_dict
+    ):
+        """Format dict items or parameters respecting the compact=True parameter.
+
+        For some reason, the builtin rendering of dict items doesn't
+        respect compact=True and will use one line per key-value if all cannot
+        fit in a single line.
+        Dict items will be rendered as <'key': value> while params will be
+        rendered as <key=value>. The implementation is mostly copy/pasting from
+        the builtin _format_items().
+        This also adds ellipsis if the number of items is greater than
+        self.n_max_elements_to_show.
+        """
+        write = stream.write
+        indent += self._indent_per_level
+        delimnl = ",\n" + " " * indent
+        delim = ""
+        width = max_width = self._width - indent + 1
+        it = iter(obj)
+        try:
+            next_ent = next(it)
+        except StopIteration:
+            return
+        last = False
+        n_items = 0
+        while not last:
+            if n_items == self.n_max_elements_to_show:
+                write(", ...")
+                break
+            n_items += 1
+            ent = next_ent
+            try:
+                next_ent = next(it)
+            except StopIteration:
+                last = True
+                max_width -= allowance
+                width -= allowance
+            if self._compact:
+                k, v = ent
+                krepr = self._repr(k, context, level)
+                vrepr = self._repr(v, context, level)
+                if not is_dict:
+                    krepr = krepr.strip("'")
+                middle = ": " if is_dict else "="
+                rep = krepr + middle + vrepr
+                w = len(rep) + 2
+                if width < w:
+                    width = max_width
+                    if delim:
+                        delim = delimnl
+                if width >= w:
+                    width -= w
+                    write(delim)
+                    delim = ", "
+                    write(rep)
+                    continue
+            write(delim)
+            delim = delimnl
+            class_ = KeyValTuple if is_dict else KeyValTupleParam
+            self._format(
+                class_(ent), stream, indent, allowance if last else 1, context, level
+            )
+
+    def _format_items(self, items, stream, indent, allowance, context, level):
+        """Format the items of an iterable (list, tuple...).
+
+        Same as the built-in _format_items, with support for ellipsis if the
+        number of elements is greater than self.n_max_elements_to_show.
+        """
+        write = stream.write
+        indent += self._indent_per_level
+        if self._indent_per_level > 1:
+            write((self._indent_per_level - 1) * " ")
+        delimnl = ",\n" + " " * indent
+        delim = ""
+        width = max_width = self._width - indent + 1
+        it = iter(items)
+        try:
+            next_ent = next(it)
+        except StopIteration:
+            return
+        last = False
+        n_items = 0
+        while not last:
+            if n_items == self.n_max_elements_to_show:
+                write(", ...")
+                break
+            n_items += 1
+            ent = next_ent
+            try:
+                next_ent = next(it)
+            except StopIteration:
+                last = True
+                max_width -= allowance
+                width -= allowance
+            if self._compact:
+                rep = self._repr(ent, context, level)
+                w = len(rep) + 2
+                if width < w:
+                    width = max_width
+                    if delim:
+                        delim = delimnl
+                if width >= w:
+                    width -= w
+                    write(delim)
+                    delim = ", "
+                    write(rep)
+                    continue
+            write(delim)
+            delim = delimnl
+            self._format(ent, stream, indent, allowance if last else 1, context, level)
+
+    def _pprint_key_val_tuple(self, obj, stream, indent, allowance, context, level):
+        """Pretty printing for key-value tuples from dict or parameters."""
+        k, v = obj
+        rep = self._repr(k, context, level)
+        if isinstance(obj, KeyValTupleParam):
+            rep = rep.strip("'")
+            middle = "="
+        else:
+            middle = ": "
+        stream.write(rep)
+        stream.write(middle)
+        self._format(
+            v, stream, indent + len(rep) + len(middle), allowance, context, level
+        )
+
+    # Follow what scikit-learn did here and copy _dispatch to prevent instances
+    # of the builtin PrettyPrinter class to call methods of
+    # _BaseObjectPrettyPrinter (see scikit-learn Github issue 12906)
+    # mypy error: "Type[PrettyPrinter]" has no attribute "_dispatch"
+    _dispatch = pprint.PrettyPrinter._dispatch.copy()  # type: ignore
+    _dispatch[BaseObject.__repr__] = _pprint_object
+    _dispatch[KeyValTuple.__repr__] = _pprint_key_val_tuple
+
+
+def _safe_repr(obj, context, maxlevels, level, changed_only=False):
+    """Safe string representation logic.
+
+    Same as the builtin _safe_repr, with added support for BaseObjects.
+    """
+    typ = type(obj)
+
+    if typ in pprint._builtin_scalars:
+        return repr(obj), True, False
+
+    r = getattr(typ, "__repr__", None)
+    if issubclass(typ, dict) and r is dict.__repr__:
+        if not obj:
+            return "{}", True, False
+        objid = id(obj)
+        if maxlevels and level >= maxlevels:
+            return "{...}", False, objid in context
+        if objid in context:
+            return pprint._recursion(obj), False, True
+        context[objid] = 1
+        readable = True
+        recursive = False
+        components = []
+        append = components.append
+        level += 1
+        saferepr = _safe_repr
+        items = sorted(obj.items(), key=pprint._safe_tuple)
+        for k, v in items:
+            krepr, kreadable, krecur = saferepr(
+                k, context, maxlevels, level, changed_only=changed_only
+            )
+            vrepr, vreadable, vrecur = saferepr(
+                v, context, maxlevels, level, changed_only=changed_only
+            )
+            append("%s: %s" % (krepr, vrepr))
+            readable = readable and kreadable and vreadable
+            if krecur or vrecur:
+                recursive = True
+        del context[objid]
+        return "{%s}" % ", ".join(components), readable, recursive
+
+    if (issubclass(typ, list) and r is list.__repr__) or (
+        issubclass(typ, tuple) and r is tuple.__repr__
+    ):
+        if issubclass(typ, list):
+            if not obj:
+                return "[]", True, False
+            format_ = "[%s]"
+        elif len(obj) == 1:
+            format_ = "(%s,)"
+        else:
+            if not obj:
+                return "()", True, False
+            format_ = "(%s)"
+        objid = id(obj)
+        if maxlevels and level >= maxlevels:
+            return format_ % "...", False, objid in context
+        if objid in context:
+            return pprint._recursion(obj), False, True
+        context[objid] = 1
+        readable = True
+        recursive = False
+        components = []
+        append = components.append
+        level += 1
+        for o in obj:
+            orepr, oreadable, orecur = _safe_repr(
+                o, context, maxlevels, level, changed_only=changed_only
+            )
+            append(orepr)
+            if not oreadable:
+                readable = False
+            if orecur:
+                recursive = True
+        del context[objid]
+        return format_ % ", ".join(components), readable, recursive
+
+    if issubclass(typ, BaseObject):
+        objid = id(obj)
+        if maxlevels and level >= maxlevels:
+            return "{...}", False, objid in context
+        if objid in context:
+            return pprint._recursion(obj), False, True
+        context[objid] = 1
+        readable = True
+        recursive = False
+        if changed_only:
+            params = _changed_params(obj)
+        else:
+            params = obj.get_params(deep=False)
+        components = []
+        append = components.append
+        level += 1
+        saferepr = _safe_repr
+        items = sorted(params.items(), key=pprint._safe_tuple)
+        for k, v in items:
+            krepr, kreadable, krecur = saferepr(
+                k, context, maxlevels, level, changed_only=changed_only
+            )
+            vrepr, vreadable, vrecur = saferepr(
+                v, context, maxlevels, level, changed_only=changed_only
+            )
+            append("%s=%s" % (krepr.strip("'"), vrepr))
+            readable = readable and kreadable and vreadable
+            if krecur or vrecur:
+                recursive = True
+        del context[objid]
+        return ("%s(%s)" % (typ.__name__, ", ".join(components)), readable, recursive)
+
+    rep = repr(obj)
+    return rep, (rep and not rep.startswith("<")), False
```

### Comparing `skbase-0.4.5/skbase/base/_tagmanager.py` & `skbase-0.4.6/skbase/base/_tagmanager.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,217 +1,217 @@
-# -*- coding: utf-8 -*-
-"""Mixin class for flag and configuration settings management."""
-# copyright: sktime developers, BSD-3-Clause License (see LICENSE file)
-
-__author__ = ["fkiraly"]
-__all__ = ["_FlagManager"]
-
-
-import inspect
-from copy import deepcopy
-
-
-class _FlagManager:
-    """Mixin class for flag and configuration settings management."""
-
-    @classmethod
-    def _get_class_flags(cls, flag_attr_name="_flags"):
-        """Get class flags from estimator class and all its parent classes.
-
-        Parameters
-        ----------
-        flag_attr_name : str, default = "_flags"
-            Name of the flag attribute that is read.
-
-        Returns
-        -------
-        collected_flags : dict
-            Dictionary of flag name : flag value pairs. Collected from _flags
-            class attribute via nested inheritance. NOT overridden by dynamic
-            flags set by set_flags or clone_flags.
-        """
-        collected_flags = {}
-
-        # We exclude the last two parent classes: sklearn.base.BaseEstimator and
-        # the basic Python object.
-        for parent_class in reversed(inspect.getmro(cls)[:-2]):
-            if hasattr(parent_class, flag_attr_name):
-                # Need the if here because mixins might not have _more_flags
-                # but might do redundant work in estimators
-                # (i.e. calling more flags on BaseEstimator multiple times)
-                more_flags = getattr(parent_class, flag_attr_name)
-                collected_flags.update(more_flags)
-
-        return deepcopy(collected_flags)
-
-    @classmethod
-    def _get_class_flag(
-        cls, flag_name, flag_value_default=None, flag_attr_name="_flags"
-    ):
-        """Get flag value from estimator class (only class flags).
-
-        Parameters
-        ----------
-        flag_name : str
-            Name of flag value.
-        flag_value_default : any type
-            Default/fallback value if flag is not found.
-        flag_attr_name : str, default = "_flags"
-            Name of the flag attribute that is read.
-
-        Returns
-        -------
-        flag_value
-            Value of `flag_name` flag in self. If not found, `flag_value_default`.
-        """
-        collected_flags = cls._get_class_flags(flag_attr_name=flag_attr_name)
-
-        return collected_flags.get(flag_name, flag_value_default)
-
-    def _init_flags(self, flag_attr_name="_flags"):
-        """Create dynamic flag dictionary in self.
-
-        Should be called in __init__ of the host class.
-        Creates attribute [flag_attr_name]_dynamic containing an empty dict.
-
-        Parameters
-        ----------
-        flag_attr_name : str, default = "_flags"
-            Name of the flag attribute that is read.
-
-        Returns
-        -------
-        self : reference to self
-        """
-        setattr(self, f"{flag_attr_name}_dynamic", {})
-        return self
-
-    def _get_flags(self, flag_attr_name="_flags"):
-        """Get flags from estimator class and dynamic flag overrides.
-
-        Parameters
-        ----------
-        flag_attr_name : str, default = "_flags"
-            Name of the flag attribute that is read.
-
-        Returns
-        -------
-        collected_flags : dict
-            Dictionary of flag name : flag value pairs. Collected from flag_attr_name
-            class attribute via nested inheritance and then any overrides
-            and new flags from [flag_attr_name]_dynamic object attribute.
-        """
-        collected_flags = self._get_class_flags(flag_attr_name=flag_attr_name)
-
-        if hasattr(self, f"{flag_attr_name}_dynamic"):
-            collected_flags.update(getattr(self, f"{flag_attr_name}_dynamic"))
-
-        return deepcopy(collected_flags)
-
-    def _get_flag(
-        self,
-        flag_name,
-        flag_value_default=None,
-        raise_error=True,
-        flag_attr_name="_flags",
-    ):
-        """Get flag value from estimator class and dynamic flag overrides.
-
-        Parameters
-        ----------
-        flag_name : str
-            Name of flag to be retrieved.
-        flag_value_default : any type, default=None
-            Default/fallback value if flag is not found
-        raise_error : bool
-            Whether a `ValueError` is raised when the flag is not found.
-        flag_attr_name : str, default = "_flags"
-            Name of the flag attribute that is read.
-
-        Returns
-        -------
-        flag_value :
-            Value of the `flag_name` flag in self. If not found, returns an error if
-            raise_error is True, otherwise it returns `flag_value_default`.
-
-        Raises
-        ------
-        ValueError
-            if `raise_error` is `True`, i.e.,
-            if `flag_name` is not in `self.get_flags().keys()`
-        """
-        collected_flags = self._get_flags(flag_attr_name=flag_attr_name)
-
-        flag_value = collected_flags.get(flag_name, flag_value_default)
-
-        if raise_error and flag_name not in collected_flags.keys():
-            raise ValueError(f"Tag with name {flag_name} could not be found.")
-
-        return flag_value
-
-    def _set_flags(self, flag_attr_name="_flags", **flag_dict):
-        """Set dynamic flags to given values.
-
-        Parameters
-        ----------
-        flag_dict : dict
-            Dictionary of flag name : flag value pairs.
-        flag_attr_name : str, default = "_flags"
-            Name of the flag attribute that is read.
-
-        Returns
-        -------
-        self
-            Reference to self.
-
-        Notes
-        -----
-        Changes object state by settting flag values in flag_dict as dynamic flags
-        in self.
-        """
-        flag_update = deepcopy(flag_dict)
-        dynamic_flags = f"{flag_attr_name}_dynamic"
-        if hasattr(self, dynamic_flags):
-            getattr(self, dynamic_flags).update(flag_update)
-        else:
-            setattr(self, dynamic_flags, flag_update)
-
-        return self
-
-    def _clone_flags(self, estimator, flag_names=None, flag_attr_name="_flags"):
-        """clone/mirror flags from another estimator as dynamic override.
-
-        Parameters
-        ----------
-        estimator : estimator inheriting from :class:BaseEstimator
-        flag_names : str or list of str, default = None
-            Names of flags to clone. If None then all flags in estimator are used
-            as `flag_names`.
-        flag_attr_name : str, default = "_flags"
-            Name of the flag attribute that is read.
-
-        Returns
-        -------
-        self
-            Reference to self.
-
-        Notes
-        -----
-        Changes object state by setting flag values in flag_set from estimator as
-        dynamic flags in self.
-        """
-        flags_est = deepcopy(estimator._get_flags(flag_attr_name=flag_attr_name))
-
-        # if flag_set is not passed, default is all flags in estimator
-        if flag_names is None:
-            flag_names = flags_est.keys()
-        else:
-            # if flag_set is passed, intersect keys with flags in estimator
-            if not isinstance(flag_names, list):
-                flag_names = [flag_names]
-            flag_names = [key for key in flag_names if key in flags_est.keys()]
-
-        update_dict = {key: flags_est[key] for key in flag_names}
-
-        self._set_flags(flag_attr_name=flag_attr_name, **update_dict)
-
-        return self
+# -*- coding: utf-8 -*-
+"""Mixin class for flag and configuration settings management."""
+# copyright: sktime developers, BSD-3-Clause License (see LICENSE file)
+
+__author__ = ["fkiraly"]
+__all__ = ["_FlagManager"]
+
+
+import inspect
+from copy import deepcopy
+
+
+class _FlagManager:
+    """Mixin class for flag and configuration settings management."""
+
+    @classmethod
+    def _get_class_flags(cls, flag_attr_name="_flags"):
+        """Get class flags from estimator class and all its parent classes.
+
+        Parameters
+        ----------
+        flag_attr_name : str, default = "_flags"
+            Name of the flag attribute that is read.
+
+        Returns
+        -------
+        collected_flags : dict
+            Dictionary of flag name : flag value pairs. Collected from _flags
+            class attribute via nested inheritance. NOT overridden by dynamic
+            flags set by set_flags or clone_flags.
+        """
+        collected_flags = {}
+
+        # We exclude the last two parent classes: sklearn.base.BaseEstimator and
+        # the basic Python object.
+        for parent_class in reversed(inspect.getmro(cls)[:-2]):
+            if hasattr(parent_class, flag_attr_name):
+                # Need the if here because mixins might not have _more_flags
+                # but might do redundant work in estimators
+                # (i.e. calling more flags on BaseEstimator multiple times)
+                more_flags = getattr(parent_class, flag_attr_name)
+                collected_flags.update(more_flags)
+
+        return deepcopy(collected_flags)
+
+    @classmethod
+    def _get_class_flag(
+        cls, flag_name, flag_value_default=None, flag_attr_name="_flags"
+    ):
+        """Get flag value from estimator class (only class flags).
+
+        Parameters
+        ----------
+        flag_name : str
+            Name of flag value.
+        flag_value_default : any type
+            Default/fallback value if flag is not found.
+        flag_attr_name : str, default = "_flags"
+            Name of the flag attribute that is read.
+
+        Returns
+        -------
+        flag_value
+            Value of `flag_name` flag in self. If not found, `flag_value_default`.
+        """
+        collected_flags = cls._get_class_flags(flag_attr_name=flag_attr_name)
+
+        return collected_flags.get(flag_name, flag_value_default)
+
+    def _init_flags(self, flag_attr_name="_flags"):
+        """Create dynamic flag dictionary in self.
+
+        Should be called in __init__ of the host class.
+        Creates attribute [flag_attr_name]_dynamic containing an empty dict.
+
+        Parameters
+        ----------
+        flag_attr_name : str, default = "_flags"
+            Name of the flag attribute that is read.
+
+        Returns
+        -------
+        self : reference to self
+        """
+        setattr(self, f"{flag_attr_name}_dynamic", {})
+        return self
+
+    def _get_flags(self, flag_attr_name="_flags"):
+        """Get flags from estimator class and dynamic flag overrides.
+
+        Parameters
+        ----------
+        flag_attr_name : str, default = "_flags"
+            Name of the flag attribute that is read.
+
+        Returns
+        -------
+        collected_flags : dict
+            Dictionary of flag name : flag value pairs. Collected from flag_attr_name
+            class attribute via nested inheritance and then any overrides
+            and new flags from [flag_attr_name]_dynamic object attribute.
+        """
+        collected_flags = self._get_class_flags(flag_attr_name=flag_attr_name)
+
+        if hasattr(self, f"{flag_attr_name}_dynamic"):
+            collected_flags.update(getattr(self, f"{flag_attr_name}_dynamic"))
+
+        return deepcopy(collected_flags)
+
+    def _get_flag(
+        self,
+        flag_name,
+        flag_value_default=None,
+        raise_error=True,
+        flag_attr_name="_flags",
+    ):
+        """Get flag value from estimator class and dynamic flag overrides.
+
+        Parameters
+        ----------
+        flag_name : str
+            Name of flag to be retrieved.
+        flag_value_default : any type, default=None
+            Default/fallback value if flag is not found
+        raise_error : bool
+            Whether a `ValueError` is raised when the flag is not found.
+        flag_attr_name : str, default = "_flags"
+            Name of the flag attribute that is read.
+
+        Returns
+        -------
+        flag_value :
+            Value of the `flag_name` flag in self. If not found, returns an error if
+            raise_error is True, otherwise it returns `flag_value_default`.
+
+        Raises
+        ------
+        ValueError
+            if `raise_error` is `True`, i.e.,
+            if `flag_name` is not in `self.get_flags().keys()`
+        """
+        collected_flags = self._get_flags(flag_attr_name=flag_attr_name)
+
+        flag_value = collected_flags.get(flag_name, flag_value_default)
+
+        if raise_error and flag_name not in collected_flags.keys():
+            raise ValueError(f"Tag with name {flag_name} could not be found.")
+
+        return flag_value
+
+    def _set_flags(self, flag_attr_name="_flags", **flag_dict):
+        """Set dynamic flags to given values.
+
+        Parameters
+        ----------
+        flag_dict : dict
+            Dictionary of flag name : flag value pairs.
+        flag_attr_name : str, default = "_flags"
+            Name of the flag attribute that is read.
+
+        Returns
+        -------
+        self
+            Reference to self.
+
+        Notes
+        -----
+        Changes object state by settting flag values in flag_dict as dynamic flags
+        in self.
+        """
+        flag_update = deepcopy(flag_dict)
+        dynamic_flags = f"{flag_attr_name}_dynamic"
+        if hasattr(self, dynamic_flags):
+            getattr(self, dynamic_flags).update(flag_update)
+        else:
+            setattr(self, dynamic_flags, flag_update)
+
+        return self
+
+    def _clone_flags(self, estimator, flag_names=None, flag_attr_name="_flags"):
+        """clone/mirror flags from another estimator as dynamic override.
+
+        Parameters
+        ----------
+        estimator : estimator inheriting from :class:BaseEstimator
+        flag_names : str or list of str, default = None
+            Names of flags to clone. If None then all flags in estimator are used
+            as `flag_names`.
+        flag_attr_name : str, default = "_flags"
+            Name of the flag attribute that is read.
+
+        Returns
+        -------
+        self
+            Reference to self.
+
+        Notes
+        -----
+        Changes object state by setting flag values in flag_set from estimator as
+        dynamic flags in self.
+        """
+        flags_est = deepcopy(estimator._get_flags(flag_attr_name=flag_attr_name))
+
+        # if flag_set is not passed, default is all flags in estimator
+        if flag_names is None:
+            flag_names = flags_est.keys()
+        else:
+            # if flag_set is passed, intersect keys with flags in estimator
+            if not isinstance(flag_names, list):
+                flag_names = [flag_names]
+            flag_names = [key for key in flag_names if key in flags_est.keys()]
+
+        update_dict = {key: flags_est[key] for key in flag_names}
+
+        self._set_flags(flag_attr_name=flag_attr_name, **update_dict)
+
+        return self
```

### Comparing `skbase-0.4.5/skbase/lookup/__init__.py` & `skbase-0.4.6/skbase/lookup/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tools to lookup information on code artifacts in a Python package or module.
-
-This module exports the following functions:
-
-package_metadata()
-    Walk package and return metadata on included classes and functions by module.
-    Users can optionally filter the information to return.
-all_objects()
-    Lookup BaseObject descendants in a package or module. Users can optionally filter
-    the information to return.
-"""
-# all_objects is based on the sktime all_estimator retrieval utility, which
-# is based on the sklearn estimator retrieval utility of the same name
-# See https://github.com/scikit-learn/scikit-learn/blob/main/COPYING and
-# https://github.com/sktime/sktime/blob/main/LICENSE
-from typing import List
-
-from skbase.lookup._lookup import all_objects, get_package_metadata
-
-__all__: List[str] = ["all_objects", "get_package_metadata"]
-__author__: List[str] = [
-    "fkiraly",
-    "mloning",
-    "katiebuc",
-    "miraep8",
-    "xloem",
-    "rnkuhns",
-]
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tools to lookup information on code artifacts in a Python package or module.
+
+This module exports the following functions:
+
+package_metadata()
+    Walk package and return metadata on included classes and functions by module.
+    Users can optionally filter the information to return.
+all_objects()
+    Lookup BaseObject descendants in a package or module. Users can optionally filter
+    the information to return.
+"""
+# all_objects is based on the sktime all_estimator retrieval utility, which
+# is based on the sklearn estimator retrieval utility of the same name
+# See https://github.com/scikit-learn/scikit-learn/blob/main/COPYING and
+# https://github.com/sktime/sktime/blob/main/LICENSE
+from typing import List
+
+from skbase.lookup._lookup import all_objects, get_package_metadata
+
+__all__: List[str] = ["all_objects", "get_package_metadata"]
+__author__: List[str] = [
+    "fkiraly",
+    "mloning",
+    "katiebuc",
+    "miraep8",
+    "xloem",
+    "rnkuhns",
+]
```

### Comparing `skbase-0.4.5/skbase/lookup/_lookup.py` & `skbase-0.4.6/skbase/lookup/_lookup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,998 +1,1009 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tools to lookup information on code artifacts in a Python package or module.
-
-This module exports the following methods for registry lookup:
-
-package_metadata()
-    Walk package and return metadata on included classes and functions by module.
-all_objects(object_types, filter_tags)
-    Look (and optionally filter) BaseObject descendants in a package or module.
-"""
-# all_objects is based on the sktime all_estimator retrieval utility, which
-# is based on the sklearn estimator retrieval utility of the same name
-# See https://github.com/scikit-learn/scikit-learn/blob/main/COPYING and
-# https://github.com/sktime/sktime/blob/main/LICENSE
-import importlib
-import inspect
-import io
-import os
-import pathlib
-import pkgutil
-import sys
-import warnings
-from collections.abc import Iterable
-from copy import deepcopy
-from operator import itemgetter
-from types import ModuleType
-from typing import Any, List, Mapping, MutableMapping, Optional, Sequence, Tuple, Union
-
-from skbase.base import BaseObject
-from skbase.validate import check_sequence
-
-__all__: List[str] = ["all_objects", "get_package_metadata"]
-__author__: List[str] = [
-    "fkiraly",
-    "mloning",
-    "katiebuc",
-    "miraep8",
-    "xloem",
-    "rnkuhns",
-]
-
-# the below is commented out to avoid a dependency on typing_extensions
-# but still left in place as it is informative regarding expected return type
-
-# class ClassInfo(TypedDict):
-#     """Type definitions for information on a module's classes."""
-
-#     klass: Type
-#     name: str
-#     description: str
-#     tags: MutableMapping[str, Any]
-#     is_concrete_implementation: bool
-#     is_base_class: bool
-#     is_base_object: bool
-#     authors: Optional[Union[List[str], str]]
-#     module_name: str
-
-
-# class FunctionInfo(TypedDict):
-#     """Information on a module's functions."""
-
-#     func: FunctionType
-#     name: str
-#     description: str
-#     module_name: str
-
-
-# class ModuleInfo(TypedDict):
-#     """Module information type definitions."""
-
-#     path: str
-#     name: str
-#     classes: MutableMapping[str, ClassInfo]
-#     functions: MutableMapping[str, FunctionInfo]
-#     __all__: List[str]
-#     authors: str
-#     is_package: bool
-#     contains_concrete_class_implementations: bool
-#     contains_base_classes: bool
-#     contains_base_objects: bool
-
-
-def _is_non_public_module(module_name: str) -> bool:
-    """Determine if a module is non-public or not.
-
-    Parameters
-    ----------
-    module_name : str
-        Name of the module.
-
-    Returns
-    -------
-    is_non_public : bool
-        Whether the module is non-public or not.
-    """
-    if not isinstance(module_name, str):
-        raise ValueError(
-            f"Parameter `module_name` should be str, but found {type(module_name)}."
-        )
-    is_non_public: bool = "._" in module_name or module_name.startswith("_")
-    return is_non_public
-
-
-def _is_ignored_module(
-    module_name: str, modules_to_ignore: Union[str, List[str], Tuple[str]] = None
-) -> bool:
-    """Determine if module is one of the ignored modules.
-
-    Ignores a module if identical with, or submodule of a module whose name
-    is in the list/tuple `modules_to_ignore`.
-
-    E.g., if `modules_to_ignore` contains the string `"foo"`, then `True` will be
-    returned for `module_name`-s `"bar.foo"`, `"foo"`, `"foo.bar"`,
-    `"bar.foo.bar"`, etc.
-
-    Paramters
-    ---------
-    module_name : str
-        Name of the module.
-    modules_to_ignore : str, list[str] or tuple[str]
-        The modules that should be ignored when walking the package.
-
-    Returns
-    -------
-    is_ignored : bool
-        Whether the module is an ignrored module or not.
-    """
-    if isinstance(modules_to_ignore, str):
-        modules_to_ignore = (modules_to_ignore,)
-    is_ignored: bool
-    if modules_to_ignore is None:
-        is_ignored = False
-    else:
-        is_ignored = any(part in modules_to_ignore for part in module_name.split("."))
-
-    return is_ignored
-
-
-def _filter_by_class(
-    klass: type, class_filter: Optional[Union[type, Sequence[type]]] = None
-) -> bool:
-    """Determine if a class is a subclass of the supplied classes.
-
-    Parameters
-    ----------
-    klass : object
-        Class to check.
-    class_filter : objects or iterable of objects
-        Classes that `klass` is checked against.
-
-    Returns
-    -------
-    is_subclass : bool
-        Whether the input class is a subclass of the `class_filter`.
-        If `class_filter` was `None`, returns `True`.
-    """
-    if class_filter is None:
-        return True
-
-    if isinstance(class_filter, Iterable) and not isinstance(class_filter, tuple):
-        class_filter = tuple(class_filter)
-    return issubclass(klass, class_filter)
-
-
-def _filter_by_tags(obj, tag_filter=None, as_dataframe=True):
-    """Check whether estimator satisfies tag_filter condition.
-
-    Parameters
-    ----------
-    obj : BaseObject, an sktime estimator
-    tag_filter : dict of (str or list of str), default=None
-        subsets the returned estimators as follows:
-        each key/value pair is statement in "and"/conjunction
-
-        * key is tag name to sub-set on
-        * value str or list of string are tag values
-        * condition is "key must be equal to value, or in set(value)"
-
-    Returns
-    -------
-    cond_sat: bool, whether estimator satisfies condition in `tag_filter`
-        if `tag_filter` was None, returns `True`
-    """
-    if tag_filter is None:
-        return True
-
-    if not isinstance(tag_filter, (str, Iterable, dict)):
-        raise TypeError(
-            "tag_filter argument of _filter_by_tags must be "
-            "a dict with str keys, str, or iterable of str, "
-            f"but found tag_filter of type {type(tag_filter)}"
-        )
-
-    if not hasattr(obj, "get_class_tag"):
-        return False
-
-    klass_tags = obj.get_class_tags().keys()
-
-    # case: tag_filter is string
-    if isinstance(tag_filter, str):
-        return tag_filter in klass_tags
-
-    # case: tag_filter is iterable of str but not dict
-    # If a iterable of strings is provided, check that all are in the returned tag_dict
-    if isinstance(tag_filter, Iterable) and not isinstance(tag_filter, dict):
-        if not all(isinstance(t, str) for t in tag_filter):
-            raise ValueError(
-                "tag_filter argument of _filter_by_tags must be "
-                f"a dict with str keys, str, or iterable of str, but found {tag_filter}"
-            )
-        return all(tag in klass_tags for tag in tag_filter)
-
-    # case: tag_filter is dict
-    if not all(isinstance(t, str) for t in tag_filter.keys()):
-        raise ValueError(
-            "tag_filter argument of _filter_by_tags must be "
-            f"a dict with str keys, str, or iterable of str, but found {tag_filter}"
-        )
-
-    cond_sat = True
-
-    for key, value in tag_filter.items():
-        if not isinstance(value, list):
-            value = [value]
-        cond_sat = cond_sat and obj.get_class_tag(key) in set(value)
-
-    return cond_sat
-
-
-def _walk(root, exclude=None, prefix=""):
-    """Recursively return all modules and sub-modules as list of strings.
-
-    Unlike pkgutil.walk_packages, does not import modules on exclusion list.
-
-    Parameters
-    ----------
-    root : str or path-like
-        Root path in which to look for submodules. Can be a string path,
-        pathlib.Path or other path-like object.
-    exclude : tuple of str or None, optional, default = None
-        List of sub-modules to ignore in the return, including sub-modules
-    prefix: str, optional, default = ""
-        This str is pre-appended to all strings in the return
-
-    Yields
-    ------
-    str : sub-module strings
-        Iterates over all sub-modules of root that do not contain any of the
-        strings on the `exclude` list string is prefixed by the string `prefix`
-    """
-    if not isinstance(root, str):
-        root = str(root)
-    for loader, module_name, is_pkg in pkgutil.iter_modules(path=[root]):
-        if not _is_ignored_module(module_name, modules_to_ignore=exclude):
-            yield f"{prefix}{module_name}", is_pkg, loader
-            if is_pkg:
-                yield from (
-                    (f"{prefix}{module_name}.{x[0]}", x[1], x[2])
-                    for x in _walk(f"{root}/{module_name}", exclude=exclude)
-                )
-
-
-def _import_module(
-    module: Union[str, importlib.machinery.SourceFileLoader],
-    suppress_import_stdout: bool = True,
-) -> ModuleType:
-    """Import a module, while optionally suppressing import standard out.
-
-    Parameters
-    ----------
-    module : str or importlib.machinery.SourceFileLoader
-        Name of the module to be imported or a SourceFileLoader to load a module.
-    suppress_import_stdout : bool, default=True
-        Whether to suppress stdout printout upon import.
-
-    Returns
-    -------
-    imported_mod : ModuleType
-        The module that was imported.
-    """
-    if isinstance(module, str):
-        if suppress_import_stdout:
-            # setup text trap, import, then restore
-            sys.stdout = io.StringIO()
-            imported_mod = importlib.import_module(module)
-            sys.stdout = sys.__stdout__
-        else:
-            imported_mod = importlib.import_module(module)
-    elif isinstance(module, importlib.machinery.SourceFileLoader):
-        if suppress_import_stdout:
-            sys.stdout = io.StringIO()
-            imported_mod = module.load_module()
-            sys.stdout = sys.__stdout__
-        else:
-            imported_mod = module.load_module()
-    else:
-        raise ValueError(
-            "`module` should be string module name or instance of "
-            "importlib.machinery.SourceFileLoader."
-        )
-    return imported_mod
-
-
-def _determine_module_path(
-    package_name: str, path: Optional[Union[str, pathlib.Path]] = None
-) -> Tuple[ModuleType, str, importlib.machinery.SourceFileLoader]:
-    """Determine a package's path information.
-
-    Parameters
-    ----------
-    package_name : str
-        The name of the package/module to return metadata for.
-
-        - If `path` is not None, this should be the name of the package/module
-          associated with the path. `package_name` (with "." appended at end)
-          will be used as prefix for any submodules/packages when walking
-          the provided `path`.
-        - If `path` is None, then package_name is assumed to be an importable
-          package or module and the `path` to `package_name` will be determined
-          from its import.
-
-    path : str or absolute pathlib.Path, default=None
-        If provided, this should be the path that should be used as root
-        to find any modules or submodules.
-
-    Returns
-    -------
-    module, path_, loader : ModuleType, str, importlib.machinery.SourceFileLoader
-        Returns the module, a string of its path and its SourceFileLoader.
-    """
-    if not isinstance(package_name, str):
-        raise ValueError(
-            "`package_name` must be the string name of a package or module."
-            "For example, 'some_package' or 'some_package.some_module'."
-        )
-
-    def _instantiate_loader(package_name: str, path: str):
-        if path.endswith(".py"):
-            loader = importlib.machinery.SourceFileLoader(package_name, path)
-        elif os.path.exists(path + "/__init__.py"):
-            loader = importlib.machinery.SourceFileLoader(
-                package_name, path + "/__init__.py"
-            )
-        else:
-            loader = importlib.machinery.SourceFileLoader(package_name, path)
-        return loader
-
-    if path is None:
-        module = _import_module(package_name, suppress_import_stdout=False)
-        if hasattr(module, "__path__") and (
-            module.__path__ is not None and len(module.__path__) > 0
-        ):
-            path_ = module.__path__[0]
-        elif hasattr(module, "__file__") and module.__file__ is not None:
-            path_ = module.__file__.split(".")[0]
-        else:
-            raise ValueError(
-                f"Unable to determine path for provided `package_name`: {package_name} "
-                "from the imported module. Try explicitly providing the `path`."
-            )
-        loader = _instantiate_loader(package_name, path_)
-    else:
-        # Make sure path is str and not a pathlib.Path
-        if isinstance(path, (pathlib.Path, str)):
-            path_ = str(path.absolute()) if isinstance(path, pathlib.Path) else path
-            # Use the provided path and package name to load the module
-            # if both available.
-            try:
-                loader = _instantiate_loader(package_name, path_)
-                module = _import_module(loader, suppress_import_stdout=False)
-            except ImportError as exc:
-                raise ValueError(
-                    f"Unable to import a package named {package_name} based "
-                    f"on provided `path`: {path_}."
-                ) from exc
-        else:
-            raise ValueError(
-                f"`path` must be a str path or pathlib.Path, but is type {type(path)}."
-            )
-
-    return module, path_, loader
-
-
-def _get_module_info(
-    module: ModuleType,
-    is_pkg: bool,
-    path: str,
-    package_base_classes: Union[type, Tuple[type, ...]],
-    exclude_non_public_items: bool = True,
-    class_filter: Optional[Union[type, Sequence[type]]] = None,
-    tag_filter: Optional[Union[str, Sequence[str], Mapping[str, Any]]] = None,
-    classes_to_exclude: Optional[Union[type, Sequence[type]]] = None,
-) -> dict:  # of ModuleInfo type
-    # Make package_base_classes a tuple if it was supplied as a class
-    base_classes_none = False
-    if isinstance(package_base_classes, Iterable):
-        package_base_classes = tuple(package_base_classes)
-    elif not isinstance(package_base_classes, tuple):
-        if package_base_classes is None:
-            base_classes_none = True
-        package_base_classes = (package_base_classes,)
-
-    exclude_classes: Optional[Sequence[type]]
-    if classes_to_exclude is None:
-        exclude_classes = classes_to_exclude
-    elif isinstance(classes_to_exclude, Sequence):
-        exclude_classes = classes_to_exclude
-    elif inspect.isclass(classes_to_exclude):
-        exclude_classes = (classes_to_exclude,)
-
-    designed_imports: List[str] = getattr(module, "__all__", [])
-    authors: Union[str, List[str]] = getattr(module, "__author__", [])
-    if isinstance(authors, (list, tuple)):
-        authors = ", ".join(authors)
-    # Compile information on classes in the module
-    module_classes: MutableMapping = {}  # of ClassInfo type
-    for name, klass in inspect.getmembers(module, inspect.isclass):
-        # Skip a class if non-public items should be excluded and it starts with "_"
-        if (
-            (exclude_non_public_items and klass.__name__.startswith("_"))
-            or (exclude_classes is not None and klass in exclude_classes)
-            or not _filter_by_tags(klass, tag_filter=tag_filter)
-            or not _filter_by_class(klass, class_filter=class_filter)
-        ):
-            continue
-        # Otherwise, store info about the class
-        if klass.__module__ == module.__name__ or name in designed_imports:
-            klass_authors = getattr(klass, "__author__", authors)
-            if isinstance(klass_authors, (list, tuple)):
-                klass_authors = ", ".join(klass_authors)
-            if base_classes_none:
-                concrete_implementation = False
-            else:
-                concrete_implementation = (
-                    issubclass(klass, package_base_classes)
-                    and klass not in package_base_classes
-                )
-            module_classes[name] = {
-                "klass": klass,
-                "name": klass.__name__,
-                "description": (
-                    "" if klass.__doc__ is None else klass.__doc__.split("\n")[0]
-                ),
-                "tags": (
-                    klass.get_class_tags() if hasattr(klass, "get_class_tags") else None
-                ),
-                "is_concrete_implementation": concrete_implementation,
-                "is_base_class": klass in package_base_classes,
-                "is_base_object": issubclass(klass, BaseObject),
-                "authors": klass_authors,
-                "module_name": module.__name__,
-            }
-
-    module_functions: MutableMapping = {}  # of FunctionInfo type
-    for name, func in inspect.getmembers(module, inspect.isfunction):
-        if func.__module__ == module.__name__ or name in designed_imports:
-            # Skip a class if non-public items should be excluded and it starts with "_"
-            if exclude_non_public_items and func.__name__.startswith("_"):
-                continue
-            # Otherwise, store info about the class
-            module_functions[name] = {
-                "func": func,
-                "name": func.__name__,
-                "description": (
-                    "" if func.__doc__ is None else func.__doc__.split("\n")[0]
-                ),
-                "module_name": module.__name__,
-            }
-
-    # Combine all the information on the module together
-    module_info = {  # of ModuleInfo type
-        "path": path,
-        "name": module.__name__,
-        "classes": module_classes,
-        "functions": module_functions,
-        "__all__": designed_imports,
-        "authors": authors,
-        "is_package": is_pkg,
-        "contains_concrete_class_implementations": any(
-            v["is_concrete_implementation"] for v in module_classes.values()
-        ),
-        "contains_base_classes": any(
-            v["is_base_class"] for v in module_classes.values()
-        ),
-        "contains_base_objects": any(
-            v["is_base_object"] for v in module_classes.values()
-        ),
-    }
-    return module_info
-
-
-def get_package_metadata(
-    package_name: str,
-    path: Optional[str] = None,
-    recursive: bool = True,
-    exclude_non_public_items: bool = True,
-    exclude_non_public_modules: bool = True,
-    modules_to_ignore: Union[str, List[str], Tuple[str]] = ("tests",),
-    package_base_classes: Union[type, Tuple[type, ...]] = (BaseObject,),
-    class_filter: Optional[Union[type, Sequence[type]]] = None,
-    tag_filter: Optional[Union[str, Sequence[str], Mapping[str, Any]]] = None,
-    classes_to_exclude: Optional[Union[type, Sequence[type]]] = None,
-    suppress_import_stdout: bool = True,
-) -> Mapping:  # of ModuleInfo type
-    """Return a dictionary mapping all package modules to their metadata.
-
-    Parameters
-    ----------
-    package_name : str
-        The name of the package/module to return metadata for.
-
-        - If `path` is not None, this should be the name of the package/module
-          associated with the path. `package_name` (with "." appended at end)
-          will be used as prefix for any submodules/packages when walking
-          the provided `path`.
-        - If `path` is None, then package_name is assumed to be an importable
-          package or module and the `path` to `package_name` will be determined
-          from its import.
-
-    path : str, default=None
-        If provided, this should be the path that should be used as root
-        to find any modules or submodules.
-    recursive : bool, default=True
-        Whether to recursively walk through submodules.
-
-        - If True, then submodules of submodules and so on are found.
-        - If False, then only first-level submodules of `package` are found.
-
-    exclude_non_public_items : bool, default=True
-        Whether to exclude nonpublic functions and classes (where name starts
-        with a leading underscore).
-    exclude_non_public_modules : bool, default=True
-        Whether to exclude nonpublic modules (modules where names start with
-        a leading underscore).
-    modules_to_ignore : str, tuple[str] or list[str], default="tests"
-        The modules that should be ignored when searching across the modules to
-        gather objects. If passed, `all_objects` ignores modules or submodules
-        of a module whose name is in the provided string(s). E.g., if
-        `modules_to_ignore` contains the string `"foo"`, then `"bar.foo"`,
-        `"foo"`, `"foo.bar"`, `"bar.foo.bar"` are ignored.
-    package_base_classes: type or Sequence[type], default = (BaseObject,)
-        The base classes used to determine if any classes found in metadata descend
-        from a base class.
-    class_filter : object or Sequence[object], default=None
-        Classes that `klass` is checked against. Only classes that are subclasses
-        of the supplied `class_filter` are returned in metadata.
-    tag_filter : str, Sequence[str] or dict[str, Any], default=None
-        Filter used to determine if `klass` has tag or expected tag values.
-
-        - If a str or list of strings is provided, the return will be filtered
-          to keep classes that have all the tag(s) specified by the strings.
-        - If a dict is provided, the return will be filtered to keep classes
-          that have all dict keys as tags. Tag values are also checked such that:
-
-          - If a dict key maps to a single value only classes with tag values equal
-            to the value are returned.
-          - If a dict key maps to multiple values (e.g., list) only classes with
-            tag values in these values are returned.
-
-    classes_to_exclude: objects or iterable of object, default=None
-        Classes to exclude from returned metadata.
-
-    Other Parameters
-    ----------------
-    suppress_import_stdout : bool, default=True
-        Whether to suppress stdout printout upon import.
-
-    Returns
-    -------
-    module_info: dict
-        Mapping of string module name (key) to a dictionary of the
-        module's metadata. The metadata dictionary includes the
-        following key:value pairs:
-
-        - "path": str path to the submodule.
-        - "name": str name of hte submodule.
-        - "classes": dictionary with submodule's class names (keys) mapped to
-          dictionaries with metadata about the class.
-        - "functions": dictionary with function names (keys) mapped to
-          dictionary with metadata about each function.
-        - "__all__": list of string code artifact names that appear in the
-          submodules __all__ attribute
-        - "authors": contents of the submodules __authors__ attribute
-        - "is_package": whether the submodule is a Python package
-        - "contains_concrete_class_implementations": whether any module classes
-          inherit from ``BaseObject`` and are not `package_base_classes`.
-        - "contains_base_classes": whether any module classes that are
-          `package_base_classes`.
-        - "contains_base_objects": whether any module classes that
-          inherit from ``BaseObject``.
-    """
-    module, path, loader = _determine_module_path(package_name, path)
-    module_info: MutableMapping = {}  # of ModuleInfo type
-    # Get any metadata at the top-level of the provided package
-    # This is because the pkgutil.walk_packages doesn't include __init__
-    # file when walking a package
-    if not _is_ignored_module(package_name, modules_to_ignore=modules_to_ignore):
-        module_info[package_name] = _get_module_info(
-            module,
-            loader.is_package(package_name),
-            path,
-            package_base_classes,
-            exclude_non_public_items=exclude_non_public_items,
-            class_filter=class_filter,
-            tag_filter=tag_filter,
-            classes_to_exclude=classes_to_exclude,
-        )
-
-    # Now walk through any submodules
-    prefix = f"{package_name}."
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=FutureWarning)
-        warnings.simplefilter("module", category=ImportWarning)
-        warnings.filterwarnings(
-            "ignore", category=UserWarning, message=".*has been moved to.*"
-        )
-        for name, is_pkg, _ in _walk(path, exclude=modules_to_ignore, prefix=prefix):
-            # Used to skip-over ignored modules and non-public modules
-            if exclude_non_public_modules and _is_non_public_module(name):
-                continue
-
-            try:
-                sub_module: ModuleType = _import_module(
-                    name, suppress_import_stdout=suppress_import_stdout
-                )
-                module_info[name] = _get_module_info(
-                    sub_module,
-                    is_pkg,
-                    path,
-                    package_base_classes,
-                    exclude_non_public_items=exclude_non_public_items,
-                    class_filter=class_filter,
-                    tag_filter=tag_filter,
-                    classes_to_exclude=classes_to_exclude,
-                )
-            except ImportError:
-                continue
-
-            if recursive and is_pkg:
-                if "." in name:
-                    name_ending = name[len(package_name) + 1 :]
-                else:
-                    name_ending = name
-
-                updated_path: str
-                if "." in name_ending:
-                    updated_path = "/".join([path, name_ending.replace(".", "/")])
-                else:
-                    updated_path = "/".join([path, name_ending])
-                module_info.update(
-                    get_package_metadata(
-                        package_name=name,
-                        path=updated_path,
-                        recursive=recursive,
-                        exclude_non_public_items=exclude_non_public_items,
-                        exclude_non_public_modules=exclude_non_public_modules,
-                        modules_to_ignore=modules_to_ignore,
-                        package_base_classes=package_base_classes,
-                        class_filter=class_filter,
-                        tag_filter=tag_filter,
-                        classes_to_exclude=classes_to_exclude,
-                        suppress_import_stdout=suppress_import_stdout,
-                    )
-                )
-
-    return module_info
-
-
-def all_objects(
-    object_types=None,
-    filter_tags=None,
-    exclude_objects=None,
-    exclude_estimators=None,
-    return_names=True,
-    as_dataframe=False,
-    return_tags=None,
-    suppress_import_stdout=True,
-    package_name="skbase",
-    path: Optional[str] = None,
-    modules_to_ignore=None,
-    ignore_modules=None,
-    class_lookup=None,
-):
-    """Get a list of all objects in a package with name `package_name`.
-
-    This function crawls the package/module to retreive all classes
-    that are descendents of BaseObject. By default it does this for the `skbase`
-    package, but users can specify `package_name` or `path` to another project
-    and `all_objects` will crawl and retrieve BaseObjects found in that project.
-
-    Parameters
-    ----------
-    object_types: class or list of classes, default=None
-
-        - If class_lookup is provided, can also be str or list of str
-          which kind of objects should be returned.
-        - If None, no filter is applied and all estimators are returned.
-        - If class or list of class, estimators are filtered to inherit from
-          one of these.
-        - If str or list of str, classes can be aliased by strings, as long
-          as `class_lookup` parameter is passed a lookup dict.
-
-    return_names: bool, default=True
-
-        - If True, estimator class name is included in the all_estimators()
-          return in the order: name, estimator class, optional tags, either as
-          a tuple or as pandas.DataFrame columns.
-        - If False, estimator class name is removed from the all_estimators()
-          return.
-
-    filter_tags: str, list[str] or dict[str, Any], default=None
-        Filter used to determine if `klass` has tag or expected tag values.
-
-        - If a str or list of strings is provided, the return will be filtered
-          to keep classes that have all the tag(s) specified by the strings.
-        - If a dict is provided, the return will be filtered to keep classes
-          that have all dict keys as tags. Tag values are also checked such that:
-
-          - If a dict key maps to a single value only classes with tag values equal
-            to the value are returned.
-          - If a dict key maps to multiple values (e.g., list) only classes with
-            tag values in these values are returned.
-
-    exclude_objects: str or list[str], default=None
-        Names of estimators to exclude.
-    as_dataframe: bool, default=False
-
-        - If False, `all_objects` will return a list (either a list of
-          `skbase` objects or a list of tuples, see Returns).
-        - If True, `all_objects` will return a `pandas.DataFrame` with named
-            columns for all of the attributes being returned.
-            this requires soft dependency `pandas` to be installed.
-
-    return_tags: str or list of str, default=None
-        Names of tags to fetch and return each object's value of. The tag values
-        named in return_tags will be fetched for each object and will be appended
-        as either columns or tuple entries.
-    package_name : str, default="skbase".
-        Should be set to default to package or module name that objects will
-        be retrieved from. Objects will be searched inside `package_name`,
-        including in sub-modules (e.g., in package_name, package_name.module1,
-        package.module2, and package.module1.module3).
-    path : str, default=None
-        If provided, this should be the path that should be used as root
-        to find `package_name` and start the search for any submodules/packages.
-        This can be left at the default value (None) if searching in an installed
-        package.
-    modules_to_ignore : str or list[str], default=None
-        The modules that should be ignored when searching across the modules to
-        gather objects. If passed, `all_objects` ignores modules or submodules
-        of a module whose name is in the provided string(s). E.g., if
-        `modules_to_ignore` contains the string `"foo"`, then `"bar.foo"`,
-        `"foo"`, `"foo.bar"`, `"bar.foo.bar"` are ignored.
-
-    class_lookup : dict[str, class], default=None
-        Dictionary of string aliases for classes used in object_types. If provided,
-        `object_types` can accept str values or a list of string values.
-
-    Other Parameters
-    ----------------
-    suppress_import_stdout : bool, default=True
-        Whether to suppress stdout printout upon import.
-
-    Returns
-    -------
-    all_estimators will return one of the following:
-
-    - a pandas.DataFrame if `as_dataframe=True`, with columns:
-
-      - "names" with the returned class names if `return_name=True`
-      - "objects" with returned classes.
-      - optional columns named based on tags passed in `return_tags`
-        if `return_tags is not None`.
-
-    - a list if `as_dataframe=False`, where list elements are:
-
-      - classes (that inherit from BaseObject) in alphabetic order by class name
-        if `return_names=False` and `return_tags=None.
-      - (name, class) tuples in alphabetic order by name if `return_names=True`
-        and `return_tags=None`.
-      - (name, class, tag-value1, ..., tag-valueN) tuples in alphabetic order by name
-        if `return_names=True` and `return_tags is not None`.
-      - (class, tag-value1, ..., tag-valueN) tuples in alphabetic order by
-        class name if `return_names=False` and `return_tags is not None`.
-
-    References
-    ----------
-    Modified version of scikit-learn's and sktime's `all_estimators()` to allow
-    users to find BaseObjects in `skbase` and other packages.
-    """
-    module, root, _ = _determine_module_path(package_name, path)
-    if modules_to_ignore is None:
-        modules_to_ignore = []
-    if exclude_objects is None:
-        exclude_objects = []
-
-    all_estimators = []
-
-    def _is_base_class(name):
-        return name.startswith("_") or name.startswith("Base")
-
-    def _is_estimator(name, klass):
-        # Check if klass is subclass of base estimators, not an base class itself and
-        # not an abstract class
-        return issubclass(klass, BaseObject) and not _is_base_class(name)
-
-    # Ignore deprecation warnings triggered at import time and from walking packages
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=FutureWarning)
-        warnings.simplefilter("module", category=ImportWarning)
-        warnings.filterwarnings(
-            "ignore", category=UserWarning, message=".*has been moved to.*"
-        )
-        prefix = f"{package_name}."
-        for module_name, _, _ in _walk(
-            root=root, exclude=modules_to_ignore, prefix=prefix
-        ):
-            # Filter modules
-            if _is_non_public_module(module_name):
-                continue
-
-            try:
-                if suppress_import_stdout:
-                    # setup text trap, import, then restore
-                    sys.stdout = io.StringIO()
-                    module = importlib.import_module(module_name)
-                    sys.stdout = sys.__stdout__
-                else:
-                    module = importlib.import_module(module_name)
-                classes = inspect.getmembers(module, inspect.isclass)
-                # Filter classes
-                estimators = [
-                    (klass.__name__, klass)
-                    for _, klass in classes
-                    if _is_estimator(klass.__name__, klass)
-                ]
-                all_estimators.extend(estimators)
-            except ModuleNotFoundError as e:
-                # Skip missing soft dependencies
-                if "soft dependency" not in str(e):
-                    raise e
-                warnings.warn(str(e), ImportWarning, stacklevel=2)
-
-    # Drop duplicates
-    all_estimators = set(all_estimators)
-
-    # Filter based on given estimator types
-    if object_types:
-        obj_types = _check_object_types(object_types, class_lookup)
-        all_estimators = [
-            (n, est) for (n, est) in all_estimators if _filter_by_class(est, obj_types)
-        ]
-
-    # Filter based on given exclude list
-    if exclude_objects:
-        exclude_objects = check_sequence(
-            exclude_objects,
-            sequence_type=list,
-            element_type=str,
-            coerce_scalar_input=True,
-            sequence_name="exclude_object",
-        )
-        all_estimators = [
-            (name, estimator)
-            for name, estimator in all_estimators
-            if name not in exclude_objects
-        ]
-
-    # Drop duplicates, sort for reproducibility
-    # itemgetter is used to ensure the sort does not extend to the 2nd item of
-    # the tuple
-    all_estimators = sorted(all_estimators, key=itemgetter(0))
-
-    if filter_tags:
-        all_estimators = [
-            (n, est) for (n, est) in all_estimators if _filter_by_tags(est, filter_tags)
-        ]
-
-    # remove names if return_names=False
-    if not return_names:
-        all_estimators = [estimator for (name, estimator) in all_estimators]
-        columns = ["object"]
-    else:
-        columns = ["name", "object"]
-
-    # add new tuple entries to all_estimators for each tag in return_tags:
-    return_tags = [] if return_tags is None else return_tags
-    if return_tags:
-        return_tags = check_sequence(
-            return_tags,
-            sequence_type=list,
-            element_type=str,
-            coerce_scalar_input=True,
-            sequence_name="return_tags",
-        )
-        # enrich all_estimators by adding the values for all return_tags tags:
-        if all_estimators:
-            if isinstance(all_estimators[0], tuple):
-                all_estimators = [
-                    (name, est) + _get_return_tags(est, return_tags)
-                    for (name, est) in all_estimators
-                ]
-            else:
-                all_estimators = [
-                    (est,) + _get_return_tags(est, return_tags)
-                    for est in all_estimators
-                ]
-        columns = columns + return_tags
-
-    # convert to pandas.DataFrame if as_dataframe=True
-    if as_dataframe:
-        all_estimators = _make_dataframe(all_estimators, columns=columns)
-
-    return all_estimators
-
-
-def _get_return_tags(obj, return_tags):
-    """Fetch a list of all tags for every_entry of all_estimators.
-
-    Parameters
-    ----------
-    obj:  BaseObject
-        A BaseObject.
-    return_tags: list of str
-        Names of tags to get values for the estimator.
-
-    Returns
-    -------
-    tags: a tuple with all the object values for all tags in return tags.
-        a value is None if it is not a valid tag for the object provided.
-    """
-    tags = tuple(obj.get_class_tag(tag) for tag in return_tags)
-    return tags
-
-
-def _check_object_types(object_types, class_lookup=None):
-    """Return list of classes corresponding to type strings.
-
-    Parameters
-    ----------
-    object_types : str, class, or list of string or class
-    class_lookup : dict[string, class], default=None
-
-    Returns
-    -------
-    list of class, i-th element is:
-        class_lookup[object_types[i]] if object_types[i] was a string
-        object_types[i] otherwise
-    if class_lookup is none, only checks whether object_types is class or list of.
-
-    Raises
-    ------
-    ValueError if object_types is not of the expected type.
-    """
-    object_types = deepcopy(object_types)
-
-    if not isinstance(object_types, list):
-        object_types = [object_types]  # make iterable
-
-    def _get_err_msg(estimator_type):
-        if class_lookup is None or not isinstance(class_lookup, dict):
-            return (
-                f"Parameter `estimator_type` must be None, a class, or a list of "
-                f"class, but found: {repr(estimator_type)}"
-            )
-        else:
-            return (
-                f"Parameter `estimator_type` must be None, a string, a class, or a list"
-                f" of [string or class]. Valid string values are: "
-                f"{tuple(class_lookup.keys())}, but found: "
-                f"{repr(estimator_type)}"
-            )
-
-    for i, estimator_type in enumerate(object_types):
-        if isinstance(estimator_type, str):
-            if not isinstance(class_lookup, dict) or (
-                estimator_type not in class_lookup.keys()
-            ):
-                raise ValueError(_get_err_msg(estimator_type))
-            estimator_type = class_lookup[estimator_type]
-            object_types[i] = estimator_type
-        elif isinstance(estimator_type, type):
-            pass
-        else:
-            raise ValueError(_get_err_msg(estimator_type))
-    return object_types
-
-
-def _make_dataframe(all_objects, columns):
-    """Create pandas.DataFrame from all_objects.
-
-    Kept as a separate function with import to isolate the pandas dependency.
-    """
-    import pandas as pd
-
-    return pd.DataFrame(all_objects, columns=columns)
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tools to lookup information on code artifacts in a Python package or module.
+
+This module exports the following methods for registry lookup:
+
+package_metadata()
+    Walk package and return metadata on included classes and functions by module.
+all_objects(object_types, filter_tags)
+    Look (and optionally filter) BaseObject descendants in a package or module.
+"""
+# all_objects is based on the sktime all_estimator retrieval utility, which
+# is based on the sklearn estimator retrieval utility of the same name
+# See https://github.com/scikit-learn/scikit-learn/blob/main/COPYING and
+# https://github.com/sktime/sktime/blob/main/LICENSE
+import importlib
+import inspect
+import io
+import os
+import pathlib
+import pkgutil
+import sys
+import warnings
+from collections.abc import Iterable
+from copy import deepcopy
+from operator import itemgetter
+from types import ModuleType
+from typing import Any, List, Mapping, MutableMapping, Optional, Sequence, Tuple, Union
+
+from skbase.base import BaseObject
+from skbase.validate import check_sequence
+
+__all__: List[str] = ["all_objects", "get_package_metadata"]
+__author__: List[str] = [
+    "fkiraly",
+    "mloning",
+    "katiebuc",
+    "miraep8",
+    "xloem",
+    "rnkuhns",
+]
+
+# the below is commented out to avoid a dependency on typing_extensions
+# but still left in place as it is informative regarding expected return type
+
+# class ClassInfo(TypedDict):
+#     """Type definitions for information on a module's classes."""
+
+#     klass: Type
+#     name: str
+#     description: str
+#     tags: MutableMapping[str, Any]
+#     is_concrete_implementation: bool
+#     is_base_class: bool
+#     is_base_object: bool
+#     authors: Optional[Union[List[str], str]]
+#     module_name: str
+
+
+# class FunctionInfo(TypedDict):
+#     """Information on a module's functions."""
+
+#     func: FunctionType
+#     name: str
+#     description: str
+#     module_name: str
+
+
+# class ModuleInfo(TypedDict):
+#     """Module information type definitions."""
+
+#     path: str
+#     name: str
+#     classes: MutableMapping[str, ClassInfo]
+#     functions: MutableMapping[str, FunctionInfo]
+#     __all__: List[str]
+#     authors: str
+#     is_package: bool
+#     contains_concrete_class_implementations: bool
+#     contains_base_classes: bool
+#     contains_base_objects: bool
+
+
+def _is_non_public_module(module_name: str) -> bool:
+    """Determine if a module is non-public or not.
+
+    Parameters
+    ----------
+    module_name : str
+        Name of the module.
+
+    Returns
+    -------
+    is_non_public : bool
+        Whether the module is non-public or not.
+    """
+    if not isinstance(module_name, str):
+        raise ValueError(
+            f"Parameter `module_name` should be str, but found {type(module_name)}."
+        )
+    is_non_public: bool = "._" in module_name or module_name.startswith("_")
+    return is_non_public
+
+
+def _is_ignored_module(
+    module_name: str, modules_to_ignore: Union[str, List[str], Tuple[str]] = None
+) -> bool:
+    """Determine if module is one of the ignored modules.
+
+    Ignores a module if identical with, or submodule of a module whose name
+    is in the list/tuple `modules_to_ignore`.
+
+    E.g., if `modules_to_ignore` contains the string `"foo"`, then `True` will be
+    returned for `module_name`-s `"bar.foo"`, `"foo"`, `"foo.bar"`,
+    `"bar.foo.bar"`, etc.
+
+    Paramters
+    ---------
+    module_name : str
+        Name of the module.
+    modules_to_ignore : str, list[str] or tuple[str]
+        The modules that should be ignored when walking the package.
+
+    Returns
+    -------
+    is_ignored : bool
+        Whether the module is an ignrored module or not.
+    """
+    if isinstance(modules_to_ignore, str):
+        modules_to_ignore = (modules_to_ignore,)
+    is_ignored: bool
+    if modules_to_ignore is None:
+        is_ignored = False
+    else:
+        is_ignored = any(part in modules_to_ignore for part in module_name.split("."))
+
+    return is_ignored
+
+
+def _filter_by_class(
+    klass: type, class_filter: Optional[Union[type, Sequence[type]]] = None
+) -> bool:
+    """Determine if a class is a subclass of the supplied classes.
+
+    Parameters
+    ----------
+    klass : object
+        Class to check.
+    class_filter : objects or iterable of objects
+        Classes that `klass` is checked against.
+
+    Returns
+    -------
+    is_subclass : bool
+        Whether the input class is a subclass of the `class_filter`.
+        If `class_filter` was `None`, returns `True`.
+    """
+    if class_filter is None:
+        return True
+
+    if isinstance(class_filter, Iterable) and not isinstance(class_filter, tuple):
+        class_filter = tuple(class_filter)
+    return issubclass(klass, class_filter)
+
+
+def _filter_by_tags(obj, tag_filter=None, as_dataframe=True):
+    """Check whether estimator satisfies tag_filter condition.
+
+    Parameters
+    ----------
+    obj : BaseObject, an sktime estimator
+    tag_filter : dict of (str or list of str), default=None
+        subsets the returned estimators as follows:
+        each key/value pair is statement in "and"/conjunction
+
+        * key is tag name to sub-set on
+        * value str or list of string are tag values
+        * condition is "key must be equal to value, or in set(value)"
+
+    Returns
+    -------
+    cond_sat: bool, whether estimator satisfies condition in `tag_filter`
+        if `tag_filter` was None, returns `True`
+    """
+    if tag_filter is None:
+        return True
+
+    if not isinstance(tag_filter, (str, Iterable, dict)):
+        raise TypeError(
+            "tag_filter argument of _filter_by_tags must be "
+            "a dict with str keys, str, or iterable of str, "
+            f"but found tag_filter of type {type(tag_filter)}"
+        )
+
+    if not hasattr(obj, "get_class_tag"):
+        return False
+
+    klass_tags = obj.get_class_tags().keys()
+
+    # case: tag_filter is string
+    if isinstance(tag_filter, str):
+        return tag_filter in klass_tags
+
+    # case: tag_filter is iterable of str but not dict
+    # If a iterable of strings is provided, check that all are in the returned tag_dict
+    if isinstance(tag_filter, Iterable) and not isinstance(tag_filter, dict):
+        if not all(isinstance(t, str) for t in tag_filter):
+            raise ValueError(
+                "tag_filter argument of _filter_by_tags must be "
+                f"a dict with str keys, str, or iterable of str, but found {tag_filter}"
+            )
+        return all(tag in klass_tags for tag in tag_filter)
+
+    # case: tag_filter is dict
+    if not all(isinstance(t, str) for t in tag_filter.keys()):
+        raise ValueError(
+            "tag_filter argument of _filter_by_tags must be "
+            f"a dict with str keys, str, or iterable of str, but found {tag_filter}"
+        )
+
+    cond_sat = True
+
+    for key, value in tag_filter.items():
+        if not isinstance(value, list):
+            value = [value]
+        cond_sat = cond_sat and obj.get_class_tag(key) in set(value)
+
+    return cond_sat
+
+
+def _walk(root, exclude=None, prefix=""):
+    """Recursively return all modules and sub-modules as list of strings.
+
+    Unlike pkgutil.walk_packages, does not import modules on exclusion list.
+
+    Parameters
+    ----------
+    root : str or path-like
+        Root path in which to look for submodules. Can be a string path,
+        pathlib.Path or other path-like object.
+    exclude : tuple of str or None, optional, default = None
+        List of sub-modules to ignore in the return, including sub-modules
+    prefix: str, optional, default = ""
+        This str is pre-appended to all strings in the return
+
+    Yields
+    ------
+    str : sub-module strings
+        Iterates over all sub-modules of root that do not contain any of the
+        strings on the `exclude` list string is prefixed by the string `prefix`
+    """
+    if not isinstance(root, str):
+        root = str(root)
+    for loader, module_name, is_pkg in pkgutil.iter_modules(path=[root]):
+        if not _is_ignored_module(module_name, modules_to_ignore=exclude):
+            yield f"{prefix}{module_name}", is_pkg, loader
+            if is_pkg:
+                yield from (
+                    (f"{prefix}{module_name}.{x[0]}", x[1], x[2])
+                    for x in _walk(f"{root}/{module_name}", exclude=exclude)
+                )
+
+
+def _import_module(
+    module: Union[str, importlib.machinery.SourceFileLoader],
+    suppress_import_stdout: bool = True,
+) -> ModuleType:
+    """Import a module, while optionally suppressing import standard out.
+
+    Parameters
+    ----------
+    module : str or importlib.machinery.SourceFileLoader
+        Name of the module to be imported or a SourceFileLoader to load a module.
+    suppress_import_stdout : bool, default=True
+        Whether to suppress stdout printout upon import.
+
+    Returns
+    -------
+    imported_mod : ModuleType
+        The module that was imported.
+    """
+    # input check
+    if not isinstance(module, (str, importlib.machinery.SourceFileLoader)):
+        raise ValueError(
+            "`module` should be string module name or instance of "
+            "importlib.machinery.SourceFileLoader."
+        )
+
+    # if suppress_import_stdout:
+    # setup text trap, import
+    if suppress_import_stdout:
+        temp_stdout = sys.stdout
+        sys.stdout = io.StringIO()
+
+    try:
+        if isinstance(module, str):
+            imported_mod = importlib.import_module(module)
+        elif isinstance(module, importlib.machinery.SourceFileLoader):
+            imported_mod = module.load_module()
+        exc = None
+    except Exception as e:
+        # we store the exception so we can restore the stdout fisrt
+        exc = e
+
+    # if we set up a text trap, restore it to the initial value
+    if suppress_import_stdout:
+        sys.stdout = temp_stdout
+
+    # if we encountered an exception, now raise it
+    if exc is not None:
+        raise exc
+
+    return imported_mod
+
+
+def _determine_module_path(
+    package_name: str, path: Optional[Union[str, pathlib.Path]] = None
+) -> Tuple[ModuleType, str, importlib.machinery.SourceFileLoader]:
+    """Determine a package's path information.
+
+    Parameters
+    ----------
+    package_name : str
+        The name of the package/module to return metadata for.
+
+        - If `path` is not None, this should be the name of the package/module
+          associated with the path. `package_name` (with "." appended at end)
+          will be used as prefix for any submodules/packages when walking
+          the provided `path`.
+        - If `path` is None, then package_name is assumed to be an importable
+          package or module and the `path` to `package_name` will be determined
+          from its import.
+
+    path : str or absolute pathlib.Path, default=None
+        If provided, this should be the path that should be used as root
+        to find any modules or submodules.
+
+    Returns
+    -------
+    module, path_, loader : ModuleType, str, importlib.machinery.SourceFileLoader
+        Returns the module, a string of its path and its SourceFileLoader.
+    """
+    if not isinstance(package_name, str):
+        raise ValueError(
+            "`package_name` must be the string name of a package or module."
+            "For example, 'some_package' or 'some_package.some_module'."
+        )
+
+    def _instantiate_loader(package_name: str, path: str):
+        if path.endswith(".py"):
+            loader = importlib.machinery.SourceFileLoader(package_name, path)
+        elif os.path.exists(path + "/__init__.py"):
+            loader = importlib.machinery.SourceFileLoader(
+                package_name, path + "/__init__.py"
+            )
+        else:
+            loader = importlib.machinery.SourceFileLoader(package_name, path)
+        return loader
+
+    if path is None:
+        module = _import_module(package_name, suppress_import_stdout=False)
+        if hasattr(module, "__path__") and (
+            module.__path__ is not None and len(module.__path__) > 0
+        ):
+            path_ = module.__path__[0]
+        elif hasattr(module, "__file__") and module.__file__ is not None:
+            path_ = module.__file__.split(".")[0]
+        else:
+            raise ValueError(
+                f"Unable to determine path for provided `package_name`: {package_name} "
+                "from the imported module. Try explicitly providing the `path`."
+            )
+        loader = _instantiate_loader(package_name, path_)
+    else:
+        # Make sure path is str and not a pathlib.Path
+        if isinstance(path, (pathlib.Path, str)):
+            path_ = str(path.absolute()) if isinstance(path, pathlib.Path) else path
+            # Use the provided path and package name to load the module
+            # if both available.
+            try:
+                loader = _instantiate_loader(package_name, path_)
+                module = _import_module(loader, suppress_import_stdout=False)
+            except ImportError as exc:
+                raise ValueError(
+                    f"Unable to import a package named {package_name} based "
+                    f"on provided `path`: {path_}."
+                ) from exc
+        else:
+            raise ValueError(
+                f"`path` must be a str path or pathlib.Path, but is type {type(path)}."
+            )
+
+    return module, path_, loader
+
+
+def _get_module_info(
+    module: ModuleType,
+    is_pkg: bool,
+    path: str,
+    package_base_classes: Union[type, Tuple[type, ...]],
+    exclude_non_public_items: bool = True,
+    class_filter: Optional[Union[type, Sequence[type]]] = None,
+    tag_filter: Optional[Union[str, Sequence[str], Mapping[str, Any]]] = None,
+    classes_to_exclude: Optional[Union[type, Sequence[type]]] = None,
+) -> dict:  # of ModuleInfo type
+    # Make package_base_classes a tuple if it was supplied as a class
+    base_classes_none = False
+    if isinstance(package_base_classes, Iterable):
+        package_base_classes = tuple(package_base_classes)
+    elif not isinstance(package_base_classes, tuple):
+        if package_base_classes is None:
+            base_classes_none = True
+        package_base_classes = (package_base_classes,)
+
+    exclude_classes: Optional[Sequence[type]]
+    if classes_to_exclude is None:
+        exclude_classes = classes_to_exclude
+    elif isinstance(classes_to_exclude, Sequence):
+        exclude_classes = classes_to_exclude
+    elif inspect.isclass(classes_to_exclude):
+        exclude_classes = (classes_to_exclude,)
+
+    designed_imports: List[str] = getattr(module, "__all__", [])
+    authors: Union[str, List[str]] = getattr(module, "__author__", [])
+    if isinstance(authors, (list, tuple)):
+        authors = ", ".join(authors)
+    # Compile information on classes in the module
+    module_classes: MutableMapping = {}  # of ClassInfo type
+    for name, klass in inspect.getmembers(module, inspect.isclass):
+        # Skip a class if non-public items should be excluded and it starts with "_"
+        if (
+            (exclude_non_public_items and klass.__name__.startswith("_"))
+            or (exclude_classes is not None and klass in exclude_classes)
+            or not _filter_by_tags(klass, tag_filter=tag_filter)
+            or not _filter_by_class(klass, class_filter=class_filter)
+        ):
+            continue
+        # Otherwise, store info about the class
+        if klass.__module__ == module.__name__ or name in designed_imports:
+            klass_authors = getattr(klass, "__author__", authors)
+            if isinstance(klass_authors, (list, tuple)):
+                klass_authors = ", ".join(klass_authors)
+            if base_classes_none:
+                concrete_implementation = False
+            else:
+                concrete_implementation = (
+                    issubclass(klass, package_base_classes)
+                    and klass not in package_base_classes
+                )
+            module_classes[name] = {
+                "klass": klass,
+                "name": klass.__name__,
+                "description": (
+                    "" if klass.__doc__ is None else klass.__doc__.split("\n")[0]
+                ),
+                "tags": (
+                    klass.get_class_tags() if hasattr(klass, "get_class_tags") else None
+                ),
+                "is_concrete_implementation": concrete_implementation,
+                "is_base_class": klass in package_base_classes,
+                "is_base_object": issubclass(klass, BaseObject),
+                "authors": klass_authors,
+                "module_name": module.__name__,
+            }
+
+    module_functions: MutableMapping = {}  # of FunctionInfo type
+    for name, func in inspect.getmembers(module, inspect.isfunction):
+        if func.__module__ == module.__name__ or name in designed_imports:
+            # Skip a class if non-public items should be excluded and it starts with "_"
+            if exclude_non_public_items and func.__name__.startswith("_"):
+                continue
+            # Otherwise, store info about the class
+            module_functions[name] = {
+                "func": func,
+                "name": func.__name__,
+                "description": (
+                    "" if func.__doc__ is None else func.__doc__.split("\n")[0]
+                ),
+                "module_name": module.__name__,
+            }
+
+    # Combine all the information on the module together
+    module_info = {  # of ModuleInfo type
+        "path": path,
+        "name": module.__name__,
+        "classes": module_classes,
+        "functions": module_functions,
+        "__all__": designed_imports,
+        "authors": authors,
+        "is_package": is_pkg,
+        "contains_concrete_class_implementations": any(
+            v["is_concrete_implementation"] for v in module_classes.values()
+        ),
+        "contains_base_classes": any(
+            v["is_base_class"] for v in module_classes.values()
+        ),
+        "contains_base_objects": any(
+            v["is_base_object"] for v in module_classes.values()
+        ),
+    }
+    return module_info
+
+
+def get_package_metadata(
+    package_name: str,
+    path: Optional[str] = None,
+    recursive: bool = True,
+    exclude_non_public_items: bool = True,
+    exclude_non_public_modules: bool = True,
+    modules_to_ignore: Union[str, List[str], Tuple[str]] = ("tests",),
+    package_base_classes: Union[type, Tuple[type, ...]] = (BaseObject,),
+    class_filter: Optional[Union[type, Sequence[type]]] = None,
+    tag_filter: Optional[Union[str, Sequence[str], Mapping[str, Any]]] = None,
+    classes_to_exclude: Optional[Union[type, Sequence[type]]] = None,
+    suppress_import_stdout: bool = True,
+) -> Mapping:  # of ModuleInfo type
+    """Return a dictionary mapping all package modules to their metadata.
+
+    Parameters
+    ----------
+    package_name : str
+        The name of the package/module to return metadata for.
+
+        - If `path` is not None, this should be the name of the package/module
+          associated with the path. `package_name` (with "." appended at end)
+          will be used as prefix for any submodules/packages when walking
+          the provided `path`.
+        - If `path` is None, then package_name is assumed to be an importable
+          package or module and the `path` to `package_name` will be determined
+          from its import.
+
+    path : str, default=None
+        If provided, this should be the path that should be used as root
+        to find any modules or submodules.
+    recursive : bool, default=True
+        Whether to recursively walk through submodules.
+
+        - If True, then submodules of submodules and so on are found.
+        - If False, then only first-level submodules of `package` are found.
+
+    exclude_non_public_items : bool, default=True
+        Whether to exclude nonpublic functions and classes (where name starts
+        with a leading underscore).
+    exclude_non_public_modules : bool, default=True
+        Whether to exclude nonpublic modules (modules where names start with
+        a leading underscore).
+    modules_to_ignore : str, tuple[str] or list[str], default="tests"
+        The modules that should be ignored when searching across the modules to
+        gather objects. If passed, `all_objects` ignores modules or submodules
+        of a module whose name is in the provided string(s). E.g., if
+        `modules_to_ignore` contains the string `"foo"`, then `"bar.foo"`,
+        `"foo"`, `"foo.bar"`, `"bar.foo.bar"` are ignored.
+    package_base_classes: type or Sequence[type], default = (BaseObject,)
+        The base classes used to determine if any classes found in metadata descend
+        from a base class.
+    class_filter : object or Sequence[object], default=None
+        Classes that `klass` is checked against. Only classes that are subclasses
+        of the supplied `class_filter` are returned in metadata.
+    tag_filter : str, Sequence[str] or dict[str, Any], default=None
+        Filter used to determine if `klass` has tag or expected tag values.
+
+        - If a str or list of strings is provided, the return will be filtered
+          to keep classes that have all the tag(s) specified by the strings.
+        - If a dict is provided, the return will be filtered to keep classes
+          that have all dict keys as tags. Tag values are also checked such that:
+
+          - If a dict key maps to a single value only classes with tag values equal
+            to the value are returned.
+          - If a dict key maps to multiple values (e.g., list) only classes with
+            tag values in these values are returned.
+
+    classes_to_exclude: objects or iterable of object, default=None
+        Classes to exclude from returned metadata.
+
+    Other Parameters
+    ----------------
+    suppress_import_stdout : bool, default=True
+        Whether to suppress stdout printout upon import.
+
+    Returns
+    -------
+    module_info: dict
+        Mapping of string module name (key) to a dictionary of the
+        module's metadata. The metadata dictionary includes the
+        following key:value pairs:
+
+        - "path": str path to the submodule.
+        - "name": str name of hte submodule.
+        - "classes": dictionary with submodule's class names (keys) mapped to
+          dictionaries with metadata about the class.
+        - "functions": dictionary with function names (keys) mapped to
+          dictionary with metadata about each function.
+        - "__all__": list of string code artifact names that appear in the
+          submodules __all__ attribute
+        - "authors": contents of the submodules __authors__ attribute
+        - "is_package": whether the submodule is a Python package
+        - "contains_concrete_class_implementations": whether any module classes
+          inherit from ``BaseObject`` and are not `package_base_classes`.
+        - "contains_base_classes": whether any module classes that are
+          `package_base_classes`.
+        - "contains_base_objects": whether any module classes that
+          inherit from ``BaseObject``.
+    """
+    module, path, loader = _determine_module_path(package_name, path)
+    module_info: MutableMapping = {}  # of ModuleInfo type
+    # Get any metadata at the top-level of the provided package
+    # This is because the pkgutil.walk_packages doesn't include __init__
+    # file when walking a package
+    if not _is_ignored_module(package_name, modules_to_ignore=modules_to_ignore):
+        module_info[package_name] = _get_module_info(
+            module,
+            loader.is_package(package_name),
+            path,
+            package_base_classes,
+            exclude_non_public_items=exclude_non_public_items,
+            class_filter=class_filter,
+            tag_filter=tag_filter,
+            classes_to_exclude=classes_to_exclude,
+        )
+
+    # Now walk through any submodules
+    prefix = f"{package_name}."
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=FutureWarning)
+        warnings.simplefilter("module", category=ImportWarning)
+        warnings.filterwarnings(
+            "ignore", category=UserWarning, message=".*has been moved to.*"
+        )
+        for name, is_pkg, _ in _walk(path, exclude=modules_to_ignore, prefix=prefix):
+            # Used to skip-over ignored modules and non-public modules
+            if exclude_non_public_modules and _is_non_public_module(name):
+                continue
+
+            try:
+                sub_module: ModuleType = _import_module(
+                    name, suppress_import_stdout=suppress_import_stdout
+                )
+                module_info[name] = _get_module_info(
+                    sub_module,
+                    is_pkg,
+                    path,
+                    package_base_classes,
+                    exclude_non_public_items=exclude_non_public_items,
+                    class_filter=class_filter,
+                    tag_filter=tag_filter,
+                    classes_to_exclude=classes_to_exclude,
+                )
+            except ImportError:
+                continue
+
+            if recursive and is_pkg:
+                if "." in name:
+                    name_ending = name[len(package_name) + 1 :]
+                else:
+                    name_ending = name
+
+                updated_path: str
+                if "." in name_ending:
+                    updated_path = "/".join([path, name_ending.replace(".", "/")])
+                else:
+                    updated_path = "/".join([path, name_ending])
+                module_info.update(
+                    get_package_metadata(
+                        package_name=name,
+                        path=updated_path,
+                        recursive=recursive,
+                        exclude_non_public_items=exclude_non_public_items,
+                        exclude_non_public_modules=exclude_non_public_modules,
+                        modules_to_ignore=modules_to_ignore,
+                        package_base_classes=package_base_classes,
+                        class_filter=class_filter,
+                        tag_filter=tag_filter,
+                        classes_to_exclude=classes_to_exclude,
+                        suppress_import_stdout=suppress_import_stdout,
+                    )
+                )
+
+    return module_info
+
+
+def all_objects(
+    object_types=None,
+    filter_tags=None,
+    exclude_objects=None,
+    exclude_estimators=None,
+    return_names=True,
+    as_dataframe=False,
+    return_tags=None,
+    suppress_import_stdout=True,
+    package_name="skbase",
+    path: Optional[str] = None,
+    modules_to_ignore=None,
+    ignore_modules=None,
+    class_lookup=None,
+):
+    """Get a list of all objects in a package with name `package_name`.
+
+    This function crawls the package/module to retreive all classes
+    that are descendents of BaseObject. By default it does this for the `skbase`
+    package, but users can specify `package_name` or `path` to another project
+    and `all_objects` will crawl and retrieve BaseObjects found in that project.
+
+    Parameters
+    ----------
+    object_types: class or list of classes, default=None
+
+        - If class_lookup is provided, can also be str or list of str
+          which kind of objects should be returned.
+        - If None, no filter is applied and all estimators are returned.
+        - If class or list of class, estimators are filtered to inherit from
+          one of these.
+        - If str or list of str, classes can be aliased by strings, as long
+          as `class_lookup` parameter is passed a lookup dict.
+
+    return_names: bool, default=True
+
+        - If True, estimator class name is included in the all_estimators()
+          return in the order: name, estimator class, optional tags, either as
+          a tuple or as pandas.DataFrame columns.
+        - If False, estimator class name is removed from the all_estimators()
+          return.
+
+    filter_tags: str, list[str] or dict[str, Any], default=None
+        Filter used to determine if `klass` has tag or expected tag values.
+
+        - If a str or list of strings is provided, the return will be filtered
+          to keep classes that have all the tag(s) specified by the strings.
+        - If a dict is provided, the return will be filtered to keep classes
+          that have all dict keys as tags. Tag values are also checked such that:
+
+          - If a dict key maps to a single value only classes with tag values equal
+            to the value are returned.
+          - If a dict key maps to multiple values (e.g., list) only classes with
+            tag values in these values are returned.
+
+    exclude_objects: str or list[str], default=None
+        Names of estimators to exclude.
+    as_dataframe: bool, default=False
+
+        - If False, `all_objects` will return a list (either a list of
+          `skbase` objects or a list of tuples, see Returns).
+        - If True, `all_objects` will return a `pandas.DataFrame` with named
+            columns for all of the attributes being returned.
+            this requires soft dependency `pandas` to be installed.
+
+    return_tags: str or list of str, default=None
+        Names of tags to fetch and return each object's value of. The tag values
+        named in return_tags will be fetched for each object and will be appended
+        as either columns or tuple entries.
+    package_name : str, default="skbase".
+        Should be set to default to package or module name that objects will
+        be retrieved from. Objects will be searched inside `package_name`,
+        including in sub-modules (e.g., in package_name, package_name.module1,
+        package.module2, and package.module1.module3).
+    path : str, default=None
+        If provided, this should be the path that should be used as root
+        to find `package_name` and start the search for any submodules/packages.
+        This can be left at the default value (None) if searching in an installed
+        package.
+    modules_to_ignore : str or list[str], default=None
+        The modules that should be ignored when searching across the modules to
+        gather objects. If passed, `all_objects` ignores modules or submodules
+        of a module whose name is in the provided string(s). E.g., if
+        `modules_to_ignore` contains the string `"foo"`, then `"bar.foo"`,
+        `"foo"`, `"foo.bar"`, `"bar.foo.bar"` are ignored.
+
+    class_lookup : dict[str, class], default=None
+        Dictionary of string aliases for classes used in object_types. If provided,
+        `object_types` can accept str values or a list of string values.
+
+    Other Parameters
+    ----------------
+    suppress_import_stdout : bool, default=True
+        Whether to suppress stdout printout upon import.
+
+    Returns
+    -------
+    all_estimators will return one of the following:
+
+    - a pandas.DataFrame if `as_dataframe=True`, with columns:
+
+      - "names" with the returned class names if `return_name=True`
+      - "objects" with returned classes.
+      - optional columns named based on tags passed in `return_tags`
+        if `return_tags is not None`.
+
+    - a list if `as_dataframe=False`, where list elements are:
+
+      - classes (that inherit from BaseObject) in alphabetic order by class name
+        if `return_names=False` and `return_tags=None.
+      - (name, class) tuples in alphabetic order by name if `return_names=True`
+        and `return_tags=None`.
+      - (name, class, tag-value1, ..., tag-valueN) tuples in alphabetic order by name
+        if `return_names=True` and `return_tags is not None`.
+      - (class, tag-value1, ..., tag-valueN) tuples in alphabetic order by
+        class name if `return_names=False` and `return_tags is not None`.
+
+    References
+    ----------
+    Modified version of scikit-learn's and sktime's `all_estimators()` to allow
+    users to find BaseObjects in `skbase` and other packages.
+    """
+    module, root, _ = _determine_module_path(package_name, path)
+    if modules_to_ignore is None:
+        modules_to_ignore = []
+    if exclude_objects is None:
+        exclude_objects = []
+
+    all_estimators = []
+
+    def _is_base_class(name):
+        return name.startswith("_") or name.startswith("Base")
+
+    def _is_estimator(name, klass):
+        # Check if klass is subclass of base estimators, not an base class itself and
+        # not an abstract class
+        return issubclass(klass, BaseObject) and not _is_base_class(name)
+
+    # Ignore deprecation warnings triggered at import time and from walking packages
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=FutureWarning)
+        warnings.simplefilter("module", category=ImportWarning)
+        warnings.filterwarnings(
+            "ignore", category=UserWarning, message=".*has been moved to.*"
+        )
+        prefix = f"{package_name}."
+        for module_name, _, _ in _walk(
+            root=root, exclude=modules_to_ignore, prefix=prefix
+        ):
+            # Filter modules
+            if _is_non_public_module(module_name):
+                continue
+
+            try:
+                if suppress_import_stdout:
+                    # setup text trap, import, then restore
+                    sys.stdout = io.StringIO()
+                    module = importlib.import_module(module_name)
+                    sys.stdout = sys.__stdout__
+                else:
+                    module = importlib.import_module(module_name)
+                classes = inspect.getmembers(module, inspect.isclass)
+                # Filter classes
+                estimators = [
+                    (klass.__name__, klass)
+                    for _, klass in classes
+                    if _is_estimator(klass.__name__, klass)
+                ]
+                all_estimators.extend(estimators)
+            except ModuleNotFoundError as e:
+                # Skip missing soft dependencies
+                if "soft dependency" not in str(e):
+                    raise e
+                warnings.warn(str(e), ImportWarning, stacklevel=2)
+
+    # Drop duplicates
+    all_estimators = set(all_estimators)
+
+    # Filter based on given estimator types
+    if object_types:
+        obj_types = _check_object_types(object_types, class_lookup)
+        all_estimators = [
+            (n, est) for (n, est) in all_estimators if _filter_by_class(est, obj_types)
+        ]
+
+    # Filter based on given exclude list
+    if exclude_objects:
+        exclude_objects = check_sequence(
+            exclude_objects,
+            sequence_type=list,
+            element_type=str,
+            coerce_scalar_input=True,
+            sequence_name="exclude_object",
+        )
+        all_estimators = [
+            (name, estimator)
+            for name, estimator in all_estimators
+            if name not in exclude_objects
+        ]
+
+    # Drop duplicates, sort for reproducibility
+    # itemgetter is used to ensure the sort does not extend to the 2nd item of
+    # the tuple
+    all_estimators = sorted(all_estimators, key=itemgetter(0))
+
+    if filter_tags:
+        all_estimators = [
+            (n, est) for (n, est) in all_estimators if _filter_by_tags(est, filter_tags)
+        ]
+
+    # remove names if return_names=False
+    if not return_names:
+        all_estimators = [estimator for (name, estimator) in all_estimators]
+        columns = ["object"]
+    else:
+        columns = ["name", "object"]
+
+    # add new tuple entries to all_estimators for each tag in return_tags:
+    return_tags = [] if return_tags is None else return_tags
+    if return_tags:
+        return_tags = check_sequence(
+            return_tags,
+            sequence_type=list,
+            element_type=str,
+            coerce_scalar_input=True,
+            sequence_name="return_tags",
+        )
+        # enrich all_estimators by adding the values for all return_tags tags:
+        if all_estimators:
+            if isinstance(all_estimators[0], tuple):
+                all_estimators = [
+                    (name, est) + _get_return_tags(est, return_tags)
+                    for (name, est) in all_estimators
+                ]
+            else:
+                all_estimators = [
+                    (est,) + _get_return_tags(est, return_tags)
+                    for est in all_estimators
+                ]
+        columns = columns + return_tags
+
+    # convert to pandas.DataFrame if as_dataframe=True
+    if as_dataframe:
+        all_estimators = _make_dataframe(all_estimators, columns=columns)
+
+    return all_estimators
+
+
+def _get_return_tags(obj, return_tags):
+    """Fetch a list of all tags for every_entry of all_estimators.
+
+    Parameters
+    ----------
+    obj:  BaseObject
+        A BaseObject.
+    return_tags: list of str
+        Names of tags to get values for the estimator.
+
+    Returns
+    -------
+    tags: a tuple with all the object values for all tags in return tags.
+        a value is None if it is not a valid tag for the object provided.
+    """
+    tags = tuple(obj.get_class_tag(tag) for tag in return_tags)
+    return tags
+
+
+def _check_object_types(object_types, class_lookup=None):
+    """Return list of classes corresponding to type strings.
+
+    Parameters
+    ----------
+    object_types : str, class, or list of string or class
+    class_lookup : dict[string, class], default=None
+
+    Returns
+    -------
+    list of class, i-th element is:
+        class_lookup[object_types[i]] if object_types[i] was a string
+        object_types[i] otherwise
+    if class_lookup is none, only checks whether object_types is class or list of.
+
+    Raises
+    ------
+    ValueError if object_types is not of the expected type.
+    """
+    object_types = deepcopy(object_types)
+
+    if not isinstance(object_types, list):
+        object_types = [object_types]  # make iterable
+
+    def _get_err_msg(estimator_type):
+        if class_lookup is None or not isinstance(class_lookup, dict):
+            return (
+                f"Parameter `estimator_type` must be None, a class, or a list of "
+                f"class, but found: {repr(estimator_type)}"
+            )
+        else:
+            return (
+                f"Parameter `estimator_type` must be None, a string, a class, or a list"
+                f" of [string or class]. Valid string values are: "
+                f"{tuple(class_lookup.keys())}, but found: "
+                f"{repr(estimator_type)}"
+            )
+
+    for i, estimator_type in enumerate(object_types):
+        if isinstance(estimator_type, str):
+            if not isinstance(class_lookup, dict) or (
+                estimator_type not in class_lookup.keys()
+            ):
+                raise ValueError(_get_err_msg(estimator_type))
+            estimator_type = class_lookup[estimator_type]
+            object_types[i] = estimator_type
+        elif isinstance(estimator_type, type):
+            pass
+        else:
+            raise ValueError(_get_err_msg(estimator_type))
+    return object_types
+
+
+def _make_dataframe(all_objects, columns):
+    """Create pandas.DataFrame from all_objects.
+
+    Kept as a separate function with import to isolate the pandas dependency.
+    """
+    import pandas as pd
+
+    return pd.DataFrame(all_objects, columns=columns)
```

### Comparing `skbase-0.4.5/skbase/lookup/tests/test_lookup.py` & `skbase-0.4.6/skbase/lookup/tests/test_lookup.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,991 +1,991 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tests for skbase lookup functionality."""
-# Elements of the lookup tests re-use code developed in sktime. These elements
-# are copyrighted by the sktime developers, BSD-3-Clause License. For
-# conditions see https://github.com/sktime/sktime/blob/main/LICENSE
-import importlib
-import pathlib
-from copy import deepcopy
-from types import ModuleType
-from typing import List
-
-import pandas as pd
-import pytest
-
-from skbase.base import BaseEstimator, BaseObject
-from skbase.base._base import TagAliaserMixin
-from skbase.lookup import all_objects, get_package_metadata
-from skbase.lookup._lookup import (
-    _determine_module_path,
-    _filter_by_class,
-    _filter_by_tags,
-    _get_return_tags,
-    _import_module,
-    _is_ignored_module,
-    _is_non_public_module,
-    _walk,
-)
-from skbase.tests.conftest import (
-    SKBASE_BASE_CLASSES,
-    SKBASE_CLASSES_BY_MODULE,
-    SKBASE_FUNCTIONS_BY_MODULE,
-    SKBASE_MODULES,
-    SKBASE_PUBLIC_CLASSES_BY_MODULE,
-    SKBASE_PUBLIC_FUNCTIONS_BY_MODULE,
-    SKBASE_PUBLIC_MODULES,
-    Parent,
-)
-from skbase.tests.mock_package.test_mock_package import (
-    MOCK_PACKAGE_OBJECTS,
-    CompositionDummy,
-    NotABaseObject,
-)
-
-__author__: List[str] = ["RNKuhns"]
-__all__: List[str] = []
-
-
-MODULE_METADATA_EXPECTED_KEYS = (
-    "path",
-    "name",
-    "classes",
-    "functions",
-    "__all__",
-    "authors",
-    "is_package",
-    "contains_concrete_class_implementations",
-    "contains_base_classes",
-    "contains_base_objects",
-)
-
-SAMPLE_METADATA = {
-    "some_module": {
-        "path": "//some_drive/some_path/",
-        "name": "some_module",
-        "classes": {
-            CompositionDummy.__name__: {
-                "klass": CompositionDummy,
-                "name": CompositionDummy.__name__,
-                "description": "This class does something.",
-                "tags": {},
-                "is_concrete_implementation": True,
-                "is_base_class": False,
-                "is_base_object": True,
-                "authors": "JDoe",
-                "module_name": "some_module",
-            },
-        },
-        "functions": {
-            get_package_metadata.__name__: {
-                "func": get_package_metadata,
-                "name": get_package_metadata.__name__,
-                "description": "This function does stuff.",
-                "module_name": "some_module",
-            },
-        },
-        "__all__": ["SomeClass", "some_function"],
-        "authors": "JDoe",
-        "is_package": True,
-        "contains_concrete_class_implementations": True,
-        "contains_base_classes": False,
-        "contains_base_objects": True,
-    }
-}
-MOD_NAMES = {
-    "public": (
-        "skbase",
-        "skbase.lookup",
-        "some_module.some_sub_module",
-        "tests.test_mock_package",
-    ),
-    "non_public": (
-        "skbase.lookup._lookup",
-        "some_module._some_non_public_sub_module",
-        "_skbase",
-    ),
-}
-REQUIRED_CLASS_METADATA_KEYS = [
-    "klass",
-    "name",
-    "description",
-    "tags",
-    "is_concrete_implementation",
-    "is_base_class",
-    "is_base_object",
-    "authors",
-    "module_name",
-]
-REQUIRED_FUNCTION_METADATA_KEYS = ["func", "name", "description", "module_name"]
-
-
-@pytest.fixture
-def mod_names():
-    """Pytest fixture to return module names for tests."""
-    return MOD_NAMES
-
-
-@pytest.fixture
-def fixture_test_lookup_mod_path():
-    """Fixture path to the lookup module determined from this file's path."""
-    return pathlib.Path(__file__).parent.parent
-
-
-@pytest.fixture
-def fixture_skbase_root_path(fixture_test_lookup_mod_path):
-    """Fixture to root path of skbase package."""
-    return fixture_test_lookup_mod_path.parent
-
-
-@pytest.fixture
-def fixture_sample_package_metadata():
-    """Fixture of sample module metadata."""
-    return SAMPLE_METADATA
-
-
-def _check_package_metadata_result(results):
-    """Check output of get_package_metadata is expected type."""
-    if not (isinstance(results, dict) and all(isinstance(k, str) for k in results)):
-        return False
-    for k, mod_metadata in results.items():
-        if not isinstance(mod_metadata, dict):
-            return False
-        # Verify expected metadata keys are in the module's metadata dict
-        if not all(k in mod_metadata for k in MODULE_METADATA_EXPECTED_KEYS):
-            return False
-        # Verify keys with string values have string values
-        if not all(
-            isinstance(mod_metadata[k], str) for k in ("path", "name", "authors")
-        ):
-            return False
-        # Verify keys with bool values have bool valeus
-        if not all(
-            isinstance(mod_metadata[k], bool)
-            for k in (
-                "is_package",
-                "contains_concrete_class_implementations",
-                "contains_base_classes",
-                "contains_base_objects",
-            )
-        ):
-            return False
-        # Verify __all__ key
-        if not (
-            isinstance(mod_metadata["__all__"], list)
-            and all(isinstance(k, str) for k in mod_metadata["__all__"])
-        ):
-            return False
-        # Verify classes key is a dict that contains string keys and dict values
-        if not (
-            isinstance(mod_metadata["classes"], dict)
-            and all(
-                isinstance(k, str) and isinstance(v, dict)
-                for k, v in mod_metadata["classes"].items()
-            )
-        ):
-            return False
-        # Then verify sub-dict values for each class have required keys
-        elif not all(
-            k in c_meta
-            for c_meta in mod_metadata["classes"].values()
-            for k in REQUIRED_CLASS_METADATA_KEYS
-        ):
-            return False
-        # Verify functions key is a dict that contains string keys and dict values
-        if not (
-            isinstance(mod_metadata["functions"], dict)
-            and all(
-                isinstance(k, str) and isinstance(v, dict)
-                for k, v in mod_metadata["functions"].items()
-            )
-        ):
-            return False
-        # Then verify sub-dict values for each function have required keys
-        elif not all(
-            k in f_meta
-            for f_meta in mod_metadata["functions"].values()
-            for k in REQUIRED_FUNCTION_METADATA_KEYS
-        ):
-            return False
-    # Otherwise return True
-    return True
-
-
-def _check_all_object_output_types(
-    objs, as_dataframe=True, return_names=True, return_tags=None
-):
-    """Check that all_objects output has expected types."""
-    # We expect at least one object to be returned
-    assert len(objs) > 0
-    if as_dataframe:
-        expected_obj_column = 1 if return_names else 0
-        expected_columns = 2 if return_names else 1
-        if isinstance(return_tags, str):
-            expected_columns += 1
-        elif isinstance(return_tags, list):
-            expected_columns += len(return_tags)
-        assert isinstance(objs, pd.DataFrame) and objs.shape[1] == expected_columns
-        # Verify all objects in the object columns are BaseObjects
-        assert (
-            objs.iloc[:, expected_obj_column]
-            .apply(issubclass, args=(BaseObject,))
-            .all()
-        )
-        # If names are returned, verify they are all strings
-        if return_names:
-            assert objs.iloc[:, 0].apply(isinstance, args=(str,)).all()
-            assert (
-                objs.iloc[:, 0] == objs.iloc[:, 1].apply(lambda x: x.__name__)
-            ).all()
-
-    else:
-        # Should return a list
-        assert isinstance(objs, list)
-        # checks return type specification (see docstring)
-        for obj in objs:
-            # return is list of objects if no names or tags requested
-            if not return_names and return_tags is None:
-                assert issubclass(obj, BaseObject)
-            elif return_names:
-                assert isinstance(obj, tuple)
-                assert isinstance(obj[0], str)
-                assert issubclass(obj[1], BaseObject)
-                assert obj[0] == obj[1].__name__
-                if return_tags is None:
-                    assert len(obj) == 2
-                elif isinstance(return_tags, str):
-                    assert len(obj) == 3
-                else:
-                    assert len(obj) == 2 + len(return_tags)
-
-
-def test_check_package_metadata_result(fixture_sample_package_metadata):
-    """Test _check_package_metadata_result works as expected."""
-
-    def _update_mod_metadata(metadata, dict_update):
-        mod_metadata = deepcopy(metadata)
-        # mod_metadata["some_module"] = mod_metadata["some_module"].copy()
-        mod_metadata["some_module"].update(dict_update.copy())
-        return mod_metadata
-
-    assert _check_package_metadata_result(fixture_sample_package_metadata) is True
-    # Input not dict returns False
-    assert _check_package_metadata_result(7) is False
-    # Input that doesn't have string keys mapping to dicts is False
-    assert _check_package_metadata_result({"something": 7}) is False
-    # If keys map to dicts that don't have expected keys then False
-    assert _check_package_metadata_result({"something": {"something_else": 7}}) is False
-    # Make sure keys with wrong type through errors
-    mod_metadata = _update_mod_metadata(fixture_sample_package_metadata, {"name": 7})
-    assert _check_package_metadata_result(mod_metadata) is False
-    # key expected to be boolean set to wrong type
-    mod_metadata = _update_mod_metadata(
-        fixture_sample_package_metadata, {"contains_base_objects": 7}
-    )
-    assert _check_package_metadata_result(mod_metadata) is False
-    # __all__ key is not list
-    mod_metadata = _update_mod_metadata(fixture_sample_package_metadata, {"__all__": 7})
-    assert _check_package_metadata_result(mod_metadata) is False
-    # classes key doesn't map to sub-dict with string keys and dict values
-    mod_metadata = _update_mod_metadata(
-        fixture_sample_package_metadata, {"classes": {"something": 7}}
-    )
-    assert _check_package_metadata_result(mod_metadata) is False
-    # functions key doesn't map to sub-dict with string keys and dict values
-    mod_metadata = _update_mod_metadata(
-        fixture_sample_package_metadata, {"functions": {"something": 7}}
-    )
-    assert _check_package_metadata_result(mod_metadata) is False
-    # Classes key maps to sub-dict with string keys and dict values, but the
-    # dict values don't have correct keys
-    mod_metadata = deepcopy(fixture_sample_package_metadata)
-    mod_metadata["some_module"]["classes"]["CompositionDummy"].pop("name")
-    assert _check_package_metadata_result(mod_metadata) is False
-    # function key maps to sub-dict with string keys and dict values, but the
-    # dict values don't have correct keys
-    mod_metadata = deepcopy(fixture_sample_package_metadata)
-    mod_metadata["some_module"]["functions"]["get_package_metadata"].pop("name")
-    assert _check_package_metadata_result(mod_metadata) is False
-
-
-def test_is_non_public_module(mod_names):
-    """Test _is_non_public_module correctly indentifies non-public modules."""
-    for mod in mod_names["public"]:
-        assert _is_non_public_module(mod) is False
-    for mod in mod_names["non_public"]:
-        assert _is_non_public_module(mod) is True
-
-
-def test_is_non_public_module_raises_error():
-    """Test _is_non_public_module raises a ValueError for non-string input."""
-    with pytest.raises(ValueError):
-        _is_non_public_module(7)
-
-
-def test_is_ignored_module(mod_names):
-    """Test _is_ignored_module correctly identifies modules in ignored sequence."""
-    # Test case when no modules are ignored
-    for mod in mod_names["public"]:
-        assert _is_ignored_module(mod) is False
-
-    # No modules should be flagged as ignored if the ignored moduels aren't encountered
-    modules_to_ignore = ("a_module_not_encountered",)
-    for mod in mod_names["public"]:
-        assert _is_ignored_module(mod, modules_to_ignore=modules_to_ignore) is False
-
-    modules_to_ignore = ("_some",)
-    for mod in mod_names["non_public"]:
-        assert _is_ignored_module(mod, modules_to_ignore=modules_to_ignore) is False
-
-    # When ignored modules are encountered then they should be flagged as True
-    modules_to_ignore = ("skbase", "test_mock_package")
-    for mod in MOD_NAMES["public"]:
-        if "skbase" in mod or "test_mock_package" in mod:
-            expected_to_ignore = True
-        else:
-            expected_to_ignore = False
-        assert (
-            _is_ignored_module(mod, modules_to_ignore=modules_to_ignore)
-            is expected_to_ignore
-        )
-
-
-def test_filter_by_class():
-    """Test _filter_by_class correctly identifies classes."""
-    # Test case when no class filter is applied (should always return True)
-    assert _filter_by_class(CompositionDummy) is True
-
-    # Test case where a signle filter is applied
-    assert _filter_by_class(Parent, BaseObject) is True
-    assert _filter_by_class(NotABaseObject, BaseObject) is False
-    assert _filter_by_class(NotABaseObject, CompositionDummy) is False
-
-    # Test case when sequence of classes supplied as filter
-    assert _filter_by_class(CompositionDummy, (BaseObject, Parent)) is True
-    assert _filter_by_class(CompositionDummy, [NotABaseObject, Parent]) is False
-
-
-def test_filter_by_tags():
-    """Test _filter_by_tags correctly filters classes by their tags or tag values."""
-    # Test case when no tag filter is applied (should always return True)
-    assert _filter_by_tags(CompositionDummy) is True
-    # Even if the class isn't a BaseObject
-    assert _filter_by_tags(NotABaseObject) is True
-
-    # Check when tag_filter is a str and present in the class
-    assert _filter_by_tags(Parent, tag_filter="A") is True
-    # Check when tag_filter is str and not present in the class
-    assert _filter_by_tags(BaseObject, tag_filter="A") is False
-
-    # Test functionality when tag present and object doesn't have tag interface
-    assert _filter_by_tags(NotABaseObject, tag_filter="A") is False
-
-    # Test functionality where tag_filter is Iterable of str
-    # all tags in iterable are in the class
-    assert _filter_by_tags(Parent, ("A", "B", "C")) is True
-    # Some tags in iterable are in class and others aren't
-    assert _filter_by_tags(Parent, ("A", "B", "C", "D", "E")) is False
-
-    # Test functionality where tag_filter is Dict[str, Any]
-    # All keys in dict are in tag_filter and values all match
-    assert _filter_by_tags(Parent, {"A": "1", "B": 2}) is True
-    # All keys in dict are in tag_filter, but at least 1 value doesn't match
-    assert _filter_by_tags(Parent, {"A": 1, "B": 2}) is False
-    # Atleast 1 key in dict is not in tag_filter
-    assert _filter_by_tags(Parent, {"E": 1, "B": 2}) is False
-
-    # Iterable tags should be all strings
-    with pytest.raises(ValueError, match=r"tag_filter"):
-        assert _filter_by_tags(Parent, ("A", "B", 3))
-
-    # Tags that aren't iterable have to be strings
-    with pytest.raises(TypeError, match=r"tag_filter"):
-        assert _filter_by_tags(Parent, 7.0)
-
-    # Dictionary tags should have string keys
-    with pytest.raises(ValueError, match=r"tag_filter"):
-        assert _filter_by_tags(Parent, {7: 11})
-
-
-def test_walk_returns_expected_format(fixture_skbase_root_path):
-    """Check walk function returns expected format."""
-
-    def _test_walk_return(p):
-        assert (
-            isinstance(p, tuple) and len(p) == 3
-        ), "_walk shoul return tuple of length 3"
-        assert (
-            isinstance(p[0], str)
-            and isinstance(p[1], bool)
-            and isinstance(p[2], importlib.machinery.FileFinder)
-        )
-
-    # Test with string path
-    for p in _walk(str(fixture_skbase_root_path)):
-        _test_walk_return(p)
-
-    # Test with pathlib.Path
-    for p in _walk(fixture_skbase_root_path):
-        _test_walk_return(p)
-
-
-def test_walk_returns_expected_exclude(fixture_test_lookup_mod_path):
-    """Check _walk returns expected result when using exclude param."""
-    results = list(_walk(str(fixture_test_lookup_mod_path), exclude="tests"))
-    assert len(results) == 1
-    assert results[0][0] == "_lookup" and results[0][1] is False
-
-
-@pytest.mark.parametrize("prefix", ["skbase."])
-def test_walk_returns_expected_prefix(fixture_skbase_root_path, prefix):
-    """Check _walk returns expected result when using prefix param."""
-    results = list(_walk(str(fixture_skbase_root_path), prefix=prefix))
-    for result in results:
-        assert result[0].startswith(prefix)
-
-
-@pytest.mark.parametrize("suppress_import_stdout", [True, False])
-def test_import_module_returns_module(
-    fixture_test_lookup_mod_path, suppress_import_stdout
-):
-    """Test that _import_module returns a module type."""
-    # Import module based on name case
-    imported_mod = _import_module(
-        "pytest", suppress_import_stdout=suppress_import_stdout
-    )
-    assert isinstance(imported_mod, ModuleType)
-
-    # Import module based on SourceFileLoader for a file path
-    # First specify path to _lookup.py relative to this file
-    path = str(fixture_test_lookup_mod_path / "_lookup.py")
-    loader = importlib.machinery.SourceFileLoader("_lookup", path)
-    imported_mod = _import_module(loader, suppress_import_stdout=suppress_import_stdout)
-    assert isinstance(imported_mod, ModuleType)
-
-
-def test_import_module_raises_error_invalid_input():
-    """Test that _import_module raises an error with invalid input."""
-    match = " ".join(
-        [
-            "`module` should be string module name or instance of",
-            "importlib.machinery.SourceFileLoader.",
-        ]
-    )
-    with pytest.raises(ValueError, match=match):
-        _import_module(7)
-
-
-def test_determine_module_path_output_types(
-    fixture_skbase_root_path, fixture_test_lookup_mod_path
-):
-    """Test _determine_module_path returns expected output types."""
-
-    def _check_determine_module_path(result):
-        assert isinstance(result[0], ModuleType)
-        assert isinstance(result[1], str)
-        assert isinstance(result[2], importlib.machinery.SourceFileLoader)
-
-    # Test with package_name and path
-    result = _determine_module_path("skbase", path=fixture_skbase_root_path)
-    _check_determine_module_path(result)
-    # Test with package_name
-    result = _determine_module_path("pytest")
-    _check_determine_module_path(result)
-
-    path = str(fixture_test_lookup_mod_path / "_lookup.py")
-    # Test with package_name and path
-    result = _determine_module_path("skbase.lookup._lookup", path=path)
-    _check_determine_module_path(result)
-
-
-def test_determine_module_path_raises_error_invalid_input(fixture_skbase_root_path):
-    """Test that _import_module raises an error with invalid input."""
-    with pytest.raises(ValueError):
-        _determine_module_path(7, path=fixture_skbase_root_path)
-
-    with pytest.raises(ValueError):
-        _determine_module_path(fixture_skbase_root_path, path=fixture_skbase_root_path)
-
-    with pytest.raises(ValueError):
-        _determine_module_path("skbase", path=7)
-
-
-@pytest.mark.parametrize("recursive", [True, False])
-@pytest.mark.parametrize("exclude_non_public_items", [True, False])
-@pytest.mark.parametrize("exclude_non_public_modules", [True, False])
-@pytest.mark.parametrize("modules_to_ignore", ["tests", ("testing", "tests"), None])
-@pytest.mark.parametrize(
-    "package_base_classes", [BaseObject, (BaseObject, BaseEstimator), None]
-)
-@pytest.mark.parametrize("suppress_import_stdout", [True, False])
-def test_get_package_metadata_returns_expected_types(
-    recursive,
-    exclude_non_public_items,
-    exclude_non_public_modules,
-    modules_to_ignore,
-    package_base_classes,
-    suppress_import_stdout,
-):
-    """Test get_package_metadata returns expected output types."""
-    results = get_package_metadata(
-        "skbase",
-        recursive=recursive,
-        exclude_non_public_items=exclude_non_public_items,
-        exclude_non_public_modules=exclude_non_public_modules,
-        modules_to_ignore=modules_to_ignore,
-        package_base_classes=package_base_classes,
-        classes_to_exclude=TagAliaserMixin,
-        suppress_import_stdout=suppress_import_stdout,
-    )
-    # Verify we return dict with str keys
-    assert _check_package_metadata_result(results) is True
-
-    # Verify correct behavior of modules_to_ignore
-    no_ignored_module_returned = [
-        not _is_ignored_module(k, modules_to_ignore=modules_to_ignore) for k in results
-    ]
-
-    assert all(no_ignored_module_returned)
-
-    klass_metadata = [
-        klass_metadata
-        for module in results.values()
-        for klass_metadata in module["classes"].values()
-    ]
-    # Verify correct behavior of exclude_non_public_items
-    if exclude_non_public_items:
-        expected_nonpublic_classes_returned = [
-            not k["name"].startswith("_") for k in klass_metadata
-        ]
-        assert all(expected_nonpublic_classes_returned)
-
-        expected_nonpublic_funcs_returned = [
-            not func_metadata["name"].startswith("_")
-            for module in results.values()
-            for func_metadata in module["functions"].values()
-        ]
-        assert all(expected_nonpublic_funcs_returned)
-
-    # Verify correct behavior of exclude_non_public_modules
-    if exclude_non_public_modules:
-        expected_nonpublic_modules_returned = [
-            not _is_non_public_module(k) for k in results
-        ]
-        assert all(expected_nonpublic_modules_returned)
-
-    if package_base_classes is not None:
-        if isinstance(package_base_classes, type):
-            package_base_classes = (package_base_classes,)
-        expected_is_base_class_returned = [
-            k["klass"] in package_base_classes
-            if k["is_base_class"]
-            else k["klass"] not in package_base_classes
-            for k in klass_metadata
-        ]
-        assert all(expected_is_base_class_returned)
-
-
-# This is separate from other get_package_metadata tests b/c right now
-# tests on broader skbase package must exclude TagAliaserMixin or they will error
-# Once TagAliaserMixin is removed or get_class_tags made fully compliant, this
-# will be combined above
-@pytest.mark.parametrize(
-    "classes_to_exclude",
-    [None, CompositionDummy, (CompositionDummy, NotABaseObject)],
-)
-def test_get_package_metadata_classes_to_exclude(classes_to_exclude):
-    """Test get_package_metadata classes_to_exclude param works as expected."""
-    results = get_package_metadata(
-        "skbase.tests",
-        recursive=True,
-        exclude_non_public_items=True,
-        exclude_non_public_modules=True,
-        modules_to_ignore=None,
-        package_base_classes=None,
-        classes_to_exclude=classes_to_exclude,
-        suppress_import_stdout=True,
-    )
-    # Verify we return dict with str keys
-    assert _check_package_metadata_result(results) is True
-    if classes_to_exclude is not None:
-        if isinstance(classes_to_exclude, type):
-            excluded_classes = (classes_to_exclude,)
-        else:
-            excluded_classes = classes_to_exclude
-        # Verify classes_to_exclude works as expected
-        classes_excluded_as_expected = [
-            klass_metadata["klass"] not in excluded_classes
-            for module in results.values()
-            for klass_metadata in module["classes"].values()
-        ]
-        assert all(classes_excluded_as_expected)
-
-
-@pytest.mark.parametrize(
-    "class_filter", [None, BaseEstimator, (BaseObject, BaseEstimator)]
-)
-def test_get_package_metadata_class_filter(class_filter):
-    """Test get_package_metadata filters by class as expected."""
-    # Results applying filter
-    results = get_package_metadata(
-        "skbase",
-        modules_to_ignore="skbase",
-        class_filter=class_filter,
-        classes_to_exclude=TagAliaserMixin,
-    )
-    filtered_classes = [
-        klass_metadata["klass"]
-        for module in results.values()
-        for klass_metadata in module["classes"].values()
-    ]
-
-    # Results without filter
-    unfiltered_results = get_package_metadata(
-        "skbase",
-        modules_to_ignore="skbase",
-        classes_to_exclude=TagAliaserMixin,
-    )
-    unfiltered_classes = [
-        klass_metadata["klass"]
-        for module in unfiltered_results.values()
-        for klass_metadata in module["classes"].values()
-    ]
-
-    # Verify filtered results have right output type
-    assert _check_package_metadata_result(results) is True
-
-    # Now verify class filter is being applied correctly
-    if class_filter is None:
-        assert len(unfiltered_classes) == len(filtered_classes)
-        assert unfiltered_classes == filtered_classes
-    else:
-        assert len(unfiltered_classes) > len(filtered_classes)
-        classes_subclass_class_filter = [
-            issubclass(klass, class_filter) for klass in filtered_classes
-        ]
-        assert all(classes_subclass_class_filter)
-
-
-@pytest.mark.parametrize("tag_filter", [None, "A", ("A", "B"), {"A": "1", "B": 2}])
-def test_get_package_metadata_tag_filter(tag_filter):
-    """Test get_package_metadata filters by tags as expected."""
-    results = get_package_metadata(
-        "skbase",
-        exclude_non_public_modules=False,
-        modules_to_ignore="skbase",
-        tag_filter=tag_filter,
-        classes_to_exclude=TagAliaserMixin,
-    )
-    filtered_classes = [
-        klass_metadata["klass"]
-        for module in results.values()
-        for klass_metadata in module["classes"].values()
-    ]
-
-    # Unfiltered results
-    unfiltered_results = get_package_metadata(
-        "skbase",
-        exclude_non_public_modules=False,
-        modules_to_ignore="skbase",
-        classes_to_exclude=TagAliaserMixin,
-    )
-    unfiltered_classes = [
-        klass_metadata["klass"]
-        for module in unfiltered_results.values()
-        for klass_metadata in module["classes"].values()
-    ]
-
-    # Verify we return dict with str keys
-    assert _check_package_metadata_result(results) is True
-
-    # Verify tag filter is being applied correctly, which implies
-    # When the filter is None the result is the same size
-    # Otherwise, with the filters used in the test, fewer classes should
-    # be returned
-    if tag_filter is None:
-        assert len(unfiltered_classes) == len(filtered_classes)
-        assert unfiltered_classes == filtered_classes
-    else:
-        assert len(unfiltered_classes) > len(filtered_classes)
-
-
-@pytest.mark.parametrize("exclude_non_public_modules", [True, False])
-@pytest.mark.parametrize("exclude_non_public_items", [True, False])
-def test_get_package_metadata_returns_expected_results(
-    exclude_non_public_modules, exclude_non_public_items
-):
-    """Test that get_package_metadata_returns expected results using skbase."""
-    results = get_package_metadata(
-        "skbase",
-        exclude_non_public_items=exclude_non_public_items,
-        exclude_non_public_modules=exclude_non_public_modules,
-        package_base_classes=SKBASE_BASE_CLASSES,
-        modules_to_ignore="tests",
-        classes_to_exclude=TagAliaserMixin,
-        suppress_import_stdout=False,
-    )
-    public_modules_excluding_tests = [
-        module
-        for module in SKBASE_PUBLIC_MODULES
-        if not _is_ignored_module(module, modules_to_ignore="tests")
-    ]
-    modules_excluding_tests = [
-        module
-        for module in SKBASE_MODULES
-        if not _is_ignored_module(module, modules_to_ignore="tests")
-    ]
-    if exclude_non_public_modules:
-        assert tuple(results.keys()) == tuple(public_modules_excluding_tests)
-    else:
-        assert tuple(results.keys()) == tuple(modules_excluding_tests)
-
-    for module in results:
-        if exclude_non_public_items:
-            module_funcs = SKBASE_PUBLIC_FUNCTIONS_BY_MODULE.get(module, ())
-            module_classes = SKBASE_PUBLIC_CLASSES_BY_MODULE.get(module, ())
-        else:
-            module_funcs = SKBASE_FUNCTIONS_BY_MODULE.get(module, ())
-            module_classes = SKBASE_CLASSES_BY_MODULE.get(module, ())
-
-        # Verify expected functions are returned
-        assert set(results[module]["functions"].keys()) == set(module_funcs)
-        # Verify expected classes are returned
-        assert set(results[module]["classes"].keys()) == set(module_classes)
-
-        # Verify class metadata attributes correct
-        for klass, klass_metadata in results[module]["classes"].items():
-            if klass_metadata["klass"] in SKBASE_BASE_CLASSES:
-                assert (
-                    klass_metadata["is_base_class"] is True
-                ), f"{klass} should be base class."
-            else:
-                assert (
-                    klass_metadata["is_base_class"] is False
-                ), f"{klass} should not be base class."
-
-            if issubclass(klass_metadata["klass"], BaseObject):
-                assert klass_metadata["is_base_object"] is True
-            else:
-                assert klass_metadata["is_base_object"] is False
-
-            if (
-                issubclass(klass_metadata["klass"], SKBASE_BASE_CLASSES)
-                and klass_metadata["klass"] not in SKBASE_BASE_CLASSES
-            ):
-                assert klass_metadata["is_concrete_implementation"] is True
-            else:
-                assert klass_metadata["is_concrete_implementation"] is False
-
-
-def test_get_return_tags():
-    """Test _get_return_tags returns expected."""
-
-    def _test_get_return_tags_output(results, num_requested_tags):
-        return isinstance(results, tuple) and len(results) == num_requested_tags
-
-    # Verify return with tags that exist
-    tags = Parent.get_class_tags()
-    tag_names = [*tags.keys()]
-    results = _get_return_tags(Parent, tag_names)
-    assert (
-        _test_get_return_tags_output(results, len(tag_names))
-        and tuple(tags.values()) == results
-    )
-
-    # Verify results when some exist and some don't exist
-    tag_names += ["a_tag_that_does_not_exist"]
-    results = _get_return_tags(Parent, tag_names)
-    assert _test_get_return_tags_output(results, len(tag_names))
-
-    # Verify return when all tags don't exist
-    tag_names = ["a_tag_that_does_not_exist"]
-    results = _get_return_tags(Parent, tag_names)
-    assert _test_get_return_tags_output(results, len(tag_names)) and results[0] is None
-
-
-@pytest.mark.parametrize("as_dataframe", [True, False])
-@pytest.mark.parametrize("return_names", [True, False])
-@pytest.mark.parametrize("return_tags", [None, "A", ["A", "a_non_existant_tag"]])
-@pytest.mark.parametrize("modules_to_ignore", ["tests", ("testing", "lookup"), None])
-@pytest.mark.parametrize("exclude_objects", [None, "Child", ["CompositionDummy"]])
-@pytest.mark.parametrize("suppress_import_stdout", [True, False])
-def test_all_objects_returns_expected_types(
-    as_dataframe,
-    return_names,
-    return_tags,
-    modules_to_ignore,
-    exclude_objects,
-    suppress_import_stdout,
-):
-    """Test that all_objects return argument has correct type."""
-    objs = all_objects(
-        package_name="skbase",
-        exclude_objects=exclude_objects,
-        return_names=return_names,
-        as_dataframe=as_dataframe,
-        return_tags=return_tags,
-        modules_to_ignore=modules_to_ignore,
-        suppress_import_stdout=suppress_import_stdout,
-    )
-    if isinstance(modules_to_ignore, str):
-        modules_to_ignore = (modules_to_ignore,)
-    if (
-        modules_to_ignore is not None
-        and "tests" in modules_to_ignore
-        # and "mock_package" in modules_to_ignore
-    ):
-        assert (
-            len(objs) == 0
-        ), "Search of `skbase` should only return objects from tests module."
-    else:
-        # We expect at least one object to be returned so we verify output type/format
-        _check_all_object_output_types(
-            objs,
-            as_dataframe=as_dataframe,
-            return_names=return_names,
-            return_tags=return_tags,
-        )
-
-
-@pytest.mark.parametrize(
-    "exclude_objects", [None, "Parent", ["Child", "CompositionDummy"]]
-)
-def test_all_objects_returns_expected_output(exclude_objects):
-    """Test that all_objects return argument has correct output for skbase."""
-    objs = all_objects(
-        package_name="skbase.tests.mock_package",
-        exclude_objects=exclude_objects,
-        return_names=True,
-        as_dataframe=True,
-        modules_to_ignore="conftest",
-        suppress_import_stdout=True,
-    )
-    klasses = objs["object"].tolist()
-    test_classes = [
-        k
-        for k in MOCK_PACKAGE_OBJECTS
-        if issubclass(k, BaseObject) and not k.__name__.startswith("_")
-    ]
-    if exclude_objects is not None:
-        if isinstance(exclude_objects, str):
-            exclude_objects = (exclude_objects,)
-        # Exclude classes from MOCK_PACKAGE_OBJECTS
-        test_classes = [k for k in test_classes if k.__name__ not in exclude_objects]
-
-    msg = f"{klasses} should match test classes {test_classes}."
-    assert set(klasses) == set(test_classes), msg
-
-
-@pytest.mark.parametrize("class_filter", [None, Parent, [Parent, BaseEstimator]])
-def test_all_objects_class_filter(class_filter):
-    """Test all_objects filters by class type as expected."""
-    # Results applying filter
-    objs = all_objects(
-        package_name="skbase",
-        return_names=True,
-        as_dataframe=True,
-        return_tags=None,
-        object_types=class_filter,
-    )
-    filtered_classes = objs.iloc[:, 1].tolist()
-    # Verify filtered results have right output type
-    _check_all_object_output_types(
-        objs, as_dataframe=True, return_names=True, return_tags=None
-    )
-
-    # Results without filter
-    objs = all_objects(
-        package_name="skbase",
-        return_names=True,
-        as_dataframe=True,
-        return_tags=None,
-    )
-    unfiltered_classes = objs.iloc[:, 1].tolist()
-
-    # Now verify class filter is being applied correctly
-    if class_filter is None:
-        assert len(unfiltered_classes) == len(filtered_classes)
-        assert unfiltered_classes == filtered_classes
-    else:
-        if not isinstance(class_filter, type):
-            class_filter = tuple(class_filter)
-        assert len(unfiltered_classes) > len(filtered_classes)
-        classes_subclass_class_filter = [
-            issubclass(klass, class_filter) for klass in filtered_classes
-        ]
-        assert all(classes_subclass_class_filter)
-
-
-@pytest.mark.parametrize("tag_filter", [None, "A", ("A", "B"), {"A": "1", "B": 2}])
-def test_all_object_tag_filter(tag_filter):
-    """Test all_objects filters by tag as expected."""
-    # Results applying filter
-    objs = all_objects(
-        package_name="skbase",
-        return_names=True,
-        as_dataframe=True,
-        return_tags=None,
-        filter_tags=tag_filter,
-    )
-    filtered_classes = objs.iloc[:, 1].tolist()
-    # Verify filtered results have right output type
-    _check_all_object_output_types(
-        objs, as_dataframe=True, return_names=True, return_tags=None
-    )
-
-    # Results without filter
-    objs = all_objects(
-        package_name="skbase",
-        return_names=True,
-        as_dataframe=True,
-        return_tags=None,
-    )
-    unfiltered_classes = objs.iloc[:, 1].tolist()
-
-    # Verify tag filter is being applied correctly, which implies
-    # When the filter is None the result is the same size
-    # Otherwise, with the filters used in the test, fewer classes should
-    # be returned
-    if tag_filter is None:
-        assert len(unfiltered_classes) == len(filtered_classes)
-        assert unfiltered_classes == filtered_classes
-    else:
-        assert len(unfiltered_classes) > len(filtered_classes)
-
-
-@pytest.mark.parametrize("class_lookup", [{"base_object": BaseObject}])
-@pytest.mark.parametrize("class_filter", [None, "base_object"])
-def test_all_object_class_lookup(class_lookup, class_filter):
-    """Test all_objects class_lookup parameter works as expected.."""
-    # Results applying filter
-    objs = all_objects(
-        package_name="skbase",
-        return_names=True,
-        as_dataframe=True,
-        return_tags=None,
-        object_types=class_filter,
-        class_lookup=class_lookup,
-    )
-    # filtered_classes = objs.iloc[:, 1].tolist()
-    # Verify filtered results have right output type
-    _check_all_object_output_types(
-        objs, as_dataframe=True, return_names=True, return_tags=None
-    )
-
-
-@pytest.mark.parametrize("class_lookup", [None, {"base_object": BaseObject}])
-@pytest.mark.parametrize("class_filter", ["invalid_alias", 7])
-def test_all_object_class_lookup_invalid_object_types_raises(
-    class_lookup, class_filter
-):
-    """Test all_objects use of object filtering raises errors as expected."""
-    # Results applying filter
-    with pytest.raises(ValueError):
-        all_objects(
-            package_name="skbase",
-            return_names=True,
-            as_dataframe=True,
-            return_tags=None,
-            object_types=class_filter,
-            class_lookup=class_lookup,
-        )
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tests for skbase lookup functionality."""
+# Elements of the lookup tests re-use code developed in sktime. These elements
+# are copyrighted by the sktime developers, BSD-3-Clause License. For
+# conditions see https://github.com/sktime/sktime/blob/main/LICENSE
+import importlib
+import pathlib
+from copy import deepcopy
+from types import ModuleType
+from typing import List
+
+import pandas as pd
+import pytest
+
+from skbase.base import BaseEstimator, BaseObject
+from skbase.base._base import TagAliaserMixin
+from skbase.lookup import all_objects, get_package_metadata
+from skbase.lookup._lookup import (
+    _determine_module_path,
+    _filter_by_class,
+    _filter_by_tags,
+    _get_return_tags,
+    _import_module,
+    _is_ignored_module,
+    _is_non_public_module,
+    _walk,
+)
+from skbase.tests.conftest import (
+    SKBASE_BASE_CLASSES,
+    SKBASE_CLASSES_BY_MODULE,
+    SKBASE_FUNCTIONS_BY_MODULE,
+    SKBASE_MODULES,
+    SKBASE_PUBLIC_CLASSES_BY_MODULE,
+    SKBASE_PUBLIC_FUNCTIONS_BY_MODULE,
+    SKBASE_PUBLIC_MODULES,
+    Parent,
+)
+from skbase.tests.mock_package.test_mock_package import (
+    MOCK_PACKAGE_OBJECTS,
+    CompositionDummy,
+    NotABaseObject,
+)
+
+__author__: List[str] = ["RNKuhns"]
+__all__: List[str] = []
+
+
+MODULE_METADATA_EXPECTED_KEYS = (
+    "path",
+    "name",
+    "classes",
+    "functions",
+    "__all__",
+    "authors",
+    "is_package",
+    "contains_concrete_class_implementations",
+    "contains_base_classes",
+    "contains_base_objects",
+)
+
+SAMPLE_METADATA = {
+    "some_module": {
+        "path": "//some_drive/some_path/",
+        "name": "some_module",
+        "classes": {
+            CompositionDummy.__name__: {
+                "klass": CompositionDummy,
+                "name": CompositionDummy.__name__,
+                "description": "This class does something.",
+                "tags": {},
+                "is_concrete_implementation": True,
+                "is_base_class": False,
+                "is_base_object": True,
+                "authors": "JDoe",
+                "module_name": "some_module",
+            },
+        },
+        "functions": {
+            get_package_metadata.__name__: {
+                "func": get_package_metadata,
+                "name": get_package_metadata.__name__,
+                "description": "This function does stuff.",
+                "module_name": "some_module",
+            },
+        },
+        "__all__": ["SomeClass", "some_function"],
+        "authors": "JDoe",
+        "is_package": True,
+        "contains_concrete_class_implementations": True,
+        "contains_base_classes": False,
+        "contains_base_objects": True,
+    }
+}
+MOD_NAMES = {
+    "public": (
+        "skbase",
+        "skbase.lookup",
+        "some_module.some_sub_module",
+        "tests.test_mock_package",
+    ),
+    "non_public": (
+        "skbase.lookup._lookup",
+        "some_module._some_non_public_sub_module",
+        "_skbase",
+    ),
+}
+REQUIRED_CLASS_METADATA_KEYS = [
+    "klass",
+    "name",
+    "description",
+    "tags",
+    "is_concrete_implementation",
+    "is_base_class",
+    "is_base_object",
+    "authors",
+    "module_name",
+]
+REQUIRED_FUNCTION_METADATA_KEYS = ["func", "name", "description", "module_name"]
+
+
+@pytest.fixture
+def mod_names():
+    """Pytest fixture to return module names for tests."""
+    return MOD_NAMES
+
+
+@pytest.fixture
+def fixture_test_lookup_mod_path():
+    """Fixture path to the lookup module determined from this file's path."""
+    return pathlib.Path(__file__).parent.parent
+
+
+@pytest.fixture
+def fixture_skbase_root_path(fixture_test_lookup_mod_path):
+    """Fixture to root path of skbase package."""
+    return fixture_test_lookup_mod_path.parent
+
+
+@pytest.fixture
+def fixture_sample_package_metadata():
+    """Fixture of sample module metadata."""
+    return SAMPLE_METADATA
+
+
+def _check_package_metadata_result(results):
+    """Check output of get_package_metadata is expected type."""
+    if not (isinstance(results, dict) and all(isinstance(k, str) for k in results)):
+        return False
+    for k, mod_metadata in results.items():
+        if not isinstance(mod_metadata, dict):
+            return False
+        # Verify expected metadata keys are in the module's metadata dict
+        if not all(k in mod_metadata for k in MODULE_METADATA_EXPECTED_KEYS):
+            return False
+        # Verify keys with string values have string values
+        if not all(
+            isinstance(mod_metadata[k], str) for k in ("path", "name", "authors")
+        ):
+            return False
+        # Verify keys with bool values have bool valeus
+        if not all(
+            isinstance(mod_metadata[k], bool)
+            for k in (
+                "is_package",
+                "contains_concrete_class_implementations",
+                "contains_base_classes",
+                "contains_base_objects",
+            )
+        ):
+            return False
+        # Verify __all__ key
+        if not (
+            isinstance(mod_metadata["__all__"], list)
+            and all(isinstance(k, str) for k in mod_metadata["__all__"])
+        ):
+            return False
+        # Verify classes key is a dict that contains string keys and dict values
+        if not (
+            isinstance(mod_metadata["classes"], dict)
+            and all(
+                isinstance(k, str) and isinstance(v, dict)
+                for k, v in mod_metadata["classes"].items()
+            )
+        ):
+            return False
+        # Then verify sub-dict values for each class have required keys
+        elif not all(
+            k in c_meta
+            for c_meta in mod_metadata["classes"].values()
+            for k in REQUIRED_CLASS_METADATA_KEYS
+        ):
+            return False
+        # Verify functions key is a dict that contains string keys and dict values
+        if not (
+            isinstance(mod_metadata["functions"], dict)
+            and all(
+                isinstance(k, str) and isinstance(v, dict)
+                for k, v in mod_metadata["functions"].items()
+            )
+        ):
+            return False
+        # Then verify sub-dict values for each function have required keys
+        elif not all(
+            k in f_meta
+            for f_meta in mod_metadata["functions"].values()
+            for k in REQUIRED_FUNCTION_METADATA_KEYS
+        ):
+            return False
+    # Otherwise return True
+    return True
+
+
+def _check_all_object_output_types(
+    objs, as_dataframe=True, return_names=True, return_tags=None
+):
+    """Check that all_objects output has expected types."""
+    # We expect at least one object to be returned
+    assert len(objs) > 0
+    if as_dataframe:
+        expected_obj_column = 1 if return_names else 0
+        expected_columns = 2 if return_names else 1
+        if isinstance(return_tags, str):
+            expected_columns += 1
+        elif isinstance(return_tags, list):
+            expected_columns += len(return_tags)
+        assert isinstance(objs, pd.DataFrame) and objs.shape[1] == expected_columns
+        # Verify all objects in the object columns are BaseObjects
+        assert (
+            objs.iloc[:, expected_obj_column]
+            .apply(issubclass, args=(BaseObject,))
+            .all()
+        )
+        # If names are returned, verify they are all strings
+        if return_names:
+            assert objs.iloc[:, 0].apply(isinstance, args=(str,)).all()
+            assert (
+                objs.iloc[:, 0] == objs.iloc[:, 1].apply(lambda x: x.__name__)
+            ).all()
+
+    else:
+        # Should return a list
+        assert isinstance(objs, list)
+        # checks return type specification (see docstring)
+        for obj in objs:
+            # return is list of objects if no names or tags requested
+            if not return_names and return_tags is None:
+                assert issubclass(obj, BaseObject)
+            elif return_names:
+                assert isinstance(obj, tuple)
+                assert isinstance(obj[0], str)
+                assert issubclass(obj[1], BaseObject)
+                assert obj[0] == obj[1].__name__
+                if return_tags is None:
+                    assert len(obj) == 2
+                elif isinstance(return_tags, str):
+                    assert len(obj) == 3
+                else:
+                    assert len(obj) == 2 + len(return_tags)
+
+
+def test_check_package_metadata_result(fixture_sample_package_metadata):
+    """Test _check_package_metadata_result works as expected."""
+
+    def _update_mod_metadata(metadata, dict_update):
+        mod_metadata = deepcopy(metadata)
+        # mod_metadata["some_module"] = mod_metadata["some_module"].copy()
+        mod_metadata["some_module"].update(dict_update.copy())
+        return mod_metadata
+
+    assert _check_package_metadata_result(fixture_sample_package_metadata) is True
+    # Input not dict returns False
+    assert _check_package_metadata_result(7) is False
+    # Input that doesn't have string keys mapping to dicts is False
+    assert _check_package_metadata_result({"something": 7}) is False
+    # If keys map to dicts that don't have expected keys then False
+    assert _check_package_metadata_result({"something": {"something_else": 7}}) is False
+    # Make sure keys with wrong type through errors
+    mod_metadata = _update_mod_metadata(fixture_sample_package_metadata, {"name": 7})
+    assert _check_package_metadata_result(mod_metadata) is False
+    # key expected to be boolean set to wrong type
+    mod_metadata = _update_mod_metadata(
+        fixture_sample_package_metadata, {"contains_base_objects": 7}
+    )
+    assert _check_package_metadata_result(mod_metadata) is False
+    # __all__ key is not list
+    mod_metadata = _update_mod_metadata(fixture_sample_package_metadata, {"__all__": 7})
+    assert _check_package_metadata_result(mod_metadata) is False
+    # classes key doesn't map to sub-dict with string keys and dict values
+    mod_metadata = _update_mod_metadata(
+        fixture_sample_package_metadata, {"classes": {"something": 7}}
+    )
+    assert _check_package_metadata_result(mod_metadata) is False
+    # functions key doesn't map to sub-dict with string keys and dict values
+    mod_metadata = _update_mod_metadata(
+        fixture_sample_package_metadata, {"functions": {"something": 7}}
+    )
+    assert _check_package_metadata_result(mod_metadata) is False
+    # Classes key maps to sub-dict with string keys and dict values, but the
+    # dict values don't have correct keys
+    mod_metadata = deepcopy(fixture_sample_package_metadata)
+    mod_metadata["some_module"]["classes"]["CompositionDummy"].pop("name")
+    assert _check_package_metadata_result(mod_metadata) is False
+    # function key maps to sub-dict with string keys and dict values, but the
+    # dict values don't have correct keys
+    mod_metadata = deepcopy(fixture_sample_package_metadata)
+    mod_metadata["some_module"]["functions"]["get_package_metadata"].pop("name")
+    assert _check_package_metadata_result(mod_metadata) is False
+
+
+def test_is_non_public_module(mod_names):
+    """Test _is_non_public_module correctly indentifies non-public modules."""
+    for mod in mod_names["public"]:
+        assert _is_non_public_module(mod) is False
+    for mod in mod_names["non_public"]:
+        assert _is_non_public_module(mod) is True
+
+
+def test_is_non_public_module_raises_error():
+    """Test _is_non_public_module raises a ValueError for non-string input."""
+    with pytest.raises(ValueError):
+        _is_non_public_module(7)
+
+
+def test_is_ignored_module(mod_names):
+    """Test _is_ignored_module correctly identifies modules in ignored sequence."""
+    # Test case when no modules are ignored
+    for mod in mod_names["public"]:
+        assert _is_ignored_module(mod) is False
+
+    # No modules should be flagged as ignored if the ignored moduels aren't encountered
+    modules_to_ignore = ("a_module_not_encountered",)
+    for mod in mod_names["public"]:
+        assert _is_ignored_module(mod, modules_to_ignore=modules_to_ignore) is False
+
+    modules_to_ignore = ("_some",)
+    for mod in mod_names["non_public"]:
+        assert _is_ignored_module(mod, modules_to_ignore=modules_to_ignore) is False
+
+    # When ignored modules are encountered then they should be flagged as True
+    modules_to_ignore = ("skbase", "test_mock_package")
+    for mod in MOD_NAMES["public"]:
+        if "skbase" in mod or "test_mock_package" in mod:
+            expected_to_ignore = True
+        else:
+            expected_to_ignore = False
+        assert (
+            _is_ignored_module(mod, modules_to_ignore=modules_to_ignore)
+            is expected_to_ignore
+        )
+
+
+def test_filter_by_class():
+    """Test _filter_by_class correctly identifies classes."""
+    # Test case when no class filter is applied (should always return True)
+    assert _filter_by_class(CompositionDummy) is True
+
+    # Test case where a signle filter is applied
+    assert _filter_by_class(Parent, BaseObject) is True
+    assert _filter_by_class(NotABaseObject, BaseObject) is False
+    assert _filter_by_class(NotABaseObject, CompositionDummy) is False
+
+    # Test case when sequence of classes supplied as filter
+    assert _filter_by_class(CompositionDummy, (BaseObject, Parent)) is True
+    assert _filter_by_class(CompositionDummy, [NotABaseObject, Parent]) is False
+
+
+def test_filter_by_tags():
+    """Test _filter_by_tags correctly filters classes by their tags or tag values."""
+    # Test case when no tag filter is applied (should always return True)
+    assert _filter_by_tags(CompositionDummy) is True
+    # Even if the class isn't a BaseObject
+    assert _filter_by_tags(NotABaseObject) is True
+
+    # Check when tag_filter is a str and present in the class
+    assert _filter_by_tags(Parent, tag_filter="A") is True
+    # Check when tag_filter is str and not present in the class
+    assert _filter_by_tags(BaseObject, tag_filter="A") is False
+
+    # Test functionality when tag present and object doesn't have tag interface
+    assert _filter_by_tags(NotABaseObject, tag_filter="A") is False
+
+    # Test functionality where tag_filter is Iterable of str
+    # all tags in iterable are in the class
+    assert _filter_by_tags(Parent, ("A", "B", "C")) is True
+    # Some tags in iterable are in class and others aren't
+    assert _filter_by_tags(Parent, ("A", "B", "C", "D", "E")) is False
+
+    # Test functionality where tag_filter is Dict[str, Any]
+    # All keys in dict are in tag_filter and values all match
+    assert _filter_by_tags(Parent, {"A": "1", "B": 2}) is True
+    # All keys in dict are in tag_filter, but at least 1 value doesn't match
+    assert _filter_by_tags(Parent, {"A": 1, "B": 2}) is False
+    # Atleast 1 key in dict is not in tag_filter
+    assert _filter_by_tags(Parent, {"E": 1, "B": 2}) is False
+
+    # Iterable tags should be all strings
+    with pytest.raises(ValueError, match=r"tag_filter"):
+        assert _filter_by_tags(Parent, ("A", "B", 3))
+
+    # Tags that aren't iterable have to be strings
+    with pytest.raises(TypeError, match=r"tag_filter"):
+        assert _filter_by_tags(Parent, 7.0)
+
+    # Dictionary tags should have string keys
+    with pytest.raises(ValueError, match=r"tag_filter"):
+        assert _filter_by_tags(Parent, {7: 11})
+
+
+def test_walk_returns_expected_format(fixture_skbase_root_path):
+    """Check walk function returns expected format."""
+
+    def _test_walk_return(p):
+        assert (
+            isinstance(p, tuple) and len(p) == 3
+        ), "_walk shoul return tuple of length 3"
+        assert (
+            isinstance(p[0], str)
+            and isinstance(p[1], bool)
+            and isinstance(p[2], importlib.machinery.FileFinder)
+        )
+
+    # Test with string path
+    for p in _walk(str(fixture_skbase_root_path)):
+        _test_walk_return(p)
+
+    # Test with pathlib.Path
+    for p in _walk(fixture_skbase_root_path):
+        _test_walk_return(p)
+
+
+def test_walk_returns_expected_exclude(fixture_test_lookup_mod_path):
+    """Check _walk returns expected result when using exclude param."""
+    results = list(_walk(str(fixture_test_lookup_mod_path), exclude="tests"))
+    assert len(results) == 1
+    assert results[0][0] == "_lookup" and results[0][1] is False
+
+
+@pytest.mark.parametrize("prefix", ["skbase."])
+def test_walk_returns_expected_prefix(fixture_skbase_root_path, prefix):
+    """Check _walk returns expected result when using prefix param."""
+    results = list(_walk(str(fixture_skbase_root_path), prefix=prefix))
+    for result in results:
+        assert result[0].startswith(prefix)
+
+
+@pytest.mark.parametrize("suppress_import_stdout", [True, False])
+def test_import_module_returns_module(
+    fixture_test_lookup_mod_path, suppress_import_stdout
+):
+    """Test that _import_module returns a module type."""
+    # Import module based on name case
+    imported_mod = _import_module(
+        "pytest", suppress_import_stdout=suppress_import_stdout
+    )
+    assert isinstance(imported_mod, ModuleType)
+
+    # Import module based on SourceFileLoader for a file path
+    # First specify path to _lookup.py relative to this file
+    path = str(fixture_test_lookup_mod_path / "_lookup.py")
+    loader = importlib.machinery.SourceFileLoader("_lookup", path)
+    imported_mod = _import_module(loader, suppress_import_stdout=suppress_import_stdout)
+    assert isinstance(imported_mod, ModuleType)
+
+
+def test_import_module_raises_error_invalid_input():
+    """Test that _import_module raises an error with invalid input."""
+    match = " ".join(
+        [
+            "`module` should be string module name or instance of",
+            "importlib.machinery.SourceFileLoader.",
+        ]
+    )
+    with pytest.raises(ValueError, match=match):
+        _import_module(7)
+
+
+def test_determine_module_path_output_types(
+    fixture_skbase_root_path, fixture_test_lookup_mod_path
+):
+    """Test _determine_module_path returns expected output types."""
+
+    def _check_determine_module_path(result):
+        assert isinstance(result[0], ModuleType)
+        assert isinstance(result[1], str)
+        assert isinstance(result[2], importlib.machinery.SourceFileLoader)
+
+    # Test with package_name and path
+    result = _determine_module_path("skbase", path=fixture_skbase_root_path)
+    _check_determine_module_path(result)
+    # Test with package_name
+    result = _determine_module_path("pytest")
+    _check_determine_module_path(result)
+
+    path = str(fixture_test_lookup_mod_path / "_lookup.py")
+    # Test with package_name and path
+    result = _determine_module_path("skbase.lookup._lookup", path=path)
+    _check_determine_module_path(result)
+
+
+def test_determine_module_path_raises_error_invalid_input(fixture_skbase_root_path):
+    """Test that _import_module raises an error with invalid input."""
+    with pytest.raises(ValueError):
+        _determine_module_path(7, path=fixture_skbase_root_path)
+
+    with pytest.raises(ValueError):
+        _determine_module_path(fixture_skbase_root_path, path=fixture_skbase_root_path)
+
+    with pytest.raises(ValueError):
+        _determine_module_path("skbase", path=7)
+
+
+@pytest.mark.parametrize("recursive", [True, False])
+@pytest.mark.parametrize("exclude_non_public_items", [True, False])
+@pytest.mark.parametrize("exclude_non_public_modules", [True, False])
+@pytest.mark.parametrize("modules_to_ignore", ["tests", ("testing", "tests"), None])
+@pytest.mark.parametrize(
+    "package_base_classes", [BaseObject, (BaseObject, BaseEstimator), None]
+)
+@pytest.mark.parametrize("suppress_import_stdout", [True, False])
+def test_get_package_metadata_returns_expected_types(
+    recursive,
+    exclude_non_public_items,
+    exclude_non_public_modules,
+    modules_to_ignore,
+    package_base_classes,
+    suppress_import_stdout,
+):
+    """Test get_package_metadata returns expected output types."""
+    results = get_package_metadata(
+        "skbase",
+        recursive=recursive,
+        exclude_non_public_items=exclude_non_public_items,
+        exclude_non_public_modules=exclude_non_public_modules,
+        modules_to_ignore=modules_to_ignore,
+        package_base_classes=package_base_classes,
+        classes_to_exclude=TagAliaserMixin,
+        suppress_import_stdout=suppress_import_stdout,
+    )
+    # Verify we return dict with str keys
+    assert _check_package_metadata_result(results) is True
+
+    # Verify correct behavior of modules_to_ignore
+    no_ignored_module_returned = [
+        not _is_ignored_module(k, modules_to_ignore=modules_to_ignore) for k in results
+    ]
+
+    assert all(no_ignored_module_returned)
+
+    klass_metadata = [
+        klass_metadata
+        for module in results.values()
+        for klass_metadata in module["classes"].values()
+    ]
+    # Verify correct behavior of exclude_non_public_items
+    if exclude_non_public_items:
+        expected_nonpublic_classes_returned = [
+            not k["name"].startswith("_") for k in klass_metadata
+        ]
+        assert all(expected_nonpublic_classes_returned)
+
+        expected_nonpublic_funcs_returned = [
+            not func_metadata["name"].startswith("_")
+            for module in results.values()
+            for func_metadata in module["functions"].values()
+        ]
+        assert all(expected_nonpublic_funcs_returned)
+
+    # Verify correct behavior of exclude_non_public_modules
+    if exclude_non_public_modules:
+        expected_nonpublic_modules_returned = [
+            not _is_non_public_module(k) for k in results
+        ]
+        assert all(expected_nonpublic_modules_returned)
+
+    if package_base_classes is not None:
+        if isinstance(package_base_classes, type):
+            package_base_classes = (package_base_classes,)
+        expected_is_base_class_returned = [
+            k["klass"] in package_base_classes
+            if k["is_base_class"]
+            else k["klass"] not in package_base_classes
+            for k in klass_metadata
+        ]
+        assert all(expected_is_base_class_returned)
+
+
+# This is separate from other get_package_metadata tests b/c right now
+# tests on broader skbase package must exclude TagAliaserMixin or they will error
+# Once TagAliaserMixin is removed or get_class_tags made fully compliant, this
+# will be combined above
+@pytest.mark.parametrize(
+    "classes_to_exclude",
+    [None, CompositionDummy, (CompositionDummy, NotABaseObject)],
+)
+def test_get_package_metadata_classes_to_exclude(classes_to_exclude):
+    """Test get_package_metadata classes_to_exclude param works as expected."""
+    results = get_package_metadata(
+        "skbase.tests",
+        recursive=True,
+        exclude_non_public_items=True,
+        exclude_non_public_modules=True,
+        modules_to_ignore=None,
+        package_base_classes=None,
+        classes_to_exclude=classes_to_exclude,
+        suppress_import_stdout=True,
+    )
+    # Verify we return dict with str keys
+    assert _check_package_metadata_result(results) is True
+    if classes_to_exclude is not None:
+        if isinstance(classes_to_exclude, type):
+            excluded_classes = (classes_to_exclude,)
+        else:
+            excluded_classes = classes_to_exclude
+        # Verify classes_to_exclude works as expected
+        classes_excluded_as_expected = [
+            klass_metadata["klass"] not in excluded_classes
+            for module in results.values()
+            for klass_metadata in module["classes"].values()
+        ]
+        assert all(classes_excluded_as_expected)
+
+
+@pytest.mark.parametrize(
+    "class_filter", [None, BaseEstimator, (BaseObject, BaseEstimator)]
+)
+def test_get_package_metadata_class_filter(class_filter):
+    """Test get_package_metadata filters by class as expected."""
+    # Results applying filter
+    results = get_package_metadata(
+        "skbase",
+        modules_to_ignore="skbase",
+        class_filter=class_filter,
+        classes_to_exclude=TagAliaserMixin,
+    )
+    filtered_classes = [
+        klass_metadata["klass"]
+        for module in results.values()
+        for klass_metadata in module["classes"].values()
+    ]
+
+    # Results without filter
+    unfiltered_results = get_package_metadata(
+        "skbase",
+        modules_to_ignore="skbase",
+        classes_to_exclude=TagAliaserMixin,
+    )
+    unfiltered_classes = [
+        klass_metadata["klass"]
+        for module in unfiltered_results.values()
+        for klass_metadata in module["classes"].values()
+    ]
+
+    # Verify filtered results have right output type
+    assert _check_package_metadata_result(results) is True
+
+    # Now verify class filter is being applied correctly
+    if class_filter is None:
+        assert len(unfiltered_classes) == len(filtered_classes)
+        assert unfiltered_classes == filtered_classes
+    else:
+        assert len(unfiltered_classes) > len(filtered_classes)
+        classes_subclass_class_filter = [
+            issubclass(klass, class_filter) for klass in filtered_classes
+        ]
+        assert all(classes_subclass_class_filter)
+
+
+@pytest.mark.parametrize("tag_filter", [None, "A", ("A", "B"), {"A": "1", "B": 2}])
+def test_get_package_metadata_tag_filter(tag_filter):
+    """Test get_package_metadata filters by tags as expected."""
+    results = get_package_metadata(
+        "skbase",
+        exclude_non_public_modules=False,
+        modules_to_ignore="skbase",
+        tag_filter=tag_filter,
+        classes_to_exclude=TagAliaserMixin,
+    )
+    filtered_classes = [
+        klass_metadata["klass"]
+        for module in results.values()
+        for klass_metadata in module["classes"].values()
+    ]
+
+    # Unfiltered results
+    unfiltered_results = get_package_metadata(
+        "skbase",
+        exclude_non_public_modules=False,
+        modules_to_ignore="skbase",
+        classes_to_exclude=TagAliaserMixin,
+    )
+    unfiltered_classes = [
+        klass_metadata["klass"]
+        for module in unfiltered_results.values()
+        for klass_metadata in module["classes"].values()
+    ]
+
+    # Verify we return dict with str keys
+    assert _check_package_metadata_result(results) is True
+
+    # Verify tag filter is being applied correctly, which implies
+    # When the filter is None the result is the same size
+    # Otherwise, with the filters used in the test, fewer classes should
+    # be returned
+    if tag_filter is None:
+        assert len(unfiltered_classes) == len(filtered_classes)
+        assert unfiltered_classes == filtered_classes
+    else:
+        assert len(unfiltered_classes) > len(filtered_classes)
+
+
+@pytest.mark.parametrize("exclude_non_public_modules", [True, False])
+@pytest.mark.parametrize("exclude_non_public_items", [True, False])
+def test_get_package_metadata_returns_expected_results(
+    exclude_non_public_modules, exclude_non_public_items
+):
+    """Test that get_package_metadata_returns expected results using skbase."""
+    results = get_package_metadata(
+        "skbase",
+        exclude_non_public_items=exclude_non_public_items,
+        exclude_non_public_modules=exclude_non_public_modules,
+        package_base_classes=SKBASE_BASE_CLASSES,
+        modules_to_ignore="tests",
+        classes_to_exclude=TagAliaserMixin,
+        suppress_import_stdout=False,
+    )
+    public_modules_excluding_tests = [
+        module
+        for module in SKBASE_PUBLIC_MODULES
+        if not _is_ignored_module(module, modules_to_ignore="tests")
+    ]
+    modules_excluding_tests = [
+        module
+        for module in SKBASE_MODULES
+        if not _is_ignored_module(module, modules_to_ignore="tests")
+    ]
+    if exclude_non_public_modules:
+        assert tuple(results.keys()) == tuple(public_modules_excluding_tests)
+    else:
+        assert tuple(results.keys()) == tuple(modules_excluding_tests)
+
+    for module in results:
+        if exclude_non_public_items:
+            module_funcs = SKBASE_PUBLIC_FUNCTIONS_BY_MODULE.get(module, ())
+            module_classes = SKBASE_PUBLIC_CLASSES_BY_MODULE.get(module, ())
+        else:
+            module_funcs = SKBASE_FUNCTIONS_BY_MODULE.get(module, ())
+            module_classes = SKBASE_CLASSES_BY_MODULE.get(module, ())
+
+        # Verify expected functions are returned
+        assert set(results[module]["functions"].keys()) == set(module_funcs)
+        # Verify expected classes are returned
+        assert set(results[module]["classes"].keys()) == set(module_classes)
+
+        # Verify class metadata attributes correct
+        for klass, klass_metadata in results[module]["classes"].items():
+            if klass_metadata["klass"] in SKBASE_BASE_CLASSES:
+                assert (
+                    klass_metadata["is_base_class"] is True
+                ), f"{klass} should be base class."
+            else:
+                assert (
+                    klass_metadata["is_base_class"] is False
+                ), f"{klass} should not be base class."
+
+            if issubclass(klass_metadata["klass"], BaseObject):
+                assert klass_metadata["is_base_object"] is True
+            else:
+                assert klass_metadata["is_base_object"] is False
+
+            if (
+                issubclass(klass_metadata["klass"], SKBASE_BASE_CLASSES)
+                and klass_metadata["klass"] not in SKBASE_BASE_CLASSES
+            ):
+                assert klass_metadata["is_concrete_implementation"] is True
+            else:
+                assert klass_metadata["is_concrete_implementation"] is False
+
+
+def test_get_return_tags():
+    """Test _get_return_tags returns expected."""
+
+    def _test_get_return_tags_output(results, num_requested_tags):
+        return isinstance(results, tuple) and len(results) == num_requested_tags
+
+    # Verify return with tags that exist
+    tags = Parent.get_class_tags()
+    tag_names = [*tags.keys()]
+    results = _get_return_tags(Parent, tag_names)
+    assert (
+        _test_get_return_tags_output(results, len(tag_names))
+        and tuple(tags.values()) == results
+    )
+
+    # Verify results when some exist and some don't exist
+    tag_names += ["a_tag_that_does_not_exist"]
+    results = _get_return_tags(Parent, tag_names)
+    assert _test_get_return_tags_output(results, len(tag_names))
+
+    # Verify return when all tags don't exist
+    tag_names = ["a_tag_that_does_not_exist"]
+    results = _get_return_tags(Parent, tag_names)
+    assert _test_get_return_tags_output(results, len(tag_names)) and results[0] is None
+
+
+@pytest.mark.parametrize("as_dataframe", [True, False])
+@pytest.mark.parametrize("return_names", [True, False])
+@pytest.mark.parametrize("return_tags", [None, "A", ["A", "a_non_existant_tag"]])
+@pytest.mark.parametrize("modules_to_ignore", ["tests", ("testing", "lookup"), None])
+@pytest.mark.parametrize("exclude_objects", [None, "Child", ["CompositionDummy"]])
+@pytest.mark.parametrize("suppress_import_stdout", [True, False])
+def test_all_objects_returns_expected_types(
+    as_dataframe,
+    return_names,
+    return_tags,
+    modules_to_ignore,
+    exclude_objects,
+    suppress_import_stdout,
+):
+    """Test that all_objects return argument has correct type."""
+    objs = all_objects(
+        package_name="skbase",
+        exclude_objects=exclude_objects,
+        return_names=return_names,
+        as_dataframe=as_dataframe,
+        return_tags=return_tags,
+        modules_to_ignore=modules_to_ignore,
+        suppress_import_stdout=suppress_import_stdout,
+    )
+    if isinstance(modules_to_ignore, str):
+        modules_to_ignore = (modules_to_ignore,)
+    if (
+        modules_to_ignore is not None
+        and "tests" in modules_to_ignore
+        # and "mock_package" in modules_to_ignore
+    ):
+        assert (
+            len(objs) == 0
+        ), "Search of `skbase` should only return objects from tests module."
+    else:
+        # We expect at least one object to be returned so we verify output type/format
+        _check_all_object_output_types(
+            objs,
+            as_dataframe=as_dataframe,
+            return_names=return_names,
+            return_tags=return_tags,
+        )
+
+
+@pytest.mark.parametrize(
+    "exclude_objects", [None, "Parent", ["Child", "CompositionDummy"]]
+)
+def test_all_objects_returns_expected_output(exclude_objects):
+    """Test that all_objects return argument has correct output for skbase."""
+    objs = all_objects(
+        package_name="skbase.tests.mock_package",
+        exclude_objects=exclude_objects,
+        return_names=True,
+        as_dataframe=True,
+        modules_to_ignore="conftest",
+        suppress_import_stdout=True,
+    )
+    klasses = objs["object"].tolist()
+    test_classes = [
+        k
+        for k in MOCK_PACKAGE_OBJECTS
+        if issubclass(k, BaseObject) and not k.__name__.startswith("_")
+    ]
+    if exclude_objects is not None:
+        if isinstance(exclude_objects, str):
+            exclude_objects = (exclude_objects,)
+        # Exclude classes from MOCK_PACKAGE_OBJECTS
+        test_classes = [k for k in test_classes if k.__name__ not in exclude_objects]
+
+    msg = f"{klasses} should match test classes {test_classes}."
+    assert set(klasses) == set(test_classes), msg
+
+
+@pytest.mark.parametrize("class_filter", [None, Parent, [Parent, BaseEstimator]])
+def test_all_objects_class_filter(class_filter):
+    """Test all_objects filters by class type as expected."""
+    # Results applying filter
+    objs = all_objects(
+        package_name="skbase",
+        return_names=True,
+        as_dataframe=True,
+        return_tags=None,
+        object_types=class_filter,
+    )
+    filtered_classes = objs.iloc[:, 1].tolist()
+    # Verify filtered results have right output type
+    _check_all_object_output_types(
+        objs, as_dataframe=True, return_names=True, return_tags=None
+    )
+
+    # Results without filter
+    objs = all_objects(
+        package_name="skbase",
+        return_names=True,
+        as_dataframe=True,
+        return_tags=None,
+    )
+    unfiltered_classes = objs.iloc[:, 1].tolist()
+
+    # Now verify class filter is being applied correctly
+    if class_filter is None:
+        assert len(unfiltered_classes) == len(filtered_classes)
+        assert unfiltered_classes == filtered_classes
+    else:
+        if not isinstance(class_filter, type):
+            class_filter = tuple(class_filter)
+        assert len(unfiltered_classes) > len(filtered_classes)
+        classes_subclass_class_filter = [
+            issubclass(klass, class_filter) for klass in filtered_classes
+        ]
+        assert all(classes_subclass_class_filter)
+
+
+@pytest.mark.parametrize("tag_filter", [None, "A", ("A", "B"), {"A": "1", "B": 2}])
+def test_all_object_tag_filter(tag_filter):
+    """Test all_objects filters by tag as expected."""
+    # Results applying filter
+    objs = all_objects(
+        package_name="skbase",
+        return_names=True,
+        as_dataframe=True,
+        return_tags=None,
+        filter_tags=tag_filter,
+    )
+    filtered_classes = objs.iloc[:, 1].tolist()
+    # Verify filtered results have right output type
+    _check_all_object_output_types(
+        objs, as_dataframe=True, return_names=True, return_tags=None
+    )
+
+    # Results without filter
+    objs = all_objects(
+        package_name="skbase",
+        return_names=True,
+        as_dataframe=True,
+        return_tags=None,
+    )
+    unfiltered_classes = objs.iloc[:, 1].tolist()
+
+    # Verify tag filter is being applied correctly, which implies
+    # When the filter is None the result is the same size
+    # Otherwise, with the filters used in the test, fewer classes should
+    # be returned
+    if tag_filter is None:
+        assert len(unfiltered_classes) == len(filtered_classes)
+        assert unfiltered_classes == filtered_classes
+    else:
+        assert len(unfiltered_classes) > len(filtered_classes)
+
+
+@pytest.mark.parametrize("class_lookup", [{"base_object": BaseObject}])
+@pytest.mark.parametrize("class_filter", [None, "base_object"])
+def test_all_object_class_lookup(class_lookup, class_filter):
+    """Test all_objects class_lookup parameter works as expected.."""
+    # Results applying filter
+    objs = all_objects(
+        package_name="skbase",
+        return_names=True,
+        as_dataframe=True,
+        return_tags=None,
+        object_types=class_filter,
+        class_lookup=class_lookup,
+    )
+    # filtered_classes = objs.iloc[:, 1].tolist()
+    # Verify filtered results have right output type
+    _check_all_object_output_types(
+        objs, as_dataframe=True, return_names=True, return_tags=None
+    )
+
+
+@pytest.mark.parametrize("class_lookup", [None, {"base_object": BaseObject}])
+@pytest.mark.parametrize("class_filter", ["invalid_alias", 7])
+def test_all_object_class_lookup_invalid_object_types_raises(
+    class_lookup, class_filter
+):
+    """Test all_objects use of object filtering raises errors as expected."""
+    # Results applying filter
+    with pytest.raises(ValueError):
+        all_objects(
+            package_name="skbase",
+            return_names=True,
+            as_dataframe=True,
+            return_tags=None,
+            object_types=class_filter,
+            class_lookup=class_lookup,
+        )
```

### Comparing `skbase-0.4.5/skbase/testing/test_all_objects.py` & `skbase-0.4.6/skbase/testing/test_all_objects.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,856 +1,856 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Suite of tests for all objects.
-
-adapted from scikit-learn's and sktime's estimator_checks
-"""
-import numbers
-import types
-from copy import deepcopy
-from inspect import getfullargspec, isclass, signature
-from typing import List
-
-import numpy as np
-import pytest
-
-from skbase.base import BaseObject
-from skbase.lookup import all_objects
-from skbase.testing.utils._conditional_fixtures import (
-    create_conditional_fixtures_and_names,
-)
-from skbase.testing.utils._dependencies import _check_soft_dependencies
-from skbase.testing.utils.inspect import _get_args
-from skbase.utils.deep_equals import deep_equals
-
-__author__: List[str] = ["fkiraly"]
-
-
-class BaseFixtureGenerator:
-    """Fixture generator for skbase testing functionality.
-
-    Test classes inheriting from this and not overriding pytest_generate_tests
-        will have object and scenario fixtures parametrized out of the box.
-
-    Descendants can override:
-    object_type_filter: str, class variable; None or scitype string
-        e.g., "forecaster", "transformer", "classifier", see BASE_CLASS_SCITYPE_LIST
-        which objects are being retrieved and tested
-    exclude_objects : str or list of str, or None, default=None
-        names of object classes to exclude in retrieval; None = no objects are excluded
-    excluded_tests : dict with str keys and list of str values, or None, default=None
-        str keys must be object names, value keys must be lists of test names
-        names of tests (values) to exclude for object with name as key
-        None = no tests are excluded
-    valid_tags : list of str or None, default = None
-        list of valid tags, None = all tags are valid
-    valid_base_types : list of str or None, default = None
-        list of valid base types (strings), None = all base types are valid
-    fixture_sequence: list of str
-        sequence of fixture variable names in conditional fixture generation
-    _generate_[variable]: object methods, all (test_name: str, **kwargs) -> list
-        generating list of fixtures for fixture variable with name [variable]
-            to be used in test with name test_name
-        can optionally use values for fixtures earlier in fixture_sequence,
-            these must be input as kwargs in a call
-    is_excluded: static method (test_name: str, est: class) -> bool
-        whether test with name test_name should be excluded for object est
-            should be used only for encoding general rules, not individual skips
-            individual skips should go on the excluded_tests list
-        requires _generate_object_class and _generate_object_instance as is
-
-    Fixtures parametrized
-    ---------------------
-    object_class: object inheriting from BaseObject
-        ranges over object classes not excluded by exclude_objects, excluded_tests
-    object_instance: instance of object inheriting from BaseObject
-        ranges over object classes not excluded by exclude_objects, excluded_tests
-        instances are generated by create_test_instance class method of object_class
-    """
-
-    # class variables which can be overridden by descendants
-    # ------------------------------------------------------
-
-    # package to search for objects
-    # expected type: str, package/module name, relative to python environment root
-    package_name = "skbase.tests.mock_package"
-
-    # which object types are generated; None=all, or scitype string like "forecaster"
-    object_type_filter = None
-
-    # list of object types (class names) to exclude
-    # expected type: list of str, str are class names
-    exclude_objects = None
-
-    # list of tests to exclude
-    # expected type: dict of lists, key:str, value: List[str]
-    # keys are class names of estimators, values are lists of test names to exclude
-    excluded_tests = None
-
-    # list of valid tags
-    # expected type: list of str, str are tag names
-    valid_tags = None
-
-    # list of valid base type names
-    # expected type: list of str, str are base type (class) names
-    valid_base_types = None
-
-    # which sequence the conditional fixtures are generated in
-    fixture_sequence = ["object_class", "object_instance"]
-
-    # which fixtures are indirect, e.g., have an additional pytest.fixture block
-    #   to generate an indirect fixture at runtime. Example: object_instance
-    #   warning: direct fixtures retain state changes within the same test
-    indirect_fixtures = ["object_instance"]
-
-    def pytest_generate_tests(self, metafunc):
-        """Test parameterization routine for pytest.
-
-        This uses create_conditional_fixtures_and_names and generator_dict
-        to create the fixtures for a mark.parametrize decoration of all tests.
-        """
-        # get name of the test
-        test_name = metafunc.function.__name__
-
-        fixture_sequence = self.fixture_sequence
-
-        fixture_vars = getfullargspec(metafunc.function)[0]
-
-        (
-            fixture_param_str,
-            fixture_prod,
-            fixture_names,
-        ) = create_conditional_fixtures_and_names(
-            test_name=test_name,
-            fixture_vars=fixture_vars,
-            generator_dict=self.generator_dict(),
-            fixture_sequence=fixture_sequence,
-            raise_exceptions=True,
-        )
-
-        # determine indirect variables for the parametrization block
-        #   this is intersection of self.indirect_vixtures with args in fixture_vars
-        indirect_vars = list(set(fixture_vars).intersection(self.indirect_fixtures))
-
-        metafunc.parametrize(
-            fixture_param_str,
-            fixture_prod,
-            ids=fixture_names,
-            indirect=indirect_vars,
-        )
-
-    def _all_objects(self):
-        """Retrieve list of all object classes of type self.object_type_filter."""
-        return all_objects(
-            object_types=getattr(self, "object_type_filter", None),
-            return_names=False,
-            exclude_estimators=self.exclude_objects,
-            package_name=self.package_name,
-        )
-
-    def generator_dict(self):
-        """Return dict with methods _generate_[variable] collected in a dict.
-
-        The returned dict is the one required by create_conditional_fixtures_and_names,
-            used in this _conditional_fixture plug-in to pytest_generate_tests, above.
-
-        Returns
-        -------
-        generator_dict : dict, with keys [variable], where
-            [variable] are all strings such that self has a static method
-                named _generate_[variable](test_name: str, **kwargs)
-            value at [variable] is a reference to _generate_[variable]
-        """
-        gens = [attr for attr in dir(self) if attr.startswith("_generate_")]
-        fixts = [gen.replace("_generate_", "") for gen in gens]
-
-        generator_dict = {}
-        for var, gen in zip(fixts, gens):
-            generator_dict[var] = getattr(self, gen)
-
-        return generator_dict
-
-    def is_excluded(self, test_name, est):
-        """Shorthand to check whether test test_name is excluded for object est."""
-        if self.excluded_tests is None:
-            return False
-        else:
-            return test_name in self.excluded_tests.get(est.__name__, [])
-
-    # the following functions define fixture generation logic for pytest_generate_tests
-    # each function is of signature (test_name:str, **kwargs) -> List of fixtures
-    # function with name _generate_[fixture_var] returns list of values for fixture_var
-    #   where fixture_var is a fixture variable used in tests
-    # the list is conditional on values of other fixtures which can be passed in kwargs
-
-    def _generate_object_class(self, test_name, **kwargs):
-        """Return object class fixtures.
-
-        Fixtures parametrized
-        ---------------------
-        object_class: object inheriting from BaseObject
-            ranges over all object classes not excluded by self.excluded_tests
-        """
-        object_classes_to_test = [
-            est for est in self._all_objects() if not self.is_excluded(test_name, est)
-        ]
-        object_names = [est.__name__ for est in object_classes_to_test]
-
-        return object_classes_to_test, object_names
-
-    def _generate_object_instance(self, test_name, **kwargs):
-        """Return object instance fixtures.
-
-        Fixtures parametrized
-        ---------------------
-        object_instance: instance of object inheriting from BaseObject
-            ranges over all object classes not excluded by self.excluded_tests
-            instances are generated by create_test_instance class method
-        """
-        # call _generate_object_class to get all the classes
-        object_classes_to_test, _ = self._generate_object_class(test_name=test_name)
-
-        # create instances from the classes
-        object_instances_to_test = []
-        object_instance_names = []
-        # retrieve all object parameters if multiple, construct instances
-        for est in object_classes_to_test:
-            all_instances_of_est, instance_names = est.create_test_instances_and_names()
-            object_instances_to_test += all_instances_of_est
-            object_instance_names += instance_names
-
-        return object_instances_to_test, object_instance_names
-
-    # this is executed before each test instance call
-    #   if this were not executed, object_instance would keep state changes
-    #   within executions of the same test with different parameters
-    @pytest.fixture(scope="function")
-    def object_instance(self, request):
-        """object_instance fixture definition for indirect use."""
-        # esetimator_instance is cloned at the start of every test
-        return request.param.clone()
-
-
-class QuickTester:
-    """Mixin class which adds the run_tests method to run tests on one object."""
-
-    def run_tests(
-        self,
-        obj,
-        raise_exceptions=False,
-        tests_to_run=None,
-        fixtures_to_run=None,
-        tests_to_exclude=None,
-        fixtures_to_exclude=None,
-    ):
-        """Run all tests on one single object.
-
-        All tests in self are run on the following object type fixtures:
-            if est is a class, then object_class = est, and
-                object_instance loops over est.create_test_instance()
-            if est is an object, then object_class = est.__class__, and
-                object_instance = est
-
-        This is compatible with pytest.mark.parametrize decoration,
-            but currently only with multiple *single variable* annotations.
-
-        Parameters
-        ----------
-        obj : object class or object instance
-        raise_exceptions : bool, optional, default=False
-            whether to return exceptions/failures in the results dict, or raise them
-                if False: returns exceptions in returned `results` dict
-                if True: raises exceptions as they occur
-        tests_to_run : str or list of str, names of tests to run. default = all tests
-            sub-sets tests that are run to the tests given here.
-        fixtures_to_run : str or list of str, pytest test-fixture combination codes.
-            which test-fixture combinations to run. Default = run all of them.
-            sub-sets tests and fixtures to run to the list given here.
-            If both tests_to_run and fixtures_to_run are provided, runs the *union*,
-            i.e., all test-fixture combinations for tests in tests_to_run,
-                plus all test-fixture combinations in fixtures_to_run.
-        tests_to_exclude : str or list of str, names of tests to exclude. default = None
-            removes tests that should not be run, after subsetting via tests_to_run.
-        fixtures_to_exclude : str or list of str, fixtures to exclude. default = None
-            removes test-fixture combinations that should not be run.
-            This is done after subsetting via fixtures_to_run.
-
-        Returns
-        -------
-        results : dict of results of the tests in self
-            keys are test/fixture strings, identical as in pytest, e.g., test[fixture]
-            entries are the string "PASSED" if the test passed,
-                or the exception raised if the test did not pass
-            returned only if all tests pass, or raise_exceptions=False
-
-        Raises
-        ------
-        if raise_exception=True, raises any exception produced by the tests directly
-
-        Examples
-        --------
-        >>> from skbase.tests.mock_package.test_mock_package import CompositionDummy
-        >>> from skbase.testing.test_all_objects import TestAllObjects
-        >>> TestAllObjects().run_tests(
-        ...     CompositionDummy,
-        ...     tests_to_run="test_constructor"
-        ... )
-        {'test_constructor[CompositionDummy]': 'PASSED'}
-        >>> TestAllObjects().run_tests(
-        ...     CompositionDummy, fixtures_to_run="test_repr[CompositionDummy-1]"
-        ... )
-        {'test_repr[CompositionDummy-1]': 'PASSED'}
-        """
-        tests_to_run = self._check_none_str_or_list_of_str(
-            tests_to_run, var_name="tests_to_run"
-        )
-        fixtures_to_run = self._check_none_str_or_list_of_str(
-            fixtures_to_run, var_name="fixtures_to_run"
-        )
-        tests_to_exclude = self._check_none_str_or_list_of_str(
-            tests_to_exclude, var_name="tests_to_exclude"
-        )
-        fixtures_to_exclude = self._check_none_str_or_list_of_str(
-            fixtures_to_exclude, var_name="fixtures_to_exclude"
-        )
-
-        # retrieve tests from self
-        test_names = [attr for attr in dir(self) if attr.startswith("test")]
-
-        # we override the generator_dict, by replacing it with temp_generator_dict:
-        #  the only object (class or instance) is est, this is overridden
-        #  the remaining fixtures are generated conditionally, without change
-        temp_generator_dict = deepcopy(self.generator_dict())
-
-        if isclass(obj):
-            object_class = obj
-        else:
-            object_class = type(obj)
-
-        def _generate_object_class(test_name, **kwargs):
-            return [object_class], [object_class.__name__]
-
-        def _generate_object_instance(test_name, **kwargs):
-            return [obj.clone()], [object_class.__name__]
-
-        def _generate_object_instance_cls(test_name, **kwargs):
-            return object_class.create_test_instances_and_names()
-
-        temp_generator_dict["object_class"] = _generate_object_class
-
-        if not isclass(obj):
-            temp_generator_dict["object_instance"] = _generate_object_instance
-        else:
-            temp_generator_dict["object_instance"] = _generate_object_instance_cls
-        # override of generator_dict end, temp_generator_dict is now prepared
-
-        # sub-setting to specific tests to run, if tests or fixtures were speified
-        if tests_to_run is None and fixtures_to_run is None:
-            test_names_subset = test_names
-        else:
-            test_names_subset = []
-            if tests_to_run is not None:
-                test_names_subset += list(set(test_names).intersection(tests_to_run))
-            if fixtures_to_run is not None:
-                # fixture codes contain the test as substring until the first "["
-                tests_from_fixt = [fixt.split("[")[0] for fixt in fixtures_to_run]
-                test_names_subset += list(set(test_names).intersection(tests_from_fixt))
-            test_names_subset = list(set(test_names_subset))
-
-        # sub-setting by removing all tests from tests_to_exclude
-        if tests_to_exclude is not None:
-            test_names_subset = list(
-                set(test_names_subset).difference(tests_to_exclude)
-            )
-
-        # the below loops run all the tests and collect the results here:
-        results = {}
-        # loop A: we loop over all the tests
-        for test_name in test_names_subset:
-            test_fun = getattr(self, test_name)
-            fixture_sequence = self.fixture_sequence
-
-            # all arguments except the first one (self)
-            fixture_vars = getfullargspec(test_fun)[0][1:]
-            fixture_vars = [var for var in fixture_sequence if var in fixture_vars]
-
-            # this call retrieves the conditional fixtures
-            #  for the test test_name, and the object
-            _, fixture_prod, fixture_names = create_conditional_fixtures_and_names(
-                test_name=test_name,
-                fixture_vars=fixture_vars,
-                generator_dict=temp_generator_dict,
-                fixture_sequence=fixture_sequence,
-                raise_exceptions=raise_exceptions,
-            )
-
-            # if function is decorated with mark.parametrize, add variable settings
-            # NOTE: currently this works only with single-variable mark.parametrize
-            if hasattr(test_fun, "pytestmark"):
-                if len([x for x in test_fun.pytestmark if x.name == "parametrize"]) > 0:
-                    # get the three lists from pytest
-                    (
-                        pytest_fixture_vars,
-                        pytest_fixture_prod,
-                        pytest_fixture_names,
-                    ) = self._get_pytest_mark_args(test_fun)
-                    # add them to the three lists from conditional fixtures
-                    fixture_vars, fixture_prod, fixture_names = self._product_fixtures(
-                        fixture_vars,
-                        fixture_prod,
-                        fixture_names,
-                        pytest_fixture_vars,
-                        pytest_fixture_prod,
-                        pytest_fixture_names,
-                    )
-
-            # loop B: for each test, we loop over all fixtures
-            for params, fixt_name in zip(fixture_prod, fixture_names):
-                # this is needed because pytest unwraps 1-tuples automatically
-                # but subsequent code assumes params is k-tuple, no matter what k is
-                if len(fixture_vars) == 1:
-                    params = (params,)
-                key = f"{test_name}[{fixt_name}]"
-                args = dict(zip(fixture_vars, params))
-
-                # we subset to test-fixtures to run by this, if given
-                #  key is identical to the pytest test-fixture string identifier
-                if fixtures_to_run is not None and key not in fixtures_to_run:
-                    continue
-                if fixtures_to_exclude is not None and key in fixtures_to_exclude:
-                    continue
-
-                if not raise_exceptions:
-                    try:
-                        test_fun(**deepcopy(args))
-                        results[key] = "PASSED"
-                    except Exception as err:
-                        results[key] = err
-                else:
-                    test_fun(**deepcopy(args))
-                    results[key] = "PASSED"
-
-        return results
-
-    @staticmethod
-    def _check_none_str_or_list_of_str(obj, var_name="obj"):
-        """Check that obj is None, str, or list of str, and coerce to list of str."""
-        if obj is not None:
-            msg = f"{var_name} must be None, str, or list of str"
-            if isinstance(obj, str):
-                obj = [obj]
-            if not isinstance(obj, list):
-                raise ValueError(msg)
-            if not np.all(isinstance(x, str) for x in obj):
-                raise ValueError(msg)
-        return obj
-
-    # todo: surely there is a pytest method that can be called instead of this?
-    #   find and replace if it exists
-    @staticmethod
-    def _get_pytest_mark_args(fun):
-        """Get args from pytest mark annotation of function.
-
-        Parameters
-        ----------
-        fun: callable, any function
-
-        Returns
-        -------
-        pytest_fixture_vars: list of str
-            names of args participating in mark.parametrize marks, in pytest order
-        pytest_fixt_list: list of tuple
-            list of value tuples from the mark parameterization
-            i-th value in each tuple corresponds to i-th arg name in pytest_fixture_vars
-        pytest_fixt_names: list of str
-            i-th element is display name for i-th fixture setting in pytest_fixt_list
-        """
-        from itertools import product
-
-        marks = [x for x in fun.pytestmark if x.name == "parametrize"]
-
-        def to_str(obj):
-            return [str(x) for x in obj]
-
-        def get_id(mark):
-            if "ids" in mark.kwargs.keys():
-                return mark.kwargs["ids"]
-            else:
-                return to_str(range(len(mark.args[1])))
-
-        pytest_fixture_vars = [x.args[0] for x in marks]
-        pytest_fixt_raw = [x.args[1] for x in marks]
-        pytest_fixt_list = product(*pytest_fixt_raw)
-        pytest_fixt_names_raw = [get_id(x) for x in marks]
-        pytest_fixt_names = product(*pytest_fixt_names_raw)
-        pytest_fixt_names = ["-".join(x) for x in pytest_fixt_names]
-
-        return pytest_fixture_vars, pytest_fixt_list, pytest_fixt_names
-
-    @staticmethod
-    def _product_fixtures(
-        fixture_vars,
-        fixture_prod,
-        fixture_names,
-        pytest_fixture_vars,
-        pytest_fixture_prod,
-        pytest_fixture_names,
-    ):
-        """Compute products of two sets of fixture vars, values, names."""
-        from itertools import product
-
-        # product of fixture variable names = concatenation
-        fixture_vars_return = fixture_vars + pytest_fixture_vars
-
-        # this is needed because pytest unwraps 1-tuples automatically
-        # but subsequent code assumes params is k-tuple, no matter what k is
-        if len(fixture_vars) == 1:
-            fixture_prod = [(x,) for x in fixture_prod]
-
-        # product of fixture products = Cartesian product plus append tuples
-        fixture_prod_return = product(fixture_prod, pytest_fixture_prod)
-        fixture_prod_return = [sum(x, ()) for x in fixture_prod_return]
-
-        # product of fixture names = Cartesian product plus concat
-        fixture_names_return = product(fixture_names, pytest_fixture_names)
-        fixture_names_return = ["-".join(x) for x in fixture_names_return]
-
-        return fixture_vars_return, fixture_prod_return, fixture_names_return
-
-
-class TestAllObjects(BaseFixtureGenerator, QuickTester):
-    """Package level tests for BaseObjects."""
-
-    def test_create_test_instance(self, object_class):
-        """Check create_test_instance logic and basic constructor functionality.
-
-        create_test_instance and create_test_instances_and_names are the
-        key methods used to create test instances in testing.
-        If this test does not pass, validity of the other tests cannot be guaranteed.
-
-        Also tests inheritance and super call logic in the constructor.
-
-        Tests that:
-
-        * create_test_instance results in an instance of estimator_class
-        * `__init__` calls `super.__init__`
-        * `_tags_dynamic` attribute for tag inspection is present after construction
-        """
-        object_instance = object_class.create_test_instance()
-
-        # Check that init does not construct object of other class than itself
-        assert isinstance(object_instance, object_class), (
-            "object returned by create_test_instance must be an instance of the class, "
-            f"found {type(object_instance)}"
-        )
-
-        msg = (
-            f"{object_class.__name__}.__init__ should call "
-            f"super({object_class.__name__}, self).__init__, "
-            "but that does not seem to be the case. Please ensure to call the "
-            f"parent class's constructor in {object_class.__name__}.__init__"
-        )
-        assert hasattr(object_instance, "_tags_dynamic"), msg
-
-    def test_create_test_instances_and_names(self, object_class):
-        """Check that create_test_instances_and_names works.
-
-        create_test_instance and create_test_instances_and_names are the
-        key methods used to create test instances in testing.
-        If this test does not pass, validity of the other tests cannot be guaranteed.
-
-        Tests expected function signature of create_test_instances_and_names.
-        """
-        objects, names = object_class.create_test_instances_and_names()
-
-        assert isinstance(objects, list), (
-            "first return of create_test_instances_and_names must be a list, "
-            f"found {type(objects)}"
-        )
-        assert isinstance(names, list), (
-            "second return of create_test_instances_and_names must be a list, "
-            f"found {type(names)}"
-        )
-
-        assert np.all(isinstance(est, object_class) for est in objects), (
-            "list elements of first return returned by create_test_instances_and_names "
-            "all must be an instance of the class"
-        )
-
-        assert np.all(isinstance(name, names) for name in names), (
-            "list elements of second return returned by create_test_instances_and_names"
-            " all must be strings"
-        )
-
-        assert len(objects) == len(names), (
-            "the two lists returned by create_test_instances_and_names must have "
-            "equal length"
-        )
-
-    def test_object_tags(self, object_class):
-        """Check conventions on object tags."""
-        assert hasattr(object_class, "get_class_tags")
-        all_tags = object_class.get_class_tags()
-        assert isinstance(all_tags, dict)
-        assert all(isinstance(key, str) for key in all_tags.keys())
-        if hasattr(object_class, "_tags"):
-            tags = object_class._tags
-            msg = (
-                f"_tags attribute of class {object_class} must be dict, "
-                f"but found {type(tags)}"
-            )
-            assert isinstance(tags, dict), msg
-            assert len(tags) > 0, f"_tags dict of class {object_class} is empty"
-            if self.valid_tags is None:
-                invalid_tags = tags
-            else:
-                invalid_tags = [
-                    tag for tag in tags.keys() if tag not in self.valid_tags
-                ]
-            assert len(invalid_tags) == 0, (
-                f"_tags of {object_class} contains invalid tags: {invalid_tags}. "
-                f"For a list of valid tags, see {self.__class__.__name__}.valid_tags."
-            )
-
-        # Avoid ambiguous class attributes
-        ambiguous_attrs = ("tags", "tags_")
-        for attr in ambiguous_attrs:
-            assert not hasattr(object_class, attr), (
-                f"Please avoid using the {attr} attribute to disambiguate it from "
-                f"object tags."
-            )
-
-    def test_inheritance(self, object_class):
-        """Check that object inherits from BaseObject."""
-        assert issubclass(object_class, BaseObject), (
-            f"object: {object_class} " f"is not a sub-class of " f"BaseObject."
-        )
-        # Usually should inherit only from one BaseObject type
-        if self.valid_base_types is not None:
-            n_base_types = sum(
-                issubclass(object_class, cls) for cls in self.valid_base_types
-            )
-            assert n_base_types == 1
-
-    # def test_has_common_interface(self, object_class):
-    #     """Check object implements the common interface."""
-    #     object = object_class
-
-    #     # Check class for type of attribute
-    #     assert isinstance(object.is_fitted, property)
-
-    #     required_methods = _list_required_methods(object_class)
-
-    #     for attr in required_methods:
-    #         assert hasattr(
-    #             object, attr
-    #         ), f"object: {object.__name__} does not implement attribute: {attr}"
-
-    def test_no_cross_test_side_effects_part1(self, object_instance):
-        """Test that there are no side effects across tests, through object state."""
-        object_instance.test__attr = 42
-
-    def test_no_cross_test_side_effects_part2(self, object_instance):
-        """Test that there are no side effects across tests, through object state."""
-        assert not hasattr(object_instance, "test__attr")
-
-    @pytest.mark.parametrize("a", [True, 42])
-    def test_no_between_test_case_side_effects(self, object_instance, a):
-        """Test that there are no side effects across instances of the same test."""
-        assert not hasattr(object_instance, "test__attr")
-        object_instance.test__attr = 42
-
-    @pytest.mark.skipif(
-        not _check_soft_dependencies("sklearn", severity="none"),
-        reason="skip test if sklearn is not available",
-    )  # sklearn is part of the dev dependency set, test should be executed with that
-    def test_get_params(self, object_instance):
-        """Check that get_params works correctly, against sklearn interface."""
-        from sklearn.utils.estimator_checks import (
-            check_get_params_invariance as _check_get_params_invariance,
-        )
-
-        params = object_instance.get_params()
-        assert isinstance(params, dict)
-        _check_get_params_invariance(
-            object_instance.__class__.__name__, object_instance
-        )
-
-    def test_set_params(self, object_instance):
-        """Check that set_params works correctly."""
-        params = object_instance.get_params()
-
-        msg = f"set_params of {type(object_instance).__name__} does not return self"
-        assert object_instance.set_params(**params) is object_instance, msg
-
-        is_equal, equals_msg = deep_equals(
-            object_instance.get_params(), params, return_msg=True
-        )
-        msg = (
-            f"get_params result of {type(object_instance).__name__} (x) does not match "
-            f"what was passed to set_params (y). Reason for discrepancy: {equals_msg}"
-        )
-        assert is_equal, msg
-
-    def test_set_params_sklearn(self, object_class):
-        """Check that set_params works correctly, mirrors sklearn check_set_params.
-
-        Instead of the "fuzz values" in sklearn's check_set_params,
-        we use the other test parameter settings (which are assumed valid).
-        This guarantees settings which play along with the __init__ content.
-        """
-        object_instance = object_class.create_test_instance()
-        test_params = object_class.get_test_params()
-        if not isinstance(test_params, list):
-            test_params = [test_params]
-
-        for params in test_params:
-            # we construct the full parameter set for params
-            # params may only have parameters that are deviating from defaults
-            # in order to set non-default parameters back to defaults
-            params_full = object_class.get_param_defaults()
-            params_full.update(params)
-
-            msg = f"set_params of {object_class.__name__} does not return self"
-            est_after_set = object_instance.set_params(**params_full)
-            assert est_after_set is object_instance, msg
-
-            is_equal, equals_msg = deep_equals(
-                object_instance.get_params(deep=False), params_full, return_msg=True
-            )
-            msg = (
-                f"get_params result of {object_class.__name__} (x) does not match "
-                f"what was passed to set_params (y). "
-                f"Reason for discrepancy: {equals_msg}"
-            )
-            assert is_equal, msg
-
-    def test_clone(self, object_instance):
-        """Check that clone method does not raise exceptions and results in a clone.
-
-        A clone of an object x is an object that:
-
-        * has same class and parameters as x
-        * is not identical with x
-        * is unfitted (even if x was fitted)
-        """
-        obj_clone = object_instance.clone()
-        assert isinstance(obj_clone, type(object_instance))
-        assert obj_clone is not object_instance
-        if hasattr(obj_clone, "is_fitted"):
-            assert not obj_clone.is_fitted
-
-    def test_repr(self, object_instance):
-        """Check we can call repr."""
-        repr(object_instance)
-
-    def test_constructor(self, object_class):
-        """Check that the constructor has sklearn compatible signature and behaviour.
-
-        Based on sklearn check_estimator testing of __init__ logic.
-        Uses create_test_instance to create an instance.
-        Assumes test_create_test_instance has passed and certified create_test_instance.
-
-        Tests that:
-
-        * constructor has no varargs
-        * tests that constructor constructs an instance of the class
-        * tests that all parameters are set in init to an attribute of the same name
-        * tests that parameter values are always copied to the attribute and not changed
-        * tests that default parameters are one of the following:
-            None, str, int, float, bool, tuple, function, joblib memory, numpy primitive
-            (other type parameters should be None, default handling should be by writing
-            the default to attribute of a different name, e.g., my_param_ not my_param)
-        """
-        msg = f"constructor __init__ of {object_class} should have no varargs"
-        assert getfullargspec(object_class.__init__).varkw is None, msg
-
-        obj = object_class.create_test_instance()
-        assert isinstance(obj, object_class)
-
-        # Ensure that each parameter is set in init
-        init_params = _get_args(type(obj).__init__)
-        invalid_attr = set(init_params) - set(vars(obj)) - {"self"}
-        assert not invalid_attr, (
-            "Object %s should store all parameters"
-            " as an attribute during init. Did not find "
-            "attributes `%s`." % (obj.__class__.__name__, sorted(invalid_attr))
-        )
-
-        # Ensure that init does nothing but set parameters
-        # No logic/interaction with other parameters
-        def param_filter(p):
-            """Identify hyper parameters of an estimator."""
-            return p.name != "self" and p.kind not in [p.VAR_KEYWORD, p.VAR_POSITIONAL]
-
-        init_params = [
-            p for p in signature(obj.__init__).parameters.values() if param_filter(p)
-        ]
-
-        params = obj.get_params()
-
-        # Filter out required parameters with no default value and parameters
-        # set for running tests
-        required_params = getattr(obj, "_required_parameters", ())
-
-        test_params = obj.get_test_params()
-        if isinstance(test_params, list):
-            test_params = test_params[0]
-        test_params = test_params.keys()
-
-        init_params = [
-            param
-            for param in init_params
-            if param.name not in required_params and param.name not in test_params
-        ]
-
-        allowed_param_types = [
-            str,
-            int,
-            float,
-            bool,
-            tuple,
-            type(None),
-            np.float64,
-            types.FunctionType,
-        ]
-        if _check_soft_dependencies("joblib", severity="none"):
-            from joblib import Memory
-
-            allowed_param_types += [Memory]
-
-        for param in init_params:
-            assert param.default != param.empty, (
-                "parameter `%s` for %s has no default value and is not "
-                "included in `_required_parameters`"
-                % (param.name, obj.__class__.__name__)
-            )
-            if type(param.default) is type:
-                assert param.default in [np.float64, np.int64]
-            else:
-                assert type(param.default) in allowed_param_types
-
-            param_value = params[param.name]
-            if isinstance(param_value, np.ndarray):
-                np.testing.assert_array_equal(param_value, param.default)
-            else:
-                if bool(
-                    isinstance(param_value, numbers.Real) and np.isnan(param_value)
-                ):
-                    # Allows to set default parameters to np.nan
-                    assert param_value is param.default, param.name
-                else:
-                    assert param_value == param.default, param.name
-
-    def test_valid_object_class_tags(self, object_class):
-        """Check that object class tags are in self.valid_tags."""
-        if self.valid_tags is None:
-            return None
-        for tag in object_class.get_class_tags().keys():
-            assert tag in self.valid_tags
-
-    def test_valid_object_tags(self, object_instance):
-        """Check that object tags are in self.valid_tags."""
-        if self.valid_tags is None:
-            return None
-        for tag in object_instance.get_tags().keys():
-            assert tag in self.valid_tags
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Suite of tests for all objects.
+
+adapted from scikit-learn's and sktime's estimator_checks
+"""
+import numbers
+import types
+from copy import deepcopy
+from inspect import getfullargspec, isclass, signature
+from typing import List
+
+import numpy as np
+import pytest
+
+from skbase.base import BaseObject
+from skbase.lookup import all_objects
+from skbase.testing.utils._conditional_fixtures import (
+    create_conditional_fixtures_and_names,
+)
+from skbase.testing.utils._dependencies import _check_soft_dependencies
+from skbase.testing.utils.inspect import _get_args
+from skbase.utils.deep_equals import deep_equals
+
+__author__: List[str] = ["fkiraly"]
+
+
+class BaseFixtureGenerator:
+    """Fixture generator for skbase testing functionality.
+
+    Test classes inheriting from this and not overriding pytest_generate_tests
+        will have object and scenario fixtures parametrized out of the box.
+
+    Descendants can override:
+    object_type_filter: str, class variable; None or scitype string
+        e.g., "forecaster", "transformer", "classifier", see BASE_CLASS_SCITYPE_LIST
+        which objects are being retrieved and tested
+    exclude_objects : str or list of str, or None, default=None
+        names of object classes to exclude in retrieval; None = no objects are excluded
+    excluded_tests : dict with str keys and list of str values, or None, default=None
+        str keys must be object names, value keys must be lists of test names
+        names of tests (values) to exclude for object with name as key
+        None = no tests are excluded
+    valid_tags : list of str or None, default = None
+        list of valid tags, None = all tags are valid
+    valid_base_types : list of str or None, default = None
+        list of valid base types (strings), None = all base types are valid
+    fixture_sequence: list of str
+        sequence of fixture variable names in conditional fixture generation
+    _generate_[variable]: object methods, all (test_name: str, **kwargs) -> list
+        generating list of fixtures for fixture variable with name [variable]
+            to be used in test with name test_name
+        can optionally use values for fixtures earlier in fixture_sequence,
+            these must be input as kwargs in a call
+    is_excluded: static method (test_name: str, est: class) -> bool
+        whether test with name test_name should be excluded for object est
+            should be used only for encoding general rules, not individual skips
+            individual skips should go on the excluded_tests list
+        requires _generate_object_class and _generate_object_instance as is
+
+    Fixtures parametrized
+    ---------------------
+    object_class: object inheriting from BaseObject
+        ranges over object classes not excluded by exclude_objects, excluded_tests
+    object_instance: instance of object inheriting from BaseObject
+        ranges over object classes not excluded by exclude_objects, excluded_tests
+        instances are generated by create_test_instance class method of object_class
+    """
+
+    # class variables which can be overridden by descendants
+    # ------------------------------------------------------
+
+    # package to search for objects
+    # expected type: str, package/module name, relative to python environment root
+    package_name = "skbase.tests.mock_package"
+
+    # which object types are generated; None=all, or scitype string like "forecaster"
+    object_type_filter = None
+
+    # list of object types (class names) to exclude
+    # expected type: list of str, str are class names
+    exclude_objects = None
+
+    # list of tests to exclude
+    # expected type: dict of lists, key:str, value: List[str]
+    # keys are class names of estimators, values are lists of test names to exclude
+    excluded_tests = None
+
+    # list of valid tags
+    # expected type: list of str, str are tag names
+    valid_tags = None
+
+    # list of valid base type names
+    # expected type: list of str, str are base type (class) names
+    valid_base_types = None
+
+    # which sequence the conditional fixtures are generated in
+    fixture_sequence = ["object_class", "object_instance"]
+
+    # which fixtures are indirect, e.g., have an additional pytest.fixture block
+    #   to generate an indirect fixture at runtime. Example: object_instance
+    #   warning: direct fixtures retain state changes within the same test
+    indirect_fixtures = ["object_instance"]
+
+    def pytest_generate_tests(self, metafunc):
+        """Test parameterization routine for pytest.
+
+        This uses create_conditional_fixtures_and_names and generator_dict
+        to create the fixtures for a mark.parametrize decoration of all tests.
+        """
+        # get name of the test
+        test_name = metafunc.function.__name__
+
+        fixture_sequence = self.fixture_sequence
+
+        fixture_vars = getfullargspec(metafunc.function)[0]
+
+        (
+            fixture_param_str,
+            fixture_prod,
+            fixture_names,
+        ) = create_conditional_fixtures_and_names(
+            test_name=test_name,
+            fixture_vars=fixture_vars,
+            generator_dict=self.generator_dict(),
+            fixture_sequence=fixture_sequence,
+            raise_exceptions=True,
+        )
+
+        # determine indirect variables for the parametrization block
+        #   this is intersection of self.indirect_vixtures with args in fixture_vars
+        indirect_vars = list(set(fixture_vars).intersection(self.indirect_fixtures))
+
+        metafunc.parametrize(
+            fixture_param_str,
+            fixture_prod,
+            ids=fixture_names,
+            indirect=indirect_vars,
+        )
+
+    def _all_objects(self):
+        """Retrieve list of all object classes of type self.object_type_filter."""
+        return all_objects(
+            object_types=getattr(self, "object_type_filter", None),
+            return_names=False,
+            exclude_estimators=self.exclude_objects,
+            package_name=self.package_name,
+        )
+
+    def generator_dict(self):
+        """Return dict with methods _generate_[variable] collected in a dict.
+
+        The returned dict is the one required by create_conditional_fixtures_and_names,
+            used in this _conditional_fixture plug-in to pytest_generate_tests, above.
+
+        Returns
+        -------
+        generator_dict : dict, with keys [variable], where
+            [variable] are all strings such that self has a static method
+                named _generate_[variable](test_name: str, **kwargs)
+            value at [variable] is a reference to _generate_[variable]
+        """
+        gens = [attr for attr in dir(self) if attr.startswith("_generate_")]
+        fixts = [gen.replace("_generate_", "") for gen in gens]
+
+        generator_dict = {}
+        for var, gen in zip(fixts, gens):
+            generator_dict[var] = getattr(self, gen)
+
+        return generator_dict
+
+    def is_excluded(self, test_name, est):
+        """Shorthand to check whether test test_name is excluded for object est."""
+        if self.excluded_tests is None:
+            return False
+        else:
+            return test_name in self.excluded_tests.get(est.__name__, [])
+
+    # the following functions define fixture generation logic for pytest_generate_tests
+    # each function is of signature (test_name:str, **kwargs) -> List of fixtures
+    # function with name _generate_[fixture_var] returns list of values for fixture_var
+    #   where fixture_var is a fixture variable used in tests
+    # the list is conditional on values of other fixtures which can be passed in kwargs
+
+    def _generate_object_class(self, test_name, **kwargs):
+        """Return object class fixtures.
+
+        Fixtures parametrized
+        ---------------------
+        object_class: object inheriting from BaseObject
+            ranges over all object classes not excluded by self.excluded_tests
+        """
+        object_classes_to_test = [
+            est for est in self._all_objects() if not self.is_excluded(test_name, est)
+        ]
+        object_names = [est.__name__ for est in object_classes_to_test]
+
+        return object_classes_to_test, object_names
+
+    def _generate_object_instance(self, test_name, **kwargs):
+        """Return object instance fixtures.
+
+        Fixtures parametrized
+        ---------------------
+        object_instance: instance of object inheriting from BaseObject
+            ranges over all object classes not excluded by self.excluded_tests
+            instances are generated by create_test_instance class method
+        """
+        # call _generate_object_class to get all the classes
+        object_classes_to_test, _ = self._generate_object_class(test_name=test_name)
+
+        # create instances from the classes
+        object_instances_to_test = []
+        object_instance_names = []
+        # retrieve all object parameters if multiple, construct instances
+        for est in object_classes_to_test:
+            all_instances_of_est, instance_names = est.create_test_instances_and_names()
+            object_instances_to_test += all_instances_of_est
+            object_instance_names += instance_names
+
+        return object_instances_to_test, object_instance_names
+
+    # this is executed before each test instance call
+    #   if this were not executed, object_instance would keep state changes
+    #   within executions of the same test with different parameters
+    @pytest.fixture(scope="function")
+    def object_instance(self, request):
+        """object_instance fixture definition for indirect use."""
+        # esetimator_instance is cloned at the start of every test
+        return request.param.clone()
+
+
+class QuickTester:
+    """Mixin class which adds the run_tests method to run tests on one object."""
+
+    def run_tests(
+        self,
+        obj,
+        raise_exceptions=False,
+        tests_to_run=None,
+        fixtures_to_run=None,
+        tests_to_exclude=None,
+        fixtures_to_exclude=None,
+    ):
+        """Run all tests on one single object.
+
+        All tests in self are run on the following object type fixtures:
+            if est is a class, then object_class = est, and
+                object_instance loops over est.create_test_instance()
+            if est is an object, then object_class = est.__class__, and
+                object_instance = est
+
+        This is compatible with pytest.mark.parametrize decoration,
+            but currently only with multiple *single variable* annotations.
+
+        Parameters
+        ----------
+        obj : object class or object instance
+        raise_exceptions : bool, optional, default=False
+            whether to return exceptions/failures in the results dict, or raise them
+                if False: returns exceptions in returned `results` dict
+                if True: raises exceptions as they occur
+        tests_to_run : str or list of str, names of tests to run. default = all tests
+            sub-sets tests that are run to the tests given here.
+        fixtures_to_run : str or list of str, pytest test-fixture combination codes.
+            which test-fixture combinations to run. Default = run all of them.
+            sub-sets tests and fixtures to run to the list given here.
+            If both tests_to_run and fixtures_to_run are provided, runs the *union*,
+            i.e., all test-fixture combinations for tests in tests_to_run,
+                plus all test-fixture combinations in fixtures_to_run.
+        tests_to_exclude : str or list of str, names of tests to exclude. default = None
+            removes tests that should not be run, after subsetting via tests_to_run.
+        fixtures_to_exclude : str or list of str, fixtures to exclude. default = None
+            removes test-fixture combinations that should not be run.
+            This is done after subsetting via fixtures_to_run.
+
+        Returns
+        -------
+        results : dict of results of the tests in self
+            keys are test/fixture strings, identical as in pytest, e.g., test[fixture]
+            entries are the string "PASSED" if the test passed,
+                or the exception raised if the test did not pass
+            returned only if all tests pass, or raise_exceptions=False
+
+        Raises
+        ------
+        if raise_exception=True, raises any exception produced by the tests directly
+
+        Examples
+        --------
+        >>> from skbase.tests.mock_package.test_mock_package import CompositionDummy
+        >>> from skbase.testing.test_all_objects import TestAllObjects
+        >>> TestAllObjects().run_tests(
+        ...     CompositionDummy,
+        ...     tests_to_run="test_constructor"
+        ... )
+        {'test_constructor[CompositionDummy]': 'PASSED'}
+        >>> TestAllObjects().run_tests(
+        ...     CompositionDummy, fixtures_to_run="test_repr[CompositionDummy-1]"
+        ... )
+        {'test_repr[CompositionDummy-1]': 'PASSED'}
+        """
+        tests_to_run = self._check_none_str_or_list_of_str(
+            tests_to_run, var_name="tests_to_run"
+        )
+        fixtures_to_run = self._check_none_str_or_list_of_str(
+            fixtures_to_run, var_name="fixtures_to_run"
+        )
+        tests_to_exclude = self._check_none_str_or_list_of_str(
+            tests_to_exclude, var_name="tests_to_exclude"
+        )
+        fixtures_to_exclude = self._check_none_str_or_list_of_str(
+            fixtures_to_exclude, var_name="fixtures_to_exclude"
+        )
+
+        # retrieve tests from self
+        test_names = [attr for attr in dir(self) if attr.startswith("test")]
+
+        # we override the generator_dict, by replacing it with temp_generator_dict:
+        #  the only object (class or instance) is est, this is overridden
+        #  the remaining fixtures are generated conditionally, without change
+        temp_generator_dict = deepcopy(self.generator_dict())
+
+        if isclass(obj):
+            object_class = obj
+        else:
+            object_class = type(obj)
+
+        def _generate_object_class(test_name, **kwargs):
+            return [object_class], [object_class.__name__]
+
+        def _generate_object_instance(test_name, **kwargs):
+            return [obj.clone()], [object_class.__name__]
+
+        def _generate_object_instance_cls(test_name, **kwargs):
+            return object_class.create_test_instances_and_names()
+
+        temp_generator_dict["object_class"] = _generate_object_class
+
+        if not isclass(obj):
+            temp_generator_dict["object_instance"] = _generate_object_instance
+        else:
+            temp_generator_dict["object_instance"] = _generate_object_instance_cls
+        # override of generator_dict end, temp_generator_dict is now prepared
+
+        # sub-setting to specific tests to run, if tests or fixtures were speified
+        if tests_to_run is None and fixtures_to_run is None:
+            test_names_subset = test_names
+        else:
+            test_names_subset = []
+            if tests_to_run is not None:
+                test_names_subset += list(set(test_names).intersection(tests_to_run))
+            if fixtures_to_run is not None:
+                # fixture codes contain the test as substring until the first "["
+                tests_from_fixt = [fixt.split("[")[0] for fixt in fixtures_to_run]
+                test_names_subset += list(set(test_names).intersection(tests_from_fixt))
+            test_names_subset = list(set(test_names_subset))
+
+        # sub-setting by removing all tests from tests_to_exclude
+        if tests_to_exclude is not None:
+            test_names_subset = list(
+                set(test_names_subset).difference(tests_to_exclude)
+            )
+
+        # the below loops run all the tests and collect the results here:
+        results = {}
+        # loop A: we loop over all the tests
+        for test_name in test_names_subset:
+            test_fun = getattr(self, test_name)
+            fixture_sequence = self.fixture_sequence
+
+            # all arguments except the first one (self)
+            fixture_vars = getfullargspec(test_fun)[0][1:]
+            fixture_vars = [var for var in fixture_sequence if var in fixture_vars]
+
+            # this call retrieves the conditional fixtures
+            #  for the test test_name, and the object
+            _, fixture_prod, fixture_names = create_conditional_fixtures_and_names(
+                test_name=test_name,
+                fixture_vars=fixture_vars,
+                generator_dict=temp_generator_dict,
+                fixture_sequence=fixture_sequence,
+                raise_exceptions=raise_exceptions,
+            )
+
+            # if function is decorated with mark.parametrize, add variable settings
+            # NOTE: currently this works only with single-variable mark.parametrize
+            if hasattr(test_fun, "pytestmark"):
+                if len([x for x in test_fun.pytestmark if x.name == "parametrize"]) > 0:
+                    # get the three lists from pytest
+                    (
+                        pytest_fixture_vars,
+                        pytest_fixture_prod,
+                        pytest_fixture_names,
+                    ) = self._get_pytest_mark_args(test_fun)
+                    # add them to the three lists from conditional fixtures
+                    fixture_vars, fixture_prod, fixture_names = self._product_fixtures(
+                        fixture_vars,
+                        fixture_prod,
+                        fixture_names,
+                        pytest_fixture_vars,
+                        pytest_fixture_prod,
+                        pytest_fixture_names,
+                    )
+
+            # loop B: for each test, we loop over all fixtures
+            for params, fixt_name in zip(fixture_prod, fixture_names):
+                # this is needed because pytest unwraps 1-tuples automatically
+                # but subsequent code assumes params is k-tuple, no matter what k is
+                if len(fixture_vars) == 1:
+                    params = (params,)
+                key = f"{test_name}[{fixt_name}]"
+                args = dict(zip(fixture_vars, params))
+
+                # we subset to test-fixtures to run by this, if given
+                #  key is identical to the pytest test-fixture string identifier
+                if fixtures_to_run is not None and key not in fixtures_to_run:
+                    continue
+                if fixtures_to_exclude is not None and key in fixtures_to_exclude:
+                    continue
+
+                if not raise_exceptions:
+                    try:
+                        test_fun(**deepcopy(args))
+                        results[key] = "PASSED"
+                    except Exception as err:
+                        results[key] = err
+                else:
+                    test_fun(**deepcopy(args))
+                    results[key] = "PASSED"
+
+        return results
+
+    @staticmethod
+    def _check_none_str_or_list_of_str(obj, var_name="obj"):
+        """Check that obj is None, str, or list of str, and coerce to list of str."""
+        if obj is not None:
+            msg = f"{var_name} must be None, str, or list of str"
+            if isinstance(obj, str):
+                obj = [obj]
+            if not isinstance(obj, list):
+                raise ValueError(msg)
+            if not np.all(isinstance(x, str) for x in obj):
+                raise ValueError(msg)
+        return obj
+
+    # todo: surely there is a pytest method that can be called instead of this?
+    #   find and replace if it exists
+    @staticmethod
+    def _get_pytest_mark_args(fun):
+        """Get args from pytest mark annotation of function.
+
+        Parameters
+        ----------
+        fun: callable, any function
+
+        Returns
+        -------
+        pytest_fixture_vars: list of str
+            names of args participating in mark.parametrize marks, in pytest order
+        pytest_fixt_list: list of tuple
+            list of value tuples from the mark parameterization
+            i-th value in each tuple corresponds to i-th arg name in pytest_fixture_vars
+        pytest_fixt_names: list of str
+            i-th element is display name for i-th fixture setting in pytest_fixt_list
+        """
+        from itertools import product
+
+        marks = [x for x in fun.pytestmark if x.name == "parametrize"]
+
+        def to_str(obj):
+            return [str(x) for x in obj]
+
+        def get_id(mark):
+            if "ids" in mark.kwargs.keys():
+                return mark.kwargs["ids"]
+            else:
+                return to_str(range(len(mark.args[1])))
+
+        pytest_fixture_vars = [x.args[0] for x in marks]
+        pytest_fixt_raw = [x.args[1] for x in marks]
+        pytest_fixt_list = product(*pytest_fixt_raw)
+        pytest_fixt_names_raw = [get_id(x) for x in marks]
+        pytest_fixt_names = product(*pytest_fixt_names_raw)
+        pytest_fixt_names = ["-".join(x) for x in pytest_fixt_names]
+
+        return pytest_fixture_vars, pytest_fixt_list, pytest_fixt_names
+
+    @staticmethod
+    def _product_fixtures(
+        fixture_vars,
+        fixture_prod,
+        fixture_names,
+        pytest_fixture_vars,
+        pytest_fixture_prod,
+        pytest_fixture_names,
+    ):
+        """Compute products of two sets of fixture vars, values, names."""
+        from itertools import product
+
+        # product of fixture variable names = concatenation
+        fixture_vars_return = fixture_vars + pytest_fixture_vars
+
+        # this is needed because pytest unwraps 1-tuples automatically
+        # but subsequent code assumes params is k-tuple, no matter what k is
+        if len(fixture_vars) == 1:
+            fixture_prod = [(x,) for x in fixture_prod]
+
+        # product of fixture products = Cartesian product plus append tuples
+        fixture_prod_return = product(fixture_prod, pytest_fixture_prod)
+        fixture_prod_return = [sum(x, ()) for x in fixture_prod_return]
+
+        # product of fixture names = Cartesian product plus concat
+        fixture_names_return = product(fixture_names, pytest_fixture_names)
+        fixture_names_return = ["-".join(x) for x in fixture_names_return]
+
+        return fixture_vars_return, fixture_prod_return, fixture_names_return
+
+
+class TestAllObjects(BaseFixtureGenerator, QuickTester):
+    """Package level tests for BaseObjects."""
+
+    def test_create_test_instance(self, object_class):
+        """Check create_test_instance logic and basic constructor functionality.
+
+        create_test_instance and create_test_instances_and_names are the
+        key methods used to create test instances in testing.
+        If this test does not pass, validity of the other tests cannot be guaranteed.
+
+        Also tests inheritance and super call logic in the constructor.
+
+        Tests that:
+
+        * create_test_instance results in an instance of estimator_class
+        * `__init__` calls `super.__init__`
+        * `_tags_dynamic` attribute for tag inspection is present after construction
+        """
+        object_instance = object_class.create_test_instance()
+
+        # Check that init does not construct object of other class than itself
+        assert isinstance(object_instance, object_class), (
+            "object returned by create_test_instance must be an instance of the class, "
+            f"found {type(object_instance)}"
+        )
+
+        msg = (
+            f"{object_class.__name__}.__init__ should call "
+            f"super({object_class.__name__}, self).__init__, "
+            "but that does not seem to be the case. Please ensure to call the "
+            f"parent class's constructor in {object_class.__name__}.__init__"
+        )
+        assert hasattr(object_instance, "_tags_dynamic"), msg
+
+    def test_create_test_instances_and_names(self, object_class):
+        """Check that create_test_instances_and_names works.
+
+        create_test_instance and create_test_instances_and_names are the
+        key methods used to create test instances in testing.
+        If this test does not pass, validity of the other tests cannot be guaranteed.
+
+        Tests expected function signature of create_test_instances_and_names.
+        """
+        objects, names = object_class.create_test_instances_and_names()
+
+        assert isinstance(objects, list), (
+            "first return of create_test_instances_and_names must be a list, "
+            f"found {type(objects)}"
+        )
+        assert isinstance(names, list), (
+            "second return of create_test_instances_and_names must be a list, "
+            f"found {type(names)}"
+        )
+
+        assert np.all(isinstance(est, object_class) for est in objects), (
+            "list elements of first return returned by create_test_instances_and_names "
+            "all must be an instance of the class"
+        )
+
+        assert np.all(isinstance(name, names) for name in names), (
+            "list elements of second return returned by create_test_instances_and_names"
+            " all must be strings"
+        )
+
+        assert len(objects) == len(names), (
+            "the two lists returned by create_test_instances_and_names must have "
+            "equal length"
+        )
+
+    def test_object_tags(self, object_class):
+        """Check conventions on object tags."""
+        assert hasattr(object_class, "get_class_tags")
+        all_tags = object_class.get_class_tags()
+        assert isinstance(all_tags, dict)
+        assert all(isinstance(key, str) for key in all_tags.keys())
+        if hasattr(object_class, "_tags"):
+            tags = object_class._tags
+            msg = (
+                f"_tags attribute of class {object_class} must be dict, "
+                f"but found {type(tags)}"
+            )
+            assert isinstance(tags, dict), msg
+            assert len(tags) > 0, f"_tags dict of class {object_class} is empty"
+            if self.valid_tags is None:
+                invalid_tags = tags
+            else:
+                invalid_tags = [
+                    tag for tag in tags.keys() if tag not in self.valid_tags
+                ]
+            assert len(invalid_tags) == 0, (
+                f"_tags of {object_class} contains invalid tags: {invalid_tags}. "
+                f"For a list of valid tags, see {self.__class__.__name__}.valid_tags."
+            )
+
+        # Avoid ambiguous class attributes
+        ambiguous_attrs = ("tags", "tags_")
+        for attr in ambiguous_attrs:
+            assert not hasattr(object_class, attr), (
+                f"Please avoid using the {attr} attribute to disambiguate it from "
+                f"object tags."
+            )
+
+    def test_inheritance(self, object_class):
+        """Check that object inherits from BaseObject."""
+        assert issubclass(object_class, BaseObject), (
+            f"object: {object_class} " f"is not a sub-class of " f"BaseObject."
+        )
+        # Usually should inherit only from one BaseObject type
+        if self.valid_base_types is not None:
+            n_base_types = sum(
+                issubclass(object_class, cls) for cls in self.valid_base_types
+            )
+            assert n_base_types == 1
+
+    # def test_has_common_interface(self, object_class):
+    #     """Check object implements the common interface."""
+    #     object = object_class
+
+    #     # Check class for type of attribute
+    #     assert isinstance(object.is_fitted, property)
+
+    #     required_methods = _list_required_methods(object_class)
+
+    #     for attr in required_methods:
+    #         assert hasattr(
+    #             object, attr
+    #         ), f"object: {object.__name__} does not implement attribute: {attr}"
+
+    def test_no_cross_test_side_effects_part1(self, object_instance):
+        """Test that there are no side effects across tests, through object state."""
+        object_instance.test__attr = 42
+
+    def test_no_cross_test_side_effects_part2(self, object_instance):
+        """Test that there are no side effects across tests, through object state."""
+        assert not hasattr(object_instance, "test__attr")
+
+    @pytest.mark.parametrize("a", [True, 42])
+    def test_no_between_test_case_side_effects(self, object_instance, a):
+        """Test that there are no side effects across instances of the same test."""
+        assert not hasattr(object_instance, "test__attr")
+        object_instance.test__attr = 42
+
+    @pytest.mark.skipif(
+        not _check_soft_dependencies("sklearn", severity="none"),
+        reason="skip test if sklearn is not available",
+    )  # sklearn is part of the dev dependency set, test should be executed with that
+    def test_get_params(self, object_instance):
+        """Check that get_params works correctly, against sklearn interface."""
+        from sklearn.utils.estimator_checks import (
+            check_get_params_invariance as _check_get_params_invariance,
+        )
+
+        params = object_instance.get_params()
+        assert isinstance(params, dict)
+        _check_get_params_invariance(
+            object_instance.__class__.__name__, object_instance
+        )
+
+    def test_set_params(self, object_instance):
+        """Check that set_params works correctly."""
+        params = object_instance.get_params()
+
+        msg = f"set_params of {type(object_instance).__name__} does not return self"
+        assert object_instance.set_params(**params) is object_instance, msg
+
+        is_equal, equals_msg = deep_equals(
+            object_instance.get_params(), params, return_msg=True
+        )
+        msg = (
+            f"get_params result of {type(object_instance).__name__} (x) does not match "
+            f"what was passed to set_params (y). Reason for discrepancy: {equals_msg}"
+        )
+        assert is_equal, msg
+
+    def test_set_params_sklearn(self, object_class):
+        """Check that set_params works correctly, mirrors sklearn check_set_params.
+
+        Instead of the "fuzz values" in sklearn's check_set_params,
+        we use the other test parameter settings (which are assumed valid).
+        This guarantees settings which play along with the __init__ content.
+        """
+        object_instance = object_class.create_test_instance()
+        test_params = object_class.get_test_params()
+        if not isinstance(test_params, list):
+            test_params = [test_params]
+
+        for params in test_params:
+            # we construct the full parameter set for params
+            # params may only have parameters that are deviating from defaults
+            # in order to set non-default parameters back to defaults
+            params_full = object_class.get_param_defaults()
+            params_full.update(params)
+
+            msg = f"set_params of {object_class.__name__} does not return self"
+            est_after_set = object_instance.set_params(**params_full)
+            assert est_after_set is object_instance, msg
+
+            is_equal, equals_msg = deep_equals(
+                object_instance.get_params(deep=False), params_full, return_msg=True
+            )
+            msg = (
+                f"get_params result of {object_class.__name__} (x) does not match "
+                f"what was passed to set_params (y). "
+                f"Reason for discrepancy: {equals_msg}"
+            )
+            assert is_equal, msg
+
+    def test_clone(self, object_instance):
+        """Check that clone method does not raise exceptions and results in a clone.
+
+        A clone of an object x is an object that:
+
+        * has same class and parameters as x
+        * is not identical with x
+        * is unfitted (even if x was fitted)
+        """
+        obj_clone = object_instance.clone()
+        assert isinstance(obj_clone, type(object_instance))
+        assert obj_clone is not object_instance
+        if hasattr(obj_clone, "is_fitted"):
+            assert not obj_clone.is_fitted
+
+    def test_repr(self, object_instance):
+        """Check we can call repr."""
+        repr(object_instance)
+
+    def test_constructor(self, object_class):
+        """Check that the constructor has sklearn compatible signature and behaviour.
+
+        Based on sklearn check_estimator testing of __init__ logic.
+        Uses create_test_instance to create an instance.
+        Assumes test_create_test_instance has passed and certified create_test_instance.
+
+        Tests that:
+
+        * constructor has no varargs
+        * tests that constructor constructs an instance of the class
+        * tests that all parameters are set in init to an attribute of the same name
+        * tests that parameter values are always copied to the attribute and not changed
+        * tests that default parameters are one of the following:
+            None, str, int, float, bool, tuple, function, joblib memory, numpy primitive
+            (other type parameters should be None, default handling should be by writing
+            the default to attribute of a different name, e.g., my_param_ not my_param)
+        """
+        msg = f"constructor __init__ of {object_class} should have no varargs"
+        assert getfullargspec(object_class.__init__).varkw is None, msg
+
+        obj = object_class.create_test_instance()
+        assert isinstance(obj, object_class)
+
+        # Ensure that each parameter is set in init
+        init_params = _get_args(type(obj).__init__)
+        invalid_attr = set(init_params) - set(vars(obj)) - {"self"}
+        assert not invalid_attr, (
+            "Object %s should store all parameters"
+            " as an attribute during init. Did not find "
+            "attributes `%s`." % (obj.__class__.__name__, sorted(invalid_attr))
+        )
+
+        # Ensure that init does nothing but set parameters
+        # No logic/interaction with other parameters
+        def param_filter(p):
+            """Identify hyper parameters of an estimator."""
+            return p.name != "self" and p.kind not in [p.VAR_KEYWORD, p.VAR_POSITIONAL]
+
+        init_params = [
+            p for p in signature(obj.__init__).parameters.values() if param_filter(p)
+        ]
+
+        params = obj.get_params()
+
+        # Filter out required parameters with no default value and parameters
+        # set for running tests
+        required_params = getattr(obj, "_required_parameters", ())
+
+        test_params = obj.get_test_params()
+        if isinstance(test_params, list):
+            test_params = test_params[0]
+        test_params = test_params.keys()
+
+        init_params = [
+            param
+            for param in init_params
+            if param.name not in required_params and param.name not in test_params
+        ]
+
+        allowed_param_types = [
+            str,
+            int,
+            float,
+            bool,
+            tuple,
+            type(None),
+            np.float64,
+            types.FunctionType,
+        ]
+        if _check_soft_dependencies("joblib", severity="none"):
+            from joblib import Memory
+
+            allowed_param_types += [Memory]
+
+        for param in init_params:
+            assert param.default != param.empty, (
+                "parameter `%s` for %s has no default value and is not "
+                "included in `_required_parameters`"
+                % (param.name, obj.__class__.__name__)
+            )
+            if type(param.default) is type:
+                assert param.default in [np.float64, np.int64]
+            else:
+                assert type(param.default) in allowed_param_types
+
+            param_value = params[param.name]
+            if isinstance(param_value, np.ndarray):
+                np.testing.assert_array_equal(param_value, param.default)
+            else:
+                if bool(
+                    isinstance(param_value, numbers.Real) and np.isnan(param_value)
+                ):
+                    # Allows to set default parameters to np.nan
+                    assert param_value is param.default, param.name
+                else:
+                    assert param_value == param.default, param.name
+
+    def test_valid_object_class_tags(self, object_class):
+        """Check that object class tags are in self.valid_tags."""
+        if self.valid_tags is None:
+            return None
+        for tag in object_class.get_class_tags().keys():
+            assert tag in self.valid_tags
+
+    def test_valid_object_tags(self, object_instance):
+        """Check that object tags are in self.valid_tags."""
+        if self.valid_tags is None:
+            return None
+        for tag in object_instance.get_tags().keys():
+            assert tag in self.valid_tags
```

### Comparing `skbase-0.4.5/skbase/testing/utils/inspect.py` & `skbase-0.4.6/skbase/testing/utils/inspect.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# -*- coding: utf-8 -*-
-"""Utilities for inspection of function arguments."""
-
-
-from inspect import signature
-
-
-def _get_args(function, varargs=False):
-    """Get function arguments."""
-    try:
-        params = signature(function).parameters
-    except ValueError:
-        # Error on builtin C function
-        return []
-    args = [
-        key
-        for key, param in params.items()
-        if param.kind not in (param.VAR_POSITIONAL, param.VAR_KEYWORD)
-    ]
-    if varargs:
-        varargs = [
-            param.name
-            for param in params.values()
-            if param.kind == param.VAR_POSITIONAL
-        ]
-        if len(varargs) == 0:
-            varargs = None
-        return args, varargs
-    else:
-        return args
+# -*- coding: utf-8 -*-
+"""Utilities for inspection of function arguments."""
+
+
+from inspect import signature
+
+
+def _get_args(function, varargs=False):
+    """Get function arguments."""
+    try:
+        params = signature(function).parameters
+    except ValueError:
+        # Error on builtin C function
+        return []
+    args = [
+        key
+        for key, param in params.items()
+        if param.kind not in (param.VAR_POSITIONAL, param.VAR_KEYWORD)
+    ]
+    if varargs:
+        varargs = [
+            param.name
+            for param in params.values()
+            if param.kind == param.VAR_POSITIONAL
+        ]
+        if len(varargs) == 0:
+            varargs = None
+        return args, varargs
+    else:
+        return args
```

### Comparing `skbase-0.4.5/skbase/testing/utils/tests/test_check_dependencies.py` & `skbase-0.4.6/skbase/testing/utils/tests/test_check_dependencies.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-# -*- coding: utf-8 -*-
-"""Tests for _check_soft_dependencies utility."""
-import pytest
-from packaging.requirements import InvalidRequirement
-
-from skbase.testing.utils._dependencies import _check_soft_dependencies
-
-
-def test_check_soft_deps():
-    """Test package availability against pyproject of skbase."""
-    # test various admissible input types, positives
-    assert _check_soft_dependencies("pytest")
-    assert _check_soft_dependencies("pytest", "numpy")
-    assert _check_soft_dependencies("pytest", "numpy")
-    assert _check_soft_dependencies(["pytest", "numpy"])
-    assert _check_soft_dependencies(("pytest", "numpy"))
-
-    # test various admissible input types, negatives
-    assert not _check_soft_dependencies("humpty", severity="none")
-    assert not _check_soft_dependencies("numpy", "dumpty", severity="none")
-    assert not _check_soft_dependencies("humpty", "numpy", severity="none")
-    assert not _check_soft_dependencies(["humpty", "humpty"], severity="none")
-    assert not _check_soft_dependencies(("humpty", "dumpty"), severity="none")
-
-    # test error raise on error severity
-    with pytest.raises(ModuleNotFoundError):
-        assert _check_soft_dependencies("humpty", severity="error")
-    with pytest.raises(ModuleNotFoundError):
-        assert _check_soft_dependencies("numpy", "dumpty", severity="error")
-
-    # test warning on warning severity
-    with pytest.warns():
-        assert not _check_soft_dependencies("humpty", severity="warning")
-    with pytest.warns():
-        assert not _check_soft_dependencies("numpy", "dumpty", severity="warning")
-
-    # test valid PEP 440 specifier strings
-    assert _check_soft_dependencies("pytest>0.0.1")
-    assert _check_soft_dependencies("pytest>=0.0.1", "numpy!=0.1.0")
-    assert not _check_soft_dependencies(("pytest", "numpy<0.1.0"), severity="none")
-    assert _check_soft_dependencies(["pytest", "numpy>0.1.0"], severity="none")
-
-    # test error on invalid PEP 440 specifier string
-    with pytest.raises(InvalidRequirement):
-        assert _check_soft_dependencies("pytest!!!!>>>0.0.1")
-    with pytest.raises(InvalidRequirement):
-        assert _check_soft_dependencies(
-            ("pytest", "!!numpy<~><>0.1.0"), severity="none"
-        )
+# -*- coding: utf-8 -*-
+"""Tests for _check_soft_dependencies utility."""
+import pytest
+from packaging.requirements import InvalidRequirement
+
+from skbase.testing.utils._dependencies import _check_soft_dependencies
+
+
+def test_check_soft_deps():
+    """Test package availability against pyproject of skbase."""
+    # test various admissible input types, positives
+    assert _check_soft_dependencies("pytest")
+    assert _check_soft_dependencies("pytest", "numpy")
+    assert _check_soft_dependencies("pytest", "numpy")
+    assert _check_soft_dependencies(["pytest", "numpy"])
+    assert _check_soft_dependencies(("pytest", "numpy"))
+
+    # test various admissible input types, negatives
+    assert not _check_soft_dependencies("humpty", severity="none")
+    assert not _check_soft_dependencies("numpy", "dumpty", severity="none")
+    assert not _check_soft_dependencies("humpty", "numpy", severity="none")
+    assert not _check_soft_dependencies(["humpty", "humpty"], severity="none")
+    assert not _check_soft_dependencies(("humpty", "dumpty"), severity="none")
+
+    # test error raise on error severity
+    with pytest.raises(ModuleNotFoundError):
+        assert _check_soft_dependencies("humpty", severity="error")
+    with pytest.raises(ModuleNotFoundError):
+        assert _check_soft_dependencies("numpy", "dumpty", severity="error")
+
+    # test warning on warning severity
+    with pytest.warns():
+        assert not _check_soft_dependencies("humpty", severity="warning")
+    with pytest.warns():
+        assert not _check_soft_dependencies("numpy", "dumpty", severity="warning")
+
+    # test valid PEP 440 specifier strings
+    assert _check_soft_dependencies("pytest>0.0.1")
+    assert _check_soft_dependencies("pytest>=0.0.1", "numpy!=0.1.0")
+    assert not _check_soft_dependencies(("pytest", "numpy<0.1.0"), severity="none")
+    assert _check_soft_dependencies(["pytest", "numpy>0.1.0"], severity="none")
+
+    # test error on invalid PEP 440 specifier string
+    with pytest.raises(InvalidRequirement):
+        assert _check_soft_dependencies("pytest!!!!>>>0.0.1")
+    with pytest.raises(InvalidRequirement):
+        assert _check_soft_dependencies(
+            ("pytest", "!!numpy<~><>0.1.0"), severity="none"
+        )
```

### Comparing `skbase-0.4.5/skbase/testing/utils/tests/test_deep_equals.py` & `skbase-0.4.6/skbase/testing/utils/tests/test_deep_equals.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-# -*- coding: utf-8 -*-
-"""Tests for deep_equals utility."""
-from copy import deepcopy
-
-import numpy as np
-import pytest
-
-from skbase.testing.utils._dependencies import _check_soft_dependencies
-from skbase.utils.deep_equals import deep_equals
-
-# examples used for comparison below
-EXAMPLES = [
-    42,
-    [],
-    ((((())))),
-    [([([([()])])])],
-    np.array([2, 3, 4]),
-    np.array([2, 4, 5]),
-    3.5,
-    4.2,
-    np.nan,
-]
-
-
-if _check_soft_dependencies("pandas", severity="none"):
-    import pandas as pd
-
-    EXAMPLES += [
-        pd.DataFrame({"a": [4, 2]}),
-        pd.DataFrame({"a": [4, 3]}),
-        (np.array([1, 2, 4]), [pd.DataFrame({"a": [4, 2]})]),
-        {"foo": [42], "bar": pd.Series([1, 2])},
-        {"bar": [42], "foo": pd.Series([1, 2])},
-    ]
-
-
-@pytest.mark.parametrize("fixture", EXAMPLES)
-def test_deep_equals_positive(fixture):
-    """Tests that deep_equals correctly identifies equal objects as equal."""
-    x = deepcopy(fixture)
-    y = deepcopy(fixture)
-
-    msg = (
-        f"deep_copy incorrectly returned False for two identical copies of "
-        f"the following object: {x}"
-    )
-    assert deep_equals(x, y), msg
-
-
-n = len(EXAMPLES)
-DIFFERENT_PAIRS = [
-    (EXAMPLES[i], EXAMPLES[j]) for i in range(n) for j in range(n) if i != j
-]
-
-
-@pytest.mark.parametrize("fixture1,fixture2", DIFFERENT_PAIRS)
-def test_deep_equals_negative(fixture1, fixture2):
-    """Tests that deep_equals correctly identifies unequal objects as unequal."""
-    x = deepcopy(fixture1)
-    y = deepcopy(fixture2)
-
-    msg = (
-        f"deep_copy incorrectly returned True when comparing "
-        f"the following, different objects: x={x}, y={y}"
-    )
-    assert not deep_equals(x, y), msg
+# -*- coding: utf-8 -*-
+"""Tests for deep_equals utility."""
+from copy import deepcopy
+
+import numpy as np
+import pytest
+
+from skbase.testing.utils._dependencies import _check_soft_dependencies
+from skbase.utils.deep_equals import deep_equals
+
+# examples used for comparison below
+EXAMPLES = [
+    42,
+    [],
+    ((((())))),
+    [([([([()])])])],
+    np.array([2, 3, 4]),
+    np.array([2, 4, 5]),
+    3.5,
+    4.2,
+    np.nan,
+]
+
+
+if _check_soft_dependencies("pandas", severity="none"):
+    import pandas as pd
+
+    EXAMPLES += [
+        pd.DataFrame({"a": [4, 2]}),
+        pd.DataFrame({"a": [4, 3]}),
+        (np.array([1, 2, 4]), [pd.DataFrame({"a": [4, 2]})]),
+        {"foo": [42], "bar": pd.Series([1, 2])},
+        {"bar": [42], "foo": pd.Series([1, 2])},
+    ]
+
+
+@pytest.mark.parametrize("fixture", EXAMPLES)
+def test_deep_equals_positive(fixture):
+    """Tests that deep_equals correctly identifies equal objects as equal."""
+    x = deepcopy(fixture)
+    y = deepcopy(fixture)
+
+    msg = (
+        f"deep_copy incorrectly returned False for two identical copies of "
+        f"the following object: {x}"
+    )
+    assert deep_equals(x, y), msg
+
+
+n = len(EXAMPLES)
+DIFFERENT_PAIRS = [
+    (EXAMPLES[i], EXAMPLES[j]) for i in range(n) for j in range(n) if i != j
+]
+
+
+@pytest.mark.parametrize("fixture1,fixture2", DIFFERENT_PAIRS)
+def test_deep_equals_negative(fixture1, fixture2):
+    """Tests that deep_equals correctly identifies unequal objects as unequal."""
+    x = deepcopy(fixture1)
+    y = deepcopy(fixture2)
+
+    msg = (
+        f"deep_copy incorrectly returned True when comparing "
+        f"the following, different objects: x={x}, y={y}"
+    )
+    assert not deep_equals(x, y), msg
```

### Comparing `skbase-0.4.5/skbase/tests/conftest.py` & `skbase-0.4.6/skbase/tests/conftest.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-# -*- coding: utf-8 -*-
-"""Common functionality for skbase unit tests."""
-from typing import List
-
-from skbase.base import BaseEstimator, BaseObject
-
-__all__: List[str] = [
-    "SKBASE_BASE_CLASSES",
-    "SKBASE_MODULES",
-    "SKBASE_PUBLIC_MODULES",
-    "SKBASE_PUBLIC_CLASSES_BY_MODULE",
-    "SKBASE_CLASSES_BY_MODULE",
-    "SKBASE_PUBLIC_FUNCTIONS_BY_MODULE",
-    "SKBASE_FUNCTIONS_BY_MODULE",
-]
-__author__: List[str] = ["fkiraly", "RNKuhns"]
-
-SKBASE_BASE_CLASSES = (BaseObject, BaseEstimator)
-SKBASE_MODULES = (
-    "skbase",
-    "skbase._exceptions",
-    "skbase._nopytest_tests",
-    "skbase.base",
-    "skbase.base._base",
-    "skbase.base._meta",
-    "skbase.base._pretty_printing",
-    "skbase.base._pretty_printing._object_html_repr",
-    "skbase.base._pretty_printing._pprint",
-    "skbase.base._tagmanager",
-    "skbase.lookup",
-    "skbase.lookup.tests",
-    "skbase.lookup.tests.test_lookup",
-    "skbase.lookup._lookup",
-    "skbase.testing",
-    "skbase.testing.test_all_objects",
-    "skbase.testing.utils",
-    "skbase.testing.utils._conditional_fixtures",
-    "skbase.testing.utils._dependencies",
-    "skbase.testing.utils.deep_equals",
-    "skbase.testing.utils.inspect",
-    "skbase.testing.utils.tests",
-    "skbase.testing.utils.tests.test_deep_equals",
-    "skbase.tests",
-    "skbase.tests.conftest",
-    "skbase.tests.test_base",
-    "skbase.tests.test_baseestimator",
-    "skbase.tests.mock_package.test_mock_package",
-    "skbase.utils",
-    "skbase.utils._check",
-    "skbase.utils._iter",
-    "skbase.utils._nested_iter",
-    "skbase.utils._utils",
-    "skbase.utils.deep_equals",
-    "skbase.utils.dependencies",
-    "skbase.utils.dependencies._dependencies",
-    "skbase.validate",
-    "skbase.validate._named_objects",
-    "skbase.validate._types",
-)
-SKBASE_PUBLIC_MODULES = (
-    "skbase",
-    "skbase.base",
-    "skbase.lookup",
-    "skbase.lookup.tests",
-    "skbase.lookup.tests.test_lookup",
-    "skbase.testing",
-    "skbase.testing.test_all_objects",
-    "skbase.testing.utils",
-    "skbase.testing.utils.deep_equals",
-    "skbase.testing.utils.inspect",
-    "skbase.testing.utils.tests",
-    "skbase.testing.utils.tests.test_deep_equals",
-    "skbase.tests",
-    "skbase.tests.conftest",
-    "skbase.tests.test_base",
-    "skbase.tests.test_baseestimator",
-    "skbase.tests.mock_package.test_mock_package",
-    "skbase.utils",
-    "skbase.utils.deep_equals",
-    "skbase.utils.dependencies",
-    "skbase.validate",
-)
-SKBASE_PUBLIC_CLASSES_BY_MODULE = {
-    "skbase._exceptions": ("FixtureGenerationError", "NotFittedError"),
-    "skbase.base": (
-        "BaseEstimator",
-        "BaseMetaEstimator",
-        "BaseMetaObject",
-        "BaseObject",
-    ),
-    "skbase.base._base": ("BaseEstimator", "BaseObject"),
-    "skbase.base._meta": ("BaseMetaObject", "BaseMetaEstimator"),
-    "skbase.base._pretty_printing._pprint": ("KeyValTuple", "KeyValTupleParam"),
-    "skbase.lookup._lookup": (),
-    "skbase.testing": ("BaseFixtureGenerator", "QuickTester", "TestAllObjects"),
-    "skbase.testing.test_all_objects": (
-        "BaseFixtureGenerator",
-        "QuickTester",
-        "TestAllObjects",
-    ),
-}
-SKBASE_CLASSES_BY_MODULE = SKBASE_PUBLIC_CLASSES_BY_MODULE.copy()
-SKBASE_CLASSES_BY_MODULE.update(
-    {
-        "skbase.base._meta": (
-            "BaseMetaObject",
-            "BaseMetaEstimator",
-            "_MetaObjectMixin",
-            "_MetaTagLogicMixin",
-        ),
-        "skbase.base._pretty_printing._object_html_repr": ("_VisualBlock",),
-        "skbase.base._pretty_printing._pprint": (
-            "KeyValTuple",
-            "KeyValTupleParam",
-            "_BaseObjectPrettyPrinter",
-        ),
-        "skbase.base._tagmanager": ("_FlagManager",),
-    }
-)
-SKBASE_PUBLIC_FUNCTIONS_BY_MODULE = {
-    "skbase.lookup": ("all_objects", "get_package_metadata"),
-    "skbase.lookup._lookup": ("all_objects", "get_package_metadata"),
-    "skbase.testing.utils._conditional_fixtures": (
-        "create_conditional_fixtures_and_names",
-    ),
-    "skbase.testing.utils.deep_equals": ("deep_equals",),
-    "skbase.validate": (
-        "check_sequence_named_objects",
-        "check_sequence",
-        "check_type",
-        "is_named_object_tuple",
-        "is_sequence",
-        "is_sequence_named_objects",
-    ),
-    "skbase.validate._named_objects": (
-        "check_sequence_named_objects",
-        "is_named_object_tuple",
-        "is_sequence_named_objects",
-    ),
-    "skbase.utils": (
-        "deep_equals",
-        "flatten",
-        "is_flat",
-        "make_strings_unique",
-        "subset_dict_keys",
-        "unflat_len",
-        "unflatten",
-    ),
-    "skbase.utils._iter": ("make_strings_unique",),
-    "skbase.utils._nested_iter": (
-        "flatten",
-        "is_flat",
-        "unflat_len",
-        "unflatten",
-    ),
-    "skbase.utils._utils": ("subset_dict_keys",),
-    "skbase.utils.deep_equals": ("deep_equals",),
-    "skbase.validate._types": ("check_sequence", "check_type", "is_sequence"),
-}
-SKBASE_FUNCTIONS_BY_MODULE = SKBASE_PUBLIC_FUNCTIONS_BY_MODULE.copy()
-SKBASE_FUNCTIONS_BY_MODULE.update(
-    {
-        "skbase.base._pretty_printing._object_html_repr": (
-            "_get_visual_block",
-            "_object_html_repr",
-            "_write_base_object_html",
-            "_write_label_html",
-        ),
-        "skbase.base._pretty_printing._pprint": ("_changed_params", "_safe_repr"),
-        "skbase.lookup._lookup": (
-            "_determine_module_path",
-            "_get_return_tags",
-            "_is_ignored_module",
-            "all_objects",
-            "_is_non_public_module",
-            "get_package_metadata",
-            "_make_dataframe",
-            "_walk",
-            "_filter_by_tags",
-            "_filter_by_class",
-            "_import_module",
-            "_check_object_types",
-            "_get_module_info",
-        ),
-        "skbase.testing.utils._dependencies": (
-            "_check_soft_dependencies",
-            "_check_python_version",
-        ),
-        "skbase.testing.utils.deep_equals": ("deep_equals",),
-        "skbase.testing.utils.inspect": ("_get_args",),
-        "skbase.utils._check": ("_is_scalar_nan",),
-        "skbase.utils.dependencies": (
-            "_check_soft_dependencies",
-            "_check_python_version",
-        ),
-        "skbase.utils._iter": (
-            "_format_seq_to_str",
-            "_remove_type_text",
-            "_scalar_to_seq",
-            "make_strings_unique",
-        ),
-        "skbase.utils._nested_iter": (
-            "flatten",
-            "is_flat",
-            "_remove_single",
-            "unflat_len",
-            "unflatten",
-        ),
-        "skbase.utils._utils": ("subset_dict_keys",),
-        "skbase.utils.deep_equals": (
-            "_coerce_list",
-            "_dict_equals",
-            "_fh_equals",
-            "_is_npnan",
-            "_is_npndarray",
-            "_is_pandas",
-            "_pandas_equals",
-            "_softdep_available",
-            "_tuple_equals",
-            "deep_equals",
-        ),
-        "skbase.utils.dependencies._dependencies": (
-            "_check_soft_dependencies",
-            "_check_python_version",
-        ),
-        "skbase.validate._named_objects": (
-            "check_sequence_named_objects",
-            "is_named_object_tuple",
-            "is_sequence_named_objects",
-            "_named_baseobject_error_msg",
-        ),
-        "skbase.validate._types": (
-            "check_sequence",
-            "check_type",
-            "is_sequence",
-            "_convert_scalar_seq_type_input_to_tuple",
-        ),
-    }
-)
-
-
-# Fixture class for testing tag system
-class Parent(BaseObject):
-    """Parent class to test BaseObject's usage."""
-
-    _tags = {"A": "1", "B": 2, "C": 1234, "3": "D"}
-
-    def __init__(self, a="something", b=7, c=None):
-        """Initialize the class."""
-        self.a = a
-        self.b = b
-        self.c = c
-        super().__init__()
-
-    def some_method(self):
-        """To be implemented by child class."""
-        pass
-
-
-# Fixture class for testing tag system, child overrides tags
-class Child(Parent):
-    """Child class that is child of FixtureClassParent."""
-
-    _tags = {"A": 42, "3": "E"}
-    __author__ = ["fkiraly", "RNKuhns"]
-
-    def some_method(self):
-        """Child class' implementation."""
-        pass
-
-    def some_other_method(self):
-        """To be implemented in the child class."""
-        pass
+# -*- coding: utf-8 -*-
+"""Common functionality for skbase unit tests."""
+from typing import List
+
+from skbase.base import BaseEstimator, BaseObject
+
+__all__: List[str] = [
+    "SKBASE_BASE_CLASSES",
+    "SKBASE_MODULES",
+    "SKBASE_PUBLIC_MODULES",
+    "SKBASE_PUBLIC_CLASSES_BY_MODULE",
+    "SKBASE_CLASSES_BY_MODULE",
+    "SKBASE_PUBLIC_FUNCTIONS_BY_MODULE",
+    "SKBASE_FUNCTIONS_BY_MODULE",
+]
+__author__: List[str] = ["fkiraly", "RNKuhns"]
+
+SKBASE_BASE_CLASSES = (BaseObject, BaseEstimator)
+SKBASE_MODULES = (
+    "skbase",
+    "skbase._exceptions",
+    "skbase._nopytest_tests",
+    "skbase.base",
+    "skbase.base._base",
+    "skbase.base._meta",
+    "skbase.base._pretty_printing",
+    "skbase.base._pretty_printing._object_html_repr",
+    "skbase.base._pretty_printing._pprint",
+    "skbase.base._tagmanager",
+    "skbase.lookup",
+    "skbase.lookup.tests",
+    "skbase.lookup.tests.test_lookup",
+    "skbase.lookup._lookup",
+    "skbase.testing",
+    "skbase.testing.test_all_objects",
+    "skbase.testing.utils",
+    "skbase.testing.utils._conditional_fixtures",
+    "skbase.testing.utils._dependencies",
+    "skbase.testing.utils.deep_equals",
+    "skbase.testing.utils.inspect",
+    "skbase.testing.utils.tests",
+    "skbase.testing.utils.tests.test_deep_equals",
+    "skbase.tests",
+    "skbase.tests.conftest",
+    "skbase.tests.test_base",
+    "skbase.tests.test_baseestimator",
+    "skbase.tests.mock_package.test_mock_package",
+    "skbase.utils",
+    "skbase.utils._check",
+    "skbase.utils._iter",
+    "skbase.utils._nested_iter",
+    "skbase.utils._utils",
+    "skbase.utils.deep_equals",
+    "skbase.utils.dependencies",
+    "skbase.utils.dependencies._dependencies",
+    "skbase.validate",
+    "skbase.validate._named_objects",
+    "skbase.validate._types",
+)
+SKBASE_PUBLIC_MODULES = (
+    "skbase",
+    "skbase.base",
+    "skbase.lookup",
+    "skbase.lookup.tests",
+    "skbase.lookup.tests.test_lookup",
+    "skbase.testing",
+    "skbase.testing.test_all_objects",
+    "skbase.testing.utils",
+    "skbase.testing.utils.deep_equals",
+    "skbase.testing.utils.inspect",
+    "skbase.testing.utils.tests",
+    "skbase.testing.utils.tests.test_deep_equals",
+    "skbase.tests",
+    "skbase.tests.conftest",
+    "skbase.tests.test_base",
+    "skbase.tests.test_baseestimator",
+    "skbase.tests.mock_package.test_mock_package",
+    "skbase.utils",
+    "skbase.utils.deep_equals",
+    "skbase.utils.dependencies",
+    "skbase.validate",
+)
+SKBASE_PUBLIC_CLASSES_BY_MODULE = {
+    "skbase._exceptions": ("FixtureGenerationError", "NotFittedError"),
+    "skbase.base": (
+        "BaseEstimator",
+        "BaseMetaEstimator",
+        "BaseMetaObject",
+        "BaseObject",
+    ),
+    "skbase.base._base": ("BaseEstimator", "BaseObject"),
+    "skbase.base._meta": ("BaseMetaObject", "BaseMetaEstimator"),
+    "skbase.base._pretty_printing._pprint": ("KeyValTuple", "KeyValTupleParam"),
+    "skbase.lookup._lookup": (),
+    "skbase.testing": ("BaseFixtureGenerator", "QuickTester", "TestAllObjects"),
+    "skbase.testing.test_all_objects": (
+        "BaseFixtureGenerator",
+        "QuickTester",
+        "TestAllObjects",
+    ),
+}
+SKBASE_CLASSES_BY_MODULE = SKBASE_PUBLIC_CLASSES_BY_MODULE.copy()
+SKBASE_CLASSES_BY_MODULE.update(
+    {
+        "skbase.base._meta": (
+            "BaseMetaObject",
+            "BaseMetaEstimator",
+            "_MetaObjectMixin",
+            "_MetaTagLogicMixin",
+        ),
+        "skbase.base._pretty_printing._object_html_repr": ("_VisualBlock",),
+        "skbase.base._pretty_printing._pprint": (
+            "KeyValTuple",
+            "KeyValTupleParam",
+            "_BaseObjectPrettyPrinter",
+        ),
+        "skbase.base._tagmanager": ("_FlagManager",),
+    }
+)
+SKBASE_PUBLIC_FUNCTIONS_BY_MODULE = {
+    "skbase.lookup": ("all_objects", "get_package_metadata"),
+    "skbase.lookup._lookup": ("all_objects", "get_package_metadata"),
+    "skbase.testing.utils._conditional_fixtures": (
+        "create_conditional_fixtures_and_names",
+    ),
+    "skbase.testing.utils.deep_equals": ("deep_equals",),
+    "skbase.validate": (
+        "check_sequence_named_objects",
+        "check_sequence",
+        "check_type",
+        "is_named_object_tuple",
+        "is_sequence",
+        "is_sequence_named_objects",
+    ),
+    "skbase.validate._named_objects": (
+        "check_sequence_named_objects",
+        "is_named_object_tuple",
+        "is_sequence_named_objects",
+    ),
+    "skbase.utils": (
+        "deep_equals",
+        "flatten",
+        "is_flat",
+        "make_strings_unique",
+        "subset_dict_keys",
+        "unflat_len",
+        "unflatten",
+    ),
+    "skbase.utils._iter": ("make_strings_unique",),
+    "skbase.utils._nested_iter": (
+        "flatten",
+        "is_flat",
+        "unflat_len",
+        "unflatten",
+    ),
+    "skbase.utils._utils": ("subset_dict_keys",),
+    "skbase.utils.deep_equals": ("deep_equals",),
+    "skbase.validate._types": ("check_sequence", "check_type", "is_sequence"),
+}
+SKBASE_FUNCTIONS_BY_MODULE = SKBASE_PUBLIC_FUNCTIONS_BY_MODULE.copy()
+SKBASE_FUNCTIONS_BY_MODULE.update(
+    {
+        "skbase.base._pretty_printing._object_html_repr": (
+            "_get_visual_block",
+            "_object_html_repr",
+            "_write_base_object_html",
+            "_write_label_html",
+        ),
+        "skbase.base._pretty_printing._pprint": ("_changed_params", "_safe_repr"),
+        "skbase.lookup._lookup": (
+            "_determine_module_path",
+            "_get_return_tags",
+            "_is_ignored_module",
+            "all_objects",
+            "_is_non_public_module",
+            "get_package_metadata",
+            "_make_dataframe",
+            "_walk",
+            "_filter_by_tags",
+            "_filter_by_class",
+            "_import_module",
+            "_check_object_types",
+            "_get_module_info",
+        ),
+        "skbase.testing.utils._dependencies": (
+            "_check_soft_dependencies",
+            "_check_python_version",
+        ),
+        "skbase.testing.utils.deep_equals": ("deep_equals",),
+        "skbase.testing.utils.inspect": ("_get_args",),
+        "skbase.utils._check": ("_is_scalar_nan",),
+        "skbase.utils.dependencies": (
+            "_check_soft_dependencies",
+            "_check_python_version",
+        ),
+        "skbase.utils._iter": (
+            "_format_seq_to_str",
+            "_remove_type_text",
+            "_scalar_to_seq",
+            "make_strings_unique",
+        ),
+        "skbase.utils._nested_iter": (
+            "flatten",
+            "is_flat",
+            "_remove_single",
+            "unflat_len",
+            "unflatten",
+        ),
+        "skbase.utils._utils": ("subset_dict_keys",),
+        "skbase.utils.deep_equals": (
+            "_coerce_list",
+            "_dict_equals",
+            "_fh_equals",
+            "_is_npnan",
+            "_is_npndarray",
+            "_is_pandas",
+            "_pandas_equals",
+            "_softdep_available",
+            "_tuple_equals",
+            "deep_equals",
+        ),
+        "skbase.utils.dependencies._dependencies": (
+            "_check_soft_dependencies",
+            "_check_python_version",
+        ),
+        "skbase.validate._named_objects": (
+            "check_sequence_named_objects",
+            "is_named_object_tuple",
+            "is_sequence_named_objects",
+            "_named_baseobject_error_msg",
+        ),
+        "skbase.validate._types": (
+            "check_sequence",
+            "check_type",
+            "is_sequence",
+            "_convert_scalar_seq_type_input_to_tuple",
+        ),
+    }
+)
+
+
+# Fixture class for testing tag system
+class Parent(BaseObject):
+    """Parent class to test BaseObject's usage."""
+
+    _tags = {"A": "1", "B": 2, "C": 1234, "3": "D"}
+
+    def __init__(self, a="something", b=7, c=None):
+        """Initialize the class."""
+        self.a = a
+        self.b = b
+        self.c = c
+        super().__init__()
+
+    def some_method(self):
+        """To be implemented by child class."""
+        pass
+
+
+# Fixture class for testing tag system, child overrides tags
+class Child(Parent):
+    """Child class that is child of FixtureClassParent."""
+
+    _tags = {"A": 42, "3": "E"}
+    __author__ = ["fkiraly", "RNKuhns"]
+
+    def some_method(self):
+        """Child class' implementation."""
+        pass
+
+    def some_other_method(self):
+        """To be implemented in the child class."""
+        pass
```

### Comparing `skbase-0.4.5/skbase/tests/mock_package/test_mock_package.py` & `skbase-0.4.6/skbase/tests/mock_package/test_mock_package.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-# -*- coding: utf-8 -*-
-"""Mock package for testing skbase functionality."""
-from copy import deepcopy
-from typing import List
-
-from skbase.base import BaseObject
-
-__all__: List[str] = [
-    "CompositionDummy",
-    "InheritsFromBaseObject",
-    "AnotherClass",
-    "NotABaseObject",
-]
-__author__: List[str] = ["fkiraly", "RNKuhns"]
-
-
-class CompositionDummy(BaseObject):
-    """Potentially composite object, for testing."""
-
-    def __init__(self, foo, bar=84):
-        self.foo = foo
-        self.foo_ = deepcopy(foo)
-        self.bar = bar
-
-        super(CompositionDummy, self).__init__()
-
-    @classmethod
-    def get_test_params(cls, parameter_set="default"):
-        """Return testing parameter settings for the estimator.
-
-        Parameters
-        ----------
-        parameter_set : str, default="default"
-            Name of the set of test parameters to return, for use in tests. If no
-            special parameters are defined for a value, will return `"default"` set.
-
-        Returns
-        -------
-        params : dict or list of dict, default = {}
-            Parameters to create testing instances of the class
-            Each dict are parameters to construct an "interesting" test instance, i.e.,
-            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
-            `create_test_instance` uses the first (or only) dictionary in `params`
-        """
-        params1 = {"foo": 42}
-        params2 = {"foo": CompositionDummy(126)}
-        return [params1, params2]
-
-
-class InheritsFromBaseObject(BaseObject):
-    """A class inheriting from BaseObject."""
-
-
-class AnotherClass(BaseObject):
-    """Another class inheritting from BaseObject."""
-
-
-class NotABaseObject:
-    """A class that is not a BaseObject."""
-
-    def __init__(self, a=7):
-        self.a = a
-
-
-class _NonPublicClass(BaseObject):
-    """A nonpublic class inheritting from BaseObject."""
-
-
-MOCK_PACKAGE_OBJECTS = [
-    AnotherClass,
-    CompositionDummy,
-    InheritsFromBaseObject,
-    _NonPublicClass,
-]
+# -*- coding: utf-8 -*-
+"""Mock package for testing skbase functionality."""
+from copy import deepcopy
+from typing import List
+
+from skbase.base import BaseObject
+
+__all__: List[str] = [
+    "CompositionDummy",
+    "InheritsFromBaseObject",
+    "AnotherClass",
+    "NotABaseObject",
+]
+__author__: List[str] = ["fkiraly", "RNKuhns"]
+
+
+class CompositionDummy(BaseObject):
+    """Potentially composite object, for testing."""
+
+    def __init__(self, foo, bar=84):
+        self.foo = foo
+        self.foo_ = deepcopy(foo)
+        self.bar = bar
+
+        super(CompositionDummy, self).__init__()
+
+    @classmethod
+    def get_test_params(cls, parameter_set="default"):
+        """Return testing parameter settings for the estimator.
+
+        Parameters
+        ----------
+        parameter_set : str, default="default"
+            Name of the set of test parameters to return, for use in tests. If no
+            special parameters are defined for a value, will return `"default"` set.
+
+        Returns
+        -------
+        params : dict or list of dict, default = {}
+            Parameters to create testing instances of the class
+            Each dict are parameters to construct an "interesting" test instance, i.e.,
+            `MyClass(**params)` or `MyClass(**params[i])` creates a valid test instance.
+            `create_test_instance` uses the first (or only) dictionary in `params`
+        """
+        params1 = {"foo": 42}
+        params2 = {"foo": CompositionDummy(126)}
+        return [params1, params2]
+
+
+class InheritsFromBaseObject(BaseObject):
+    """A class inheriting from BaseObject."""
+
+
+class AnotherClass(BaseObject):
+    """Another class inheritting from BaseObject."""
+
+
+class NotABaseObject:
+    """A class that is not a BaseObject."""
+
+    def __init__(self, a=7):
+        self.a = a
+
+
+class _NonPublicClass(BaseObject):
+    """A nonpublic class inheritting from BaseObject."""
+
+
+MOCK_PACKAGE_OBJECTS = [
+    AnotherClass,
+    CompositionDummy,
+    InheritsFromBaseObject,
+    _NonPublicClass,
+]
```

### Comparing `skbase-0.4.5/skbase/tests/test_base.py` & `skbase-0.4.6/skbase/tests/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,1186 +1,1202 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-# Elements of these tests re-use code developed in scikit-learn. These elements
-# are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
-# conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
-"""Tests for BaseObject universal base class.
-
-tests in this module:
-
-    test_get_class_tags  - tests get_class_tags inheritance logic
-    test_get_class_tag   - tests get_class_tag logic, incl default value
-    test_get_tags        - tests get_tags inheritance logic
-    test_get_tag         - tests get_tag logic, incl default value
-    test_set_tags        - tests set_tags logic and related get_tags inheritance
-
-    test_reset           - tests reset logic on a simple, non-composite estimator
-    test_reset_composite - tests reset logic on a composite estimator
-    test_components      - tests logic for returning components of composite estimator
-"""
-
-__author__ = ["fkiraly", "RNKuhns"]
-
-__all__ = [
-    "test_get_class_tags",
-    "test_get_class_tag",
-    "test_get_tags",
-    "test_get_tag",
-    "test_get_tag_raises",
-    "test_set_tags",
-    "test_set_tags_works_with_missing_tags_dynamic_attribute",
-    "test_clone_tags",
-    "test_is_composite",
-    "test_components",
-    "test_components_raises_error_base_class_is_not_class",
-    "test_components_raises_error_base_class_is_not_baseobject_subclass",
-    "test_reset",
-    "test_reset_composite",
-    "test_get_init_signature",
-    "test_get_init_signature_raises_error_for_invalid_signature",
-    "test_get_param_names",
-    "test_get_params",
-    "test_get_params_invariance",
-    "test_get_params_after_set_params",
-    "test_set_params",
-    "test_set_params_raises_error_non_existent_param",
-    "test_set_params_raises_error_non_interface_composite",
-    "test_raises_on_get_params_for_param_arg_not_assigned_to_attribute",
-    "test_set_params_with_no_param_to_set_returns_object",
-    "test_clone",
-    "test_clone_2",
-    "test_clone_raises_error_for_nonconforming_objects",
-    "test_clone_param_is_none",
-    "test_clone_empty_array",
-    "test_clone_sparse_matrix",
-    "test_clone_nan",
-    "test_clone_estimator_types",
-    "test_clone_class_rather_than_instance_raises_error",
-    "test_baseobject_repr",
-    "test_baseobject_str",
-    "test_baseobject_repr_mimebundle_",
-    "test_repr_html_wraps",
-    "test_get_test_params",
-    "test_get_test_params_raises_error_when_params_required",
-    "test_create_test_instance",
-    "test_create_test_instances_and_names",
-    "test_has_implementation_of",
-    "test_eq_dunder",
-]
-
-import inspect
-from copy import deepcopy
-from typing import Any, Dict, Type
-
-import numpy as np
-import pytest
-import scipy.sparse as sp
-
-from skbase.base import BaseEstimator, BaseObject
-from skbase.testing.utils._dependencies import _check_soft_dependencies
-from skbase.tests.conftest import Child, Parent
-from skbase.tests.mock_package.test_mock_package import CompositionDummy
-
-
-# TODO: Determine if we need to add sklearn style test of
-# test_set_params_passes_all_parameters
-class ResetTester(BaseObject):
-    """Class for testing reset functionality."""
-
-    clsvar = 210
-
-    def __init__(self, a, b=42):
-        self.a = a
-        self.b = b
-        self.c = 84
-        super().__init__()
-
-    def foo(self, d=126):
-        """Foo gets done."""
-        self.d = deepcopy(d)
-        self._d = deepcopy(d)
-        self.d_ = deepcopy(d)
-        self.f__o__o = 252
-
-
-class InvalidInitSignatureTester(BaseObject):
-    """Class for testing invalid signature."""
-
-    def __init__(self, a, *args):
-        super().__init__()
-
-
-class RequiredParam(BaseObject):
-    """BaseObject class with _required_parameters."""
-
-    _required_parameters = ["a"]
-
-    def __init__(self, a, b=7):
-        self.a = a
-        self.b = b
-        super().__init__()
-
-
-class NoParamInterface:
-    """Simple class without BaseObject's param interface for testing get_params."""
-
-    def __init__(self, a=7, b=12):
-        self.a = a
-        self.b = b
-        super().__init__()
-
-
-class Buggy(BaseObject):
-    """A buggy BaseObject that does not set its parameters right."""
-
-    def __init__(self, a=None):
-        self.a = 1
-        self._a = a
-        super().__init__()
-
-
-class ModifyParam(BaseObject):
-    """A non-conforming BaseObject that modifies parameters in init."""
-
-    def __init__(self, a=7):
-        self.a = deepcopy(a)
-        super().__init__()
-
-
-@pytest.fixture
-def fixture_object():
-    """Pytest fixture of BaseObject class."""
-    return BaseObject
-
-
-@pytest.fixture
-def fixture_class_parent():
-    """Pytest fixture for Parent class."""
-    return Parent
-
-
-@pytest.fixture
-def fixture_class_child():
-    """Pytest fixture for Child class."""
-    return Child
-
-
-@pytest.fixture
-def fixture_class_parent_instance():
-    """Pytest fixture for instance of Parent class."""
-    return Parent()
-
-
-@pytest.fixture
-def fixture_class_child_instance():
-    """Pytest fixture for instance of Child class."""
-    return Child()
-
-
-# Fixture class for testing tag system, object overrides class tags
-@pytest.fixture
-def fixture_tag_class_object():
-    """Fixture class for testing tag system, object overrides class tags."""
-    fixture_class_child = Child()
-    fixture_class_child._tags_dynamic = {"A": 42424241, "B": 3}
-    return fixture_class_child
-
-
-@pytest.fixture
-def fixture_composition_dummy():
-    """Pytest fixture for CompositionDummy."""
-    return CompositionDummy
-
-
-@pytest.fixture
-def fixture_reset_tester():
-    """Pytest fixture for ResetTester."""
-    return ResetTester
-
-
-@pytest.fixture
-def fixture_class_child_tags(fixture_class_child: Type[Child]):
-    """Pytest fixture for tags of Child."""
-    return fixture_class_child.get_class_tags()
-
-
-@pytest.fixture
-def fixture_object_instance_set_tags(fixture_tag_class_object: Child):
-    """Fixture class instance to test tag setting."""
-    fixture_tag_set = {"A": 42424243, "E": 3}
-    return fixture_tag_class_object.set_tags(**fixture_tag_set)
-
-
-@pytest.fixture
-def fixture_object_tags():
-    """Fixture object tags."""
-    return {"A": 42424241, "B": 3, "C": 1234, "3": "E"}
-
-
-@pytest.fixture
-def fixture_object_set_tags():
-    """Fixture object tags."""
-    return {"A": 42424243, "B": 3, "C": 1234, "3": "E", "E": 3}
-
-
-@pytest.fixture
-def fixture_object_dynamic_tags():
-    """Fixture object tags."""
-    return {"A": 42424243, "B": 3, "E": 3}
-
-
-@pytest.fixture
-def fixture_invalid_init():
-    """Pytest fixture class for InvalidInitSignatureTester."""
-    return InvalidInitSignatureTester
-
-
-@pytest.fixture
-def fixture_required_param():
-    """Pytest fixture class for RequiredParam."""
-    return RequiredParam
-
-
-@pytest.fixture
-def fixture_buggy():
-    """Pytest fixture class for RequiredParam."""
-    return Buggy
-
-
-@pytest.fixture
-def fixture_modify_param():
-    """Pytest fixture class for RequiredParam."""
-    return ModifyParam
-
-
-@pytest.fixture
-def fixture_class_parent_expected_params():
-    """Pytest fixture class for expected params of Parent."""
-    return {"a": "something", "b": 7, "c": None}
-
-
-@pytest.fixture
-def fixture_class_instance_no_param_interface():
-    """Pytest fixture class instance for NoParamInterface."""
-    return NoParamInterface()
-
-
-def test_get_class_tags(
-    fixture_class_child: Type[Child], fixture_class_child_tags: Any
-):
-    """Test get_class_tags class method of BaseObject for correctness.
-
-    Raises
-    ------
-    AssertError if inheritance logic in get_class_tags is incorrect
-    """
-    child_tags = fixture_class_child.get_class_tags()
-
-    msg = "Inheritance logic in BaseObject.get_class_tags is incorrect"
-
-    assert child_tags == fixture_class_child_tags, msg
-
-
-def test_get_class_tag(fixture_class_child: Type[Child], fixture_class_child_tags: Any):
-    """Test get_class_tag class method of BaseObject for correctness.
-
-    Raises
-    ------
-    AssertError if inheritance logic in get_tag is incorrect
-    AssertError if default override logic in get_tag is incorrect
-    """
-    child_tags = {}
-
-    for key in fixture_class_child_tags:
-        child_tags[key] = fixture_class_child.get_class_tag(key)
-
-    child_tag_default = fixture_class_child.get_class_tag("foo", "bar")
-    child_tag_default_none = fixture_class_child.get_class_tag("bar")
-
-    msg = "Inheritance logic in BaseObject.get_class_tag is incorrect"
-
-    for key in fixture_class_child_tags:
-        assert child_tags[key] == fixture_class_child_tags[key], msg
-
-    msg = "Default override logic in BaseObject.get_class_tag is incorrect"
-
-    assert child_tag_default == "bar", msg
-    assert child_tag_default_none is None, msg
-
-
-def test_get_tags(fixture_tag_class_object: Child, fixture_object_tags: Dict[str, Any]):
-    """Test get_tags method of BaseObject for correctness.
-
-    Raises
-    ------
-    AssertError if inheritance logic in get_tags is incorrect
-    """
-    object_tags = fixture_tag_class_object.get_tags()
-
-    msg = "Inheritance logic in BaseObject.get_tags is incorrect"
-
-    assert object_tags == fixture_object_tags, msg
-
-
-def test_get_tag(fixture_tag_class_object: Child, fixture_object_tags: Dict[str, Any]):
-    """Test get_tag method of BaseObject for correctness.
-
-    Raises
-    ------
-    AssertError if inheritance logic in get_tag is incorrect
-    AssertError if default override logic in get_tag is incorrect
-    """
-    object_tags = {}
-    object_tags_keys = fixture_object_tags.keys()
-
-    for key in object_tags_keys:
-        object_tags[key] = fixture_tag_class_object.get_tag(key, raise_error=False)
-
-    object_tag_default = fixture_tag_class_object.get_tag(
-        "foo", "bar", raise_error=False
-    )
-    object_tag_default_none = fixture_tag_class_object.get_tag("bar", raise_error=False)
-
-    msg = "Inheritance logic in BaseObject.get_tag is incorrect"
-
-    for key in object_tags_keys:
-        assert object_tags[key] == fixture_object_tags[key], msg
-
-    msg = "Default override logic in BaseObject.get_tag is incorrect"
-
-    assert object_tag_default == "bar", msg
-    assert object_tag_default_none is None, msg
-
-
-def test_get_tag_raises(fixture_tag_class_object: Child):
-    """Test that get_tag method raises error for unknown tag.
-
-    Raises
-    ------
-    AssertError if get_tag does not raise error for unknown tag.
-    """
-    with pytest.raises(ValueError, match=r"Tag with name"):
-        fixture_tag_class_object.get_tag("bar")
-
-
-def test_set_tags(
-    fixture_object_instance_set_tags: Any,
-    fixture_object_set_tags: Dict[str, Any],
-    fixture_object_dynamic_tags: Dict[str, int],
-):
-    """Test set_tags method of BaseObject for correctness.
-
-    Raises
-    ------
-    AssertionError if override logic in set_tags is incorrect
-    """
-    msg = "Setter/override logic in BaseObject.set_tags is incorrect"
-
-    assert (
-        fixture_object_instance_set_tags._tags_dynamic == fixture_object_dynamic_tags
-    ), msg
-    assert fixture_object_instance_set_tags.get_tags() == fixture_object_set_tags, msg
-
-
-def test_set_tags_works_with_missing_tags_dynamic_attribute(
-    fixture_tag_class_object: Child,
-):
-    """Test set_tags will still work if _tags_dynamic is missing."""
-    base_obj = deepcopy(fixture_tag_class_object)
-    delattr(base_obj, "_tags_dynamic")
-    assert not hasattr(base_obj, "_tags_dynamic")
-    base_obj.set_tags(some_tag="something")
-    tags = base_obj.get_tags()
-    assert hasattr(base_obj, "_tags_dynamic")
-    assert "some_tag" in tags and tags["some_tag"] == "something"
-
-
-def test_clone_tags():
-    """Test clone_tags works as expected."""
-
-    class TestClass(BaseObject):
-        _tags = {"some_tag": True, "another_tag": 37}
-
-    class AnotherTestClass(BaseObject):
-        pass
-
-    # Simple example of cloning all tags with no tags overlapping
-    base_obj = AnotherTestClass()
-    test_obj = TestClass()
-    assert base_obj.get_tags() == {}
-    base_obj.clone_tags(test_obj)
-    assert base_obj.get_class_tags() == {}
-    assert base_obj.get_tags() == test_obj.get_tags()
-
-    # Simple examples cloning named tags with no tags overlapping
-    base_obj = AnotherTestClass()
-    test_obj = TestClass()
-    assert base_obj.get_tags() == {}
-    base_obj.clone_tags(test_obj, tag_names="some_tag")
-    assert base_obj.get_class_tags() == {}
-    assert base_obj.get_tags() == {"some_tag": True}
-    base_obj.clone_tags(test_obj, tag_names=["another_tag"])
-    assert base_obj.get_class_tags() == {}
-    assert base_obj.get_tags() == test_obj.get_tags()
-
-    # Overlapping tag example where there is tags in each object that aren't
-    # in the other object
-    another_base_obj = AnotherTestClass()
-    another_base_obj.set_tags(some_tag=False, a_new_tag="words")
-    another_base_obj_tags = another_base_obj.get_tags()
-    test_obj = TestClass()
-    assert test_obj.get_tags() == TestClass.get_class_tags()
-    test_obj.clone_tags(another_base_obj)
-    test_obj_tags = test_obj.get_tags()
-    assert test_obj.get_class_tags() == TestClass.get_class_tags()
-    # Verify all tags in another_base_obj were cloned into test_obj
-    for tag in another_base_obj_tags:
-        assert test_obj_tags.get(tag) == another_base_obj_tags[tag]
-    # Verify tag that was in test_obj but not another_base_obj still has same value
-    # and there aren't any other tags
-    assert (
-        "another_tag" in test_obj_tags
-        and test_obj_tags["another_tag"] == 37
-        and len(test_obj_tags) == 3
-    )
-
-    # Overlapping tag example using named tags in clone
-    another_base_obj = AnotherTestClass()
-    another_base_obj.set_tags(some_tag=False, a_new_tag="words")
-    another_base_obj_tags = another_base_obj.get_tags()
-    test_obj = TestClass()
-    assert test_obj.get_tags() == TestClass.get_class_tags()
-    test_obj.clone_tags(another_base_obj, tag_names=["a_new_tag"])
-    test_obj_tags = test_obj.get_tags()
-    assert test_obj.get_class_tags() == TestClass.get_class_tags()
-    assert test_obj_tags.get("a_new_tag") == "words"
-
-    # Verify all tags in another_base_obj were cloned into test_obj
-    test_obj = TestClass()
-    test_obj.clone_tags(another_base_obj)
-    test_obj_tags = test_obj.get_tags()
-    for tag in another_base_obj_tags:
-        assert test_obj_tags.get(tag) == another_base_obj_tags[tag]
-
-
-def test_is_composite(fixture_composition_dummy: Type[CompositionDummy]):
-    """Test is_composite tag for correctness.
-
-    Raises
-    ------
-    AssertionError if logic behind is_composite is incorrect
-    """
-    non_composite = fixture_composition_dummy(foo=42)
-    composite = fixture_composition_dummy(foo=non_composite)
-
-    assert not non_composite.is_composite()
-    assert composite.is_composite()
-
-
-def test_components(
-    fixture_object: Type[BaseObject],
-    fixture_class_parent: Type[Parent],
-    fixture_composition_dummy: Type[CompositionDummy],
-):
-    """Test component retrieval.
-
-    Raises
-    ------
-    AssertionError if logic behind _components is incorrect, logic tested:
-        calling _components on a non-composite returns an empty dict
-        calling _components on a composite returns name/BaseObject pair in dict,
-        and BaseObject returned is identical with attribute of the same name
-    """
-    non_composite = fixture_composition_dummy(foo=42)
-    composite = fixture_composition_dummy(foo=non_composite)
-
-    non_comp_comps = non_composite._components()
-    comp_comps = composite._components()
-    comp_comps_baseobject_filter = composite._components(fixture_object)
-    comp_comps_filter = composite._components(fixture_class_parent)
-
-    assert isinstance(non_comp_comps, dict)
-    assert set(non_comp_comps.keys()) == set()
-
-    assert isinstance(comp_comps, dict)
-    assert set(comp_comps.keys()) == {"foo_"}
-    assert comp_comps["foo_"] == composite.foo_
-    assert comp_comps["foo_"] is composite.foo_
-    assert comp_comps["foo_"] == composite.foo
-    assert comp_comps["foo_"] is not composite.foo
-
-    assert comp_comps == comp_comps_baseobject_filter
-    assert comp_comps_filter == {}
-
-
-def test_components_raises_error_base_class_is_not_class(
-    fixture_object: Type[BaseObject], fixture_composition_dummy: Type[CompositionDummy]
-):
-    """Test _component method raises error if base_class param is not class."""
-    non_composite = fixture_composition_dummy(foo=42)
-    composite = fixture_composition_dummy(foo=non_composite)
-    with pytest.raises(
-        TypeError, match="base_class must be a class, but found <class 'int'>"
-    ):
-        composite._components(7)
-
-    msg = "base_class must be a class, but found <class 'skbase.base._base.BaseObject'>"
-    with pytest.raises(
-        TypeError,
-        match=msg,
-    ):
-        composite._components(fixture_object())
-
-
-def test_components_raises_error_base_class_is_not_baseobject_subclass(
-    fixture_composition_dummy: Type[CompositionDummy],
-):
-    """Test _component method raises error if base_class is not BaseObject subclass."""
-
-    class SomeClass:
-        pass
-
-    composite = fixture_composition_dummy(foo=SomeClass())
-    with pytest.raises(TypeError, match="base_class must be a subclass of BaseObject"):
-        composite._components(SomeClass)
-
-
-# Test parameter interface (get_params, set_params, reset and related methods)
-# Some tests of get_params and set_params are adapted from sklearn tests
-def test_reset(fixture_reset_tester: Type[ResetTester]):
-    """Test reset method for correct behaviour, on a simple estimator.
-
-    Raises
-    ------
-    AssertionError if logic behind reset is incorrect, logic tested:
-        reset should remove any object attributes that are not hyper-parameters,
-        with the exception of attributes containing double-underscore "__"
-        reset should not remove class attributes or methods
-        reset should set hyper-parameters as in pre-reset state
-    """
-    x = fixture_reset_tester(168)
-    x.foo()
-
-    x.reset()
-
-    assert hasattr(x, "a") and x.a == 168
-    assert hasattr(x, "b") and x.b == 42
-    assert hasattr(x, "c") and x.c == 84
-    assert hasattr(x, "clsvar") and x.clsvar == 210
-    assert not hasattr(x, "d")
-    assert not hasattr(x, "_d")
-    assert not hasattr(x, "d_")
-    assert hasattr(x, "f__o__o") and x.f__o__o == 252
-    assert hasattr(x, "foo")
-
-
-def test_reset_composite(fixture_reset_tester: Type[ResetTester]):
-    """Test reset method for correct behaviour, on a composite estimator."""
-    y = fixture_reset_tester(42)
-    x = fixture_reset_tester(a=y)
-
-    x.foo(y)
-    x.d.foo()
-
-    x.reset()
-
-    assert hasattr(x, "a")
-    assert not hasattr(x, "d")
-    assert not hasattr(x.a, "d")
-
-
-def test_get_init_signature(fixture_class_parent: Type[Parent]):
-    """Test error is raised when invalid init signature is used."""
-    init_sig = fixture_class_parent._get_init_signature()
-    init_sig_is_list = isinstance(init_sig, list)
-    init_sig_elements_are_params = all(
-        isinstance(p, inspect.Parameter) for p in init_sig
-    )
-    assert (
-        init_sig_is_list and init_sig_elements_are_params
-    ), "`_get_init_signature` is not returning expected result."
-
-
-def test_get_init_signature_raises_error_for_invalid_signature(
-    fixture_invalid_init: Type[InvalidInitSignatureTester],
-):
-    """Test error is raised when invalid init signature is used."""
-    with pytest.raises(RuntimeError):
-        fixture_invalid_init._get_init_signature()
-
-
-def test_get_param_names(
-    fixture_object: Type[BaseObject],
-    fixture_class_parent: Type[Parent],
-    fixture_class_parent_expected_params: Dict[str, Any],
-):
-    """Test that get_param_names returns list of string parameter names."""
-    param_names = fixture_class_parent.get_param_names()
-    assert param_names == sorted([*fixture_class_parent_expected_params])
-
-    param_names = fixture_object.get_param_names()
-    assert param_names == []
-
-
-def test_get_params(
-    fixture_class_parent: Type[Parent],
-    fixture_class_parent_expected_params: Dict[str, Any],
-    fixture_class_instance_no_param_interface: NoParamInterface,
-    fixture_composition_dummy: Type[CompositionDummy],
-):
-    """Test get_params returns expected parameters."""
-    # Simple test of returned params
-    base_obj = fixture_class_parent()
-    params = base_obj.get_params()
-    assert params == fixture_class_parent_expected_params
-
-    # Test get_params with composite object
-    composite = fixture_composition_dummy(foo=base_obj, bar=84)
-    params = composite.get_params()
-    assert "foo__a" in params and "foo__b" in params and "foo__c" in params
-    assert "bar" in params and params["bar"] == 84
-    assert "foo" in params and isinstance(params["foo"], fixture_class_parent)
-    assert "foo__a" not in composite.get_params(deep=False)
-
-    # Since NoParamInterface does not have get_params we should just return
-    # "foo" and "bar" in params and no other parameters
-    composite = fixture_composition_dummy(foo=fixture_class_instance_no_param_interface)
-    params = composite.get_params()
-    assert "foo" in params and "bar" in params and len(params) == 2
-
-
-def test_get_params_invariance(
-    fixture_class_parent: Type[Parent],
-    fixture_composition_dummy: Type[CompositionDummy],
-):
-    """Test that get_params(deep=False) is subset of get_params(deep=True)."""
-    composite = fixture_composition_dummy(foo=fixture_class_parent(), bar=84)
-    shallow_params = composite.get_params(deep=False)
-    deep_params = composite.get_params(deep=True)
-    assert all(item in deep_params.items() for item in shallow_params.items())
-
-
-def test_get_params_after_set_params(fixture_class_parent: Type[Parent]):
-    """Test that get_params returns the same thing before and after set_params.
-
-    Based on scikit-learn check in check_estimator.
-    """
-    base_obj = fixture_class_parent()
-
-    orig_params = base_obj.get_params(deep=False)
-    msg = "get_params result does not match what was passed to set_params"
-
-    base_obj.set_params(**orig_params)
-    curr_params = base_obj.get_params(deep=False)
-    assert set(orig_params.keys()) == set(curr_params.keys()), msg
-    for k, v in curr_params.items():
-        assert orig_params[k] is v, msg
-
-    # some fuzz values
-    test_values = [-np.inf, np.inf, None]
-
-    test_params = deepcopy(orig_params)
-    for param_name in orig_params.keys():
-        default_value = orig_params[param_name]
-        for value in test_values:
-            test_params[param_name] = value
-            try:
-                base_obj.set_params(**test_params)
-            except (TypeError, ValueError):
-                params_before_exception = curr_params
-                curr_params = base_obj.get_params(deep=False)
-                assert set(params_before_exception.keys()) == set(curr_params.keys())
-                for k, v in curr_params.items():
-                    assert params_before_exception[k] is v
-            else:
-                curr_params = base_obj.get_params(deep=False)
-                assert set(test_params.keys()) == set(curr_params.keys()), msg
-                for k, v in curr_params.items():
-                    assert test_params[k] is v, msg
-        test_params[param_name] = default_value
-
-
-def test_set_params(
-    fixture_class_parent: Type[Parent],
-    fixture_class_parent_expected_params: Dict[str, Any],
-    fixture_composition_dummy: Type[CompositionDummy],
-):
-    """Test set_params works as expected."""
-    # Simple case of setting a parameter
-    base_obj = fixture_class_parent()
-    base_obj.set_params(b="updated param value")
-    expected_params = deepcopy(fixture_class_parent_expected_params)
-    expected_params["b"] = "updated param value"
-    assert base_obj.get_params() == expected_params
-
-    # Setting parameter of a composite class
-    composite = fixture_composition_dummy(foo=fixture_class_parent(), bar=84)
-    composite.set_params(bar=95, foo__b="updated param value")
-    params = composite.get_params()
-    assert params["bar"] == 95
-    assert (
-        params["foo__b"] == "updated param value"
-        and composite.foo.b == "updated param value"
-    )
-
-
-def test_set_params_raises_error_non_existent_param(
-    fixture_class_parent_instance: Parent,
-    fixture_composition_dummy: Type[CompositionDummy],
-):
-    """Test set_params raises an error when passed a non-existent parameter name."""
-    # non-existing parameter in svc
-    with pytest.raises(ValueError):
-        fixture_class_parent_instance.set_params(
-            non_existant_param="updated param value"
-        )
-
-    # non-existing parameter of composite
-    composite = fixture_composition_dummy(foo=fixture_class_parent_instance, bar=84)
-    with pytest.raises(ValueError):
-        composite.set_params(foo__non_existant_param=True)
-
-
-def test_set_params_raises_error_non_interface_composite(
-    fixture_class_instance_no_param_interface: NoParamInterface,
-    fixture_composition_dummy: Type[CompositionDummy],
-):
-    """Test set_params raises error when setting param of non-conforming composite."""
-    # When a composite is made up of a class that doesn't have the BaseObject
-    # parameter interface, we should get a AttributeError when trying to
-    # set the composite's params
-    composite = fixture_composition_dummy(foo=fixture_class_instance_no_param_interface)
-    with pytest.raises(AttributeError):
-        composite.set_params(foo__a=88)
-
-
-def test_raises_on_get_params_for_param_arg_not_assigned_to_attribute():
-    """Test get_params raises error if param not assigned to same named attribute."""
-
-    class BadObject(BaseObject):
-        # Here we don't assign param to self.param as expected in interface
-        def __init__(self, param=5):
-            super().__init__()
-
-    est = BadObject()
-    msg = "'BadObject' object has no attribute 'param'"
-
-    with pytest.raises(AttributeError, match=msg):
-        est.get_params()
-
-
-def test_set_params_with_no_param_to_set_returns_object(
-    fixture_class_parent: Type[Parent],
-):
-    """Test set_params correctly returns self when no parameters are set."""
-    base_obj = fixture_class_parent()
-    orig_params = deepcopy(base_obj.get_params())
-    base_obj_set_params = base_obj.set_params()
-    assert (
-        isinstance(base_obj_set_params, fixture_class_parent)
-        and base_obj_set_params.get_params() == orig_params
-    )
-
-
-# This section tests the clone functionality
-# These have been adapted from sklearn's tests of clone to use the clone
-# method that is included as part of the BaseObject interface
-def test_clone(fixture_class_parent_instance: Parent):
-    """Test that clone is making a deep copy as expected."""
-    # Creates a BaseObject and makes a copy of its original state
-    # (which, in this case, is the current state of the BaseObject),
-    # and check that the obtained copy is a correct deep copy.
-    new_base_obj = fixture_class_parent_instance.clone()
-    assert fixture_class_parent_instance is not new_base_obj
-    assert fixture_class_parent_instance.get_params() == new_base_obj.get_params()
-
-
-def test_clone_2(fixture_class_parent_instance: Parent):
-    """Test that clone does not copy attributes not set in constructor."""
-    # We first create an estimator, give it an own attribute, and
-    # make a copy of its original state. Then we check that the copy doesn't
-    # have the specific attribute we manually added to the initial estimator.
-
-    # base_obj = fixture_class_parent(a=7.0, b="some_str")
-    fixture_class_parent_instance.own_attribute = "test"
-    new_base_obj = fixture_class_parent_instance.clone()
-    assert not hasattr(new_base_obj, "own_attribute")
-
-
-def test_clone_raises_error_for_nonconforming_objects(
-    fixture_invalid_init: Type[InvalidInitSignatureTester],
-    fixture_buggy: Type[Buggy],
-    fixture_modify_param: Type[ModifyParam],
-):
-    """Test that clone raises an error on nonconforming BaseObjects."""
-    buggy = fixture_buggy()
-    buggy.set_config(**{"check_clone": True})
-    buggy.a = 2
-    with pytest.raises(RuntimeError):
-        buggy.clone()
-
-    varg_obj = fixture_invalid_init(a=7)
-    varg_obj.set_config(**{"check_clone": True})
-    with pytest.raises(RuntimeError):
-        varg_obj.clone()
-
-    # fkiraly note: I don't think this class violates the contract,
-    # as equality is defined as via deepcopy
-    # leaving the code here for reference and potential discussion
-    #
-    # obj_that_modifies = fixture_modify_param(a=[0])
-    # obj_that_modifies.set_config(**{"check_clone": True})
-    # with pytest.raises(RuntimeError):
-    #     obj_that_modifies.clone()
-
-
-@pytest.mark.skipif(
-    not _check_soft_dependencies("sklearn", severity="none"),
-    reason="skip test if sklearn is not available",
-)  # sklearn is part of the dev dependency set, test should be executed with that
-def test_clone_param_is_none(fixture_class_parent: Type[Parent]):
-    """Test clone with keyword parameter set to None."""
-    from sklearn.base import clone
-
-    base_obj = fixture_class_parent(c=None)
-    new_base_obj = clone(base_obj)
-    new_base_obj2 = base_obj.clone()
-    assert base_obj.c is new_base_obj.c
-    assert base_obj.c is new_base_obj2.c
-
-
-@pytest.mark.skipif(
-    not _check_soft_dependencies("sklearn", severity="none"),
-    reason="skip test if sklearn is not available",
-)  # sklearn is part of the dev dependency set, test should be executed with that
-def test_clone_empty_array(fixture_class_parent: Type[Parent]):
-    """Test clone with keyword parameter is scipy sparse matrix.
-
-    This test is based on scikit-learn regression test to make sure clone
-    works with default parameter set to scipy sparse matrix.
-    """
-    from sklearn.base import clone
-
-    # Regression test for cloning estimators with empty arrays
-    base_obj = fixture_class_parent(c=np.array([]))
-    new_base_obj = clone(base_obj)
-    new_base_obj2 = base_obj.clone()
-    np.testing.assert_array_equal(base_obj.c, new_base_obj.c)
-    np.testing.assert_array_equal(base_obj.c, new_base_obj2.c)
-
-
-@pytest.mark.skipif(
-    not _check_soft_dependencies("sklearn", severity="none"),
-    reason="skip test if sklearn is not available",
-)  # sklearn is part of the dev dependency set, test should be executed with that
-def test_clone_sparse_matrix(fixture_class_parent: Type[Parent]):
-    """Test clone with keyword parameter is scipy sparse matrix.
-
-    This test is based on scikit-learn regression test to make sure clone
-    works with default parameter set to scipy sparse matrix.
-    """
-    from sklearn.base import clone
-
-    base_obj = fixture_class_parent(c=sp.csr_matrix(np.array([[0]])))
-    new_base_obj = clone(base_obj)
-    new_base_obj2 = base_obj.clone()
-    np.testing.assert_array_equal(base_obj.c, new_base_obj.c)
-    np.testing.assert_array_equal(base_obj.c, new_base_obj2.c)
-
-
-@pytest.mark.skipif(
-    not _check_soft_dependencies("sklearn", severity="none"),
-    reason="skip test if sklearn is not available",
-)  # sklearn is part of the dev dependency set, test should be executed with that
-def test_clone_nan(fixture_class_parent: Type[Parent]):
-    """Test clone with keyword parameter is np.nan.
-
-    This test is based on scikit-learn regression test to make sure clone
-    works with default parameter set to np.nan.
-    """
-    from sklearn.base import clone
-
-    # Regression test for cloning estimators with default parameter as np.nan
-    base_obj = fixture_class_parent(c=np.nan)
-    new_base_obj = clone(base_obj)
-    new_base_obj2 = base_obj.clone()
-
-    assert base_obj.c is new_base_obj.c
-    assert base_obj.c is new_base_obj2.c
-
-
-def test_clone_estimator_types(fixture_class_parent: Type[Parent]):
-    """Test clone works for parameters that are types rather than instances."""
-    base_obj = fixture_class_parent(c=fixture_class_parent)
-    new_base_obj = base_obj.clone()
-
-    assert base_obj.c == new_base_obj.c
-
-
-@pytest.mark.skipif(
-    not _check_soft_dependencies("sklearn", severity="none"),
-    reason="skip test if sklearn is not available",
-)  # sklearn is part of the dev dependency set, test should be executed with that
-def test_clone_class_rather_than_instance_raises_error(
-    fixture_class_parent: Type[Parent],
-):
-    """Test clone raises expected error when cloning a class instead of an instance."""
-    from sklearn.base import clone
-
-    msg = "You should provide an instance of scikit-learn estimator"
-    with pytest.raises(TypeError, match=msg):
-        clone(fixture_class_parent)
-
-
-# Tests of BaseObject pretty printing representation inspired by sklearn
-def test_baseobject_repr(
-    fixture_class_parent: Type[Parent],
-    fixture_composition_dummy: Type[CompositionDummy],
-):
-    """Test BaseObject repr works as expected."""
-    # Simple test where all parameters are left at defaults
-    # Should not see parameters and values in printed representation
-
-    base_obj = fixture_class_parent()
-    assert repr(base_obj) == "Parent()"
-
-    # Check that local config works as expected
-    base_obj.set_config(print_changed_only=False)
-    assert repr(base_obj) == "Parent(a='something', b=7, c=None)"
-
-    # Test with dict parameter (note that dict is sorted by keys when printed)
-    # not printed in order it was created
-    base_obj = fixture_class_parent(c={"c": 1, "a": 2})
-    assert repr(base_obj) == "Parent(c={'a': 2, 'c': 1})"
-
-    # Now test when one params values are named object tuples
-    named_objs = [
-        ("step 1", fixture_class_parent()),
-        ("step 2", fixture_class_parent()),
-    ]
-    base_obj = fixture_class_parent(c=named_objs)
-    assert repr(base_obj) == "Parent(c=[('step 1', Parent()), ('step 2', Parent())])"
-
-    # Or when they are just lists of tuples or just tuples as param
-    base_obj = fixture_class_parent(c=[("one", 1), ("two", 2)])
-    assert repr(base_obj) == "Parent(c=[('one', 1), ('two', 2)])"
-
-    base_obj = fixture_class_parent(c=(1, 2, 3))
-    assert repr(base_obj) == "Parent(c=(1, 2, 3))"
-
-    simple_composite = fixture_composition_dummy(foo=fixture_class_parent())
-    assert repr(simple_composite) == "CompositionDummy(foo=Parent())"
-
-    long_base_obj_repr = fixture_class_parent(a=["long_params"] * 1000)
-    assert len(repr(long_base_obj_repr)) == 535
-
-    named_objs = [(f"Step {i+1}", Child()) for i in range(25)]
-    base_comp = CompositionDummy(foo=Parent(c=Child(c=named_objs)))
-    assert len(repr(base_comp)) == 1362
-
-
-def test_baseobject_str(fixture_class_parent_instance: Parent):
-    """Test BaseObject string representation works."""
-    assert (
-        str(fixture_class_parent_instance) == "Parent()"
-    ), "String representation of instance not working."
-
-    # Check that local config works as expected
-    fixture_class_parent_instance.set_config(print_changed_only=False)
-    assert str(fixture_class_parent_instance) == "Parent(a='something', b=7, c=None)"
-
-
-def test_baseobject_repr_mimebundle_(fixture_class_parent_instance: Parent):
-    """Test display configuration controls output."""
-    # Checks the display configuration flag controls the json output
-    fixture_class_parent_instance.set_config(display="diagram")
-    output = fixture_class_parent_instance._repr_mimebundle_()
-    assert "text/plain" in output
-    assert "text/html" in output
-
-    fixture_class_parent_instance.set_config(display="text")
-    output = fixture_class_parent_instance._repr_mimebundle_()
-    assert "text/plain" in output
-    assert "text/html" not in output
-
-
-def test_repr_html_wraps(fixture_class_parent_instance: Parent):
-    """Test display configuration flag controls the html output."""
-    fixture_class_parent_instance.set_config(display="diagram")
-    output = fixture_class_parent_instance._repr_html_()
-    assert "<style>" in output
-
-    fixture_class_parent_instance.set_config(display="text")
-    msg = "_repr_html_ is only defined when"
-    with pytest.raises(AttributeError, match=msg):
-        fixture_class_parent_instance._repr_html_()
-
-
-# Test BaseObject's ability to generate test instances
-def test_get_test_params(fixture_class_parent_instance: Parent):
-    """Test get_test_params returns empty dictionary."""
-    base_obj = fixture_class_parent_instance
-    test_params = base_obj.get_test_params()
-    assert isinstance(test_params, dict) and len(test_params) == 0
-
-
-def test_get_test_params_raises_error_when_params_required(
-    fixture_required_param: Type[RequiredParam],
-):
-    """Test get_test_params raises an error when parameters are required."""
-    with pytest.raises(ValueError):
-        fixture_required_param(7).get_test_params()
-
-
-def test_create_test_instance(
-    fixture_class_parent: Type[Parent], fixture_class_parent_instance: Parent
-):
-    """Test first that create_test_instance logic works."""
-    base_obj = fixture_class_parent.create_test_instance()
-
-    # Check that init does not construct object of other class than itself
-    assert isinstance(base_obj, fixture_class_parent_instance.__class__), (
-        "Object returned by create_test_instance must be an instance of the class, "
-        f"but found {type(base_obj)}."
-    )
-
-    msg = (
-        f"{fixture_class_parent.__name__}.__init__ should call "
-        f"super({fixture_class_parent.__name__}, self).__init__, "
-        "but that does not seem to be the case. Please ensure to call the "
-        f"parent class's constructor in {fixture_class_parent.__name__}.__init__"
-    )
-    assert hasattr(base_obj, "_tags_dynamic"), msg
-
-
-def test_create_test_instances_and_names(fixture_class_parent_instance: Parent):
-    """Test that create_test_instances_and_names works."""
-    base_objs, names = fixture_class_parent_instance.create_test_instances_and_names()
-
-    assert isinstance(base_objs, list), (
-        "First return of create_test_instances_and_names must be a list, "
-        f"but found {type(base_objs)}."
-    )
-    assert isinstance(names, list), (
-        "Second return of create_test_instances_and_names must be a list, "
-        f"but found {type(names)}."
-    )
-
-    assert all(
-        isinstance(est, fixture_class_parent_instance.__class__) for est in base_objs
-    ), (
-        "List elements of first return returned by create_test_instances_and_names "
-        "all must be an instance of the class"
-    )
-
-    assert all(isinstance(name, str) for name in names), (
-        "List elements of second return returned by create_test_instances_and_names"
-        " all must be strings."
-    )
-
-    assert len(base_objs) == len(names), (
-        "The two lists returned by create_test_instances_and_names must have "
-        "equal length."
-    )
-
-
-# Tests _has_implementation_of interface
-def test_has_implementation_of(
-    fixture_class_parent_instance: Parent, fixture_class_child_instance: Child
-):
-    """Test _has_implementation_of detects methods in class with overrides in mro."""
-    # When the class overrides a parent classes method should return True
-    assert fixture_class_child_instance._has_implementation_of("some_method")
-    # When class implements method first time it shoudl return False
-    assert not fixture_class_child_instance._has_implementation_of("some_other_method")
-
-    # If the method is defined the first time in the parent class it should not
-    # return _has_implementation_of == True
-    assert not fixture_class_parent_instance._has_implementation_of("some_method")
-
-
-class ConfigTester(BaseObject):
-    _config = {"foo_config": 42, "bar": "a"}
-
-    clsvar = 210
-
-    def __init__(self, a, b=42):
-        self.a = a
-        self.b = b
-        self.c = 84
-
-
-class AnotherConfigTester(BaseObject):
-    _config = {"print_changed_only": False, "bar": "a"}
-
-    clsvar = 210
-
-    def __init__(self, a, b=42):
-        self.a = a
-        self.b = b
-        self.c = 84
-
-
-class FittableCompositionDummy(BaseEstimator):
-    """Potentially composite object, for testing."""
-
-    def __init__(self, foo, bar=84):
-        self.foo = foo
-        self.foo_ = deepcopy(foo)
-        self.bar = bar
-
-    def fit(self):
-        if hasattr(self.foo_, "fit"):
-            self.foo_.fit()
-        self._is_fitted = True
-
-
-def test_eq_dunder():
-    """Tests equality dunder for BaseObject descendants.
-
-    Equality should be determined only by get_params results.
-
-    Raises
-    ------
-    AssertionError if logic behind __eq__ is incorrect, logic tested:
-        equality of non-composites depends only on params, not on identity
-        equality of composites depends only on params, not on identity
-        result is not affected by fitting the estimator
-    """
-    non_composite = FittableCompositionDummy(foo=42)
-    non_composite_2 = FittableCompositionDummy(foo=42)
-    non_composite_3 = FittableCompositionDummy(foo=84)
-
-    composite = FittableCompositionDummy(foo=non_composite)
-    composite_2 = FittableCompositionDummy(foo=non_composite_2)
-    composite_3 = FittableCompositionDummy(foo=non_composite_3)
-
-    # test basic equality - expected equalitiesi as per parameters
-    assert non_composite == non_composite
-    assert composite == composite
-    assert non_composite == non_composite_2
-    assert non_composite != non_composite_3
-    assert non_composite_2 != non_composite_3
-    assert composite == composite_2
-    assert composite != composite_3
-    assert composite_2 != composite_3
-
-    # test interaction with clone and copy
-    assert non_composite.clone() == non_composite
-    assert composite.clone() == composite
-    assert deepcopy(non_composite) == non_composite
-    assert deepcopy(composite) == composite
-
-    # test that equality is not be affected by fitting
-    composite.fit()
-    non_composite_2.fit()
-    # composite_2 is an unfitted version of composite
-    # composite is an unfitted version of non_composite_2
-
-    assert non_composite == non_composite
-    assert composite == composite
-    assert non_composite == non_composite_2
-    assert non_composite != non_composite_3
-    assert non_composite_2 != non_composite_3
-    assert composite == composite_2
-    assert composite != composite_3
-    assert composite_2 != composite_3
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+# Elements of these tests re-use code developed in scikit-learn. These elements
+# are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
+# conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
+"""Tests for BaseObject universal base class.
+
+tests in this module:
+
+    test_get_class_tags  - tests get_class_tags inheritance logic
+    test_get_class_tag   - tests get_class_tag logic, incl default value
+    test_get_tags        - tests get_tags inheritance logic
+    test_get_tag         - tests get_tag logic, incl default value
+    test_set_tags        - tests set_tags logic and related get_tags inheritance
+
+    test_reset           - tests reset logic on a simple, non-composite estimator
+    test_reset_composite - tests reset logic on a composite estimator
+    test_components      - tests logic for returning components of composite estimator
+"""
+
+__author__ = ["fkiraly", "RNKuhns"]
+
+__all__ = [
+    "test_get_class_tags",
+    "test_get_class_tag",
+    "test_get_tags",
+    "test_get_tag",
+    "test_get_tag_raises",
+    "test_set_tags",
+    "test_set_tags_works_with_missing_tags_dynamic_attribute",
+    "test_clone_tags",
+    "test_is_composite",
+    "test_components",
+    "test_components_raises_error_base_class_is_not_class",
+    "test_components_raises_error_base_class_is_not_baseobject_subclass",
+    "test_reset",
+    "test_reset_composite",
+    "test_get_init_signature",
+    "test_get_init_signature_raises_error_for_invalid_signature",
+    "test_get_param_names",
+    "test_get_params",
+    "test_get_params_invariance",
+    "test_get_params_after_set_params",
+    "test_set_params",
+    "test_set_params_raises_error_non_existent_param",
+    "test_set_params_raises_error_non_interface_composite",
+    "test_raises_on_get_params_for_param_arg_not_assigned_to_attribute",
+    "test_set_params_with_no_param_to_set_returns_object",
+    "test_clone",
+    "test_clone_2",
+    "test_clone_raises_error_for_nonconforming_objects",
+    "test_clone_param_is_none",
+    "test_clone_empty_array",
+    "test_clone_sparse_matrix",
+    "test_clone_nan",
+    "test_clone_estimator_types",
+    "test_clone_class_rather_than_instance_raises_error",
+    "test_clone_sklearn_composite",
+    "test_baseobject_repr",
+    "test_baseobject_str",
+    "test_baseobject_repr_mimebundle_",
+    "test_repr_html_wraps",
+    "test_get_test_params",
+    "test_get_test_params_raises_error_when_params_required",
+    "test_create_test_instance",
+    "test_create_test_instances_and_names",
+    "test_has_implementation_of",
+    "test_eq_dunder",
+]
+
+import inspect
+from copy import deepcopy
+from typing import Any, Dict, Type
+
+import numpy as np
+import pytest
+import scipy.sparse as sp
+
+from skbase.base import BaseEstimator, BaseObject
+from skbase.testing.utils._dependencies import _check_soft_dependencies
+from skbase.tests.conftest import Child, Parent
+from skbase.tests.mock_package.test_mock_package import CompositionDummy
+
+
+# TODO: Determine if we need to add sklearn style test of
+# test_set_params_passes_all_parameters
+class ResetTester(BaseObject):
+    """Class for testing reset functionality."""
+
+    clsvar = 210
+
+    def __init__(self, a, b=42):
+        self.a = a
+        self.b = b
+        self.c = 84
+        super().__init__()
+
+    def foo(self, d=126):
+        """Foo gets done."""
+        self.d = deepcopy(d)
+        self._d = deepcopy(d)
+        self.d_ = deepcopy(d)
+        self.f__o__o = 252
+
+
+class InvalidInitSignatureTester(BaseObject):
+    """Class for testing invalid signature."""
+
+    def __init__(self, a, *args):
+        super().__init__()
+
+
+class RequiredParam(BaseObject):
+    """BaseObject class with _required_parameters."""
+
+    _required_parameters = ["a"]
+
+    def __init__(self, a, b=7):
+        self.a = a
+        self.b = b
+        super().__init__()
+
+
+class NoParamInterface:
+    """Simple class without BaseObject's param interface for testing get_params."""
+
+    def __init__(self, a=7, b=12):
+        self.a = a
+        self.b = b
+        super().__init__()
+
+
+class Buggy(BaseObject):
+    """A buggy BaseObject that does not set its parameters right."""
+
+    def __init__(self, a=None):
+        self.a = 1
+        self._a = a
+        super().__init__()
+
+
+class ModifyParam(BaseObject):
+    """A non-conforming BaseObject that modifies parameters in init."""
+
+    def __init__(self, a=7):
+        self.a = deepcopy(a)
+        super().__init__()
+
+
+@pytest.fixture
+def fixture_object():
+    """Pytest fixture of BaseObject class."""
+    return BaseObject
+
+
+@pytest.fixture
+def fixture_class_parent():
+    """Pytest fixture for Parent class."""
+    return Parent
+
+
+@pytest.fixture
+def fixture_class_child():
+    """Pytest fixture for Child class."""
+    return Child
+
+
+@pytest.fixture
+def fixture_class_parent_instance():
+    """Pytest fixture for instance of Parent class."""
+    return Parent()
+
+
+@pytest.fixture
+def fixture_class_child_instance():
+    """Pytest fixture for instance of Child class."""
+    return Child()
+
+
+# Fixture class for testing tag system, object overrides class tags
+@pytest.fixture
+def fixture_tag_class_object():
+    """Fixture class for testing tag system, object overrides class tags."""
+    fixture_class_child = Child()
+    fixture_class_child._tags_dynamic = {"A": 42424241, "B": 3}
+    return fixture_class_child
+
+
+@pytest.fixture
+def fixture_composition_dummy():
+    """Pytest fixture for CompositionDummy."""
+    return CompositionDummy
+
+
+@pytest.fixture
+def fixture_reset_tester():
+    """Pytest fixture for ResetTester."""
+    return ResetTester
+
+
+@pytest.fixture
+def fixture_class_child_tags(fixture_class_child: Type[Child]):
+    """Pytest fixture for tags of Child."""
+    return fixture_class_child.get_class_tags()
+
+
+@pytest.fixture
+def fixture_object_instance_set_tags(fixture_tag_class_object: Child):
+    """Fixture class instance to test tag setting."""
+    fixture_tag_set = {"A": 42424243, "E": 3}
+    return fixture_tag_class_object.set_tags(**fixture_tag_set)
+
+
+@pytest.fixture
+def fixture_object_tags():
+    """Fixture object tags."""
+    return {"A": 42424241, "B": 3, "C": 1234, "3": "E"}
+
+
+@pytest.fixture
+def fixture_object_set_tags():
+    """Fixture object tags."""
+    return {"A": 42424243, "B": 3, "C": 1234, "3": "E", "E": 3}
+
+
+@pytest.fixture
+def fixture_object_dynamic_tags():
+    """Fixture object tags."""
+    return {"A": 42424243, "B": 3, "E": 3}
+
+
+@pytest.fixture
+def fixture_invalid_init():
+    """Pytest fixture class for InvalidInitSignatureTester."""
+    return InvalidInitSignatureTester
+
+
+@pytest.fixture
+def fixture_required_param():
+    """Pytest fixture class for RequiredParam."""
+    return RequiredParam
+
+
+@pytest.fixture
+def fixture_buggy():
+    """Pytest fixture class for RequiredParam."""
+    return Buggy
+
+
+@pytest.fixture
+def fixture_modify_param():
+    """Pytest fixture class for RequiredParam."""
+    return ModifyParam
+
+
+@pytest.fixture
+def fixture_class_parent_expected_params():
+    """Pytest fixture class for expected params of Parent."""
+    return {"a": "something", "b": 7, "c": None}
+
+
+@pytest.fixture
+def fixture_class_instance_no_param_interface():
+    """Pytest fixture class instance for NoParamInterface."""
+    return NoParamInterface()
+
+
+def test_get_class_tags(
+    fixture_class_child: Type[Child], fixture_class_child_tags: Any
+):
+    """Test get_class_tags class method of BaseObject for correctness.
+
+    Raises
+    ------
+    AssertError if inheritance logic in get_class_tags is incorrect
+    """
+    child_tags = fixture_class_child.get_class_tags()
+
+    msg = "Inheritance logic in BaseObject.get_class_tags is incorrect"
+
+    assert child_tags == fixture_class_child_tags, msg
+
+
+def test_get_class_tag(fixture_class_child: Type[Child], fixture_class_child_tags: Any):
+    """Test get_class_tag class method of BaseObject for correctness.
+
+    Raises
+    ------
+    AssertError if inheritance logic in get_tag is incorrect
+    AssertError if default override logic in get_tag is incorrect
+    """
+    child_tags = {}
+
+    for key in fixture_class_child_tags:
+        child_tags[key] = fixture_class_child.get_class_tag(key)
+
+    child_tag_default = fixture_class_child.get_class_tag("foo", "bar")
+    child_tag_default_none = fixture_class_child.get_class_tag("bar")
+
+    msg = "Inheritance logic in BaseObject.get_class_tag is incorrect"
+
+    for key in fixture_class_child_tags:
+        assert child_tags[key] == fixture_class_child_tags[key], msg
+
+    msg = "Default override logic in BaseObject.get_class_tag is incorrect"
+
+    assert child_tag_default == "bar", msg
+    assert child_tag_default_none is None, msg
+
+
+def test_get_tags(fixture_tag_class_object: Child, fixture_object_tags: Dict[str, Any]):
+    """Test get_tags method of BaseObject for correctness.
+
+    Raises
+    ------
+    AssertError if inheritance logic in get_tags is incorrect
+    """
+    object_tags = fixture_tag_class_object.get_tags()
+
+    msg = "Inheritance logic in BaseObject.get_tags is incorrect"
+
+    assert object_tags == fixture_object_tags, msg
+
+
+def test_get_tag(fixture_tag_class_object: Child, fixture_object_tags: Dict[str, Any]):
+    """Test get_tag method of BaseObject for correctness.
+
+    Raises
+    ------
+    AssertError if inheritance logic in get_tag is incorrect
+    AssertError if default override logic in get_tag is incorrect
+    """
+    object_tags = {}
+    object_tags_keys = fixture_object_tags.keys()
+
+    for key in object_tags_keys:
+        object_tags[key] = fixture_tag_class_object.get_tag(key, raise_error=False)
+
+    object_tag_default = fixture_tag_class_object.get_tag(
+        "foo", "bar", raise_error=False
+    )
+    object_tag_default_none = fixture_tag_class_object.get_tag("bar", raise_error=False)
+
+    msg = "Inheritance logic in BaseObject.get_tag is incorrect"
+
+    for key in object_tags_keys:
+        assert object_tags[key] == fixture_object_tags[key], msg
+
+    msg = "Default override logic in BaseObject.get_tag is incorrect"
+
+    assert object_tag_default == "bar", msg
+    assert object_tag_default_none is None, msg
+
+
+def test_get_tag_raises(fixture_tag_class_object: Child):
+    """Test that get_tag method raises error for unknown tag.
+
+    Raises
+    ------
+    AssertError if get_tag does not raise error for unknown tag.
+    """
+    with pytest.raises(ValueError, match=r"Tag with name"):
+        fixture_tag_class_object.get_tag("bar")
+
+
+def test_set_tags(
+    fixture_object_instance_set_tags: Any,
+    fixture_object_set_tags: Dict[str, Any],
+    fixture_object_dynamic_tags: Dict[str, int],
+):
+    """Test set_tags method of BaseObject for correctness.
+
+    Raises
+    ------
+    AssertionError if override logic in set_tags is incorrect
+    """
+    msg = "Setter/override logic in BaseObject.set_tags is incorrect"
+
+    assert (
+        fixture_object_instance_set_tags._tags_dynamic == fixture_object_dynamic_tags
+    ), msg
+    assert fixture_object_instance_set_tags.get_tags() == fixture_object_set_tags, msg
+
+
+def test_set_tags_works_with_missing_tags_dynamic_attribute(
+    fixture_tag_class_object: Child,
+):
+    """Test set_tags will still work if _tags_dynamic is missing."""
+    base_obj = deepcopy(fixture_tag_class_object)
+    delattr(base_obj, "_tags_dynamic")
+    assert not hasattr(base_obj, "_tags_dynamic")
+    base_obj.set_tags(some_tag="something")
+    tags = base_obj.get_tags()
+    assert hasattr(base_obj, "_tags_dynamic")
+    assert "some_tag" in tags and tags["some_tag"] == "something"
+
+
+def test_clone_tags():
+    """Test clone_tags works as expected."""
+
+    class TestClass(BaseObject):
+        _tags = {"some_tag": True, "another_tag": 37}
+
+    class AnotherTestClass(BaseObject):
+        pass
+
+    # Simple example of cloning all tags with no tags overlapping
+    base_obj = AnotherTestClass()
+    test_obj = TestClass()
+    assert base_obj.get_tags() == {}
+    base_obj.clone_tags(test_obj)
+    assert base_obj.get_class_tags() == {}
+    assert base_obj.get_tags() == test_obj.get_tags()
+
+    # Simple examples cloning named tags with no tags overlapping
+    base_obj = AnotherTestClass()
+    test_obj = TestClass()
+    assert base_obj.get_tags() == {}
+    base_obj.clone_tags(test_obj, tag_names="some_tag")
+    assert base_obj.get_class_tags() == {}
+    assert base_obj.get_tags() == {"some_tag": True}
+    base_obj.clone_tags(test_obj, tag_names=["another_tag"])
+    assert base_obj.get_class_tags() == {}
+    assert base_obj.get_tags() == test_obj.get_tags()
+
+    # Overlapping tag example where there is tags in each object that aren't
+    # in the other object
+    another_base_obj = AnotherTestClass()
+    another_base_obj.set_tags(some_tag=False, a_new_tag="words")
+    another_base_obj_tags = another_base_obj.get_tags()
+    test_obj = TestClass()
+    assert test_obj.get_tags() == TestClass.get_class_tags()
+    test_obj.clone_tags(another_base_obj)
+    test_obj_tags = test_obj.get_tags()
+    assert test_obj.get_class_tags() == TestClass.get_class_tags()
+    # Verify all tags in another_base_obj were cloned into test_obj
+    for tag in another_base_obj_tags:
+        assert test_obj_tags.get(tag) == another_base_obj_tags[tag]
+    # Verify tag that was in test_obj but not another_base_obj still has same value
+    # and there aren't any other tags
+    assert (
+        "another_tag" in test_obj_tags
+        and test_obj_tags["another_tag"] == 37
+        and len(test_obj_tags) == 3
+    )
+
+    # Overlapping tag example using named tags in clone
+    another_base_obj = AnotherTestClass()
+    another_base_obj.set_tags(some_tag=False, a_new_tag="words")
+    another_base_obj_tags = another_base_obj.get_tags()
+    test_obj = TestClass()
+    assert test_obj.get_tags() == TestClass.get_class_tags()
+    test_obj.clone_tags(another_base_obj, tag_names=["a_new_tag"])
+    test_obj_tags = test_obj.get_tags()
+    assert test_obj.get_class_tags() == TestClass.get_class_tags()
+    assert test_obj_tags.get("a_new_tag") == "words"
+
+    # Verify all tags in another_base_obj were cloned into test_obj
+    test_obj = TestClass()
+    test_obj.clone_tags(another_base_obj)
+    test_obj_tags = test_obj.get_tags()
+    for tag in another_base_obj_tags:
+        assert test_obj_tags.get(tag) == another_base_obj_tags[tag]
+
+
+def test_is_composite(fixture_composition_dummy: Type[CompositionDummy]):
+    """Test is_composite tag for correctness.
+
+    Raises
+    ------
+    AssertionError if logic behind is_composite is incorrect
+    """
+    non_composite = fixture_composition_dummy(foo=42)
+    composite = fixture_composition_dummy(foo=non_composite)
+
+    assert not non_composite.is_composite()
+    assert composite.is_composite()
+
+
+def test_components(
+    fixture_object: Type[BaseObject],
+    fixture_class_parent: Type[Parent],
+    fixture_composition_dummy: Type[CompositionDummy],
+):
+    """Test component retrieval.
+
+    Raises
+    ------
+    AssertionError if logic behind _components is incorrect, logic tested:
+        calling _components on a non-composite returns an empty dict
+        calling _components on a composite returns name/BaseObject pair in dict,
+        and BaseObject returned is identical with attribute of the same name
+    """
+    non_composite = fixture_composition_dummy(foo=42)
+    composite = fixture_composition_dummy(foo=non_composite)
+
+    non_comp_comps = non_composite._components()
+    comp_comps = composite._components()
+    comp_comps_baseobject_filter = composite._components(fixture_object)
+    comp_comps_filter = composite._components(fixture_class_parent)
+
+    assert isinstance(non_comp_comps, dict)
+    assert set(non_comp_comps.keys()) == set()
+
+    assert isinstance(comp_comps, dict)
+    assert set(comp_comps.keys()) == {"foo_"}
+    assert comp_comps["foo_"] == composite.foo_
+    assert comp_comps["foo_"] is composite.foo_
+    assert comp_comps["foo_"] == composite.foo
+    assert comp_comps["foo_"] is not composite.foo
+
+    assert comp_comps == comp_comps_baseobject_filter
+    assert comp_comps_filter == {}
+
+
+def test_components_raises_error_base_class_is_not_class(
+    fixture_object: Type[BaseObject], fixture_composition_dummy: Type[CompositionDummy]
+):
+    """Test _component method raises error if base_class param is not class."""
+    non_composite = fixture_composition_dummy(foo=42)
+    composite = fixture_composition_dummy(foo=non_composite)
+    with pytest.raises(
+        TypeError, match="base_class must be a class, but found <class 'int'>"
+    ):
+        composite._components(7)
+
+    msg = "base_class must be a class, but found <class 'skbase.base._base.BaseObject'>"
+    with pytest.raises(
+        TypeError,
+        match=msg,
+    ):
+        composite._components(fixture_object())
+
+
+def test_components_raises_error_base_class_is_not_baseobject_subclass(
+    fixture_composition_dummy: Type[CompositionDummy],
+):
+    """Test _component method raises error if base_class is not BaseObject subclass."""
+
+    class SomeClass:
+        pass
+
+    composite = fixture_composition_dummy(foo=SomeClass())
+    with pytest.raises(TypeError, match="base_class must be a subclass of BaseObject"):
+        composite._components(SomeClass)
+
+
+# Test parameter interface (get_params, set_params, reset and related methods)
+# Some tests of get_params and set_params are adapted from sklearn tests
+def test_reset(fixture_reset_tester: Type[ResetTester]):
+    """Test reset method for correct behaviour, on a simple estimator.
+
+    Raises
+    ------
+    AssertionError if logic behind reset is incorrect, logic tested:
+        reset should remove any object attributes that are not hyper-parameters,
+        with the exception of attributes containing double-underscore "__"
+        reset should not remove class attributes or methods
+        reset should set hyper-parameters as in pre-reset state
+    """
+    x = fixture_reset_tester(168)
+    x.foo()
+
+    x.reset()
+
+    assert hasattr(x, "a") and x.a == 168
+    assert hasattr(x, "b") and x.b == 42
+    assert hasattr(x, "c") and x.c == 84
+    assert hasattr(x, "clsvar") and x.clsvar == 210
+    assert not hasattr(x, "d")
+    assert not hasattr(x, "_d")
+    assert not hasattr(x, "d_")
+    assert hasattr(x, "f__o__o") and x.f__o__o == 252
+    assert hasattr(x, "foo")
+
+
+def test_reset_composite(fixture_reset_tester: Type[ResetTester]):
+    """Test reset method for correct behaviour, on a composite estimator."""
+    y = fixture_reset_tester(42)
+    x = fixture_reset_tester(a=y)
+
+    x.foo(y)
+    x.d.foo()
+
+    x.reset()
+
+    assert hasattr(x, "a")
+    assert not hasattr(x, "d")
+    assert not hasattr(x.a, "d")
+
+
+def test_get_init_signature(fixture_class_parent: Type[Parent]):
+    """Test error is raised when invalid init signature is used."""
+    init_sig = fixture_class_parent._get_init_signature()
+    init_sig_is_list = isinstance(init_sig, list)
+    init_sig_elements_are_params = all(
+        isinstance(p, inspect.Parameter) for p in init_sig
+    )
+    assert (
+        init_sig_is_list and init_sig_elements_are_params
+    ), "`_get_init_signature` is not returning expected result."
+
+
+def test_get_init_signature_raises_error_for_invalid_signature(
+    fixture_invalid_init: Type[InvalidInitSignatureTester],
+):
+    """Test error is raised when invalid init signature is used."""
+    with pytest.raises(RuntimeError):
+        fixture_invalid_init._get_init_signature()
+
+
+def test_get_param_names(
+    fixture_object: Type[BaseObject],
+    fixture_class_parent: Type[Parent],
+    fixture_class_parent_expected_params: Dict[str, Any],
+):
+    """Test that get_param_names returns list of string parameter names."""
+    param_names = fixture_class_parent.get_param_names()
+    assert param_names == sorted([*fixture_class_parent_expected_params])
+
+    param_names = fixture_object.get_param_names()
+    assert param_names == []
+
+
+def test_get_params(
+    fixture_class_parent: Type[Parent],
+    fixture_class_parent_expected_params: Dict[str, Any],
+    fixture_class_instance_no_param_interface: NoParamInterface,
+    fixture_composition_dummy: Type[CompositionDummy],
+):
+    """Test get_params returns expected parameters."""
+    # Simple test of returned params
+    base_obj = fixture_class_parent()
+    params = base_obj.get_params()
+    assert params == fixture_class_parent_expected_params
+
+    # Test get_params with composite object
+    composite = fixture_composition_dummy(foo=base_obj, bar=84)
+    params = composite.get_params()
+    assert "foo__a" in params and "foo__b" in params and "foo__c" in params
+    assert "bar" in params and params["bar"] == 84
+    assert "foo" in params and isinstance(params["foo"], fixture_class_parent)
+    assert "foo__a" not in composite.get_params(deep=False)
+
+    # Since NoParamInterface does not have get_params we should just return
+    # "foo" and "bar" in params and no other parameters
+    composite = fixture_composition_dummy(foo=fixture_class_instance_no_param_interface)
+    params = composite.get_params()
+    assert "foo" in params and "bar" in params and len(params) == 2
+
+
+def test_get_params_invariance(
+    fixture_class_parent: Type[Parent],
+    fixture_composition_dummy: Type[CompositionDummy],
+):
+    """Test that get_params(deep=False) is subset of get_params(deep=True)."""
+    composite = fixture_composition_dummy(foo=fixture_class_parent(), bar=84)
+    shallow_params = composite.get_params(deep=False)
+    deep_params = composite.get_params(deep=True)
+    assert all(item in deep_params.items() for item in shallow_params.items())
+
+
+def test_get_params_after_set_params(fixture_class_parent: Type[Parent]):
+    """Test that get_params returns the same thing before and after set_params.
+
+    Based on scikit-learn check in check_estimator.
+    """
+    base_obj = fixture_class_parent()
+
+    orig_params = base_obj.get_params(deep=False)
+    msg = "get_params result does not match what was passed to set_params"
+
+    base_obj.set_params(**orig_params)
+    curr_params = base_obj.get_params(deep=False)
+    assert set(orig_params.keys()) == set(curr_params.keys()), msg
+    for k, v in curr_params.items():
+        assert orig_params[k] is v, msg
+
+    # some fuzz values
+    test_values = [-np.inf, np.inf, None]
+
+    test_params = deepcopy(orig_params)
+    for param_name in orig_params.keys():
+        default_value = orig_params[param_name]
+        for value in test_values:
+            test_params[param_name] = value
+            try:
+                base_obj.set_params(**test_params)
+            except (TypeError, ValueError):
+                params_before_exception = curr_params
+                curr_params = base_obj.get_params(deep=False)
+                assert set(params_before_exception.keys()) == set(curr_params.keys())
+                for k, v in curr_params.items():
+                    assert params_before_exception[k] is v
+            else:
+                curr_params = base_obj.get_params(deep=False)
+                assert set(test_params.keys()) == set(curr_params.keys()), msg
+                for k, v in curr_params.items():
+                    assert test_params[k] is v, msg
+        test_params[param_name] = default_value
+
+
+def test_set_params(
+    fixture_class_parent: Type[Parent],
+    fixture_class_parent_expected_params: Dict[str, Any],
+    fixture_composition_dummy: Type[CompositionDummy],
+):
+    """Test set_params works as expected."""
+    # Simple case of setting a parameter
+    base_obj = fixture_class_parent()
+    base_obj.set_params(b="updated param value")
+    expected_params = deepcopy(fixture_class_parent_expected_params)
+    expected_params["b"] = "updated param value"
+    assert base_obj.get_params() == expected_params
+
+    # Setting parameter of a composite class
+    composite = fixture_composition_dummy(foo=fixture_class_parent(), bar=84)
+    composite.set_params(bar=95, foo__b="updated param value")
+    params = composite.get_params()
+    assert params["bar"] == 95
+    assert (
+        params["foo__b"] == "updated param value"
+        and composite.foo.b == "updated param value"
+    )
+
+
+def test_set_params_raises_error_non_existent_param(
+    fixture_class_parent_instance: Parent,
+    fixture_composition_dummy: Type[CompositionDummy],
+):
+    """Test set_params raises an error when passed a non-existent parameter name."""
+    # non-existing parameter in svc
+    with pytest.raises(ValueError):
+        fixture_class_parent_instance.set_params(
+            non_existant_param="updated param value"
+        )
+
+    # non-existing parameter of composite
+    composite = fixture_composition_dummy(foo=fixture_class_parent_instance, bar=84)
+    with pytest.raises(ValueError):
+        composite.set_params(foo__non_existant_param=True)
+
+
+def test_set_params_raises_error_non_interface_composite(
+    fixture_class_instance_no_param_interface: NoParamInterface,
+    fixture_composition_dummy: Type[CompositionDummy],
+):
+    """Test set_params raises error when setting param of non-conforming composite."""
+    # When a composite is made up of a class that doesn't have the BaseObject
+    # parameter interface, we should get a AttributeError when trying to
+    # set the composite's params
+    composite = fixture_composition_dummy(foo=fixture_class_instance_no_param_interface)
+    with pytest.raises(AttributeError):
+        composite.set_params(foo__a=88)
+
+
+def test_raises_on_get_params_for_param_arg_not_assigned_to_attribute():
+    """Test get_params raises error if param not assigned to same named attribute."""
+
+    class BadObject(BaseObject):
+        # Here we don't assign param to self.param as expected in interface
+        def __init__(self, param=5):
+            super().__init__()
+
+    est = BadObject()
+    msg = "'BadObject' object has no attribute 'param'"
+
+    with pytest.raises(AttributeError, match=msg):
+        est.get_params()
+
+
+def test_set_params_with_no_param_to_set_returns_object(
+    fixture_class_parent: Type[Parent],
+):
+    """Test set_params correctly returns self when no parameters are set."""
+    base_obj = fixture_class_parent()
+    orig_params = deepcopy(base_obj.get_params())
+    base_obj_set_params = base_obj.set_params()
+    assert (
+        isinstance(base_obj_set_params, fixture_class_parent)
+        and base_obj_set_params.get_params() == orig_params
+    )
+
+
+# This section tests the clone functionality
+# These have been adapted from sklearn's tests of clone to use the clone
+# method that is included as part of the BaseObject interface
+def test_clone(fixture_class_parent_instance: Parent):
+    """Test that clone is making a deep copy as expected."""
+    # Creates a BaseObject and makes a copy of its original state
+    # (which, in this case, is the current state of the BaseObject),
+    # and check that the obtained copy is a correct deep copy.
+    new_base_obj = fixture_class_parent_instance.clone()
+    assert fixture_class_parent_instance is not new_base_obj
+    assert fixture_class_parent_instance.get_params() == new_base_obj.get_params()
+
+
+def test_clone_2(fixture_class_parent_instance: Parent):
+    """Test that clone does not copy attributes not set in constructor."""
+    # We first create an estimator, give it an own attribute, and
+    # make a copy of its original state. Then we check that the copy doesn't
+    # have the specific attribute we manually added to the initial estimator.
+
+    # base_obj = fixture_class_parent(a=7.0, b="some_str")
+    fixture_class_parent_instance.own_attribute = "test"
+    new_base_obj = fixture_class_parent_instance.clone()
+    assert not hasattr(new_base_obj, "own_attribute")
+
+
+def test_clone_raises_error_for_nonconforming_objects(
+    fixture_invalid_init: Type[InvalidInitSignatureTester],
+    fixture_buggy: Type[Buggy],
+    fixture_modify_param: Type[ModifyParam],
+):
+    """Test that clone raises an error on nonconforming BaseObjects."""
+    buggy = fixture_buggy()
+    buggy.set_config(**{"check_clone": True})
+    buggy.a = 2
+    with pytest.raises(RuntimeError):
+        buggy.clone()
+
+    varg_obj = fixture_invalid_init(a=7)
+    varg_obj.set_config(**{"check_clone": True})
+    with pytest.raises(RuntimeError):
+        varg_obj.clone()
+
+    # fkiraly note: I don't think this class violates the contract,
+    # as equality is defined as via deepcopy
+    # leaving the code here for reference and potential discussion
+    #
+    # obj_that_modifies = fixture_modify_param(a=[0])
+    # obj_that_modifies.set_config(**{"check_clone": True})
+    # with pytest.raises(RuntimeError):
+    #     obj_that_modifies.clone()
+
+
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
+def test_clone_param_is_none(fixture_class_parent: Type[Parent]):
+    """Test clone with keyword parameter set to None."""
+    from sklearn.base import clone
+
+    base_obj = fixture_class_parent(c=None)
+    new_base_obj = clone(base_obj)
+    new_base_obj2 = base_obj.clone()
+    assert base_obj.c is new_base_obj.c
+    assert base_obj.c is new_base_obj2.c
+
+
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
+def test_clone_empty_array(fixture_class_parent: Type[Parent]):
+    """Test clone with keyword parameter is scipy sparse matrix.
+
+    This test is based on scikit-learn regression test to make sure clone
+    works with default parameter set to scipy sparse matrix.
+    """
+    from sklearn.base import clone
+
+    # Regression test for cloning estimators with empty arrays
+    base_obj = fixture_class_parent(c=np.array([]))
+    new_base_obj = clone(base_obj)
+    new_base_obj2 = base_obj.clone()
+    np.testing.assert_array_equal(base_obj.c, new_base_obj.c)
+    np.testing.assert_array_equal(base_obj.c, new_base_obj2.c)
+
+
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
+def test_clone_sparse_matrix(fixture_class_parent: Type[Parent]):
+    """Test clone with keyword parameter is scipy sparse matrix.
+
+    This test is based on scikit-learn regression test to make sure clone
+    works with default parameter set to scipy sparse matrix.
+    """
+    from sklearn.base import clone
+
+    base_obj = fixture_class_parent(c=sp.csr_matrix(np.array([[0]])))
+    new_base_obj = clone(base_obj)
+    new_base_obj2 = base_obj.clone()
+    np.testing.assert_array_equal(base_obj.c, new_base_obj.c)
+    np.testing.assert_array_equal(base_obj.c, new_base_obj2.c)
+
+
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
+def test_clone_nan(fixture_class_parent: Type[Parent]):
+    """Test clone with keyword parameter is np.nan.
+
+    This test is based on scikit-learn regression test to make sure clone
+    works with default parameter set to np.nan.
+    """
+    from sklearn.base import clone
+
+    # Regression test for cloning estimators with default parameter as np.nan
+    base_obj = fixture_class_parent(c=np.nan)
+    new_base_obj = clone(base_obj)
+    new_base_obj2 = base_obj.clone()
+
+    assert base_obj.c is new_base_obj.c
+    assert base_obj.c is new_base_obj2.c
+
+
+def test_clone_estimator_types(fixture_class_parent: Type[Parent]):
+    """Test clone works for parameters that are types rather than instances."""
+    base_obj = fixture_class_parent(c=fixture_class_parent)
+    new_base_obj = base_obj.clone()
+
+    assert base_obj.c == new_base_obj.c
+
+
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
+def test_clone_class_rather_than_instance_raises_error(
+    fixture_class_parent: Type[Parent],
+):
+    """Test clone raises expected error when cloning a class instead of an instance."""
+    from sklearn.base import clone
+
+    msg = "You should provide an instance of scikit-learn estimator"
+    with pytest.raises(TypeError, match=msg):
+        clone(fixture_class_parent)
+
+
+@pytest.mark.skipif(
+    not _check_soft_dependencies("sklearn", severity="none"),
+    reason="skip test if sklearn is not available",
+)  # sklearn is part of the dev dependency set, test should be executed with that
+def test_clone_sklearn_composite(fixture_class_parent: Type[Parent]):
+    """Test clone with keyword parameter set to None."""
+    from sklearn.ensemble import GradientBoostingRegressor
+
+    sklearn_obj = GradientBoostingRegressor(random_state=5, learning_rate=0.02)
+    composite = ResetTester(a=sklearn_obj)
+    composite_set = composite.clone().set_params(a__random_state=42)
+    assert composite.get_params()["a__random_state"] == 5
+    assert composite_set.get_params()["a__random_state"] == 42
+
+
+# Tests of BaseObject pretty printing representation inspired by sklearn
+def test_baseobject_repr(
+    fixture_class_parent: Type[Parent],
+    fixture_composition_dummy: Type[CompositionDummy],
+):
+    """Test BaseObject repr works as expected."""
+    # Simple test where all parameters are left at defaults
+    # Should not see parameters and values in printed representation
+
+    base_obj = fixture_class_parent()
+    assert repr(base_obj) == "Parent()"
+
+    # Check that local config works as expected
+    base_obj.set_config(print_changed_only=False)
+    assert repr(base_obj) == "Parent(a='something', b=7, c=None)"
+
+    # Test with dict parameter (note that dict is sorted by keys when printed)
+    # not printed in order it was created
+    base_obj = fixture_class_parent(c={"c": 1, "a": 2})
+    assert repr(base_obj) == "Parent(c={'a': 2, 'c': 1})"
+
+    # Now test when one params values are named object tuples
+    named_objs = [
+        ("step 1", fixture_class_parent()),
+        ("step 2", fixture_class_parent()),
+    ]
+    base_obj = fixture_class_parent(c=named_objs)
+    assert repr(base_obj) == "Parent(c=[('step 1', Parent()), ('step 2', Parent())])"
+
+    # Or when they are just lists of tuples or just tuples as param
+    base_obj = fixture_class_parent(c=[("one", 1), ("two", 2)])
+    assert repr(base_obj) == "Parent(c=[('one', 1), ('two', 2)])"
+
+    base_obj = fixture_class_parent(c=(1, 2, 3))
+    assert repr(base_obj) == "Parent(c=(1, 2, 3))"
+
+    simple_composite = fixture_composition_dummy(foo=fixture_class_parent())
+    assert repr(simple_composite) == "CompositionDummy(foo=Parent())"
+
+    long_base_obj_repr = fixture_class_parent(a=["long_params"] * 1000)
+    assert len(repr(long_base_obj_repr)) == 535
+
+    named_objs = [(f"Step {i+1}", Child()) for i in range(25)]
+    base_comp = CompositionDummy(foo=Parent(c=Child(c=named_objs)))
+    assert len(repr(base_comp)) == 1362
+
+
+def test_baseobject_str(fixture_class_parent_instance: Parent):
+    """Test BaseObject string representation works."""
+    assert (
+        str(fixture_class_parent_instance) == "Parent()"
+    ), "String representation of instance not working."
+
+    # Check that local config works as expected
+    fixture_class_parent_instance.set_config(print_changed_only=False)
+    assert str(fixture_class_parent_instance) == "Parent(a='something', b=7, c=None)"
+
+
+def test_baseobject_repr_mimebundle_(fixture_class_parent_instance: Parent):
+    """Test display configuration controls output."""
+    # Checks the display configuration flag controls the json output
+    fixture_class_parent_instance.set_config(display="diagram")
+    output = fixture_class_parent_instance._repr_mimebundle_()
+    assert "text/plain" in output
+    assert "text/html" in output
+
+    fixture_class_parent_instance.set_config(display="text")
+    output = fixture_class_parent_instance._repr_mimebundle_()
+    assert "text/plain" in output
+    assert "text/html" not in output
+
+
+def test_repr_html_wraps(fixture_class_parent_instance: Parent):
+    """Test display configuration flag controls the html output."""
+    fixture_class_parent_instance.set_config(display="diagram")
+    output = fixture_class_parent_instance._repr_html_()
+    assert "<style>" in output
+
+    fixture_class_parent_instance.set_config(display="text")
+    msg = "_repr_html_ is only defined when"
+    with pytest.raises(AttributeError, match=msg):
+        fixture_class_parent_instance._repr_html_()
+
+
+# Test BaseObject's ability to generate test instances
+def test_get_test_params(fixture_class_parent_instance: Parent):
+    """Test get_test_params returns empty dictionary."""
+    base_obj = fixture_class_parent_instance
+    test_params = base_obj.get_test_params()
+    assert isinstance(test_params, dict) and len(test_params) == 0
+
+
+def test_get_test_params_raises_error_when_params_required(
+    fixture_required_param: Type[RequiredParam],
+):
+    """Test get_test_params raises an error when parameters are required."""
+    with pytest.raises(ValueError):
+        fixture_required_param(7).get_test_params()
+
+
+def test_create_test_instance(
+    fixture_class_parent: Type[Parent], fixture_class_parent_instance: Parent
+):
+    """Test first that create_test_instance logic works."""
+    base_obj = fixture_class_parent.create_test_instance()
+
+    # Check that init does not construct object of other class than itself
+    assert isinstance(base_obj, fixture_class_parent_instance.__class__), (
+        "Object returned by create_test_instance must be an instance of the class, "
+        f"but found {type(base_obj)}."
+    )
+
+    msg = (
+        f"{fixture_class_parent.__name__}.__init__ should call "
+        f"super({fixture_class_parent.__name__}, self).__init__, "
+        "but that does not seem to be the case. Please ensure to call the "
+        f"parent class's constructor in {fixture_class_parent.__name__}.__init__"
+    )
+    assert hasattr(base_obj, "_tags_dynamic"), msg
+
+
+def test_create_test_instances_and_names(fixture_class_parent_instance: Parent):
+    """Test that create_test_instances_and_names works."""
+    base_objs, names = fixture_class_parent_instance.create_test_instances_and_names()
+
+    assert isinstance(base_objs, list), (
+        "First return of create_test_instances_and_names must be a list, "
+        f"but found {type(base_objs)}."
+    )
+    assert isinstance(names, list), (
+        "Second return of create_test_instances_and_names must be a list, "
+        f"but found {type(names)}."
+    )
+
+    assert all(
+        isinstance(est, fixture_class_parent_instance.__class__) for est in base_objs
+    ), (
+        "List elements of first return returned by create_test_instances_and_names "
+        "all must be an instance of the class"
+    )
+
+    assert all(isinstance(name, str) for name in names), (
+        "List elements of second return returned by create_test_instances_and_names"
+        " all must be strings."
+    )
+
+    assert len(base_objs) == len(names), (
+        "The two lists returned by create_test_instances_and_names must have "
+        "equal length."
+    )
+
+
+# Tests _has_implementation_of interface
+def test_has_implementation_of(
+    fixture_class_parent_instance: Parent, fixture_class_child_instance: Child
+):
+    """Test _has_implementation_of detects methods in class with overrides in mro."""
+    # When the class overrides a parent classes method should return True
+    assert fixture_class_child_instance._has_implementation_of("some_method")
+    # When class implements method first time it shoudl return False
+    assert not fixture_class_child_instance._has_implementation_of("some_other_method")
+
+    # If the method is defined the first time in the parent class it should not
+    # return _has_implementation_of == True
+    assert not fixture_class_parent_instance._has_implementation_of("some_method")
+
+
+class ConfigTester(BaseObject):
+    _config = {"foo_config": 42, "bar": "a"}
+
+    clsvar = 210
+
+    def __init__(self, a, b=42):
+        self.a = a
+        self.b = b
+        self.c = 84
+
+
+class AnotherConfigTester(BaseObject):
+    _config = {"print_changed_only": False, "bar": "a"}
+
+    clsvar = 210
+
+    def __init__(self, a, b=42):
+        self.a = a
+        self.b = b
+        self.c = 84
+
+
+class FittableCompositionDummy(BaseEstimator):
+    """Potentially composite object, for testing."""
+
+    def __init__(self, foo, bar=84):
+        self.foo = foo
+        self.foo_ = deepcopy(foo)
+        self.bar = bar
+
+    def fit(self):
+        if hasattr(self.foo_, "fit"):
+            self.foo_.fit()
+        self._is_fitted = True
+
+
+def test_eq_dunder():
+    """Tests equality dunder for BaseObject descendants.
+
+    Equality should be determined only by get_params results.
+
+    Raises
+    ------
+    AssertionError if logic behind __eq__ is incorrect, logic tested:
+        equality of non-composites depends only on params, not on identity
+        equality of composites depends only on params, not on identity
+        result is not affected by fitting the estimator
+    """
+    non_composite = FittableCompositionDummy(foo=42)
+    non_composite_2 = FittableCompositionDummy(foo=42)
+    non_composite_3 = FittableCompositionDummy(foo=84)
+
+    composite = FittableCompositionDummy(foo=non_composite)
+    composite_2 = FittableCompositionDummy(foo=non_composite_2)
+    composite_3 = FittableCompositionDummy(foo=non_composite_3)
+
+    # test basic equality - expected equalitiesi as per parameters
+    assert non_composite == non_composite
+    assert composite == composite
+    assert non_composite == non_composite_2
+    assert non_composite != non_composite_3
+    assert non_composite_2 != non_composite_3
+    assert composite == composite_2
+    assert composite != composite_3
+    assert composite_2 != composite_3
+
+    # test interaction with clone and copy
+    assert non_composite.clone() == non_composite
+    assert composite.clone() == composite
+    assert deepcopy(non_composite) == non_composite
+    assert deepcopy(composite) == composite
+
+    # test that equality is not be affected by fitting
+    composite.fit()
+    non_composite_2.fit()
+    # composite_2 is an unfitted version of composite
+    # composite is an unfitted version of non_composite_2
+
+    assert non_composite == non_composite
+    assert composite == composite
+    assert non_composite == non_composite_2
+    assert non_composite != non_composite_3
+    assert non_composite_2 != non_composite_3
+    assert composite == composite_2
+    assert composite != composite_3
+    assert composite_2 != composite_3
```

### Comparing `skbase-0.4.5/skbase/tests/test_baseestimator.py` & `skbase-0.4.6/skbase/tests/test_baseestimator.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,130 +1,130 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tests for BaseEstimator class.
-
-tests in this module:
-
-    test_baseestimator_inheritance - Test BaseEstimator inherits from BaseObject.
-    test_has_is_fitted - Test that BaseEstimator has is_fitted interface.
-    test_has_check_is_fitted - Test that BaseEstimator has check_is_fitted inteface.
-    test_is_fitted  - Test that is_fitted property returns _is_fitted as expected.
-    test_check_is_fitted_raises_error_when_unfitted - Test check_is_fitted raises error.
-"""
-
-__author__ = ["fkiraly", "RNKuhns"]
-import inspect
-from copy import deepcopy
-
-import pytest
-
-from skbase._exceptions import NotFittedError
-from skbase.base import BaseEstimator, BaseObject
-
-
-@pytest.fixture
-def fixture_estimator():
-    """Pytest fixture of BaseEstimator class."""
-    return BaseEstimator
-
-
-@pytest.fixture
-def fixture_estimator_instance():
-    """Pytest fixture of BaseEstimator instance."""
-    return BaseEstimator()
-
-
-def test_baseestimator_inheritance(fixture_estimator, fixture_estimator_instance):
-    """Check BaseEstimator correctly inherits from BaseObject."""
-    estimator_is_subclass_of_baseobejct = issubclass(fixture_estimator, BaseObject)
-    estimator_instance_is_baseobject_instance = isinstance(
-        fixture_estimator_instance, BaseObject
-    )
-    assert (
-        estimator_is_subclass_of_baseobejct
-        and estimator_instance_is_baseobject_instance
-    ), "`BaseEstimator` does not correctly inherit from `BaseObject`."
-
-
-def test_has_is_fitted(fixture_estimator_instance):
-    """Test BaseEstimator has `is_fitted` property."""
-    has_private_is_fitted = hasattr(fixture_estimator_instance, "_is_fitted")
-    has_is_fitted = hasattr(fixture_estimator_instance, "is_fitted")
-    assert (
-        has_private_is_fitted and has_is_fitted
-    ), "BaseEstimator does not have `is_fitted` property;"
-
-
-def test_has_check_is_fitted(fixture_estimator_instance):
-    """Test BaseEstimator has `check_is_fitted` method."""
-    has_check_is_fitted = hasattr(fixture_estimator_instance, "check_is_fitted")
-    is_method = inspect.ismethod(fixture_estimator_instance.check_is_fitted)
-    assert (
-        has_check_is_fitted and is_method
-    ), "`BaseEstimator` does not have `check_is_fitted` method."
-
-
-def test_is_fitted(fixture_estimator_instance):
-    """Test BaseEstimator `is_fitted` property returns expected value."""
-    expected_value_unfitted = (
-        fixture_estimator_instance.is_fitted == fixture_estimator_instance._is_fitted
-    )
-    assert (
-        expected_value_unfitted
-    ), "`BaseEstimator` property `is_fitted` does not return `_is_fitted` value."
-
-
-def test_check_is_fitted_raises_error_when_unfitted(fixture_estimator_instance):
-    """Test BaseEstimator `check_is_fitted` method raises an error."""
-    name = fixture_estimator_instance.__class__.__name__
-    match = f"This instance of {name} has not been fitted yet. Please call `fit` first."
-    with pytest.raises(NotFittedError, match=match):
-        fixture_estimator_instance.check_is_fitted()
-
-    fixture_estimator_instance._is_fitted = True
-    assert fixture_estimator_instance.check_is_fitted() is None
-
-
-class FittableCompositionDummy(BaseEstimator):
-    """Potentially composite object, for testing."""
-
-    def __init__(self, foo, bar=84):
-        self.foo = foo
-        self.foo_ = deepcopy(foo)
-        self.bar = bar
-
-    def fit(self):
-        """Fit, dummy."""
-        if hasattr(self.foo_, "fit"):
-            self.foo_.fit()
-        self._is_fitted = True
-
-
-def test_get_fitted_params():
-    """Tests fitted parameter retrieval.
-
-    Raises
-    ------
-    AssertionError if logic behind get_fitted_params is incorrect, logic tested:
-        calling get_fitted_params on a non-composite fittable returns the fitted param
-        calling get_fitted_params on a composite returns all nested params
-    """
-    non_composite = FittableCompositionDummy(foo=42)
-    composite = FittableCompositionDummy(foo=deepcopy(non_composite))
-
-    non_composite.fit()
-    composite.fit()
-
-    non_comp_f_params = non_composite.get_fitted_params()
-    comp_f_params = composite.get_fitted_params()
-    comp_f_params_shallow = composite.get_fitted_params(deep=False)
-
-    assert isinstance(non_comp_f_params, dict)
-    assert set(non_comp_f_params.keys()) == {"foo"}
-
-    assert isinstance(comp_f_params, dict)
-    assert set(comp_f_params) == {"foo", "foo__foo"}
-    assert set(comp_f_params_shallow) == {"foo"}
-    assert comp_f_params["foo"] is composite.foo_
-    assert comp_f_params["foo"] is not composite.foo
-    assert comp_f_params_shallow["foo"] is composite.foo_
-    assert comp_f_params_shallow["foo"] is not composite.foo
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tests for BaseEstimator class.
+
+tests in this module:
+
+    test_baseestimator_inheritance - Test BaseEstimator inherits from BaseObject.
+    test_has_is_fitted - Test that BaseEstimator has is_fitted interface.
+    test_has_check_is_fitted - Test that BaseEstimator has check_is_fitted inteface.
+    test_is_fitted  - Test that is_fitted property returns _is_fitted as expected.
+    test_check_is_fitted_raises_error_when_unfitted - Test check_is_fitted raises error.
+"""
+
+__author__ = ["fkiraly", "RNKuhns"]
+import inspect
+from copy import deepcopy
+
+import pytest
+
+from skbase._exceptions import NotFittedError
+from skbase.base import BaseEstimator, BaseObject
+
+
+@pytest.fixture
+def fixture_estimator():
+    """Pytest fixture of BaseEstimator class."""
+    return BaseEstimator
+
+
+@pytest.fixture
+def fixture_estimator_instance():
+    """Pytest fixture of BaseEstimator instance."""
+    return BaseEstimator()
+
+
+def test_baseestimator_inheritance(fixture_estimator, fixture_estimator_instance):
+    """Check BaseEstimator correctly inherits from BaseObject."""
+    estimator_is_subclass_of_baseobejct = issubclass(fixture_estimator, BaseObject)
+    estimator_instance_is_baseobject_instance = isinstance(
+        fixture_estimator_instance, BaseObject
+    )
+    assert (
+        estimator_is_subclass_of_baseobejct
+        and estimator_instance_is_baseobject_instance
+    ), "`BaseEstimator` does not correctly inherit from `BaseObject`."
+
+
+def test_has_is_fitted(fixture_estimator_instance):
+    """Test BaseEstimator has `is_fitted` property."""
+    has_private_is_fitted = hasattr(fixture_estimator_instance, "_is_fitted")
+    has_is_fitted = hasattr(fixture_estimator_instance, "is_fitted")
+    assert (
+        has_private_is_fitted and has_is_fitted
+    ), "BaseEstimator does not have `is_fitted` property;"
+
+
+def test_has_check_is_fitted(fixture_estimator_instance):
+    """Test BaseEstimator has `check_is_fitted` method."""
+    has_check_is_fitted = hasattr(fixture_estimator_instance, "check_is_fitted")
+    is_method = inspect.ismethod(fixture_estimator_instance.check_is_fitted)
+    assert (
+        has_check_is_fitted and is_method
+    ), "`BaseEstimator` does not have `check_is_fitted` method."
+
+
+def test_is_fitted(fixture_estimator_instance):
+    """Test BaseEstimator `is_fitted` property returns expected value."""
+    expected_value_unfitted = (
+        fixture_estimator_instance.is_fitted == fixture_estimator_instance._is_fitted
+    )
+    assert (
+        expected_value_unfitted
+    ), "`BaseEstimator` property `is_fitted` does not return `_is_fitted` value."
+
+
+def test_check_is_fitted_raises_error_when_unfitted(fixture_estimator_instance):
+    """Test BaseEstimator `check_is_fitted` method raises an error."""
+    name = fixture_estimator_instance.__class__.__name__
+    match = f"This instance of {name} has not been fitted yet. Please call `fit` first."
+    with pytest.raises(NotFittedError, match=match):
+        fixture_estimator_instance.check_is_fitted()
+
+    fixture_estimator_instance._is_fitted = True
+    assert fixture_estimator_instance.check_is_fitted() is None
+
+
+class FittableCompositionDummy(BaseEstimator):
+    """Potentially composite object, for testing."""
+
+    def __init__(self, foo, bar=84):
+        self.foo = foo
+        self.foo_ = deepcopy(foo)
+        self.bar = bar
+
+    def fit(self):
+        """Fit, dummy."""
+        if hasattr(self.foo_, "fit"):
+            self.foo_.fit()
+        self._is_fitted = True
+
+
+def test_get_fitted_params():
+    """Tests fitted parameter retrieval.
+
+    Raises
+    ------
+    AssertionError if logic behind get_fitted_params is incorrect, logic tested:
+        calling get_fitted_params on a non-composite fittable returns the fitted param
+        calling get_fitted_params on a composite returns all nested params
+    """
+    non_composite = FittableCompositionDummy(foo=42)
+    composite = FittableCompositionDummy(foo=deepcopy(non_composite))
+
+    non_composite.fit()
+    composite.fit()
+
+    non_comp_f_params = non_composite.get_fitted_params()
+    comp_f_params = composite.get_fitted_params()
+    comp_f_params_shallow = composite.get_fitted_params(deep=False)
+
+    assert isinstance(non_comp_f_params, dict)
+    assert set(non_comp_f_params.keys()) == {"foo"}
+
+    assert isinstance(comp_f_params, dict)
+    assert set(comp_f_params) == {"foo", "foo__foo"}
+    assert set(comp_f_params_shallow) == {"foo"}
+    assert comp_f_params["foo"] is composite.foo_
+    assert comp_f_params["foo"] is not composite.foo
+    assert comp_f_params_shallow["foo"] is composite.foo_
+    assert comp_f_params_shallow["foo"] is not composite.foo
```

### Comparing `skbase-0.4.5/skbase/tests/test_exceptions.py` & `skbase-0.4.6/skbase/tests/test_exceptions.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# -*- coding: utf-8 -*-
-"""Tests for skbase exceptions.
-
-tests in this module:
-
-    test_exceptions_raise_error - Test that skbase exceptions raise expected error.
-"""
-from typing import List
-
-import pytest
-
-from skbase._exceptions import FixtureGenerationError, NotFittedError
-
-__author__: List[str] = ["RNKuhns"]
-
-ALL_EXCEPTIONS = [FixtureGenerationError, NotFittedError]
-
-
-@pytest.mark.parametrize("skbase_exception", ALL_EXCEPTIONS)
-def test_exceptions_raise_error(skbase_exception):
-    """Test that skbase exceptions raise an error as expected."""
-    with pytest.raises(skbase_exception):
-        raise skbase_exception()
+# -*- coding: utf-8 -*-
+"""Tests for skbase exceptions.
+
+tests in this module:
+
+    test_exceptions_raise_error - Test that skbase exceptions raise expected error.
+"""
+from typing import List
+
+import pytest
+
+from skbase._exceptions import FixtureGenerationError, NotFittedError
+
+__author__: List[str] = ["RNKuhns"]
+
+ALL_EXCEPTIONS = [FixtureGenerationError, NotFittedError]
+
+
+@pytest.mark.parametrize("skbase_exception", ALL_EXCEPTIONS)
+def test_exceptions_raise_error(skbase_exception):
+    """Test that skbase exceptions raise an error as expected."""
+    with pytest.raises(skbase_exception):
+        raise skbase_exception()
```

### Comparing `skbase-0.4.5/skbase/tests/test_meta.py` & `skbase-0.4.6/skbase/tests/test_meta.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tests for BaseMetaObject and BaseMetaEstimator mixins.
-
-tests in this module:
-
-
-"""
-
-__author__ = ["RNKuhns"]
-import inspect
-
-import pytest
-
-from skbase._exceptions import NotFittedError
-from skbase.base import BaseEstimator, BaseObject
-from skbase.base._meta import (
-    BaseMetaEstimator,
-    BaseMetaObject,
-    _MetaObjectMixin,
-    _MetaTagLogicMixin,
-)
-
-
-class MetaObjectTester(BaseMetaObject):
-    """Class to test meta object functionality."""
-
-    def __init__(self, a=7, b="something", c=None, steps=None):
-        self.a = a
-        self.b = b
-        self.c = c
-        self.steps = steps
-
-
-class MetaEstimatorTester(BaseMetaEstimator):
-    """Class to test meta estimator functionality."""
-
-    def __init__(self, a=7, b="something", c=None, steps=None):
-        self.a = a
-        self.b = b
-        self.c = c
-        self.steps = steps
-
-
-@pytest.fixture
-def fixture_metaestimator_instance():
-    return BaseMetaEstimator()
-
-
-@pytest.fixture
-def fixture_meta_object():
-    return MetaObjectTester()
-
-
-@pytest.fixture
-def fixture_meta_estimator():
-    return MetaEstimatorTester()
-
-
-def test_is_composit_returns_true(fixture_meta_object, fixture_meta_estimator):
-    """Test that `is_composite` method returns True."""
-    msg = "`is_composite` should always be True for subclasses of "
-    assert fixture_meta_object.is_composite() is True, msg + "`BaseMetaObject`."
-    assert fixture_meta_estimator.is_composite() is True, msg + "`BaseMetaEstimator`."
-
-
-def test_basemetaestimator_inheritance(fixture_metaestimator_instance):
-    """Check BaseMetaEstimator correctly inherits from BaseEstimator and BaseObject."""
-    estimator_is_subclass_of_baseobejct = issubclass(BaseMetaEstimator, BaseObject)
-    estimator_instance_is_baseobject_instance = isinstance(
-        fixture_metaestimator_instance, BaseObject
-    )
-
-    # Verify that BaseMetaEstimator is an estimator
-    assert (
-        estimator_is_subclass_of_baseobejct
-        and estimator_instance_is_baseobject_instance
-    ), "`BaseMetaEstimator` not correctly subclassing `BaseEstimator` and `BaseObject`."
-
-    # Verify expected MRO inherittence order
-    assert BaseMetaEstimator.__mro__[:-2] == (
-        BaseMetaEstimator,
-        _MetaObjectMixin,
-        _MetaTagLogicMixin,
-        BaseEstimator,
-        BaseObject,
-    ), "`BaseMetaEstimator` has incorrect mro."
-
-
-def test_basemetaestimator_has_is_fitted(fixture_metaestimator_instance):
-    """Test BaseEstimator has `is_fitted` property."""
-    has_private_is_fitted = hasattr(fixture_metaestimator_instance, "_is_fitted")
-    has_is_fitted = hasattr(fixture_metaestimator_instance, "is_fitted")
-    assert (
-        has_private_is_fitted and has_is_fitted
-    ), "`BaseMetaEstimator` does not have `is_fitted` property or `_is_fitted` attr."
-
-
-def test_basemetaestimator_has_check_is_fitted(fixture_metaestimator_instance):
-    """Test BaseEstimator has `check_is_fitted` method."""
-    has_check_is_fitted = hasattr(fixture_metaestimator_instance, "check_is_fitted")
-    is_method = inspect.ismethod(fixture_metaestimator_instance.check_is_fitted)
-    assert (
-        has_check_is_fitted and is_method
-    ), "`BaseMetaEstimator` does not have `check_is_fitted` method."
-
-
-@pytest.mark.parametrize("is_fitted_value", (True, False))
-def test_basemetaestimator_is_fitted(fixture_metaestimator_instance, is_fitted_value):
-    """Test BaseEstimator `is_fitted` property returns expected value."""
-    fixture_metaestimator_instance._is_fitted = is_fitted_value
-    expected_value_unfitted = (
-        fixture_metaestimator_instance.is_fitted
-        == fixture_metaestimator_instance._is_fitted
-    )
-    assert (
-        expected_value_unfitted
-    ), "`BaseMetaEstimator` property `is_fitted` does not return `_is_fitted` value."
-
-
-def test_basemetaestimator_check_is_fitted_raises_error_when_unfitted(
-    fixture_metaestimator_instance,
-):
-    """Test BaseEstimator `check_is_fitted` method raises an error."""
-    name = fixture_metaestimator_instance.__class__.__name__
-    match = f"This instance of {name} has not been fitted yet. Please call `fit` first."
-    with pytest.raises(NotFittedError, match=match):
-        fixture_metaestimator_instance.check_is_fitted()
-
-    fixture_metaestimator_instance._is_fitted = True
-    assert fixture_metaestimator_instance.check_is_fitted() is None
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tests for BaseMetaObject and BaseMetaEstimator mixins.
+
+tests in this module:
+
+
+"""
+
+__author__ = ["RNKuhns"]
+import inspect
+
+import pytest
+
+from skbase._exceptions import NotFittedError
+from skbase.base import BaseEstimator, BaseObject
+from skbase.base._meta import (
+    BaseMetaEstimator,
+    BaseMetaObject,
+    _MetaObjectMixin,
+    _MetaTagLogicMixin,
+)
+
+
+class MetaObjectTester(BaseMetaObject):
+    """Class to test meta object functionality."""
+
+    def __init__(self, a=7, b="something", c=None, steps=None):
+        self.a = a
+        self.b = b
+        self.c = c
+        self.steps = steps
+
+
+class MetaEstimatorTester(BaseMetaEstimator):
+    """Class to test meta estimator functionality."""
+
+    def __init__(self, a=7, b="something", c=None, steps=None):
+        self.a = a
+        self.b = b
+        self.c = c
+        self.steps = steps
+
+
+@pytest.fixture
+def fixture_metaestimator_instance():
+    return BaseMetaEstimator()
+
+
+@pytest.fixture
+def fixture_meta_object():
+    return MetaObjectTester()
+
+
+@pytest.fixture
+def fixture_meta_estimator():
+    return MetaEstimatorTester()
+
+
+def test_is_composit_returns_true(fixture_meta_object, fixture_meta_estimator):
+    """Test that `is_composite` method returns True."""
+    msg = "`is_composite` should always be True for subclasses of "
+    assert fixture_meta_object.is_composite() is True, msg + "`BaseMetaObject`."
+    assert fixture_meta_estimator.is_composite() is True, msg + "`BaseMetaEstimator`."
+
+
+def test_basemetaestimator_inheritance(fixture_metaestimator_instance):
+    """Check BaseMetaEstimator correctly inherits from BaseEstimator and BaseObject."""
+    estimator_is_subclass_of_baseobejct = issubclass(BaseMetaEstimator, BaseObject)
+    estimator_instance_is_baseobject_instance = isinstance(
+        fixture_metaestimator_instance, BaseObject
+    )
+
+    # Verify that BaseMetaEstimator is an estimator
+    assert (
+        estimator_is_subclass_of_baseobejct
+        and estimator_instance_is_baseobject_instance
+    ), "`BaseMetaEstimator` not correctly subclassing `BaseEstimator` and `BaseObject`."
+
+    # Verify expected MRO inherittence order
+    assert BaseMetaEstimator.__mro__[:-2] == (
+        BaseMetaEstimator,
+        _MetaObjectMixin,
+        _MetaTagLogicMixin,
+        BaseEstimator,
+        BaseObject,
+    ), "`BaseMetaEstimator` has incorrect mro."
+
+
+def test_basemetaestimator_has_is_fitted(fixture_metaestimator_instance):
+    """Test BaseEstimator has `is_fitted` property."""
+    has_private_is_fitted = hasattr(fixture_metaestimator_instance, "_is_fitted")
+    has_is_fitted = hasattr(fixture_metaestimator_instance, "is_fitted")
+    assert (
+        has_private_is_fitted and has_is_fitted
+    ), "`BaseMetaEstimator` does not have `is_fitted` property or `_is_fitted` attr."
+
+
+def test_basemetaestimator_has_check_is_fitted(fixture_metaestimator_instance):
+    """Test BaseEstimator has `check_is_fitted` method."""
+    has_check_is_fitted = hasattr(fixture_metaestimator_instance, "check_is_fitted")
+    is_method = inspect.ismethod(fixture_metaestimator_instance.check_is_fitted)
+    assert (
+        has_check_is_fitted and is_method
+    ), "`BaseMetaEstimator` does not have `check_is_fitted` method."
+
+
+@pytest.mark.parametrize("is_fitted_value", (True, False))
+def test_basemetaestimator_is_fitted(fixture_metaestimator_instance, is_fitted_value):
+    """Test BaseEstimator `is_fitted` property returns expected value."""
+    fixture_metaestimator_instance._is_fitted = is_fitted_value
+    expected_value_unfitted = (
+        fixture_metaestimator_instance.is_fitted
+        == fixture_metaestimator_instance._is_fitted
+    )
+    assert (
+        expected_value_unfitted
+    ), "`BaseMetaEstimator` property `is_fitted` does not return `_is_fitted` value."
+
+
+def test_basemetaestimator_check_is_fitted_raises_error_when_unfitted(
+    fixture_metaestimator_instance,
+):
+    """Test BaseEstimator `check_is_fitted` method raises an error."""
+    name = fixture_metaestimator_instance.__class__.__name__
+    match = f"This instance of {name} has not been fitted yet. Please call `fit` first."
+    with pytest.raises(NotFittedError, match=match):
+        fixture_metaestimator_instance.check_is_fitted()
+
+    fixture_metaestimator_instance._is_fitted = True
+    assert fixture_metaestimator_instance.check_is_fitted() is None
```

### Comparing `skbase-0.4.5/skbase/utils/__init__.py` & `skbase-0.4.6/skbase/utils/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Utility functionality used through `skbase`."""
-from typing import List
-
-from skbase.utils._iter import make_strings_unique
-from skbase.utils._nested_iter import flatten, is_flat, unflat_len, unflatten
-from skbase.utils._utils import subset_dict_keys
-from skbase.utils.deep_equals import deep_equals
-
-__author__: List[str] = ["RNKuhns", "fkiraly"]
-__all__: List[str] = [
-    "deep_equals",
-    "flatten",
-    "is_flat",
-    "make_strings_unique",
-    "subset_dict_keys",
-    "unflat_len",
-    "unflatten",
-]
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Utility functionality used through `skbase`."""
+from typing import List
+
+from skbase.utils._iter import make_strings_unique
+from skbase.utils._nested_iter import flatten, is_flat, unflat_len, unflatten
+from skbase.utils._utils import subset_dict_keys
+from skbase.utils.deep_equals import deep_equals
+
+__author__: List[str] = ["RNKuhns", "fkiraly"]
+__all__: List[str] = [
+    "deep_equals",
+    "flatten",
+    "is_flat",
+    "make_strings_unique",
+    "subset_dict_keys",
+    "unflat_len",
+    "unflatten",
+]
```

### Comparing `skbase-0.4.5/skbase/utils/_check.py` & `skbase-0.4.6/skbase/utils/_check.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-# Elements of _is_scalar_nan re-use code developed in scikit-learn. These elements
-# are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
-# conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
-
-"""Utility functions to perform various types of checks."""
-from __future__ import annotations
-
-import math
-import numbers
-from typing import Any
-
-__all__ = ["_is_scalar_nan"]
-__author__ = ["RNKuhns"]
-
-
-def _is_scalar_nan(x: Any) -> bool:
-    """Test if x is NaN.
-
-    This function is meant to overcome the issue that np.isnan does not allow
-    non-numerical types as input, and that np.nan is not float('nan').
-
-    Parameters
-    ----------
-    x : Any
-        The item to be checked to determine if it is a scalar nan value.
-
-    Returns
-    -------
-    bool
-        True if `x` is a scalar nan value
-
-    Notes
-    -----
-    This code follows scikit-learn's implementation.
-
-    Examples
-    --------
-    >>> import numpy as np
-    >>> from skbase.utils._check import _is_scalar_nan
-    >>> _is_scalar_nan(np.nan)
-    True
-    >>> _is_scalar_nan(float("nan"))
-    True
-    >>> _is_scalar_nan(None)
-    False
-    >>> _is_scalar_nan("")
-    False
-    >>> _is_scalar_nan([np.nan])
-    False
-    """
-    return isinstance(x, numbers.Real) and math.isnan(x)
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+# Elements of _is_scalar_nan re-use code developed in scikit-learn. These elements
+# are copyrighted by the scikit-learn developers, BSD-3-Clause License. For
+# conditions see https://github.com/scikit-learn/scikit-learn/blob/main/COPYING
+
+"""Utility functions to perform various types of checks."""
+from __future__ import annotations
+
+import math
+import numbers
+from typing import Any
+
+__all__ = ["_is_scalar_nan"]
+__author__ = ["RNKuhns"]
+
+
+def _is_scalar_nan(x: Any) -> bool:
+    """Test if x is NaN.
+
+    This function is meant to overcome the issue that np.isnan does not allow
+    non-numerical types as input, and that np.nan is not float('nan').
+
+    Parameters
+    ----------
+    x : Any
+        The item to be checked to determine if it is a scalar nan value.
+
+    Returns
+    -------
+    bool
+        True if `x` is a scalar nan value
+
+    Notes
+    -----
+    This code follows scikit-learn's implementation.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from skbase.utils._check import _is_scalar_nan
+    >>> _is_scalar_nan(np.nan)
+    True
+    >>> _is_scalar_nan(float("nan"))
+    True
+    >>> _is_scalar_nan(None)
+    False
+    >>> _is_scalar_nan("")
+    False
+    >>> _is_scalar_nan([np.nan])
+    False
+    """
+    return isinstance(x, numbers.Real) and math.isnan(x)
```

### Comparing `skbase-0.4.5/skbase/utils/_iter.py` & `skbase-0.4.6/skbase/utils/_iter.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,238 +1,238 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Functionality for working with sequences."""
-import collections
-import re
-from collections.abc import Sequence
-from typing import Any, List, Optional, Tuple, Union, overload
-
-from skbase.utils._nested_iter import _remove_single, flatten, is_flat, unflatten
-
-__author__: List[str] = ["RNKuhns"]
-__all__: List[str] = [
-    "_scalar_to_seq",
-    "_remove_type_text",
-    "_format_seq_to_str",
-    "make_strings_unique",
-]
-
-
-def _scalar_to_seq(scalar: Any, sequence_type: type = None) -> Sequence:
-    """Convert a scalar input to a sequence.
-
-    If the input is already a sequence it is returned unchanged. Unlike standard
-    Python, a string is treated as a scalar instead of a sequence.
-
-    Parameters
-    ----------
-    scalar : Any
-        A scalar input to be converted to a sequence.
-    sequence_type : type, default=None
-        A sequence type (e.g., list, tuple) that is used to set the return type. This
-        is ignored if `scalar` is already a sequence other than a str (which is
-        treated like a scalar type for this function instead of sequence of
-        characters).
-
-        - If None, then the returned sequence will be a tuple containing a single
-          scalar element.
-        - If `sequence_type` is a valid sequence type then the returned
-          sequence will be a sequence of that type containing the single scalar
-          value.
-
-    Returns
-    -------
-    Sequence
-        A sequence of the specified `sequence_type` that contains just the single
-        scalar value.
-
-    Examples
-    --------
-    >>> from skbase.utils._iter import _scalar_to_seq
-    >>> _scalar_to_seq(7)
-    (7,)
-    >>> _scalar_to_seq("some_str")
-    ('some_str',)
-    >>> _scalar_to_seq("some_str", sequence_type=list)
-    ['some_str']
-    >>> _scalar_to_seq((1, 2))
-    (1, 2)
-    """
-    # We'll treat str like regular scalar and not a sequence
-    if isinstance(scalar, Sequence) and not isinstance(scalar, str):
-        return scalar
-    elif sequence_type is None:
-        return (scalar,)
-    elif issubclass(sequence_type, Sequence) and sequence_type != Sequence:
-        # Note calling (scalar,) is done to avoid str unpacking
-        return sequence_type((scalar,))  # type: ignore
-    else:
-        raise ValueError(
-            "`sequence_type` must be a subclass of collections.abc.Sequence."
-        )
-
-
-def _remove_type_text(input_):
-    """Remove <class > wrapper from printed type str."""
-    if not isinstance(input_, str):
-        input_ = str(input_)
-
-    m = re.match("^<class '(.*)'>$", input_)
-    if m:
-        return m[1]
-    else:
-        return input_
-
-
-def _format_seq_to_str(
-    seq: Union[str, Sequence],
-    sep: str = ", ",
-    last_sep: Optional[str] = None,
-    remove_type_text: bool = True,
-) -> str:
-    """Format a sequence to a string of delimitted elements.
-
-    This is useful to format sequences into a pretty printing format for
-    creating error messages or warnings.
-
-    Parameters
-    ----------
-    seq : Sequence
-        The input sequence to convert to a str of the elements separated by `sep`.
-    sep : str
-        The separator to use when creating the str output.
-    last_sep : str, default=None
-        The separator to use prior to last element.
-
-        - If None, then `sep` is used. So (7, 9, 11) return "7", "9", "11" for
-          ``sep=", "``.
-        - If last_sep is a str, then it is used prior to last element. So
-          (7, 9, 11) would be "7", "9" and "11" if ``last_sep="and"``.
-
-    remove_type_text : bool, default=True
-        Whether to remove the <class > text wrapping the class type name, when
-        formatting types.
-
-        - If True, then input sequence [list, tuple] returns "list, tuple"
-        - If False, then input sequence [list, tuple] returns
-          "<class 'list'>, <class 'tuple'>".
-
-    Returns
-    -------
-    str
-        The sequence of inputs converted to a string. For example, if `seq`
-        is (7, 9, "cart") and ``last_sep is None`` then the output is
-        "7", "9", "cart".
-
-    Examples
-    --------
-    >>> from skbase.base import BaseEstimator, BaseObject
-    >>> from skbase.utils._iter import _format_seq_to_str
-    >>> seq = [1, 2, 3, 4]
-    >>> _format_seq_to_str(seq)
-    '1, 2, 3, 4'
-    >>> _format_seq_to_str(seq, last_sep="and")
-    '1, 2, 3 and 4'
-    >>> _format_seq_to_str((BaseObject, BaseEstimator))
-    'skbase.base._base.BaseObject, skbase.base._base.BaseEstimator'
-    """
-    if isinstance(seq, str):
-        return seq
-    # Allow casting of scalars to strings
-    elif isinstance(seq, (int, float, bool, type)):
-        return _remove_type_text(seq)
-    elif not isinstance(seq, Sequence):
-        raise TypeError(
-            "`seq` must be a sequence or scalar str, int, float, bool or class."
-        )
-
-    seq_str = [str(e) for e in seq]
-    if remove_type_text:
-        seq_str = [_remove_type_text(s) for s in seq_str]
-
-    if last_sep is None:
-        output_str = sep.join(seq_str)
-    else:
-        if len(seq_str) == 1:
-            output_str = _remove_single(seq_str)
-        else:
-            output_str = sep.join(e for e in seq_str[:-1])
-            output_str = output_str + f" {last_sep} " + seq_str[-1]
-
-    return output_str
-
-
-@overload
-def make_strings_unique(str_list: Tuple[str, ...]) -> Tuple[str, ...]:
-    ...  # pragma: no cover
-
-
-@overload
-def make_strings_unique(str_list: List[str]) -> List[str]:
-    ...  # pragma: no cover
-
-
-def make_strings_unique(
-    str_list: Union[List[str], Tuple[str, ...]]
-) -> Union[List[str], Tuple[str, ...]]:
-    """Make a list or tuple of strings unique by appending number of occurrence.
-
-    Supports making string elements unique for nested list/tuple input.
-
-    Parameters
-    ----------
-    str_list : nested list/tuple structure with string elements
-        The list or tuple with string elements that should be made unique.
-
-    Returns
-    -------
-    list[str] | tuple[str]
-        The input strings coerced to have unique names.
-
-        - If no duplicates then the output list/tuple is same as input.
-        - Otherwise, the integer number of occurrence is appended onto duplicate
-          strings. If this results in duplicates (b/c another string in input had
-          the name of a string and integer of occurrence) this is repeated until
-          no duplicates exist.
-
-    Examples
-    --------
-    >>> from skbase.utils import make_strings_unique
-    >>> some_strs = ["abc", "abc", "bcd"]
-    >>> make_strings_unique(some_strs)
-    ['abc_1', 'abc_2', 'bcd']
-    >>> some_strs = ["abc", "abc", "bcd", "abc_1"]
-    >>> make_strings_unique(some_strs)
-    ['abc_1_1', 'abc_2', 'bcd', 'abc_1_2']
-    """
-    # if strlist is not flat, flatten and apply method, then unflatten
-    if not is_flat(str_list):
-        flat_str_list = flatten(str_list)
-        unique_flat_str_list = make_strings_unique(flat_str_list)
-        unique_strs = unflatten(unique_flat_str_list, str_list)
-        return unique_strs
-
-    # if strlist is a tuple, convert to list, apply this function, then convert back
-    if isinstance(str_list, tuple):
-        unique_strs = make_strings_unique(list(str_list))
-        unique_strs = tuple(unique_strs)
-        return unique_strs
-
-    # now we can assume that strlist is a flat list
-    # if already unique, just return
-    if len(set(str_list)) == len(str_list):
-        return str_list
-
-    str_count = collections.Counter(str_list)
-    # if any duplicates, we append _integer of occurrence to non-uniques
-    now_count: collections.Counter = collections.Counter()
-    unique_strs = str_list
-    for i, x in enumerate(unique_strs):
-        if str_count[x] > 1:
-            now_count.update([x])
-            unique_strs[i] = x + "_" + str(now_count[x])
-
-    # repeat until all are unique
-    #   the algorithm recurses, but will always terminate
-    #   because potential clashes are lexicographically increasing
-    return make_strings_unique(unique_strs)
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Functionality for working with sequences."""
+import collections
+import re
+from collections.abc import Sequence
+from typing import Any, List, Optional, Tuple, Union, overload
+
+from skbase.utils._nested_iter import _remove_single, flatten, is_flat, unflatten
+
+__author__: List[str] = ["RNKuhns"]
+__all__: List[str] = [
+    "_scalar_to_seq",
+    "_remove_type_text",
+    "_format_seq_to_str",
+    "make_strings_unique",
+]
+
+
+def _scalar_to_seq(scalar: Any, sequence_type: type = None) -> Sequence:
+    """Convert a scalar input to a sequence.
+
+    If the input is already a sequence it is returned unchanged. Unlike standard
+    Python, a string is treated as a scalar instead of a sequence.
+
+    Parameters
+    ----------
+    scalar : Any
+        A scalar input to be converted to a sequence.
+    sequence_type : type, default=None
+        A sequence type (e.g., list, tuple) that is used to set the return type. This
+        is ignored if `scalar` is already a sequence other than a str (which is
+        treated like a scalar type for this function instead of sequence of
+        characters).
+
+        - If None, then the returned sequence will be a tuple containing a single
+          scalar element.
+        - If `sequence_type` is a valid sequence type then the returned
+          sequence will be a sequence of that type containing the single scalar
+          value.
+
+    Returns
+    -------
+    Sequence
+        A sequence of the specified `sequence_type` that contains just the single
+        scalar value.
+
+    Examples
+    --------
+    >>> from skbase.utils._iter import _scalar_to_seq
+    >>> _scalar_to_seq(7)
+    (7,)
+    >>> _scalar_to_seq("some_str")
+    ('some_str',)
+    >>> _scalar_to_seq("some_str", sequence_type=list)
+    ['some_str']
+    >>> _scalar_to_seq((1, 2))
+    (1, 2)
+    """
+    # We'll treat str like regular scalar and not a sequence
+    if isinstance(scalar, Sequence) and not isinstance(scalar, str):
+        return scalar
+    elif sequence_type is None:
+        return (scalar,)
+    elif issubclass(sequence_type, Sequence) and sequence_type != Sequence:
+        # Note calling (scalar,) is done to avoid str unpacking
+        return sequence_type((scalar,))  # type: ignore
+    else:
+        raise ValueError(
+            "`sequence_type` must be a subclass of collections.abc.Sequence."
+        )
+
+
+def _remove_type_text(input_):
+    """Remove <class > wrapper from printed type str."""
+    if not isinstance(input_, str):
+        input_ = str(input_)
+
+    m = re.match("^<class '(.*)'>$", input_)
+    if m:
+        return m[1]
+    else:
+        return input_
+
+
+def _format_seq_to_str(
+    seq: Union[str, Sequence],
+    sep: str = ", ",
+    last_sep: Optional[str] = None,
+    remove_type_text: bool = True,
+) -> str:
+    """Format a sequence to a string of delimitted elements.
+
+    This is useful to format sequences into a pretty printing format for
+    creating error messages or warnings.
+
+    Parameters
+    ----------
+    seq : Sequence
+        The input sequence to convert to a str of the elements separated by `sep`.
+    sep : str
+        The separator to use when creating the str output.
+    last_sep : str, default=None
+        The separator to use prior to last element.
+
+        - If None, then `sep` is used. So (7, 9, 11) return "7", "9", "11" for
+          ``sep=", "``.
+        - If last_sep is a str, then it is used prior to last element. So
+          (7, 9, 11) would be "7", "9" and "11" if ``last_sep="and"``.
+
+    remove_type_text : bool, default=True
+        Whether to remove the <class > text wrapping the class type name, when
+        formatting types.
+
+        - If True, then input sequence [list, tuple] returns "list, tuple"
+        - If False, then input sequence [list, tuple] returns
+          "<class 'list'>, <class 'tuple'>".
+
+    Returns
+    -------
+    str
+        The sequence of inputs converted to a string. For example, if `seq`
+        is (7, 9, "cart") and ``last_sep is None`` then the output is
+        "7", "9", "cart".
+
+    Examples
+    --------
+    >>> from skbase.base import BaseEstimator, BaseObject
+    >>> from skbase.utils._iter import _format_seq_to_str
+    >>> seq = [1, 2, 3, 4]
+    >>> _format_seq_to_str(seq)
+    '1, 2, 3, 4'
+    >>> _format_seq_to_str(seq, last_sep="and")
+    '1, 2, 3 and 4'
+    >>> _format_seq_to_str((BaseObject, BaseEstimator))
+    'skbase.base._base.BaseObject, skbase.base._base.BaseEstimator'
+    """
+    if isinstance(seq, str):
+        return seq
+    # Allow casting of scalars to strings
+    elif isinstance(seq, (int, float, bool, type)):
+        return _remove_type_text(seq)
+    elif not isinstance(seq, Sequence):
+        raise TypeError(
+            "`seq` must be a sequence or scalar str, int, float, bool or class."
+        )
+
+    seq_str = [str(e) for e in seq]
+    if remove_type_text:
+        seq_str = [_remove_type_text(s) for s in seq_str]
+
+    if last_sep is None:
+        output_str = sep.join(seq_str)
+    else:
+        if len(seq_str) == 1:
+            output_str = _remove_single(seq_str)
+        else:
+            output_str = sep.join(e for e in seq_str[:-1])
+            output_str = output_str + f" {last_sep} " + seq_str[-1]
+
+    return output_str
+
+
+@overload
+def make_strings_unique(str_list: Tuple[str, ...]) -> Tuple[str, ...]:
+    ...  # pragma: no cover
+
+
+@overload
+def make_strings_unique(str_list: List[str]) -> List[str]:
+    ...  # pragma: no cover
+
+
+def make_strings_unique(
+    str_list: Union[List[str], Tuple[str, ...]]
+) -> Union[List[str], Tuple[str, ...]]:
+    """Make a list or tuple of strings unique by appending number of occurrence.
+
+    Supports making string elements unique for nested list/tuple input.
+
+    Parameters
+    ----------
+    str_list : nested list/tuple structure with string elements
+        The list or tuple with string elements that should be made unique.
+
+    Returns
+    -------
+    list[str] | tuple[str]
+        The input strings coerced to have unique names.
+
+        - If no duplicates then the output list/tuple is same as input.
+        - Otherwise, the integer number of occurrence is appended onto duplicate
+          strings. If this results in duplicates (b/c another string in input had
+          the name of a string and integer of occurrence) this is repeated until
+          no duplicates exist.
+
+    Examples
+    --------
+    >>> from skbase.utils import make_strings_unique
+    >>> some_strs = ["abc", "abc", "bcd"]
+    >>> make_strings_unique(some_strs)
+    ['abc_1', 'abc_2', 'bcd']
+    >>> some_strs = ["abc", "abc", "bcd", "abc_1"]
+    >>> make_strings_unique(some_strs)
+    ['abc_1_1', 'abc_2', 'bcd', 'abc_1_2']
+    """
+    # if strlist is not flat, flatten and apply method, then unflatten
+    if not is_flat(str_list):
+        flat_str_list = flatten(str_list)
+        unique_flat_str_list = make_strings_unique(flat_str_list)
+        unique_strs = unflatten(unique_flat_str_list, str_list)
+        return unique_strs
+
+    # if strlist is a tuple, convert to list, apply this function, then convert back
+    if isinstance(str_list, tuple):
+        unique_strs = make_strings_unique(list(str_list))
+        unique_strs = tuple(unique_strs)
+        return unique_strs
+
+    # now we can assume that strlist is a flat list
+    # if already unique, just return
+    if len(set(str_list)) == len(str_list):
+        return str_list
+
+    str_count = collections.Counter(str_list)
+    # if any duplicates, we append _integer of occurrence to non-uniques
+    now_count: collections.Counter = collections.Counter()
+    unique_strs = str_list
+    for i, x in enumerate(unique_strs):
+        if str_count[x] > 1:
+            now_count.update([x])
+            unique_strs[i] = x + "_" + str(now_count[x])
+
+    # repeat until all are unique
+    #   the algorithm recurses, but will always terminate
+    #   because potential clashes are lexicographically increasing
+    return make_strings_unique(unique_strs)
```

### Comparing `skbase-0.4.5/skbase/utils/_nested_iter.py` & `skbase-0.4.6/skbase/utils/_nested_iter.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Functionality for working with nested sequences."""
-import collections
-from typing import List
-
-__author__: List[str] = ["RNKuhns", "fkiraly"]
-__all__: List[str] = [
-    "flatten",
-    "is_flat",
-    "_remove_single",
-    "unflat_len",
-    "unflatten",
-]
-
-
-def _remove_single(x):
-    """Remove tuple wrapping from singleton.
-
-    If the input has length 1, then the single value is extracted from the input.
-    Otherwise, the input is returned unchanged.
-
-    Parameters
-    ----------
-    x : Sequence
-        The sequence to remove a singleton value from.
-
-    Returns
-    -------
-    Any
-        The singleton value of x if x[0] is a singleton, otherwise x.
-
-    Examples
-    --------
-    >>> from skbase.utils._nested_iter import _remove_single
-    >>> _remove_single([1])
-    1
-    >>> _remove_single([1, 2, 3])
-    [1, 2, 3]
-    """
-    if len(x) == 1:
-        return x[0]
-    else:
-        return x
-
-
-def flatten(obj):
-    """Flatten nested list/tuple structure.
-
-    Converts a nested iterable or sequence to a flat output iterable/sequence
-    with the same and order of elements.
-
-    Parameters
-    ----------
-    obj : Any
-        The object to be flattened from a nested iterable/sequence structure.
-
-    Returns
-    -------
-    Sequence or Iterable
-        flat iterable/sequence, containing non-list/tuple elements in obj in
-        same order as in obj.
-
-    Examples
-    --------
-    >>> from skbase.utils import flatten
-    >>> flatten([1, 2, [3, (4, 5)], 6])
-    [1, 2, 3, 4, 5, 6]
-    """
-    if not isinstance(
-        obj, (collections.abc.Iterable, collections.abc.Sequence)
-    ) or isinstance(obj, str):
-        return [obj]
-    else:
-        return type(obj)([y for x in obj for y in flatten(x)])
-
-
-def unflatten(obj, template):
-    """Invert flattening given given template for nested list/tuple structure.
-
-    Converts an input list or tuple to a nested structure as provided in `template`
-    while preserving the order of elements in the input.
-
-    Parameters
-    ----------
-    obj : list or tuple
-        The object to be unflattened.
-    template : nested list/tuple structure
-        Number of non-list/tuple elements of obj and template must be equal.
-
-    Returns
-    -------
-    list or tuple
-        Input coerced to have elements with nested list/tuples structure exactly
-        as `template` and elements in sequence exactly as `obj`.
-
-    Examples
-    --------
-    >>> from skbase.utils import unflatten
-    >>> unflatten([1, 2, 3, 4, 5, 6], [6, 3, [5, (2, 4)], 1])
-    [1, 2, [3, (4, 5)], 6]
-    """
-    if not isinstance(template, (list, tuple)):
-        return obj[0]
-
-    list_or_tuple = type(template)
-    ls = [unflat_len(x) for x in template]
-    for i in range(1, len(ls)):
-        ls[i] += ls[i - 1]
-    ls = [0] + ls
-
-    res = [unflatten(obj[ls[i] : ls[i + 1]], template[i]) for i in range(len(ls) - 1)]
-
-    return list_or_tuple(res)
-
-
-def unflat_len(obj):
-    """Return number of elements in nested iterable or sequence structure.
-
-    Determines the total number of elements in a nested iterable/sequence structure.
-    Input that is not a iterable or sequence is considered to have length 1.
-
-    Parameters
-    ----------
-    obj : Any
-        Object to determine the unflat length.
-
-    Returns
-    -------
-    int
-        The unflat length of the input.
-
-    Examples
-    --------
-    >>> from skbase.utils import unflat_len
-    >>> unflat_len(7)
-    1
-    >>> unflat_len((1, 2))
-    2
-    >>> unflat_len([1, (2, 3), 4, 5])
-    5
-    """
-    if not isinstance(
-        obj, (collections.abc.Iterable, collections.abc.Sequence)
-    ) or isinstance(obj, str):
-        return 1
-    else:
-        return sum([unflat_len(x) for x in obj])
-
-
-def is_flat(obj):
-    """Check whether iterable or sequence is flat.
-
-    If any elements are iterables or sequences the object is considered to not be flat.
-
-    Parameters
-    ----------
-    obj : Any
-        The object to check to see if it is flat (does not have nested iterable).
-
-    Returns
-    -------
-    bool
-        Whether or not the input `obj` contains nested iterables.
-
-    Examples
-    --------
-    >>> from skbase.utils import is_flat
-    >>> is_flat([1, 2, 3, 4, 5])
-    True
-    >>> is_flat([1, (2, 3), 4, 5])
-    False
-    """
-    elements_flat = (
-        isinstance(x, (collections.abc.Iterable, collections.abc.Sequence))
-        and not isinstance(x, str)
-        for x in obj
-    )
-    return not any(elements_flat)
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Functionality for working with nested sequences."""
+import collections
+from typing import List
+
+__author__: List[str] = ["RNKuhns", "fkiraly"]
+__all__: List[str] = [
+    "flatten",
+    "is_flat",
+    "_remove_single",
+    "unflat_len",
+    "unflatten",
+]
+
+
+def _remove_single(x):
+    """Remove tuple wrapping from singleton.
+
+    If the input has length 1, then the single value is extracted from the input.
+    Otherwise, the input is returned unchanged.
+
+    Parameters
+    ----------
+    x : Sequence
+        The sequence to remove a singleton value from.
+
+    Returns
+    -------
+    Any
+        The singleton value of x if x[0] is a singleton, otherwise x.
+
+    Examples
+    --------
+    >>> from skbase.utils._nested_iter import _remove_single
+    >>> _remove_single([1])
+    1
+    >>> _remove_single([1, 2, 3])
+    [1, 2, 3]
+    """
+    if len(x) == 1:
+        return x[0]
+    else:
+        return x
+
+
+def flatten(obj):
+    """Flatten nested list/tuple structure.
+
+    Converts a nested iterable or sequence to a flat output iterable/sequence
+    with the same and order of elements.
+
+    Parameters
+    ----------
+    obj : Any
+        The object to be flattened from a nested iterable/sequence structure.
+
+    Returns
+    -------
+    Sequence or Iterable
+        flat iterable/sequence, containing non-list/tuple elements in obj in
+        same order as in obj.
+
+    Examples
+    --------
+    >>> from skbase.utils import flatten
+    >>> flatten([1, 2, [3, (4, 5)], 6])
+    [1, 2, 3, 4, 5, 6]
+    """
+    if not isinstance(
+        obj, (collections.abc.Iterable, collections.abc.Sequence)
+    ) or isinstance(obj, str):
+        return [obj]
+    else:
+        return type(obj)([y for x in obj for y in flatten(x)])
+
+
+def unflatten(obj, template):
+    """Invert flattening given given template for nested list/tuple structure.
+
+    Converts an input list or tuple to a nested structure as provided in `template`
+    while preserving the order of elements in the input.
+
+    Parameters
+    ----------
+    obj : list or tuple
+        The object to be unflattened.
+    template : nested list/tuple structure
+        Number of non-list/tuple elements of obj and template must be equal.
+
+    Returns
+    -------
+    list or tuple
+        Input coerced to have elements with nested list/tuples structure exactly
+        as `template` and elements in sequence exactly as `obj`.
+
+    Examples
+    --------
+    >>> from skbase.utils import unflatten
+    >>> unflatten([1, 2, 3, 4, 5, 6], [6, 3, [5, (2, 4)], 1])
+    [1, 2, [3, (4, 5)], 6]
+    """
+    if not isinstance(template, (list, tuple)):
+        return obj[0]
+
+    list_or_tuple = type(template)
+    ls = [unflat_len(x) for x in template]
+    for i in range(1, len(ls)):
+        ls[i] += ls[i - 1]
+    ls = [0] + ls
+
+    res = [unflatten(obj[ls[i] : ls[i + 1]], template[i]) for i in range(len(ls) - 1)]
+
+    return list_or_tuple(res)
+
+
+def unflat_len(obj):
+    """Return number of elements in nested iterable or sequence structure.
+
+    Determines the total number of elements in a nested iterable/sequence structure.
+    Input that is not a iterable or sequence is considered to have length 1.
+
+    Parameters
+    ----------
+    obj : Any
+        Object to determine the unflat length.
+
+    Returns
+    -------
+    int
+        The unflat length of the input.
+
+    Examples
+    --------
+    >>> from skbase.utils import unflat_len
+    >>> unflat_len(7)
+    1
+    >>> unflat_len((1, 2))
+    2
+    >>> unflat_len([1, (2, 3), 4, 5])
+    5
+    """
+    if not isinstance(
+        obj, (collections.abc.Iterable, collections.abc.Sequence)
+    ) or isinstance(obj, str):
+        return 1
+    else:
+        return sum([unflat_len(x) for x in obj])
+
+
+def is_flat(obj):
+    """Check whether iterable or sequence is flat.
+
+    If any elements are iterables or sequences the object is considered to not be flat.
+
+    Parameters
+    ----------
+    obj : Any
+        The object to check to see if it is flat (does not have nested iterable).
+
+    Returns
+    -------
+    bool
+        Whether or not the input `obj` contains nested iterables.
+
+    Examples
+    --------
+    >>> from skbase.utils import is_flat
+    >>> is_flat([1, 2, 3, 4, 5])
+    True
+    >>> is_flat([1, (2, 3), 4, 5])
+    False
+    """
+    elements_flat = (
+        isinstance(x, (collections.abc.Iterable, collections.abc.Sequence))
+        and not isinstance(x, str)
+        for x in obj
+    )
+    return not any(elements_flat)
```

### Comparing `skbase-0.4.5/skbase/utils/deep_equals.py` & `skbase-0.4.6/skbase/utils/deep_equals.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,358 +1,358 @@
-# -*- coding: utf-8 -*-
-"""Testing utility to compare equality in value for nested objects.
-
-Objects compared can have one of the following valid types:
-    types compatible with != comparison
-    pd.Series, pd.DataFrame, np.ndarray
-    lists, tuples, or dicts of a valid type (recursive)
-"""
-from inspect import isclass
-from typing import List
-
-__author__: List[str] = ["fkiraly"]
-__all__: List[str] = ["deep_equals"]
-
-
-# flag variables for available soft dependencies
-# we are not using _check_soft_dependencies in order to keep
-# this utility uncoupled from the dependency on "packaging", of _check_soft_dependencies
-def _softdep_available(importname):
-    from importlib import import_module
-
-    try:
-        import_module(importname)
-    except ModuleNotFoundError:
-        return False
-    else:
-        return True
-
-
-numpy_available = _softdep_available("numpy")
-pandas_available = _softdep_available("pandas")
-
-
-def deep_equals(x, y, return_msg=False):
-    """Test two objects for equality in value.
-
-    Correct if x/y are one of the following valid types:
-        types compatible with != comparison
-        pd.Series, pd.DataFrame, np.ndarray
-        lists, tuples, or dicts of a valid type (recursive)
-
-    Important note:
-        this function will return "not equal" if types of x,y are different
-        for instant, bool and numpy.bool are *not* considered equal
-
-    Parameters
-    ----------
-    x : object
-    y : object
-    return_msg : bool, optional, default=False
-        whether to return informative message about what is not equal
-
-    Returns
-    -------
-    is_equal: bool - True if x and y are equal in value
-        x and y do not need to be equal in reference
-    msg : str, only returned if return_msg = True
-        indication of what is the reason for not being equal
-            concatenation of the following strings:
-            .type - type is not equal
-            .class - both objects are classes but not equal
-            .len - length is not equal
-            .value - value is not equal
-            .keys - if dict, keys of dict are not equal
-                    if class/object, names of attributes and methods are not equal
-            .dtype - dtype of pandas or numpy object is not equal
-            .index - index of pandas object is not equal
-            .series_equals, .df_equals, .index_equals - .equals of pd returns False
-            [i] - if tuple/list: i-th element not equal
-            [key] - if dict: value at key is not equal
-            [colname] - if pandas.DataFrame: column with name colname is not equal
-            != - call to generic != returns False
-    """
-
-    def ret(is_equal, msg):
-        if return_msg:
-            if is_equal:
-                msg = ""
-            return is_equal, msg
-        else:
-            return is_equal
-
-    if type(x) != type(y):
-        return ret(False, f".type, x.type = {type(x)} != y.type = {type(y)}")
-
-    # we now know all types are the same
-    # so now we compare values
-
-    if numpy_available:
-        import numpy as np
-
-    # pandas is a soft dependency, so we compare pandas objects separately
-    #   and only if pandas is installed in the environment
-    if _is_pandas(x) and pandas_available:
-        res = _pandas_equals(x, y, return_msg=return_msg)
-        if res is not None:
-            return _pandas_equals(x, y, return_msg=return_msg)
-
-    if numpy_available and _is_npndarray(x):
-        if x.dtype != y.dtype:
-            return ret(False, f".dtype, x.dtype = {x.dtype} != y.dtype = {y.dtype}")
-        return ret(np.array_equal(x, y, equal_nan=True), ".values")
-    # recursion through lists, tuples and dicts
-    elif isinstance(x, (list, tuple)):
-        return ret(*_tuple_equals(x, y, return_msg=True))
-    elif isinstance(x, dict):
-        return ret(*_dict_equals(x, y, return_msg=True))
-    elif _is_npnan(x):
-        return ret(_is_npnan(y), f"type(x)={type(x)} != type(y)={type(y)}")
-    elif isclass(x):
-        return ret(x == y, f".class, x={x.__name__} != y={y.__name__}")
-    elif type(x).__name__ == "ForecastingHorizon":
-        return ret(*_fh_equals(x, y, return_msg=True))
-    # this elif covers case where != is boolean
-    # some types return a vector upon !=, this is covered in the next elif
-    elif isinstance(x == y, bool):
-        return ret(x == y, f" !=, {x} != {y}")
-    # deal with the case where != returns a vector
-    elif numpy_available and np.any(x != y) or any(_coerce_list(x != y)):
-        return ret(False, f" !=, {x} != {y}")
-
-    return ret(True, "")
-
-
-def _is_pandas(x):
-    clstr = type(x).__name__
-    if clstr in ["DataFrame", "Series"]:
-        return True
-    if clstr.endswith("Index"):
-        return True
-    else:
-        return False
-
-
-def _is_npndarray(x):
-    clstr = type(x).__name__
-    return clstr == "ndarray"
-
-
-def _is_npnan(x):
-    if numpy_available:
-        import numpy as np
-
-        return isinstance(x, float) and np.isnan(x)
-
-    else:
-        return False
-
-
-def _coerce_list(x):
-    """Coerce x to list."""
-    if not isinstance(x, (list, tuple)):
-        x = [x]
-    if isinstance(x, tuple):
-        x = list(x)
-
-    return x
-
-
-def _pandas_equals(x, y, return_msg=False):
-    import pandas as pd
-
-    def ret(is_equal, msg):
-        if return_msg:
-            if is_equal:
-                msg = ""
-            return is_equal, msg
-        else:
-            return is_equal
-
-    if isinstance(x, pd.Series):
-        if x.dtype != y.dtype:
-            return ret(False, f".dtype, x.dtype= {x.dtype} != y.dtype = {y.dtype}")
-        # if columns are object, recurse over entries and index
-        if x.dtype == "object":
-            index_equal = x.index.equals(y.index)
-            values_equal, values_msg = deep_equals(
-                list(x.to_array()), list(y.to_array()), return_msg=True
-            )
-            if not values_equal:
-                msg = ".values" + values_msg
-            elif not index_equal:
-                msg = f".index, x.index: {x.index}, y.index: {y.index}"
-            else:
-                msg = ""
-            return ret(index_equal and values_equal, msg)
-        else:
-            return ret(x.equals(y), f".series_equals, x = {x} != y = {y}")
-    elif isinstance(x, pd.DataFrame):
-        if not x.columns.equals(y.columns):
-            return ret(
-                False, f".columns, x.columns = {x.columns} != y.columns = {y.columns}"
-            )
-        # if columns are equal and at least one is object, recurse over Series
-        if sum(x.dtypes == "object") > 0:
-            for c in x.columns:
-                is_equal, msg = deep_equals(x[c], y[c], return_msg=True)
-                if not is_equal:
-                    return ret(False, f"[{c!r}]" + msg)
-            return ret(True, "")
-        else:
-            return ret(x.equals(y), f".df_equals, x = {x} != y = {y}")
-    elif isinstance(x, pd.Index):
-        return ret(x.equals(y), f".index_equals, x = {x} != y = {y}")
-
-
-def _tuple_equals(x, y, return_msg=False):
-    """Test two tuples or lists for equality.
-
-    Correct if tuples/lists contain the following valid types:
-        types compatible with != comparison
-        pd.Series, pd.DataFrame, np.ndarray
-        lists, tuples, or dicts of a valid type (recursive)
-
-    Parameters
-    ----------
-    x: tuple or list
-    y: tuple or list
-    return_msg : bool, optional, default=False
-        whether to return informative message about what is not equal
-
-    Returns
-    -------
-    is_equal: bool - True if x and y are equal in value
-        x and y do not need to be equal in reference
-    msg : str, only returned if return_msg = True
-        indication of what is the reason for not being equal
-            concatenation of the following elements:
-            .len - length is not equal
-            [i] - i-th element not equal
-    """
-
-    def ret(is_equal, msg):
-        if return_msg:
-            if is_equal:
-                msg = ""
-            return is_equal, msg
-        else:
-            return is_equal
-
-    n = len(x)
-
-    if n != len(y):
-        return ret(False, f".len, x.len = {n} != y.len = {len(y)}")
-
-    # we now know dicts are same length
-    for i in range(n):
-        xi = x[i]
-        yi = y[i]
-
-        # recurse through xi/yi
-        is_equal, msg = deep_equals(xi, yi, return_msg=True)
-        if not is_equal:
-            return ret(False, f"[{i}]" + msg)
-
-    return ret(True, "")
-
-
-def _dict_equals(x, y, return_msg=False):
-    """Test two dicts for equality.
-
-    Correct if dicts contain the following valid types:
-        types compatible with != comparison
-        pd.Series, pd.DataFrame, np.ndarray
-        lists, tuples, or dicts of a valid type (recursive)
-
-    Parameters
-    ----------
-    x: dict
-    y: dict
-    return_msg : bool, optional, default=False
-        whether to return informative message about what is not equal
-
-    Returns
-    -------
-    is_equal: bool - True if x and y are equal in value
-        x and y do not need to be equal in reference
-    msg : str, only returned if return_msg = True
-        indication of what is the reason for not being equal
-            concatenation of the following strings:
-            .keys - keys are not equal
-            [key] - values at key is not equal
-    """
-
-    def ret(is_equal, msg):
-        if return_msg:
-            if is_equal:
-                msg = ""
-            return is_equal, msg
-        else:
-            return is_equal
-
-    xkeys = set(x.keys())
-    ykeys = set(y.keys())
-
-    if xkeys != ykeys:
-        xmy = xkeys.difference(ykeys)
-        ymx = ykeys.difference(xkeys)
-        diffmsg = ".keys,"
-        if len(xmy) > 0:
-            diffmsg += f" x.keys-y.keys = {xmy}."
-        if len(ymx) > 0:
-            diffmsg += f" y.keys-x.keys = {ymx}."
-        return ret(False, diffmsg)
-
-    # we now know that xkeys == ykeys
-    for key in xkeys:
-        xi = x[key]
-        yi = y[key]
-
-        # recurse through xi/yi
-        is_equal, msg = deep_equals(xi, yi, return_msg=True)
-        if not is_equal:
-            return ret(False, f"[{key}]" + msg)
-
-    return ret(True, "")
-
-
-def _fh_equals(x, y, return_msg=False):
-    """Test two forecasting horizons for equality.
-
-    Correct if both x and y are ForecastingHorizon
-
-    Parameters
-    ----------
-    x: ForcastingHorizon
-    y: ForcastingHorizon
-    return_msg : bool, optional, default=False
-        whether to return informative message about what is not equal
-
-    Returns
-    -------
-    is_equal: bool - True if x and y are equal in value
-        x and y do not need to be equal in reference
-    msg : str, only returned if return_msg = True
-        indication of what is the reason for not being equal
-            concatenation of the following strings:
-            .is_relative - x is absolute and y is relative, or vice versa
-            .values - values of x and y are not equal
-    """
-
-    def ret(is_equal, msg):
-        if return_msg:
-            if is_equal:
-                msg = ""
-            return is_equal, msg
-        else:
-            return is_equal
-
-    if x.is_relative != y.is_relative:
-        return ret(False, ".is_relative")
-
-    # recurse through values of x, y
-    is_equal, msg = deep_equals(x._values, y._values, return_msg=True)
-    if not is_equal:
-        return ret(False, ".values" + msg)
-
-    return ret(True, "")
+# -*- coding: utf-8 -*-
+"""Testing utility to compare equality in value for nested objects.
+
+Objects compared can have one of the following valid types:
+    types compatible with != comparison
+    pd.Series, pd.DataFrame, np.ndarray
+    lists, tuples, or dicts of a valid type (recursive)
+"""
+from inspect import isclass
+from typing import List
+
+__author__: List[str] = ["fkiraly"]
+__all__: List[str] = ["deep_equals"]
+
+
+# flag variables for available soft dependencies
+# we are not using _check_soft_dependencies in order to keep
+# this utility uncoupled from the dependency on "packaging", of _check_soft_dependencies
+def _softdep_available(importname):
+    from importlib import import_module
+
+    try:
+        import_module(importname)
+    except ModuleNotFoundError:
+        return False
+    else:
+        return True
+
+
+numpy_available = _softdep_available("numpy")
+pandas_available = _softdep_available("pandas")
+
+
+def deep_equals(x, y, return_msg=False):
+    """Test two objects for equality in value.
+
+    Correct if x/y are one of the following valid types:
+        types compatible with != comparison
+        pd.Series, pd.DataFrame, np.ndarray
+        lists, tuples, or dicts of a valid type (recursive)
+
+    Important note:
+        this function will return "not equal" if types of x,y are different
+        for instant, bool and numpy.bool are *not* considered equal
+
+    Parameters
+    ----------
+    x : object
+    y : object
+    return_msg : bool, optional, default=False
+        whether to return informative message about what is not equal
+
+    Returns
+    -------
+    is_equal: bool - True if x and y are equal in value
+        x and y do not need to be equal in reference
+    msg : str, only returned if return_msg = True
+        indication of what is the reason for not being equal
+            concatenation of the following strings:
+            .type - type is not equal
+            .class - both objects are classes but not equal
+            .len - length is not equal
+            .value - value is not equal
+            .keys - if dict, keys of dict are not equal
+                    if class/object, names of attributes and methods are not equal
+            .dtype - dtype of pandas or numpy object is not equal
+            .index - index of pandas object is not equal
+            .series_equals, .df_equals, .index_equals - .equals of pd returns False
+            [i] - if tuple/list: i-th element not equal
+            [key] - if dict: value at key is not equal
+            [colname] - if pandas.DataFrame: column with name colname is not equal
+            != - call to generic != returns False
+    """
+
+    def ret(is_equal, msg):
+        if return_msg:
+            if is_equal:
+                msg = ""
+            return is_equal, msg
+        else:
+            return is_equal
+
+    if type(x) != type(y):
+        return ret(False, f".type, x.type = {type(x)} != y.type = {type(y)}")
+
+    # we now know all types are the same
+    # so now we compare values
+
+    if numpy_available:
+        import numpy as np
+
+    # pandas is a soft dependency, so we compare pandas objects separately
+    #   and only if pandas is installed in the environment
+    if _is_pandas(x) and pandas_available:
+        res = _pandas_equals(x, y, return_msg=return_msg)
+        if res is not None:
+            return _pandas_equals(x, y, return_msg=return_msg)
+
+    if numpy_available and _is_npndarray(x):
+        if x.dtype != y.dtype:
+            return ret(False, f".dtype, x.dtype = {x.dtype} != y.dtype = {y.dtype}")
+        return ret(np.array_equal(x, y, equal_nan=True), ".values")
+    # recursion through lists, tuples and dicts
+    elif isinstance(x, (list, tuple)):
+        return ret(*_tuple_equals(x, y, return_msg=True))
+    elif isinstance(x, dict):
+        return ret(*_dict_equals(x, y, return_msg=True))
+    elif _is_npnan(x):
+        return ret(_is_npnan(y), f"type(x)={type(x)} != type(y)={type(y)}")
+    elif isclass(x):
+        return ret(x == y, f".class, x={x.__name__} != y={y.__name__}")
+    elif type(x).__name__ == "ForecastingHorizon":
+        return ret(*_fh_equals(x, y, return_msg=True))
+    # this elif covers case where != is boolean
+    # some types return a vector upon !=, this is covered in the next elif
+    elif isinstance(x == y, bool):
+        return ret(x == y, f" !=, {x} != {y}")
+    # deal with the case where != returns a vector
+    elif numpy_available and np.any(x != y) or any(_coerce_list(x != y)):
+        return ret(False, f" !=, {x} != {y}")
+
+    return ret(True, "")
+
+
+def _is_pandas(x):
+    clstr = type(x).__name__
+    if clstr in ["DataFrame", "Series"]:
+        return True
+    if clstr.endswith("Index"):
+        return True
+    else:
+        return False
+
+
+def _is_npndarray(x):
+    clstr = type(x).__name__
+    return clstr == "ndarray"
+
+
+def _is_npnan(x):
+    if numpy_available:
+        import numpy as np
+
+        return isinstance(x, float) and np.isnan(x)
+
+    else:
+        return False
+
+
+def _coerce_list(x):
+    """Coerce x to list."""
+    if not isinstance(x, (list, tuple)):
+        x = [x]
+    if isinstance(x, tuple):
+        x = list(x)
+
+    return x
+
+
+def _pandas_equals(x, y, return_msg=False):
+    import pandas as pd
+
+    def ret(is_equal, msg):
+        if return_msg:
+            if is_equal:
+                msg = ""
+            return is_equal, msg
+        else:
+            return is_equal
+
+    if isinstance(x, pd.Series):
+        if x.dtype != y.dtype:
+            return ret(False, f".dtype, x.dtype= {x.dtype} != y.dtype = {y.dtype}")
+        # if columns are object, recurse over entries and index
+        if x.dtype == "object":
+            index_equal = x.index.equals(y.index)
+            values_equal, values_msg = deep_equals(
+                list(x.to_array()), list(y.to_array()), return_msg=True
+            )
+            if not values_equal:
+                msg = ".values" + values_msg
+            elif not index_equal:
+                msg = f".index, x.index: {x.index}, y.index: {y.index}"
+            else:
+                msg = ""
+            return ret(index_equal and values_equal, msg)
+        else:
+            return ret(x.equals(y), f".series_equals, x = {x} != y = {y}")
+    elif isinstance(x, pd.DataFrame):
+        if not x.columns.equals(y.columns):
+            return ret(
+                False, f".columns, x.columns = {x.columns} != y.columns = {y.columns}"
+            )
+        # if columns are equal and at least one is object, recurse over Series
+        if sum(x.dtypes == "object") > 0:
+            for c in x.columns:
+                is_equal, msg = deep_equals(x[c], y[c], return_msg=True)
+                if not is_equal:
+                    return ret(False, f"[{c!r}]" + msg)
+            return ret(True, "")
+        else:
+            return ret(x.equals(y), f".df_equals, x = {x} != y = {y}")
+    elif isinstance(x, pd.Index):
+        return ret(x.equals(y), f".index_equals, x = {x} != y = {y}")
+
+
+def _tuple_equals(x, y, return_msg=False):
+    """Test two tuples or lists for equality.
+
+    Correct if tuples/lists contain the following valid types:
+        types compatible with != comparison
+        pd.Series, pd.DataFrame, np.ndarray
+        lists, tuples, or dicts of a valid type (recursive)
+
+    Parameters
+    ----------
+    x: tuple or list
+    y: tuple or list
+    return_msg : bool, optional, default=False
+        whether to return informative message about what is not equal
+
+    Returns
+    -------
+    is_equal: bool - True if x and y are equal in value
+        x and y do not need to be equal in reference
+    msg : str, only returned if return_msg = True
+        indication of what is the reason for not being equal
+            concatenation of the following elements:
+            .len - length is not equal
+            [i] - i-th element not equal
+    """
+
+    def ret(is_equal, msg):
+        if return_msg:
+            if is_equal:
+                msg = ""
+            return is_equal, msg
+        else:
+            return is_equal
+
+    n = len(x)
+
+    if n != len(y):
+        return ret(False, f".len, x.len = {n} != y.len = {len(y)}")
+
+    # we now know dicts are same length
+    for i in range(n):
+        xi = x[i]
+        yi = y[i]
+
+        # recurse through xi/yi
+        is_equal, msg = deep_equals(xi, yi, return_msg=True)
+        if not is_equal:
+            return ret(False, f"[{i}]" + msg)
+
+    return ret(True, "")
+
+
+def _dict_equals(x, y, return_msg=False):
+    """Test two dicts for equality.
+
+    Correct if dicts contain the following valid types:
+        types compatible with != comparison
+        pd.Series, pd.DataFrame, np.ndarray
+        lists, tuples, or dicts of a valid type (recursive)
+
+    Parameters
+    ----------
+    x: dict
+    y: dict
+    return_msg : bool, optional, default=False
+        whether to return informative message about what is not equal
+
+    Returns
+    -------
+    is_equal: bool - True if x and y are equal in value
+        x and y do not need to be equal in reference
+    msg : str, only returned if return_msg = True
+        indication of what is the reason for not being equal
+            concatenation of the following strings:
+            .keys - keys are not equal
+            [key] - values at key is not equal
+    """
+
+    def ret(is_equal, msg):
+        if return_msg:
+            if is_equal:
+                msg = ""
+            return is_equal, msg
+        else:
+            return is_equal
+
+    xkeys = set(x.keys())
+    ykeys = set(y.keys())
+
+    if xkeys != ykeys:
+        xmy = xkeys.difference(ykeys)
+        ymx = ykeys.difference(xkeys)
+        diffmsg = ".keys,"
+        if len(xmy) > 0:
+            diffmsg += f" x.keys-y.keys = {xmy}."
+        if len(ymx) > 0:
+            diffmsg += f" y.keys-x.keys = {ymx}."
+        return ret(False, diffmsg)
+
+    # we now know that xkeys == ykeys
+    for key in xkeys:
+        xi = x[key]
+        yi = y[key]
+
+        # recurse through xi/yi
+        is_equal, msg = deep_equals(xi, yi, return_msg=True)
+        if not is_equal:
+            return ret(False, f"[{key}]" + msg)
+
+    return ret(True, "")
+
+
+def _fh_equals(x, y, return_msg=False):
+    """Test two forecasting horizons for equality.
+
+    Correct if both x and y are ForecastingHorizon
+
+    Parameters
+    ----------
+    x: ForcastingHorizon
+    y: ForcastingHorizon
+    return_msg : bool, optional, default=False
+        whether to return informative message about what is not equal
+
+    Returns
+    -------
+    is_equal: bool - True if x and y are equal in value
+        x and y do not need to be equal in reference
+    msg : str, only returned if return_msg = True
+        indication of what is the reason for not being equal
+            concatenation of the following strings:
+            .is_relative - x is absolute and y is relative, or vice versa
+            .values - values of x and y are not equal
+    """
+
+    def ret(is_equal, msg):
+        if return_msg:
+            if is_equal:
+                msg = ""
+            return is_equal, msg
+        else:
+            return is_equal
+
+    if x.is_relative != y.is_relative:
+        return ret(False, ".is_relative")
+
+    # recurse through values of x, y
+    is_equal, msg = deep_equals(x._values, y._values, return_msg=True)
+    if not is_equal:
+        return ret(False, ".values" + msg)
+
+    return ret(True, "")
```

### Comparing `skbase-0.4.5/skbase/utils/dependencies/_dependencies.py` & `skbase-0.4.6/skbase/utils/dependencies/_dependencies.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,253 +1,253 @@
-# -*- coding: utf-8 -*-
-"""Utility to check soft dependency imports, and raise warnings or errors."""
-import io
-import sys
-import warnings
-from importlib import import_module
-from inspect import isclass
-from typing import List
-
-from packaging.requirements import InvalidRequirement, Requirement
-from packaging.specifiers import InvalidSpecifier, SpecifierSet
-
-__author__: List[str] = ["fkiraly", "mloning"]
-
-
-def _check_soft_dependencies(
-    *packages,
-    package_import_alias=None,
-    severity="error",
-    obj=None,
-    suppress_import_stdout=False,
-):
-    """Check if required soft dependencies are installed and raise error or warning.
-
-    Parameters
-    ----------
-    packages : str or list/tuple of str, or length-1-tuple containing list/tuple of str
-        str should be package names and/or package version specifications to check.
-        Each str must be a PEP 440 compatibe specifier string, for a single package.
-        For instance, the PEP 440 compatible package name such as "pandas";
-        or a package requirement specifier string such as "pandas>1.2.3".
-        arg can be str, kwargs tuple, or tuple/list of str, following calls are valid:
-        `_check_soft_dependencies("package1")`
-        `_check_soft_dependencies("package1", "package2")`
-        `_check_soft_dependencies(("package1", "package2"))`
-        `_check_soft_dependencies(["package1", "package2"])`
-    package_import_alias : dict with str keys and values, optional, default=empty
-        key-value pairs are package name, import name
-        import name is str used in python import, i.e., from import_name import ...
-        should be provided if import name differs from package name
-    severity : str, "error" (default), "warning", "none"
-        behaviour for raising errors or warnings
-        "error" - raises a `ModuleNotFoundException` if one of packages is not installed
-        "warning" - raises a warning if one of packages is not installed
-            function returns False if one of packages is not installed, otherwise True
-        "none" - does not raise exception or warning
-            function returns False if one of packages is not installed, otherwise True
-    obj : python class, object, str, or None, default=None
-        if self is passed here when _check_soft_dependencies is called within __init__,
-        or a class is passed when it is called at the start of a single-class module,
-        the error message is more informative and will refer to the class/object;
-        if str is passed, will be used as name of the class/object or module
-    suppress_import_stdout : bool, optional. Default=False
-        whether to suppress stdout printout upon import.
-
-    Raises
-    ------
-    ModuleNotFoundError
-        error with informative message, asking to install required soft dependencies
-
-    Returns
-    -------
-    boolean - whether all packages are installed, only if no exception is raised
-    """
-    if len(packages) == 1 and isinstance(packages[0], (tuple, list)):
-        packages = packages[0]
-    if not all(isinstance(x, str) for x in packages):
-        raise TypeError("packages must be str or tuple of str")
-
-    if package_import_alias is None:
-        package_import_alias = {}
-    msg = "package_import_alias must be a dict with str keys and values"
-    if not isinstance(package_import_alias, dict):
-        raise TypeError(msg)
-    if not all(isinstance(x, str) for x in package_import_alias.keys()):
-        raise TypeError(msg)
-    if not all(isinstance(x, str) for x in package_import_alias.values()):
-        raise TypeError(msg)
-
-    if obj is None:
-        class_name = "This functionality"
-    elif not isclass(obj):
-        class_name = type(obj).__name__
-    elif isclass(obj):
-        class_name = obj.__name__
-    elif isinstance(obj, str):
-        class_name = obj
-    else:
-        raise TypeError("obj must be a class, an object, a str, or None")
-
-    for package in packages:
-        try:
-            req = Requirement(package)
-        except InvalidRequirement:
-            msg_version = (
-                f"wrong format for package requirement string, "
-                f'must be PEP 440 compatible requirement string, e.g., "pandas"'
-                f' or "pandas>1.1", but found {package!r}'
-            )
-            raise InvalidRequirement(msg_version) from None
-
-        package_name = req.name
-        package_version_req = req.specifier
-
-        # determine the package import
-        if package_name in package_import_alias.keys():
-            package_import_name = package_import_alias[package_name]
-        else:
-            package_import_name = package_name
-        # attempt import - if not possible, we know we need to raise warning/exception
-        try:
-            if suppress_import_stdout:
-                # setup text trap, import, then restore
-                sys.stdout = io.StringIO()
-                pkg_ref = import_module(package_import_name)
-                sys.stdout = sys.__stdout__
-            else:
-                pkg_ref = import_module(package_import_name)
-        # if package cannot be imported, make the user aware of installation requirement
-        except ModuleNotFoundError as e:
-            msg = (
-                f"{e}. "
-                f"{class_name} requires package {package!r} to be present "
-                f"in the python environment, but {package!r} was not found. "
-            )
-            if obj is not None:
-                msg = msg + (
-                    f"{package!r} is a dependency of {class_name} and required "
-                    f"to construct it. "
-                )
-            msg = msg + (
-                f"Please run: `pip install {package}` to "
-                f"install the {package} package. "
-            )
-
-            if severity == "error":
-                raise ModuleNotFoundError(msg) from e
-            elif severity == "warning":
-                warnings.warn(msg, stacklevel=2)
-                return False
-            elif severity == "none":
-                return False
-            else:
-                raise RuntimeError(
-                    "Error in calling _check_soft_dependencies, severity "
-                    'argument must be "error", "warning", or "none",'
-                    f"found {severity!r}."
-                ) from e
-
-        # now we check compatibility with the version specifier if non-empty
-        if package_version_req != SpecifierSet(""):
-            pkg_env_version = pkg_ref.__version__
-
-            msg = (
-                f"{class_name} requires package {package!r} to be present "
-                f"in the python environment, with version {package_version_req}, "
-                f"but incompatible version {pkg_env_version} was found. "
-            )
-            if obj is not None:
-                msg = msg + (
-                    f"{package!r}, with version {package_version_req},"
-                    f"is a dependency of {class_name} and required to construct it. "
-                )
-
-            # raise error/warning or return False if version is incompatible
-            if pkg_env_version not in package_version_req:
-                if severity == "error":
-                    raise ModuleNotFoundError(msg)
-                elif severity == "warning":
-                    warnings.warn(msg, stacklevel=2)
-                elif severity == "none":
-                    return False
-                else:
-                    raise RuntimeError(
-                        "Error in calling _check_soft_dependencies, severity argument"
-                        f' must be "error", "warning", or "none", found {severity!r}.'
-                    )
-
-    # if package can be imported and no version issue was caught for any string,
-    # then obj is compatible with the requirements and we should return True
-    return True
-
-
-def _check_python_version(obj, package=None, msg=None, severity="error"):
-    """Check if system python version is compatible with requirements of obj.
-
-    Parameters
-    ----------
-    obj : BaseObject descendant
-        used to check python version
-    package : str, default = None
-        if given, will be used in error message as package name
-    msg : str, optional, default = default message (msg below)
-        error message to be returned in the `ModuleNotFoundError`, overrides default
-    severity : str, "error" (default), "warning", or "none"
-        whether the check should raise an error, a warning, or nothing
-
-    Returns
-    -------
-    compatible : bool, whether obj is compatible with system python version
-        check is using the python_version tag of obj
-
-    Raises
-    ------
-    ModuleNotFoundError
-        User friendly error if obj has python_version tag that is
-        incompatible with the system python version. If package is given,
-        error message gives package as the reason for incompatibility.
-    """
-    est_specifier_tag = obj.get_class_tag("python_version", tag_value_default="None")
-    if est_specifier_tag in ["None", None]:
-        return True
-
-    try:
-        est_specifier = SpecifierSet(est_specifier_tag)
-    except InvalidSpecifier:
-        msg_version = (
-            f"wrong format for python_version tag, "
-            f'must be PEP 440 compatible specifier string, e.g., "<3.9, >= 3.6.3",'
-            f" but found {est_specifier_tag!r}"
-        )
-        raise InvalidSpecifier(msg_version) from None
-
-    # python sys version, e.g., "3.8.12"
-    sys_version = sys.version.split(" ")[0]
-
-    if sys_version in est_specifier:
-        return True
-    # now we know that est_version is not compatible with sys_version
-
-    if not isinstance(msg, str):
-        msg = (
-            f"{type(obj).__name__} requires python version to be {est_specifier},"
-            f" but system python version is {sys.version}."
-        )
-
-        if package is not None:
-            msg += (
-                f" This is due to python version requirements of the {package} package."
-            )
-
-    if severity == "error":
-        raise ModuleNotFoundError(msg)
-    elif severity == "warning":
-        warnings.warn(msg, stacklevel=2)
-    elif severity == "none":
-        return False
-    else:
-        raise RuntimeError(
-            "Error in calling _check_python_version, severity "
-            f'argument must be "error", "warning", or "none", found {severity!r}.'
-        )
-    return True
+# -*- coding: utf-8 -*-
+"""Utility to check soft dependency imports, and raise warnings or errors."""
+import io
+import sys
+import warnings
+from importlib import import_module
+from inspect import isclass
+from typing import List
+
+from packaging.requirements import InvalidRequirement, Requirement
+from packaging.specifiers import InvalidSpecifier, SpecifierSet
+
+__author__: List[str] = ["fkiraly", "mloning"]
+
+
+def _check_soft_dependencies(
+    *packages,
+    package_import_alias=None,
+    severity="error",
+    obj=None,
+    suppress_import_stdout=False,
+):
+    """Check if required soft dependencies are installed and raise error or warning.
+
+    Parameters
+    ----------
+    packages : str or list/tuple of str, or length-1-tuple containing list/tuple of str
+        str should be package names and/or package version specifications to check.
+        Each str must be a PEP 440 compatibe specifier string, for a single package.
+        For instance, the PEP 440 compatible package name such as "pandas";
+        or a package requirement specifier string such as "pandas>1.2.3".
+        arg can be str, kwargs tuple, or tuple/list of str, following calls are valid:
+        `_check_soft_dependencies("package1")`
+        `_check_soft_dependencies("package1", "package2")`
+        `_check_soft_dependencies(("package1", "package2"))`
+        `_check_soft_dependencies(["package1", "package2"])`
+    package_import_alias : dict with str keys and values, optional, default=empty
+        key-value pairs are package name, import name
+        import name is str used in python import, i.e., from import_name import ...
+        should be provided if import name differs from package name
+    severity : str, "error" (default), "warning", "none"
+        behaviour for raising errors or warnings
+        "error" - raises a `ModuleNotFoundException` if one of packages is not installed
+        "warning" - raises a warning if one of packages is not installed
+            function returns False if one of packages is not installed, otherwise True
+        "none" - does not raise exception or warning
+            function returns False if one of packages is not installed, otherwise True
+    obj : python class, object, str, or None, default=None
+        if self is passed here when _check_soft_dependencies is called within __init__,
+        or a class is passed when it is called at the start of a single-class module,
+        the error message is more informative and will refer to the class/object;
+        if str is passed, will be used as name of the class/object or module
+    suppress_import_stdout : bool, optional. Default=False
+        whether to suppress stdout printout upon import.
+
+    Raises
+    ------
+    ModuleNotFoundError
+        error with informative message, asking to install required soft dependencies
+
+    Returns
+    -------
+    boolean - whether all packages are installed, only if no exception is raised
+    """
+    if len(packages) == 1 and isinstance(packages[0], (tuple, list)):
+        packages = packages[0]
+    if not all(isinstance(x, str) for x in packages):
+        raise TypeError("packages must be str or tuple of str")
+
+    if package_import_alias is None:
+        package_import_alias = {}
+    msg = "package_import_alias must be a dict with str keys and values"
+    if not isinstance(package_import_alias, dict):
+        raise TypeError(msg)
+    if not all(isinstance(x, str) for x in package_import_alias.keys()):
+        raise TypeError(msg)
+    if not all(isinstance(x, str) for x in package_import_alias.values()):
+        raise TypeError(msg)
+
+    if obj is None:
+        class_name = "This functionality"
+    elif not isclass(obj):
+        class_name = type(obj).__name__
+    elif isclass(obj):
+        class_name = obj.__name__
+    elif isinstance(obj, str):
+        class_name = obj
+    else:
+        raise TypeError("obj must be a class, an object, a str, or None")
+
+    for package in packages:
+        try:
+            req = Requirement(package)
+        except InvalidRequirement:
+            msg_version = (
+                f"wrong format for package requirement string, "
+                f'must be PEP 440 compatible requirement string, e.g., "pandas"'
+                f' or "pandas>1.1", but found {package!r}'
+            )
+            raise InvalidRequirement(msg_version) from None
+
+        package_name = req.name
+        package_version_req = req.specifier
+
+        # determine the package import
+        if package_name in package_import_alias.keys():
+            package_import_name = package_import_alias[package_name]
+        else:
+            package_import_name = package_name
+        # attempt import - if not possible, we know we need to raise warning/exception
+        try:
+            if suppress_import_stdout:
+                # setup text trap, import, then restore
+                sys.stdout = io.StringIO()
+                pkg_ref = import_module(package_import_name)
+                sys.stdout = sys.__stdout__
+            else:
+                pkg_ref = import_module(package_import_name)
+        # if package cannot be imported, make the user aware of installation requirement
+        except ModuleNotFoundError as e:
+            msg = (
+                f"{e}. "
+                f"{class_name} requires package {package!r} to be present "
+                f"in the python environment, but {package!r} was not found. "
+            )
+            if obj is not None:
+                msg = msg + (
+                    f"{package!r} is a dependency of {class_name} and required "
+                    f"to construct it. "
+                )
+            msg = msg + (
+                f"Please run: `pip install {package}` to "
+                f"install the {package} package. "
+            )
+
+            if severity == "error":
+                raise ModuleNotFoundError(msg) from e
+            elif severity == "warning":
+                warnings.warn(msg, stacklevel=2)
+                return False
+            elif severity == "none":
+                return False
+            else:
+                raise RuntimeError(
+                    "Error in calling _check_soft_dependencies, severity "
+                    'argument must be "error", "warning", or "none",'
+                    f"found {severity!r}."
+                ) from e
+
+        # now we check compatibility with the version specifier if non-empty
+        if package_version_req != SpecifierSet(""):
+            pkg_env_version = pkg_ref.__version__
+
+            msg = (
+                f"{class_name} requires package {package!r} to be present "
+                f"in the python environment, with version {package_version_req}, "
+                f"but incompatible version {pkg_env_version} was found. "
+            )
+            if obj is not None:
+                msg = msg + (
+                    f"{package!r}, with version {package_version_req},"
+                    f"is a dependency of {class_name} and required to construct it. "
+                )
+
+            # raise error/warning or return False if version is incompatible
+            if pkg_env_version not in package_version_req:
+                if severity == "error":
+                    raise ModuleNotFoundError(msg)
+                elif severity == "warning":
+                    warnings.warn(msg, stacklevel=2)
+                elif severity == "none":
+                    return False
+                else:
+                    raise RuntimeError(
+                        "Error in calling _check_soft_dependencies, severity argument"
+                        f' must be "error", "warning", or "none", found {severity!r}.'
+                    )
+
+    # if package can be imported and no version issue was caught for any string,
+    # then obj is compatible with the requirements and we should return True
+    return True
+
+
+def _check_python_version(obj, package=None, msg=None, severity="error"):
+    """Check if system python version is compatible with requirements of obj.
+
+    Parameters
+    ----------
+    obj : BaseObject descendant
+        used to check python version
+    package : str, default = None
+        if given, will be used in error message as package name
+    msg : str, optional, default = default message (msg below)
+        error message to be returned in the `ModuleNotFoundError`, overrides default
+    severity : str, "error" (default), "warning", or "none"
+        whether the check should raise an error, a warning, or nothing
+
+    Returns
+    -------
+    compatible : bool, whether obj is compatible with system python version
+        check is using the python_version tag of obj
+
+    Raises
+    ------
+    ModuleNotFoundError
+        User friendly error if obj has python_version tag that is
+        incompatible with the system python version. If package is given,
+        error message gives package as the reason for incompatibility.
+    """
+    est_specifier_tag = obj.get_class_tag("python_version", tag_value_default="None")
+    if est_specifier_tag in ["None", None]:
+        return True
+
+    try:
+        est_specifier = SpecifierSet(est_specifier_tag)
+    except InvalidSpecifier:
+        msg_version = (
+            f"wrong format for python_version tag, "
+            f'must be PEP 440 compatible specifier string, e.g., "<3.9, >= 3.6.3",'
+            f" but found {est_specifier_tag!r}"
+        )
+        raise InvalidSpecifier(msg_version) from None
+
+    # python sys version, e.g., "3.8.12"
+    sys_version = sys.version.split(" ")[0]
+
+    if sys_version in est_specifier:
+        return True
+    # now we know that est_version is not compatible with sys_version
+
+    if not isinstance(msg, str):
+        msg = (
+            f"{type(obj).__name__} requires python version to be {est_specifier},"
+            f" but system python version is {sys.version}."
+        )
+
+        if package is not None:
+            msg += (
+                f" This is due to python version requirements of the {package} package."
+            )
+
+    if severity == "error":
+        raise ModuleNotFoundError(msg)
+    elif severity == "warning":
+        warnings.warn(msg, stacklevel=2)
+    elif severity == "none":
+        return False
+    else:
+        raise RuntimeError(
+            "Error in calling _check_python_version, severity "
+            f'argument must be "error", "warning", or "none", found {severity!r}.'
+        )
+    return True
```

### Comparing `skbase-0.4.5/skbase/utils/tests/test_check.py` & `skbase-0.4.6/skbase/utils/tests/test_check.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tests of the utility functionality for performing various checks.
-
-tests in this module include:
-
-- test_is_scalar_nan_output to verify _is_scalar_nan outputs expected value for
-  different inputs.
-"""
-import numpy as np
-
-from skbase.utils._check import _is_scalar_nan
-
-__author__ = ["RNKuhns"]
-
-
-def test_is_scalar_nan_output():
-    """Test that _is_scalar_nan outputs expected value for different inputs."""
-    assert _is_scalar_nan(np.nan) is True
-    assert _is_scalar_nan(float("nan")) is True
-    assert _is_scalar_nan(None) is False
-    assert _is_scalar_nan("") is False
-    assert _is_scalar_nan([np.nan]) is False
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tests of the utility functionality for performing various checks.
+
+tests in this module include:
+
+- test_is_scalar_nan_output to verify _is_scalar_nan outputs expected value for
+  different inputs.
+"""
+import numpy as np
+
+from skbase.utils._check import _is_scalar_nan
+
+__author__ = ["RNKuhns"]
+
+
+def test_is_scalar_nan_output():
+    """Test that _is_scalar_nan outputs expected value for different inputs."""
+    assert _is_scalar_nan(np.nan) is True
+    assert _is_scalar_nan(float("nan")) is True
+    assert _is_scalar_nan(None) is False
+    assert _is_scalar_nan("") is False
+    assert _is_scalar_nan([np.nan]) is False
```

### Comparing `skbase-0.4.5/skbase/utils/tests/test_iter.py` & `skbase-0.4.6/skbase/utils/tests/test_iter.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tests of the functionality for working with iterables.
-
-tests in this module incdlue:
-
-- test_format_seq_to_str: verify that _format_seq_to_str outputs expected format.
-- test_format_seq_to_str_raises: verify _format_seq_to_str raises error on unexpected
-  output.
-- test_scalar_to_seq_expected_output: verify that _scalar_to_seq returns exepcted
-  output.
-- test_scalar_to_seq_raises: verify that _scalar_to_seq raises error when an
-  invalid value is provided for sequence_type parameter.
-- test_make_strings_unique_output: verify make_strings_unique output is expected.
-"""
-import pytest
-
-from skbase.base import BaseEstimator, BaseObject
-from skbase.utils._iter import _format_seq_to_str, _scalar_to_seq, make_strings_unique
-
-__author__ = ["RNKuhns"]
-
-
-def test_format_seq_to_str():
-    """Test _format_seq_to_str returns expected output."""
-    # Test basic functionality (including ability to handle str and non-str)
-    seq = [1, 2, "3", 4]
-    assert _format_seq_to_str(seq) == "1, 2, 3, 4"
-
-    # Test use of last_sep
-    assert _format_seq_to_str(seq, last_sep="and") == "1, 2, 3 and 4"
-    assert _format_seq_to_str(seq, last_sep="or") == "1, 2, 3 or 4"
-
-    # Test use of different sep argument
-    assert _format_seq_to_str(seq, sep=";") == "1;2;3;4"
-
-    # Verify things work with BaseObject and BaseEstimator instances
-    seq = [BaseEstimator(), BaseObject(), 1]
-    assert _format_seq_to_str(seq) == "BaseEstimator(), BaseObject(), 1"
-
-    # Test use of last_sep
-    assert (
-        _format_seq_to_str(seq, last_sep="and") == "BaseEstimator(), BaseObject() and 1"
-    )
-    assert (
-        _format_seq_to_str(seq, last_sep="or") == "BaseEstimator(), BaseObject() or 1"
-    )
-
-    # Test use of different sep argument
-    assert _format_seq_to_str(seq, sep=";") == "BaseEstimator();BaseObject();1"
-
-    # Test using remove_type_text keyword
-    assert (
-        _format_seq_to_str([list, tuple], remove_type_text=False)
-        == "<class 'list'>, <class 'tuple'>"
-    )
-    assert _format_seq_to_str([list, tuple], remove_type_text=True) == "list, tuple"
-    assert (
-        _format_seq_to_str([list, tuple], last_sep="and", remove_type_text=True)
-        == "list and tuple"
-    )
-
-    # Test with scalar inputs
-    assert _format_seq_to_str(7) == "7"  # int, float, bool primitives cast to str
-    assert _format_seq_to_str("some_str") == "some_str"
-    # Verify that keywords don't affect output
-    assert _format_seq_to_str(7, sep=";") == "7"
-    assert _format_seq_to_str(7, last_sep="or") == "7"
-    # Verify with types
-    assert _format_seq_to_str(object) == "object"
-    assert _format_seq_to_str(int) == "int"
-
-
-def test_format_seq_to_str_raises():
-    """Test _format_seq_to_str raises error when input is unexpected type."""
-    with pytest.raises(TypeError, match="`seq` must be a sequence or scalar.*"):
-        _format_seq_to_str((c for c in [1, 2, 3]))
-
-
-def test_scalar_to_seq_expected_output():
-    """Test _scalar_to_seq returns expected output."""
-    assert _scalar_to_seq(7) == (7,)
-    # Verify it works with scalar classes and objects
-    assert _scalar_to_seq(BaseObject) == (BaseObject,)
-    assert _scalar_to_seq(BaseObject()) == (BaseObject(),)
-    # Verify strings treated like scalar not sequence
-    assert _scalar_to_seq("some_str") == ("some_str",)
-    assert _scalar_to_seq("some_str", sequence_type=list) == ["some_str"]
-
-    # Verify sequences returned unchanged
-    assert _scalar_to_seq((1, 2)) == (1, 2)
-
-
-def test_scalar_to_seq_raises():
-    """Test scalar_to_seq raises error when `sequence_type` is unexpected type."""
-    with pytest.raises(
-        ValueError,
-        match="`sequence_type` must be a subclass of collections.abc.Sequence.",
-    ):
-        _scalar_to_seq(7, sequence_type=int)
-
-    with pytest.raises(
-        ValueError,
-        match="`sequence_type` must be a subclass of collections.abc.Sequence.",
-    ):
-        _scalar_to_seq(7, sequence_type=dict)
-
-
-def test_make_strings_unique_output():
-    """Test make_strings_unique outputs expected unique strings."""
-    # case with already unique string list
-    some_strs = ["abc", "bcd"]
-    assert make_strings_unique(some_strs) == ["abc", "bcd"]
-    # Case where some strings repeated
-    some_strs = ["abc", "abc", "bcd"]
-    assert make_strings_unique(some_strs) == ["abc_1", "abc_2", "bcd"]
-    # Case when input is tuple
-    assert make_strings_unique(tuple(some_strs)) == ("abc_1", "abc_2", "bcd")
-
-    # Case where more than one level of making things unique is needed
-    some_strs = ["abc", "abc", "bcd", "abc_1"]
-    assert make_strings_unique(some_strs) == ["abc_1_1", "abc_2", "bcd", "abc_1_2"]
-
-    # Case when input is not flat
-    some_strs = ["abc_1", ("abc_2", "bcd")]
-    assert make_strings_unique(some_strs) == ["abc_1", ("abc_2", "bcd")]
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tests of the functionality for working with iterables.
+
+tests in this module incdlue:
+
+- test_format_seq_to_str: verify that _format_seq_to_str outputs expected format.
+- test_format_seq_to_str_raises: verify _format_seq_to_str raises error on unexpected
+  output.
+- test_scalar_to_seq_expected_output: verify that _scalar_to_seq returns exepcted
+  output.
+- test_scalar_to_seq_raises: verify that _scalar_to_seq raises error when an
+  invalid value is provided for sequence_type parameter.
+- test_make_strings_unique_output: verify make_strings_unique output is expected.
+"""
+import pytest
+
+from skbase.base import BaseEstimator, BaseObject
+from skbase.utils._iter import _format_seq_to_str, _scalar_to_seq, make_strings_unique
+
+__author__ = ["RNKuhns"]
+
+
+def test_format_seq_to_str():
+    """Test _format_seq_to_str returns expected output."""
+    # Test basic functionality (including ability to handle str and non-str)
+    seq = [1, 2, "3", 4]
+    assert _format_seq_to_str(seq) == "1, 2, 3, 4"
+
+    # Test use of last_sep
+    assert _format_seq_to_str(seq, last_sep="and") == "1, 2, 3 and 4"
+    assert _format_seq_to_str(seq, last_sep="or") == "1, 2, 3 or 4"
+
+    # Test use of different sep argument
+    assert _format_seq_to_str(seq, sep=";") == "1;2;3;4"
+
+    # Verify things work with BaseObject and BaseEstimator instances
+    seq = [BaseEstimator(), BaseObject(), 1]
+    assert _format_seq_to_str(seq) == "BaseEstimator(), BaseObject(), 1"
+
+    # Test use of last_sep
+    assert (
+        _format_seq_to_str(seq, last_sep="and") == "BaseEstimator(), BaseObject() and 1"
+    )
+    assert (
+        _format_seq_to_str(seq, last_sep="or") == "BaseEstimator(), BaseObject() or 1"
+    )
+
+    # Test use of different sep argument
+    assert _format_seq_to_str(seq, sep=";") == "BaseEstimator();BaseObject();1"
+
+    # Test using remove_type_text keyword
+    assert (
+        _format_seq_to_str([list, tuple], remove_type_text=False)
+        == "<class 'list'>, <class 'tuple'>"
+    )
+    assert _format_seq_to_str([list, tuple], remove_type_text=True) == "list, tuple"
+    assert (
+        _format_seq_to_str([list, tuple], last_sep="and", remove_type_text=True)
+        == "list and tuple"
+    )
+
+    # Test with scalar inputs
+    assert _format_seq_to_str(7) == "7"  # int, float, bool primitives cast to str
+    assert _format_seq_to_str("some_str") == "some_str"
+    # Verify that keywords don't affect output
+    assert _format_seq_to_str(7, sep=";") == "7"
+    assert _format_seq_to_str(7, last_sep="or") == "7"
+    # Verify with types
+    assert _format_seq_to_str(object) == "object"
+    assert _format_seq_to_str(int) == "int"
+
+
+def test_format_seq_to_str_raises():
+    """Test _format_seq_to_str raises error when input is unexpected type."""
+    with pytest.raises(TypeError, match="`seq` must be a sequence or scalar.*"):
+        _format_seq_to_str((c for c in [1, 2, 3]))
+
+
+def test_scalar_to_seq_expected_output():
+    """Test _scalar_to_seq returns expected output."""
+    assert _scalar_to_seq(7) == (7,)
+    # Verify it works with scalar classes and objects
+    assert _scalar_to_seq(BaseObject) == (BaseObject,)
+    assert _scalar_to_seq(BaseObject()) == (BaseObject(),)
+    # Verify strings treated like scalar not sequence
+    assert _scalar_to_seq("some_str") == ("some_str",)
+    assert _scalar_to_seq("some_str", sequence_type=list) == ["some_str"]
+
+    # Verify sequences returned unchanged
+    assert _scalar_to_seq((1, 2)) == (1, 2)
+
+
+def test_scalar_to_seq_raises():
+    """Test scalar_to_seq raises error when `sequence_type` is unexpected type."""
+    with pytest.raises(
+        ValueError,
+        match="`sequence_type` must be a subclass of collections.abc.Sequence.",
+    ):
+        _scalar_to_seq(7, sequence_type=int)
+
+    with pytest.raises(
+        ValueError,
+        match="`sequence_type` must be a subclass of collections.abc.Sequence.",
+    ):
+        _scalar_to_seq(7, sequence_type=dict)
+
+
+def test_make_strings_unique_output():
+    """Test make_strings_unique outputs expected unique strings."""
+    # case with already unique string list
+    some_strs = ["abc", "bcd"]
+    assert make_strings_unique(some_strs) == ["abc", "bcd"]
+    # Case where some strings repeated
+    some_strs = ["abc", "abc", "bcd"]
+    assert make_strings_unique(some_strs) == ["abc_1", "abc_2", "bcd"]
+    # Case when input is tuple
+    assert make_strings_unique(tuple(some_strs)) == ("abc_1", "abc_2", "bcd")
+
+    # Case where more than one level of making things unique is needed
+    some_strs = ["abc", "abc", "bcd", "abc_1"]
+    assert make_strings_unique(some_strs) == ["abc_1_1", "abc_2", "bcd", "abc_1_2"]
+
+    # Case when input is not flat
+    some_strs = ["abc_1", ("abc_2", "bcd")]
+    assert make_strings_unique(some_strs) == ["abc_1", ("abc_2", "bcd")]
```

### Comparing `skbase-0.4.5/skbase/utils/tests/test_nested_iter.py` & `skbase-0.4.6/skbase/utils/tests/test_nested_iter.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tests of the functionality for working with iterables.
-
-tests in this module incdlue:
-
-- test_remove_single
-- test_flatten
-- test_unflatten
-- test_unflat_len
-- test_is_flat
-"""
-# import pytest
-
-from skbase.base import BaseEstimator, BaseObject
-from skbase.utils._nested_iter import (
-    _remove_single,
-    flatten,
-    is_flat,
-    unflat_len,
-    unflatten,
-)
-
-__author__ = ["RNKuhns"]
-
-
-def test_remove_single():
-    """Test _remove_single output is as expected."""
-    # Verify that length > 1 sequence not impacted.
-    assert _remove_single([1, 2, 3]) == [1, 2, 3]
-
-    # Verify single member of sequence is removed as expected
-    assert _remove_single([1]) == 1
-
-
-def test_flatten():
-    """Test flatten output is as expected."""
-    assert flatten([1, 2, [3, (4, 5)], 6]) == [1, 2, 3, 4, 5, 6]
-
-    # Verify functionality with classes and objects
-    assert flatten((BaseObject, 7, (BaseObject, BaseEstimator))) == (
-        BaseObject,
-        7,
-        BaseObject,
-        BaseEstimator,
-    )
-    assert flatten((BaseObject(), 7, (BaseObject, BaseEstimator()))) == (
-        BaseObject(),
-        7,
-        BaseObject,
-        BaseEstimator(),
-    )
-
-
-def test_unflatten():
-    """Test output of unflatten."""
-    assert unflatten([1, 2, 3, 4, 5, 6], [6, 3, [5, (2, 4)], 1]) == [
-        1,
-        2,
-        [3, (4, 5)],
-        6,
-    ]
-
-
-def test_unflat_len():
-    """Test output of unflat_len."""
-    assert unflat_len(7) == 1
-    assert unflat_len((1, 2)) == 2
-    assert unflat_len([1, (2, 3), 4, 5]) == 5
-    assert unflat_len([1, 2, (c for c in (2, 3, 4))]) == 5
-    assert unflat_len((c for c in [1, 2, (c for c in (2, 3, 4))])) == 5
-
-
-def test_is_flat():
-    """Test output of is_flat."""
-    assert is_flat([1, 2, 3, 4, 5]) is True
-    assert is_flat([1, (2, 3), 4, 5]) is False
-    # Check with flat generator
-    assert is_flat((c for c in [1, 2, 3])) is True
-    # Check with nested generator
-    assert is_flat([1, 2, (c for c in (2, 3, 4))]) is False
-    # Check with generator nested in a generator
-    assert is_flat((c for c in [1, 2, (c for c in (2, 3, 4))])) is False
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tests of the functionality for working with iterables.
+
+tests in this module incdlue:
+
+- test_remove_single
+- test_flatten
+- test_unflatten
+- test_unflat_len
+- test_is_flat
+"""
+# import pytest
+
+from skbase.base import BaseEstimator, BaseObject
+from skbase.utils._nested_iter import (
+    _remove_single,
+    flatten,
+    is_flat,
+    unflat_len,
+    unflatten,
+)
+
+__author__ = ["RNKuhns"]
+
+
+def test_remove_single():
+    """Test _remove_single output is as expected."""
+    # Verify that length > 1 sequence not impacted.
+    assert _remove_single([1, 2, 3]) == [1, 2, 3]
+
+    # Verify single member of sequence is removed as expected
+    assert _remove_single([1]) == 1
+
+
+def test_flatten():
+    """Test flatten output is as expected."""
+    assert flatten([1, 2, [3, (4, 5)], 6]) == [1, 2, 3, 4, 5, 6]
+
+    # Verify functionality with classes and objects
+    assert flatten((BaseObject, 7, (BaseObject, BaseEstimator))) == (
+        BaseObject,
+        7,
+        BaseObject,
+        BaseEstimator,
+    )
+    assert flatten((BaseObject(), 7, (BaseObject, BaseEstimator()))) == (
+        BaseObject(),
+        7,
+        BaseObject,
+        BaseEstimator(),
+    )
+
+
+def test_unflatten():
+    """Test output of unflatten."""
+    assert unflatten([1, 2, 3, 4, 5, 6], [6, 3, [5, (2, 4)], 1]) == [
+        1,
+        2,
+        [3, (4, 5)],
+        6,
+    ]
+
+
+def test_unflat_len():
+    """Test output of unflat_len."""
+    assert unflat_len(7) == 1
+    assert unflat_len((1, 2)) == 2
+    assert unflat_len([1, (2, 3), 4, 5]) == 5
+    assert unflat_len([1, 2, (c for c in (2, 3, 4))]) == 5
+    assert unflat_len((c for c in [1, 2, (c for c in (2, 3, 4))])) == 5
+
+
+def test_is_flat():
+    """Test output of is_flat."""
+    assert is_flat([1, 2, 3, 4, 5]) is True
+    assert is_flat([1, (2, 3), 4, 5]) is False
+    # Check with flat generator
+    assert is_flat((c for c in [1, 2, 3])) is True
+    # Check with nested generator
+    assert is_flat([1, 2, (c for c in (2, 3, 4))]) is False
+    # Check with generator nested in a generator
+    assert is_flat((c for c in [1, 2, (c for c in (2, 3, 4))])) is False
```

### Comparing `skbase-0.4.5/skbase/utils/tests/test_utils.py` & `skbase-0.4.6/skbase/utils/tests/test_utils.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tests of the functionality for miscellaneous utilities.
-
-tests in this module incdlue:
-
-- test_subset_dict_keys_output: verify that subset_dict_keys outputs expected format.
-"""
-from skbase.utils import subset_dict_keys
-
-__author__ = ["RNKuhns"]
-
-
-def test_subset_dict_keys_output():
-    """Test subset_dict_keys outputs expected result."""
-    some_dict = {"some_param__a": 1, "some_param__b": 2, "some_param__c": 3}
-
-    assert subset_dict_keys(some_dict, "some_param__a") == {"some_param__a": 1}
-
-    assert subset_dict_keys(some_dict, ("some_param__a", "some_param__b")) == {
-        "some_param__a": 1,
-        "some_param__b": 2,
-    }
-
-    assert subset_dict_keys(some_dict, ("a", "b"), prefix="some_param") == {
-        "a": 1,
-        "b": 2,
-    }
-
-    assert subset_dict_keys(
-        some_dict, ("a", "b"), prefix="some_param", remove_prefix=False
-    ) == {"some_param__a": 1, "some_param__b": 2}
-
-    assert subset_dict_keys(
-        some_dict, (c for c in ("some_param__a", "some_param__b"))
-    ) == {"some_param__a": 1, "some_param__b": 2}
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tests of the functionality for miscellaneous utilities.
+
+tests in this module incdlue:
+
+- test_subset_dict_keys_output: verify that subset_dict_keys outputs expected format.
+"""
+from skbase.utils import subset_dict_keys
+
+__author__ = ["RNKuhns"]
+
+
+def test_subset_dict_keys_output():
+    """Test subset_dict_keys outputs expected result."""
+    some_dict = {"some_param__a": 1, "some_param__b": 2, "some_param__c": 3}
+
+    assert subset_dict_keys(some_dict, "some_param__a") == {"some_param__a": 1}
+
+    assert subset_dict_keys(some_dict, ("some_param__a", "some_param__b")) == {
+        "some_param__a": 1,
+        "some_param__b": 2,
+    }
+
+    assert subset_dict_keys(some_dict, ("a", "b"), prefix="some_param") == {
+        "a": 1,
+        "b": 2,
+    }
+
+    assert subset_dict_keys(
+        some_dict, ("a", "b"), prefix="some_param", remove_prefix=False
+    ) == {"some_param__a": 1, "some_param__b": 2}
+
+    assert subset_dict_keys(
+        some_dict, (c for c in ("some_param__a", "some_param__b"))
+    ) == {"some_param__a": 1, "some_param__b": 2}
```

### Comparing `skbase-0.4.5/skbase/validate/__init__.py` & `skbase-0.4.6/skbase/validate/__init__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tools for validating and comparing BaseObjects and collections of BaseObjects."""
-from typing import List
-
-from skbase.validate._named_objects import (
-    check_sequence_named_objects,
-    is_named_object_tuple,
-    is_sequence_named_objects,
-)
-from skbase.validate._types import check_sequence, check_type, is_sequence
-
-__author__: List[str] = ["RNKuhns", "fkiraly"]
-__all__: List[str] = [
-    "check_sequence",
-    "check_sequence_named_objects",
-    "check_type",
-    "is_named_object_tuple",
-    "is_sequence",
-    "is_sequence_named_objects",
-]
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tools for validating and comparing BaseObjects and collections of BaseObjects."""
+from typing import List
+
+from skbase.validate._named_objects import (
+    check_sequence_named_objects,
+    is_named_object_tuple,
+    is_sequence_named_objects,
+)
+from skbase.validate._types import check_sequence, check_type, is_sequence
+
+__author__: List[str] = ["RNKuhns", "fkiraly"]
+__all__: List[str] = [
+    "check_sequence",
+    "check_sequence_named_objects",
+    "check_type",
+    "is_named_object_tuple",
+    "is_sequence",
+    "is_sequence_named_objects",
+]
```

### Comparing `skbase-0.4.5/skbase/validate/_named_objects.py` & `skbase-0.4.6/skbase/validate/_named_objects.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,403 +1,403 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Validate if an input is one of the allowed named object formats."""
-import collections.abc
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-    overload,
-)
-
-from skbase.base import BaseObject
-
-__all__: List[str] = [
-    "check_sequence_named_objects",
-    "is_named_object_tuple",
-    "is_sequence_named_objects",
-]
-__author__: List[str] = ["RNKuhns"]
-
-
-def _named_baseobject_error_msg(
-    sequence_name: Optional[str] = None, allow_dict: bool = True
-):
-    """Create error message for non-comformance with named BaseObject api."""
-    name_str = f"{sequence_name}" if sequence_name is not None else "Input"
-    allowed_types = "a sequence of (string name, BaseObject instance) tuples"
-
-    if allow_dict:
-        allowed_types += " or dict[str, BaseObject instance]"
-    msg = f"Invalid {name_str!r}, {name_str!r} should be {allowed_types}."
-    return msg
-
-
-def is_named_object_tuple(
-    obj: Any, object_type: Optional[Union[type, Tuple[type, ...]]] = None
-) -> bool:
-    """Indicate if input is a a tuple of format (str, `object_type`).
-
-    Used to validate that input follows named object tuple API format.
-
-    Parameters
-    ----------
-    obj : Any
-        The object to be checked to see if it is a (str, `object_type`) tuple.
-    object_type : class or tuple of class, default=BaseObject
-        Class(es) that all objects are checked to be an instance of. If None,
-        then :class:``skbase.base.BaseObject`` is used as default.
-
-    Returns
-    -------
-    bool
-        True if obj is (str, `object_type`) tuple, otherwise False.
-
-    See Also
-    --------
-    is_sequence_named_objects :
-        Indicate (True/False) if an input sequence follows the named object API.
-    check_sequence_named_objects :
-        Validate input to see if it follows sequence of named objects API. An error
-        is raised for input that does not conform to the API format.
-
-    Examples
-    --------
-    >>> from skbase.base import BaseObject, BaseEstimator
-    >>> from skbase.validate import is_named_object_tuple
-
-    Default checks for object to be an instance of BaseOBject
-
-    >>> is_named_object_tuple(("Step 1", BaseObject()))
-    True
-
-    >>> is_named_object_tuple(("Step 2", BaseEstimator()))
-    True
-
-    If a different `object_type` is provided then it is used in the isinstance check
-
-    >>> is_named_object_tuple(("Step 1", BaseObject()), object_type=BaseEstimator)
-    False
-
-    >>> is_named_object_tuple(("Step 1", BaseEstimator()), object_type=BaseEstimator)
-    True
-
-    If the input is does not follow named object tuple format then False is returned
-
-    >>> is_named_object_tuple({"Step 1": BaseEstimator()})
-    False
-
-    >>> is_named_object_tuple((1, BaseObject()))
-    False
-    """
-    if object_type is None:
-        object_type = BaseObject
-    if not isinstance(obj, tuple) or len(obj) != 2:
-        return False
-    if not isinstance(obj[0], str) or not isinstance(obj[1], object_type):
-        return False
-    return True
-
-
-def is_sequence_named_objects(
-    seq_to_check: Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]],
-    allow_dict: bool = True,
-    require_unique_names=False,
-    object_type: Optional[Union[type, Tuple[type]]] = None,
-) -> bool:
-    """Indicate if input is a sequence of named BaseObject instances.
-
-    This can be a sequence of (str, BaseObject instance) tuples or
-    a dictionary with string names as keys and BaseObject instances as values
-    (if ``allow_dict=True``).
-
-    Parameters
-    ----------
-    seq_to_check : Sequence((str, BaseObject)) or Dict[str, BaseObject]
-        The input to check for conformance with the named object interface.
-        Conforming input are:
-
-        - Sequence that contains (str, BaseObject instance) tuples
-        - Dictionary with string names as keys and BaseObject instances as values
-          if ``allow_dict=True``
-
-    allow_dict : bool, default=True
-        Whether a dictionary of named objects is allowed as conforming named object
-        type.
-
-        - If True, then a dictionary with string keys and BaseObject instances
-          is allowed format for providing a sequence of named objects.
-        - If False, then only sequences that contain (str, BaseObject instance)
-          tuples are considered conforming with the named object parameter API.
-
-    require_unique_names : bool, default=False
-        Whether names used in the sequence of named BaseObject instances
-        must be unique.
-
-        - If True and the names are not unique, then False is always returned.
-        - If False, then whether or not the function returns True or False
-          depends on whether `seq_to_check` follows sequence of named
-          BaseObject format.
-
-    object_type : class or tuple[class], default=None
-        The class type(s) that is used to ensure that all elements of named objects
-        match the expected type.
-
-    Returns
-    -------
-    bool
-        Whether the input `seq_to_check` is a sequence that follows the API for
-        nameed base object instances.
-
-    Raises
-    ------
-    ValueError
-        If `seq_to_check` is not a sequence or ``allow_dict is False`` and
-        `seq_to_check` is a dictionary.
-
-    See Also
-    --------
-    is_named_object_tuple :
-        Indicate (True/False) if input follows the named object API format for
-        a single named object (e.g., tupe[str, expected class type]).
-    check_sequence_named_objects :
-        Validate input to see if it follows sequence of named objects API. An error
-        is raised for input that does not conform to the API format.
-
-    Examples
-    --------
-    >>> from skbase.base import BaseObject, BaseEstimator
-    >>> from skbase.validate import is_sequence_named_objects
-    >>> named_objects = [("Step 1", BaseObject()), ("Step 2", BaseObject())]
-    >>> is_sequence_named_objects(named_objects)
-    True
-
-    Dictionaries are optionally allowed as sequences of named BaseObjects
-
-    >>> dict_named_objects = {"Step 1": BaseObject(), "Step 2": BaseObject()}
-    >>> is_sequence_named_objects(dict_named_objects)
-    True
-    >>> is_sequence_named_objects(dict_named_objects, allow_dict=False)
-    False
-
-    Invalid format due to object names not being strings
-
-    >>> incorrectly_named_objects = [(1, BaseObject()), (2, BaseObject())]
-    >>> is_sequence_named_objects(incorrectly_named_objects)
-    False
-
-    Invalid format due to named items not being BaseObject instances
-
-    >>> named_items = [("1", 7), ("2", 42)]
-    >>> is_sequence_named_objects(named_items)
-    False
-
-    The validation can require the object elements to be a certain class type
-
-    >>> named_objects = [("Step 1", BaseObject()), ("Step 2", BaseObject())]
-    >>> is_sequence_named_objects(named_objects, object_type=BaseEstimator)
-    False
-    >>> named_objects = [("Step 1", BaseEstimator()), ("Step 2", BaseEstimator())]
-    >>> is_sequence_named_objects(named_objects, object_type=BaseEstimator)
-    True
-    """
-    # Want to end quickly if the input isn't sequence or is a dict and we
-    # aren't allowing dicts
-    if object_type is None:
-        object_type = BaseObject
-
-    is_dict = isinstance(seq_to_check, dict)
-    if (not is_dict and not isinstance(seq_to_check, collections.abc.Sequence)) or (
-        not allow_dict and is_dict
-    ):
-        return False
-
-    all_expected_format: bool
-    all_unique_names: bool
-    if is_dict:
-        if TYPE_CHECKING:  # pragma: no cover
-            assert isinstance(seq_to_check, dict)  # nosec B101
-        elements_expected_format = [
-            isinstance(name, str) and isinstance(obj, object_type)
-            for name, obj in seq_to_check.items()
-        ]
-        all_unique_names = True
-    else:
-        names = []
-        elements_expected_format = []
-        for it in seq_to_check:
-            if is_named_object_tuple(it, object_type=object_type):
-                elements_expected_format.append(True)
-                names.append(it[0])
-            else:
-                elements_expected_format.append(False)
-        all_unique_names = len(set(names)) == len(names)
-
-    all_expected_format = all(elements_expected_format)
-
-    if not all_expected_format or (require_unique_names and not all_unique_names):
-        is_expected_format = False
-    else:
-        is_expected_format = True
-
-    return is_expected_format
-
-
-@overload
-def check_sequence_named_objects(
-    seq_to_check: Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]],
-    allow_dict: bool = True,
-    require_unique_names=False,
-    object_type: Optional[Union[type, Tuple[type]]] = None,
-    sequence_name: Optional[str] = None,
-) -> Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]]:
-    ...  # pragma: no cover
-
-
-@overload
-def check_sequence_named_objects(
-    seq_to_check: Sequence[Tuple[str, BaseObject]],
-    allow_dict: bool,
-    require_unique_names=False,
-    object_type: Optional[Union[type, Tuple[type]]] = None,
-    sequence_name: Optional[str] = None,
-) -> Sequence[Tuple[str, BaseObject]]:
-    ...  # pragma: no cover
-
-
-@overload
-def check_sequence_named_objects(
-    seq_to_check: Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]],
-    allow_dict: bool = True,
-    require_unique_names=False,
-    object_type: Optional[Union[type, Tuple[type]]] = None,
-    sequence_name: Optional[str] = None,
-) -> Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]]:
-    ...  # pragma: no cover
-
-
-def check_sequence_named_objects(
-    seq_to_check: Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]],
-    allow_dict: bool = True,
-    require_unique_names=False,
-    object_type: Optional[Union[type, Tuple[type]]] = None,
-    sequence_name: Optional[str] = None,
-) -> Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]]:
-    """Check if input is a sequence of named BaseObject instances.
-
-    `seq_to_check` is returned unchanged when it follows the allowed named
-    BaseObject convention. The allowed format includes a sequence of
-    (str, BaseObject instance) tuples. A dictionary with string names as keys
-    and BaseObject instances as values is also allowed if ``allow_dict is True``.
-
-    Parameters
-    ----------
-    seq_to_check : Sequence((str, BaseObject)) or Dict[str, BaseObject]
-        The input to check for conformance with the named object interface.
-        Conforming input are:
-
-        - Sequence that contains (str, BaseObject instance) tuples
-        - Dictionary with string names as keys and BaseObject instances as values
-          if ``allow_dict=True``
-
-    allow_dict : bool, default=True
-        Whether a dictionary of named objects is allowed as conforming named object
-        type.
-
-        - If True, then a dictionary with string keys and BaseObject instances
-          is allowed format for providing a sequence of named objects.
-        - If False, then only sequences that contain (str, BaseObject instance)
-          tuples are considered conforming with the named object parameter API.
-
-    require_unique_names : bool, default=False
-        Whether names used in the sequence of named BaseObject instances
-        must be unique.
-
-        - If True and the names are not unique, then False is always returned.
-        - If False, then whether or not the function returns True or False
-          depends on whether `seq_to_check` follows sequence of named BaseObject format.
-
-    object_type : class or tuple[class], default=None
-        The class type(s) that is used to ensure that all elements of named objects
-        match the expected type.
-    sequence_name : str, default=None
-        Optional name used to refer to the input `seq_to_check` when
-        raising any errors. Ignored ``raise_error=False``.
-
-    Returns
-    -------
-    Sequence((str, BaseObject)) or Dict[str, BaseObject]
-        The `seq_to_check` is returned if it is a conforming named object type.
-
-        - If ``allow_dict=True`` then return type is Sequence((str, BaseObject))
-          or Dict[str, BaseObject]
-        - If ``allow_dict=False`` then return type is Sequence((str, BaseObject))
-
-    Raises
-    ------
-    ValueError
-        If `seq_to_check` does not conform to the named BaseObject API.
-
-    See Also
-    --------
-    is_named_object_tuple :
-        Indicate (True/False) if input follows the named object API format for
-        a single named object (e.g., tupe[str, expected class type]).
-    is_sequence_named_objects :
-        Indicate (True/False) if an input sequence follows the named object API.
-
-    Examples
-    --------
-    >>> from skbase.base import BaseObject, BaseEstimator
-    >>> from skbase.validate import check_sequence_named_objects
-    >>> named_objects = [("Step 1", BaseObject()), ("Step 2", BaseObject())]
-    >>> check_sequence_named_objects(named_objects)
-    [('Step 1', BaseObject()), ('Step 2', BaseObject())]
-
-    Dictionaries are optionally allowed as sequences of named BaseObjects
-
-    >>> named_objects = {"Step 1": BaseObject(), "Step 2": BaseObject()}
-    >>> check_sequence_named_objects(named_objects)
-    {'Step 1': BaseObject(), 'Step 2': BaseObject()}
-
-    Raises error since dictionaries are not allowed when allow_dict is False
-
-    >>> check_sequence_named_objects(named_objects, allow_dict=False) # doctest: +SKIP
-
-    Raises error due to invalid format due to object names not being strings
-
-    >>> incorrectly_named_objects = [(1, BaseObject()), (2, BaseObject())]
-    >>> check_sequence_named_objects(incorrectly_named_objects)  # doctest: +SKIP
-
-    Raises error due to invalid format since named items are not BaseObject instances
-
-    >>> named_items = [("1", 7), ("2", 42)]
-    >>> check_sequence_named_objects(named_items)  # doctest: +SKIP
-
-    The validation can require the object elements to be a certain class type
-
-    >>> named_objects = [("Step 1", BaseObject()), ("Step 2", BaseObject())]
-    >>> check_sequence_named_objects( \
-    named_objects, object_type=BaseEstimator) # doctest: +SKIP
-    >>> named_objects = [("Step 1", BaseEstimator()), ("Step 2", BaseEstimator())]
-    >>> check_sequence_named_objects(named_objects, object_type=BaseEstimator)
-    [('Step 1', BaseEstimator()), ('Step 2', BaseEstimator())]
-    """
-    is_expected_format = is_sequence_named_objects(
-        seq_to_check,
-        allow_dict=allow_dict,
-        require_unique_names=require_unique_names,
-        object_type=object_type,
-    )
-    # Raise error is format is not expected.
-    if not is_expected_format:
-        msg = _named_baseobject_error_msg(
-            sequence_name=sequence_name, allow_dict=allow_dict
-        )
-        raise ValueError(msg)
-
-    return seq_to_check
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Validate if an input is one of the allowed named object formats."""
+import collections.abc
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+    overload,
+)
+
+from skbase.base import BaseObject
+
+__all__: List[str] = [
+    "check_sequence_named_objects",
+    "is_named_object_tuple",
+    "is_sequence_named_objects",
+]
+__author__: List[str] = ["RNKuhns"]
+
+
+def _named_baseobject_error_msg(
+    sequence_name: Optional[str] = None, allow_dict: bool = True
+):
+    """Create error message for non-comformance with named BaseObject api."""
+    name_str = f"{sequence_name}" if sequence_name is not None else "Input"
+    allowed_types = "a sequence of (string name, BaseObject instance) tuples"
+
+    if allow_dict:
+        allowed_types += " or dict[str, BaseObject instance]"
+    msg = f"Invalid {name_str!r}, {name_str!r} should be {allowed_types}."
+    return msg
+
+
+def is_named_object_tuple(
+    obj: Any, object_type: Optional[Union[type, Tuple[type, ...]]] = None
+) -> bool:
+    """Indicate if input is a a tuple of format (str, `object_type`).
+
+    Used to validate that input follows named object tuple API format.
+
+    Parameters
+    ----------
+    obj : Any
+        The object to be checked to see if it is a (str, `object_type`) tuple.
+    object_type : class or tuple of class, default=BaseObject
+        Class(es) that all objects are checked to be an instance of. If None,
+        then :class:``skbase.base.BaseObject`` is used as default.
+
+    Returns
+    -------
+    bool
+        True if obj is (str, `object_type`) tuple, otherwise False.
+
+    See Also
+    --------
+    is_sequence_named_objects :
+        Indicate (True/False) if an input sequence follows the named object API.
+    check_sequence_named_objects :
+        Validate input to see if it follows sequence of named objects API. An error
+        is raised for input that does not conform to the API format.
+
+    Examples
+    --------
+    >>> from skbase.base import BaseObject, BaseEstimator
+    >>> from skbase.validate import is_named_object_tuple
+
+    Default checks for object to be an instance of BaseOBject
+
+    >>> is_named_object_tuple(("Step 1", BaseObject()))
+    True
+
+    >>> is_named_object_tuple(("Step 2", BaseEstimator()))
+    True
+
+    If a different `object_type` is provided then it is used in the isinstance check
+
+    >>> is_named_object_tuple(("Step 1", BaseObject()), object_type=BaseEstimator)
+    False
+
+    >>> is_named_object_tuple(("Step 1", BaseEstimator()), object_type=BaseEstimator)
+    True
+
+    If the input is does not follow named object tuple format then False is returned
+
+    >>> is_named_object_tuple({"Step 1": BaseEstimator()})
+    False
+
+    >>> is_named_object_tuple((1, BaseObject()))
+    False
+    """
+    if object_type is None:
+        object_type = BaseObject
+    if not isinstance(obj, tuple) or len(obj) != 2:
+        return False
+    if not isinstance(obj[0], str) or not isinstance(obj[1], object_type):
+        return False
+    return True
+
+
+def is_sequence_named_objects(
+    seq_to_check: Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]],
+    allow_dict: bool = True,
+    require_unique_names=False,
+    object_type: Optional[Union[type, Tuple[type]]] = None,
+) -> bool:
+    """Indicate if input is a sequence of named BaseObject instances.
+
+    This can be a sequence of (str, BaseObject instance) tuples or
+    a dictionary with string names as keys and BaseObject instances as values
+    (if ``allow_dict=True``).
+
+    Parameters
+    ----------
+    seq_to_check : Sequence((str, BaseObject)) or Dict[str, BaseObject]
+        The input to check for conformance with the named object interface.
+        Conforming input are:
+
+        - Sequence that contains (str, BaseObject instance) tuples
+        - Dictionary with string names as keys and BaseObject instances as values
+          if ``allow_dict=True``
+
+    allow_dict : bool, default=True
+        Whether a dictionary of named objects is allowed as conforming named object
+        type.
+
+        - If True, then a dictionary with string keys and BaseObject instances
+          is allowed format for providing a sequence of named objects.
+        - If False, then only sequences that contain (str, BaseObject instance)
+          tuples are considered conforming with the named object parameter API.
+
+    require_unique_names : bool, default=False
+        Whether names used in the sequence of named BaseObject instances
+        must be unique.
+
+        - If True and the names are not unique, then False is always returned.
+        - If False, then whether or not the function returns True or False
+          depends on whether `seq_to_check` follows sequence of named
+          BaseObject format.
+
+    object_type : class or tuple[class], default=None
+        The class type(s) that is used to ensure that all elements of named objects
+        match the expected type.
+
+    Returns
+    -------
+    bool
+        Whether the input `seq_to_check` is a sequence that follows the API for
+        nameed base object instances.
+
+    Raises
+    ------
+    ValueError
+        If `seq_to_check` is not a sequence or ``allow_dict is False`` and
+        `seq_to_check` is a dictionary.
+
+    See Also
+    --------
+    is_named_object_tuple :
+        Indicate (True/False) if input follows the named object API format for
+        a single named object (e.g., tupe[str, expected class type]).
+    check_sequence_named_objects :
+        Validate input to see if it follows sequence of named objects API. An error
+        is raised for input that does not conform to the API format.
+
+    Examples
+    --------
+    >>> from skbase.base import BaseObject, BaseEstimator
+    >>> from skbase.validate import is_sequence_named_objects
+    >>> named_objects = [("Step 1", BaseObject()), ("Step 2", BaseObject())]
+    >>> is_sequence_named_objects(named_objects)
+    True
+
+    Dictionaries are optionally allowed as sequences of named BaseObjects
+
+    >>> dict_named_objects = {"Step 1": BaseObject(), "Step 2": BaseObject()}
+    >>> is_sequence_named_objects(dict_named_objects)
+    True
+    >>> is_sequence_named_objects(dict_named_objects, allow_dict=False)
+    False
+
+    Invalid format due to object names not being strings
+
+    >>> incorrectly_named_objects = [(1, BaseObject()), (2, BaseObject())]
+    >>> is_sequence_named_objects(incorrectly_named_objects)
+    False
+
+    Invalid format due to named items not being BaseObject instances
+
+    >>> named_items = [("1", 7), ("2", 42)]
+    >>> is_sequence_named_objects(named_items)
+    False
+
+    The validation can require the object elements to be a certain class type
+
+    >>> named_objects = [("Step 1", BaseObject()), ("Step 2", BaseObject())]
+    >>> is_sequence_named_objects(named_objects, object_type=BaseEstimator)
+    False
+    >>> named_objects = [("Step 1", BaseEstimator()), ("Step 2", BaseEstimator())]
+    >>> is_sequence_named_objects(named_objects, object_type=BaseEstimator)
+    True
+    """
+    # Want to end quickly if the input isn't sequence or is a dict and we
+    # aren't allowing dicts
+    if object_type is None:
+        object_type = BaseObject
+
+    is_dict = isinstance(seq_to_check, dict)
+    if (not is_dict and not isinstance(seq_to_check, collections.abc.Sequence)) or (
+        not allow_dict and is_dict
+    ):
+        return False
+
+    all_expected_format: bool
+    all_unique_names: bool
+    if is_dict:
+        if TYPE_CHECKING:  # pragma: no cover
+            assert isinstance(seq_to_check, dict)  # nosec B101
+        elements_expected_format = [
+            isinstance(name, str) and isinstance(obj, object_type)
+            for name, obj in seq_to_check.items()
+        ]
+        all_unique_names = True
+    else:
+        names = []
+        elements_expected_format = []
+        for it in seq_to_check:
+            if is_named_object_tuple(it, object_type=object_type):
+                elements_expected_format.append(True)
+                names.append(it[0])
+            else:
+                elements_expected_format.append(False)
+        all_unique_names = len(set(names)) == len(names)
+
+    all_expected_format = all(elements_expected_format)
+
+    if not all_expected_format or (require_unique_names and not all_unique_names):
+        is_expected_format = False
+    else:
+        is_expected_format = True
+
+    return is_expected_format
+
+
+@overload
+def check_sequence_named_objects(
+    seq_to_check: Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]],
+    allow_dict: bool = True,
+    require_unique_names=False,
+    object_type: Optional[Union[type, Tuple[type]]] = None,
+    sequence_name: Optional[str] = None,
+) -> Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]]:
+    ...  # pragma: no cover
+
+
+@overload
+def check_sequence_named_objects(
+    seq_to_check: Sequence[Tuple[str, BaseObject]],
+    allow_dict: bool,
+    require_unique_names=False,
+    object_type: Optional[Union[type, Tuple[type]]] = None,
+    sequence_name: Optional[str] = None,
+) -> Sequence[Tuple[str, BaseObject]]:
+    ...  # pragma: no cover
+
+
+@overload
+def check_sequence_named_objects(
+    seq_to_check: Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]],
+    allow_dict: bool = True,
+    require_unique_names=False,
+    object_type: Optional[Union[type, Tuple[type]]] = None,
+    sequence_name: Optional[str] = None,
+) -> Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]]:
+    ...  # pragma: no cover
+
+
+def check_sequence_named_objects(
+    seq_to_check: Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]],
+    allow_dict: bool = True,
+    require_unique_names=False,
+    object_type: Optional[Union[type, Tuple[type]]] = None,
+    sequence_name: Optional[str] = None,
+) -> Union[Sequence[Tuple[str, BaseObject]], Dict[str, BaseObject]]:
+    """Check if input is a sequence of named BaseObject instances.
+
+    `seq_to_check` is returned unchanged when it follows the allowed named
+    BaseObject convention. The allowed format includes a sequence of
+    (str, BaseObject instance) tuples. A dictionary with string names as keys
+    and BaseObject instances as values is also allowed if ``allow_dict is True``.
+
+    Parameters
+    ----------
+    seq_to_check : Sequence((str, BaseObject)) or Dict[str, BaseObject]
+        The input to check for conformance with the named object interface.
+        Conforming input are:
+
+        - Sequence that contains (str, BaseObject instance) tuples
+        - Dictionary with string names as keys and BaseObject instances as values
+          if ``allow_dict=True``
+
+    allow_dict : bool, default=True
+        Whether a dictionary of named objects is allowed as conforming named object
+        type.
+
+        - If True, then a dictionary with string keys and BaseObject instances
+          is allowed format for providing a sequence of named objects.
+        - If False, then only sequences that contain (str, BaseObject instance)
+          tuples are considered conforming with the named object parameter API.
+
+    require_unique_names : bool, default=False
+        Whether names used in the sequence of named BaseObject instances
+        must be unique.
+
+        - If True and the names are not unique, then False is always returned.
+        - If False, then whether or not the function returns True or False
+          depends on whether `seq_to_check` follows sequence of named BaseObject format.
+
+    object_type : class or tuple[class], default=None
+        The class type(s) that is used to ensure that all elements of named objects
+        match the expected type.
+    sequence_name : str, default=None
+        Optional name used to refer to the input `seq_to_check` when
+        raising any errors. Ignored ``raise_error=False``.
+
+    Returns
+    -------
+    Sequence((str, BaseObject)) or Dict[str, BaseObject]
+        The `seq_to_check` is returned if it is a conforming named object type.
+
+        - If ``allow_dict=True`` then return type is Sequence((str, BaseObject))
+          or Dict[str, BaseObject]
+        - If ``allow_dict=False`` then return type is Sequence((str, BaseObject))
+
+    Raises
+    ------
+    ValueError
+        If `seq_to_check` does not conform to the named BaseObject API.
+
+    See Also
+    --------
+    is_named_object_tuple :
+        Indicate (True/False) if input follows the named object API format for
+        a single named object (e.g., tupe[str, expected class type]).
+    is_sequence_named_objects :
+        Indicate (True/False) if an input sequence follows the named object API.
+
+    Examples
+    --------
+    >>> from skbase.base import BaseObject, BaseEstimator
+    >>> from skbase.validate import check_sequence_named_objects
+    >>> named_objects = [("Step 1", BaseObject()), ("Step 2", BaseObject())]
+    >>> check_sequence_named_objects(named_objects)
+    [('Step 1', BaseObject()), ('Step 2', BaseObject())]
+
+    Dictionaries are optionally allowed as sequences of named BaseObjects
+
+    >>> named_objects = {"Step 1": BaseObject(), "Step 2": BaseObject()}
+    >>> check_sequence_named_objects(named_objects)
+    {'Step 1': BaseObject(), 'Step 2': BaseObject()}
+
+    Raises error since dictionaries are not allowed when allow_dict is False
+
+    >>> check_sequence_named_objects(named_objects, allow_dict=False) # doctest: +SKIP
+
+    Raises error due to invalid format due to object names not being strings
+
+    >>> incorrectly_named_objects = [(1, BaseObject()), (2, BaseObject())]
+    >>> check_sequence_named_objects(incorrectly_named_objects)  # doctest: +SKIP
+
+    Raises error due to invalid format since named items are not BaseObject instances
+
+    >>> named_items = [("1", 7), ("2", 42)]
+    >>> check_sequence_named_objects(named_items)  # doctest: +SKIP
+
+    The validation can require the object elements to be a certain class type
+
+    >>> named_objects = [("Step 1", BaseObject()), ("Step 2", BaseObject())]
+    >>> check_sequence_named_objects( \
+    named_objects, object_type=BaseEstimator) # doctest: +SKIP
+    >>> named_objects = [("Step 1", BaseEstimator()), ("Step 2", BaseEstimator())]
+    >>> check_sequence_named_objects(named_objects, object_type=BaseEstimator)
+    [('Step 1', BaseEstimator()), ('Step 2', BaseEstimator())]
+    """
+    is_expected_format = is_sequence_named_objects(
+        seq_to_check,
+        allow_dict=allow_dict,
+        require_unique_names=require_unique_names,
+        object_type=object_type,
+    )
+    # Raise error is format is not expected.
+    if not is_expected_format:
+        msg = _named_baseobject_error_msg(
+            sequence_name=sequence_name, allow_dict=allow_dict
+        )
+        raise ValueError(msg)
+
+    return seq_to_check
```

### Comparing `skbase-0.4.5/skbase/validate/_types.py` & `skbase-0.4.6/skbase/validate/_types.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,345 +1,345 @@
-#!/usr/bin/env python3 -u
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tools for validating types."""
-import collections
-import inspect
-from typing import Any, List, Optional, Sequence, Tuple, Union
-
-from skbase.utils._iter import _format_seq_to_str, _remove_type_text, _scalar_to_seq
-
-__author__: List[str] = ["RNKuhns", "fkiraly"]
-__all__: List[str] = ["check_sequence", "check_type", "is_sequence"]
-
-
-def check_type(
-    input_: Any,
-    expected_type: type,
-    allow_none: bool = False,
-    input_name: Optional[str] = None,
-    use_subclass: bool = False,
-) -> Any:
-    """Check the input is the expected type.
-
-    Validates that the input is the type specified in `expected_type`, while optionally
-    allowing None values as well (if ``allow_none=True``). For flexibility,
-    the check can use ``issubclass`` instead of ``isinstance`` if ``use_subclass=True``.
-
-    Parameters
-    ----------
-    input_ : Any
-        The input to be type checked.
-    expected_type : type
-        The type that `input_` is expected to be.
-    allow_none : bool, default=False
-        Whether `input_` can be None in addition to being instance of `expected_type`.
-    input_name : str, default=None
-        The name to use when referring to `input_` in any raised error messages.
-        If None, then "input" is used as `input_name`.
-    use_subclass : bool, default=False
-        Whether to check the type using issubclass instead of isinstance.
-
-        - If True, then check uses issubclass.
-        - If False (default), then check uses isinstance.
-
-    Returns
-    -------
-    Any
-        The input object.
-
-    Raises
-    ------
-    TypeError
-        If input does match expected type using isinstance by default
-        or using issubclass in check if ``use_subclass=True``.
-
-    Examples
-    --------
-    >>> from skbase.base import BaseEstimator, BaseObject
-    >>> from skbase.validate import check_type
-    >>> check_type(7, expected_type=int)
-    7
-    >>> check_type(7.2, expected_type=(int, float))
-    7.2
-    >>> check_type(BaseEstimator(), BaseObject)
-    BaseEstimator()
-    >>> check_type(BaseEstimator, expected_type=BaseObject, use_subclass=True)
-    <class 'skbase.base._base.BaseEstimator'>
-
-    An error is raised if the input is not the expected type
-
-    >>> check_type(7, expected_type=str) # doctest: +SKIP
-    TypeError: `input` should be type <class 'str'>, but found <class 'str'>.
-    """
-    # process expected_type parameter
-    if not isinstance(expected_type, (type, tuple)):
-        msg = " ".join(
-            [
-                "`expected_type` should be type or tuple[type, ...],"
-                f"but found {_remove_type_text(expected_type)}."
-            ]
-        )
-        raise TypeError(msg)
-
-    # Assign default name to input_name parameter in case it is None
-    if input_name is None:
-        input_name = "input"
-
-    # Check the type of input_
-    type_check = issubclass if use_subclass else isinstance
-    if (allow_none and input_ is None) or type_check(input_, expected_type):
-        return input_
-    else:
-        chk_msg = "subclass type" if use_subclass else "be type"
-        expected_type_str = _remove_type_text(expected_type)
-        input_type_str = _remove_type_text(type(input_))
-        if allow_none:
-            type_msg = f"{expected_type_str} or None"
-        else:
-            type_msg = f"{expected_type_str}"
-        raise TypeError(
-            f"`{input_name}` should {chk_msg} {type_msg}, but found {input_type_str}."
-        )
-
-
-def _convert_scalar_seq_type_input_to_tuple(
-    type_input: Optional[Union[type, Tuple[type, ...]]],
-    none_default: Optional[type] = None,
-    type_input_subclass: Optional[type] = None,
-    input_name: str = None,
-) -> Tuple[type, ...]:
-    """Convert input that is scalar or sequence of types to always be a tuple."""
-    if none_default is None:
-        none_default = collections.abc.Sequence
-
-    seq_output: Tuple[type, ...]
-    if type_input is None:
-        seq_output = (none_default,)
-    # if a sequence of types received as sequence_type, convert to tuple of types
-    elif isinstance(type_input, collections.abc.Sequence) and all(
-        isinstance(e, type) for e in type_input
-    ):
-        seq_output = tuple(type_input)
-    elif (isinstance(type_input, type) or inspect.isclass(type_input)) and (
-        type_input_subclass is None or issubclass(type_input, type_input_subclass)
-    ):
-        seq_output = (type_input,)
-    else:
-        name_str = "type_input" if input_name is None else input_name
-        raise TypeError(f"`{name_str}` should be a type or tuple of types.")
-
-    return seq_output
-
-
-def is_sequence(
-    input_seq: Any,
-    sequence_type: Optional[Union[type, Tuple[type, ...]]] = None,
-    element_type: Optional[Union[type, Tuple[type, ...]]] = None,
-) -> bool:
-    """Indicate if an object is a sequence with optional check of element types.
-
-    If `element_type` is supplied all elements are also checked against provided types.
-
-    Parameters
-    ----------
-    input_seq : Any
-        The input sequence to be validated.
-    sequence_type : type or tuple[type, ...], default=None
-        The allowed sequence type(s) that `input_seq` can be an instance of.
-
-        - If None, then collections.abc.Sequence is used (all sequence types are valid)
-        - If `sequence_type` is a type or tuple of types, then only the specified
-          types are considered valid.
-
-    element_type : type or tuple[type], default=None
-        The allowed type(s) for elements of `input_seq`.
-
-        - If None, then the elements of `input_seq` are not checked when determining
-          if `input_seq` is a valid sequence.
-        - If `element_type` is a type or tuple of types, then the elements of
-          `input_seq` are checked to make sure they are all instances of
-          the supplied `element_type`.
-
-    Returns
-    -------
-    bool
-        Whether the input is a valid sequence based on the supplied `sequence_type`
-        and `element_type`.
-
-    Examples
-    --------
-    >>> from skbase.base import BaseEstimator, BaseObject
-    >>> from skbase.validate import is_sequence
-    >>> is_sequence([1, 2, 3])
-    True
-    >>> is_sequence(7)
-    False
-
-    Generators are not sequences
-
-    >>> is_sequence((c for c in [1, 2, 3]))
-    False
-
-    The expected sequence type can be included in the check
-
-    >>> is_sequence([1, 2, 3, 4], sequence_type=list)
-    True
-    >>> is_sequence([1, 2, 3, 4], sequence_type=tuple)
-    False
-
-    The type of the elements can also be checked
-
-    >>> is_sequence([1, 2, 3], element_type=int)
-    True
-    >>> is_sequence([1, 2, 3, 4], sequence_type=list, element_type=int)
-    True
-    >>> is_sequence([1, 2, 3, 4], sequence_type=list, element_type=float)
-    False
-    >>> is_sequence([1, 2, 3, 4], sequence_type=list, element_type=(int, float))
-    True
-    >>> is_sequence((BaseObject(), BaseEstimator()), element_type=BaseObject)
-    True
-    """
-    sequence_type_ = _convert_scalar_seq_type_input_to_tuple(
-        sequence_type,
-        input_name="sequence_type",
-        type_input_subclass=collections.abc.Sequence,
-    )
-
-    is_valid_sequence = isinstance(input_seq, sequence_type_)
-
-    # Optionally verify elements have correct types
-    if element_type is not None:
-        element_type_ = _convert_scalar_seq_type_input_to_tuple(
-            element_type, input_name="element_type"
-        )
-        element_types_okay = all(isinstance(e, element_type_) for e in input_seq)
-        if not element_types_okay:
-            is_valid_sequence = False
-
-    return is_valid_sequence
-
-
-def check_sequence(
-    input_seq: Sequence[Any],
-    sequence_type: Optional[Union[type, Tuple[type, ...]]] = None,
-    element_type: Optional[Union[type, Tuple[type, ...]]] = None,
-    coerce_output_type_to: type = None,
-    coerce_scalar_input: bool = False,
-    sequence_name: str = None,
-) -> Sequence[Any]:
-    """Check whether an object is a sequence with optional check of element types.
-
-    If `element_type` is supplied all elements are also checked against provided types.
-
-    Parameters
-    ----------
-    input_seq : Any
-        The input sequence to be validated.
-    sequence_type : type or tuple[type], default=None
-        The allowed sequence type that `seq` can be an instance of.
-    element_type : type or tuple[type], default=None
-        The allowed type(s) for elements of `seq`.
-    coerce_output_type_to : sequence type
-        The sequence type that the output sequence should be coerced to.
-
-        - If None, then the output sequence is the same as input sequence.
-        - If a sequence type (e.g., list, tuple) is provided then the output sequence
-          is coerced to that type.
-
-    coerce_scalar_input : bool, default=False
-        Whether scalar input should be coerced to a sequence type prior to running
-        the check. If True, a scalar input like will be coerced to a tuple containing
-        a single scalar. To output a sequence type other than a tuple, set the
-        `coerce_output_type_to` keyword to the desired sequence type (e.g., list).
-    sequence_name : str, default=None
-        Name of `input_seq` to use if error messages are raised.
-
-    Returns
-    -------
-    Sequence
-        The input sequence if has expected type.
-
-    Raises
-    ------
-    TypeError :
-        If `seq` is not instance of `sequence_type` or ``element_type is not None`` and
-        all elements are not instances of `element_type`.
-
-    Examples
-    --------
-    >>> from skbase.base import BaseEstimator, BaseObject
-    >>> from skbase.validate import is_sequence
-
-    >>> check_sequence([1, 2, 3])
-    [1, 2, 3]
-
-    Generators are not sequences so an error is raised
-
-    >>> check_sequence((c for c in [1, 2, 3])) # doctest: +SKIP
-
-    The check can require a certain type of sequence
-
-    >>> check_sequence([1, 2, 3, 4], sequence_type=list)
-    [1, 2, 3, 4]
-
-    Expected to raise and error because the input is not a tuple
-
-    >>> check_sequence([1, 2, 3, 4], sequence_type=tuple) # doctest: +SKIP
-
-    It is also possible to check the type of sequence elements
-
-    >>> check_sequence([1, 2, 3], element_type=int)
-    [1, 2, 3]
-    >>> check_sequence([1, 2, 3, 4], sequence_type=list, element_type=(int, float))
-    [1, 2, 3, 4]
-
-    The check also works with BaseObjects
-
-    >>> check_sequence((BaseObject(), BaseEstimator()), element_type=BaseObject)
-    (BaseObject(), BaseEstimator())
-    """
-    if coerce_scalar_input:
-        if isinstance(sequence_type, tuple):
-            # If multiple sequence types allowed then use first one
-            input_seq = _scalar_to_seq(input_seq, sequence_type=sequence_type[0])
-        else:
-            input_seq = _scalar_to_seq(input_seq, sequence_type=sequence_type)
-
-    is_valid_seqeunce = is_sequence(
-        input_seq,
-        sequence_type=sequence_type,
-        element_type=element_type,
-    )
-    # Raise error is format is not expected.
-    if not is_valid_seqeunce:
-        name_str = "Input sequence" if sequence_name is None else f"`{sequence_name}`"
-        if sequence_type is None:
-            seq_str = "a sequence"
-        else:
-            sequence_type_ = _convert_scalar_seq_type_input_to_tuple(
-                sequence_type,
-                input_name="sequence_type",
-                type_input_subclass=collections.abc.Sequence,
-            )
-            seq_str = _format_seq_to_str(
-                sequence_type_, last_sep="or", remove_type_text=True
-            )
-
-        msg = f"Invalid sequence: {name_str} expected to be a {seq_str}."
-
-        if element_type is not None:
-            element_type_ = _convert_scalar_seq_type_input_to_tuple(
-                element_type, input_name="element_type"
-            )
-            element_str = _format_seq_to_str(
-                element_type_, last_sep="or", remove_type_text=True
-            )
-            msg = msg[:-1] + f" with elements of type {element_str}."
-
-        raise TypeError(msg)
-
-    if coerce_output_type_to is not None:
-        return coerce_output_type_to(input_seq)
-
-    return input_seq
+#!/usr/bin/env python3 -u
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tools for validating types."""
+import collections
+import inspect
+from typing import Any, List, Optional, Sequence, Tuple, Union
+
+from skbase.utils._iter import _format_seq_to_str, _remove_type_text, _scalar_to_seq
+
+__author__: List[str] = ["RNKuhns", "fkiraly"]
+__all__: List[str] = ["check_sequence", "check_type", "is_sequence"]
+
+
+def check_type(
+    input_: Any,
+    expected_type: type,
+    allow_none: bool = False,
+    input_name: Optional[str] = None,
+    use_subclass: bool = False,
+) -> Any:
+    """Check the input is the expected type.
+
+    Validates that the input is the type specified in `expected_type`, while optionally
+    allowing None values as well (if ``allow_none=True``). For flexibility,
+    the check can use ``issubclass`` instead of ``isinstance`` if ``use_subclass=True``.
+
+    Parameters
+    ----------
+    input_ : Any
+        The input to be type checked.
+    expected_type : type
+        The type that `input_` is expected to be.
+    allow_none : bool, default=False
+        Whether `input_` can be None in addition to being instance of `expected_type`.
+    input_name : str, default=None
+        The name to use when referring to `input_` in any raised error messages.
+        If None, then "input" is used as `input_name`.
+    use_subclass : bool, default=False
+        Whether to check the type using issubclass instead of isinstance.
+
+        - If True, then check uses issubclass.
+        - If False (default), then check uses isinstance.
+
+    Returns
+    -------
+    Any
+        The input object.
+
+    Raises
+    ------
+    TypeError
+        If input does match expected type using isinstance by default
+        or using issubclass in check if ``use_subclass=True``.
+
+    Examples
+    --------
+    >>> from skbase.base import BaseEstimator, BaseObject
+    >>> from skbase.validate import check_type
+    >>> check_type(7, expected_type=int)
+    7
+    >>> check_type(7.2, expected_type=(int, float))
+    7.2
+    >>> check_type(BaseEstimator(), BaseObject)
+    BaseEstimator()
+    >>> check_type(BaseEstimator, expected_type=BaseObject, use_subclass=True)
+    <class 'skbase.base._base.BaseEstimator'>
+
+    An error is raised if the input is not the expected type
+
+    >>> check_type(7, expected_type=str) # doctest: +SKIP
+    TypeError: `input` should be type <class 'str'>, but found <class 'str'>.
+    """
+    # process expected_type parameter
+    if not isinstance(expected_type, (type, tuple)):
+        msg = " ".join(
+            [
+                "`expected_type` should be type or tuple[type, ...],"
+                f"but found {_remove_type_text(expected_type)}."
+            ]
+        )
+        raise TypeError(msg)
+
+    # Assign default name to input_name parameter in case it is None
+    if input_name is None:
+        input_name = "input"
+
+    # Check the type of input_
+    type_check = issubclass if use_subclass else isinstance
+    if (allow_none and input_ is None) or type_check(input_, expected_type):
+        return input_
+    else:
+        chk_msg = "subclass type" if use_subclass else "be type"
+        expected_type_str = _remove_type_text(expected_type)
+        input_type_str = _remove_type_text(type(input_))
+        if allow_none:
+            type_msg = f"{expected_type_str} or None"
+        else:
+            type_msg = f"{expected_type_str}"
+        raise TypeError(
+            f"`{input_name}` should {chk_msg} {type_msg}, but found {input_type_str}."
+        )
+
+
+def _convert_scalar_seq_type_input_to_tuple(
+    type_input: Optional[Union[type, Tuple[type, ...]]],
+    none_default: Optional[type] = None,
+    type_input_subclass: Optional[type] = None,
+    input_name: str = None,
+) -> Tuple[type, ...]:
+    """Convert input that is scalar or sequence of types to always be a tuple."""
+    if none_default is None:
+        none_default = collections.abc.Sequence
+
+    seq_output: Tuple[type, ...]
+    if type_input is None:
+        seq_output = (none_default,)
+    # if a sequence of types received as sequence_type, convert to tuple of types
+    elif isinstance(type_input, collections.abc.Sequence) and all(
+        isinstance(e, type) for e in type_input
+    ):
+        seq_output = tuple(type_input)
+    elif (isinstance(type_input, type) or inspect.isclass(type_input)) and (
+        type_input_subclass is None or issubclass(type_input, type_input_subclass)
+    ):
+        seq_output = (type_input,)
+    else:
+        name_str = "type_input" if input_name is None else input_name
+        raise TypeError(f"`{name_str}` should be a type or tuple of types.")
+
+    return seq_output
+
+
+def is_sequence(
+    input_seq: Any,
+    sequence_type: Optional[Union[type, Tuple[type, ...]]] = None,
+    element_type: Optional[Union[type, Tuple[type, ...]]] = None,
+) -> bool:
+    """Indicate if an object is a sequence with optional check of element types.
+
+    If `element_type` is supplied all elements are also checked against provided types.
+
+    Parameters
+    ----------
+    input_seq : Any
+        The input sequence to be validated.
+    sequence_type : type or tuple[type, ...], default=None
+        The allowed sequence type(s) that `input_seq` can be an instance of.
+
+        - If None, then collections.abc.Sequence is used (all sequence types are valid)
+        - If `sequence_type` is a type or tuple of types, then only the specified
+          types are considered valid.
+
+    element_type : type or tuple[type], default=None
+        The allowed type(s) for elements of `input_seq`.
+
+        - If None, then the elements of `input_seq` are not checked when determining
+          if `input_seq` is a valid sequence.
+        - If `element_type` is a type or tuple of types, then the elements of
+          `input_seq` are checked to make sure they are all instances of
+          the supplied `element_type`.
+
+    Returns
+    -------
+    bool
+        Whether the input is a valid sequence based on the supplied `sequence_type`
+        and `element_type`.
+
+    Examples
+    --------
+    >>> from skbase.base import BaseEstimator, BaseObject
+    >>> from skbase.validate import is_sequence
+    >>> is_sequence([1, 2, 3])
+    True
+    >>> is_sequence(7)
+    False
+
+    Generators are not sequences
+
+    >>> is_sequence((c for c in [1, 2, 3]))
+    False
+
+    The expected sequence type can be included in the check
+
+    >>> is_sequence([1, 2, 3, 4], sequence_type=list)
+    True
+    >>> is_sequence([1, 2, 3, 4], sequence_type=tuple)
+    False
+
+    The type of the elements can also be checked
+
+    >>> is_sequence([1, 2, 3], element_type=int)
+    True
+    >>> is_sequence([1, 2, 3, 4], sequence_type=list, element_type=int)
+    True
+    >>> is_sequence([1, 2, 3, 4], sequence_type=list, element_type=float)
+    False
+    >>> is_sequence([1, 2, 3, 4], sequence_type=list, element_type=(int, float))
+    True
+    >>> is_sequence((BaseObject(), BaseEstimator()), element_type=BaseObject)
+    True
+    """
+    sequence_type_ = _convert_scalar_seq_type_input_to_tuple(
+        sequence_type,
+        input_name="sequence_type",
+        type_input_subclass=collections.abc.Sequence,
+    )
+
+    is_valid_sequence = isinstance(input_seq, sequence_type_)
+
+    # Optionally verify elements have correct types
+    if element_type is not None:
+        element_type_ = _convert_scalar_seq_type_input_to_tuple(
+            element_type, input_name="element_type"
+        )
+        element_types_okay = all(isinstance(e, element_type_) for e in input_seq)
+        if not element_types_okay:
+            is_valid_sequence = False
+
+    return is_valid_sequence
+
+
+def check_sequence(
+    input_seq: Sequence[Any],
+    sequence_type: Optional[Union[type, Tuple[type, ...]]] = None,
+    element_type: Optional[Union[type, Tuple[type, ...]]] = None,
+    coerce_output_type_to: type = None,
+    coerce_scalar_input: bool = False,
+    sequence_name: str = None,
+) -> Sequence[Any]:
+    """Check whether an object is a sequence with optional check of element types.
+
+    If `element_type` is supplied all elements are also checked against provided types.
+
+    Parameters
+    ----------
+    input_seq : Any
+        The input sequence to be validated.
+    sequence_type : type or tuple[type], default=None
+        The allowed sequence type that `seq` can be an instance of.
+    element_type : type or tuple[type], default=None
+        The allowed type(s) for elements of `seq`.
+    coerce_output_type_to : sequence type
+        The sequence type that the output sequence should be coerced to.
+
+        - If None, then the output sequence is the same as input sequence.
+        - If a sequence type (e.g., list, tuple) is provided then the output sequence
+          is coerced to that type.
+
+    coerce_scalar_input : bool, default=False
+        Whether scalar input should be coerced to a sequence type prior to running
+        the check. If True, a scalar input like will be coerced to a tuple containing
+        a single scalar. To output a sequence type other than a tuple, set the
+        `coerce_output_type_to` keyword to the desired sequence type (e.g., list).
+    sequence_name : str, default=None
+        Name of `input_seq` to use if error messages are raised.
+
+    Returns
+    -------
+    Sequence
+        The input sequence if has expected type.
+
+    Raises
+    ------
+    TypeError :
+        If `seq` is not instance of `sequence_type` or ``element_type is not None`` and
+        all elements are not instances of `element_type`.
+
+    Examples
+    --------
+    >>> from skbase.base import BaseEstimator, BaseObject
+    >>> from skbase.validate import is_sequence
+
+    >>> check_sequence([1, 2, 3])
+    [1, 2, 3]
+
+    Generators are not sequences so an error is raised
+
+    >>> check_sequence((c for c in [1, 2, 3])) # doctest: +SKIP
+
+    The check can require a certain type of sequence
+
+    >>> check_sequence([1, 2, 3, 4], sequence_type=list)
+    [1, 2, 3, 4]
+
+    Expected to raise and error because the input is not a tuple
+
+    >>> check_sequence([1, 2, 3, 4], sequence_type=tuple) # doctest: +SKIP
+
+    It is also possible to check the type of sequence elements
+
+    >>> check_sequence([1, 2, 3], element_type=int)
+    [1, 2, 3]
+    >>> check_sequence([1, 2, 3, 4], sequence_type=list, element_type=(int, float))
+    [1, 2, 3, 4]
+
+    The check also works with BaseObjects
+
+    >>> check_sequence((BaseObject(), BaseEstimator()), element_type=BaseObject)
+    (BaseObject(), BaseEstimator())
+    """
+    if coerce_scalar_input:
+        if isinstance(sequence_type, tuple):
+            # If multiple sequence types allowed then use first one
+            input_seq = _scalar_to_seq(input_seq, sequence_type=sequence_type[0])
+        else:
+            input_seq = _scalar_to_seq(input_seq, sequence_type=sequence_type)
+
+    is_valid_seqeunce = is_sequence(
+        input_seq,
+        sequence_type=sequence_type,
+        element_type=element_type,
+    )
+    # Raise error is format is not expected.
+    if not is_valid_seqeunce:
+        name_str = "Input sequence" if sequence_name is None else f"`{sequence_name}`"
+        if sequence_type is None:
+            seq_str = "a sequence"
+        else:
+            sequence_type_ = _convert_scalar_seq_type_input_to_tuple(
+                sequence_type,
+                input_name="sequence_type",
+                type_input_subclass=collections.abc.Sequence,
+            )
+            seq_str = _format_seq_to_str(
+                sequence_type_, last_sep="or", remove_type_text=True
+            )
+
+        msg = f"Invalid sequence: {name_str} expected to be a {seq_str}."
+
+        if element_type is not None:
+            element_type_ = _convert_scalar_seq_type_input_to_tuple(
+                element_type, input_name="element_type"
+            )
+            element_str = _format_seq_to_str(
+                element_type_, last_sep="or", remove_type_text=True
+            )
+            msg = msg[:-1] + f" with elements of type {element_str}."
+
+        raise TypeError(msg)
+
+    if coerce_output_type_to is not None:
+        return coerce_output_type_to(input_seq)
+
+    return input_seq
```

### Comparing `skbase-0.4.5/skbase/validate/tests/test_iterable_named_objects.py` & `skbase-0.4.6/skbase/validate/tests/test_iterable_named_objects.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,200 +1,200 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tests of the functionality for validating iterables of named objects.
-
-tests in this module include:
-
-- test_is_named_object_tuple_output
-- test_is_sequence_named_objects_output
-- test_check_sequence_named_objects_output
-"""
-
-__author__ = ["RNKuhns"]
-import pytest
-
-from skbase.base import BaseEstimator, BaseObject
-from skbase.validate import (
-    check_sequence_named_objects,
-    is_named_object_tuple,
-    is_sequence_named_objects,
-)
-
-
-@pytest.fixture
-def fixture_object_instance():
-    """Pytest fixture of BaseObject instance."""
-    return BaseObject()
-
-
-@pytest.fixture
-def fixture_estimator_instance():
-    """Pytest fixture of BaseEstimator instance."""
-    return BaseEstimator()
-
-
-def test_is_named_object_tuple_output(
-    fixture_estimator_instance, fixture_object_instance
-):
-    """Test is_named_object_tuple returns expected value."""
-    # Default checks for object to be an instance of BaseOBject
-    assert is_named_object_tuple(("Step 1", fixture_object_instance)) is True
-    assert is_named_object_tuple(("Step 2", fixture_estimator_instance)) is True
-
-    # If a different `object_type` is provided then it is used in the isinstance check
-
-    assert (
-        is_named_object_tuple(
-            ("Step 1", fixture_object_instance), object_type=BaseEstimator
-        )
-        is False
-    )
-    assert (
-        is_named_object_tuple(
-            ("Step 1", fixture_estimator_instance), object_type=BaseEstimator
-        )
-        is True
-    )
-
-    # If the input is does not follow named object tuple format then False is returned
-    # This checks for named object tuples, so dictionary input is not allowed
-    assert is_named_object_tuple({"Step 1": fixture_estimator_instance}) is False
-    # First element of tuple must be string
-    assert is_named_object_tuple((1, fixture_object_instance)) is False
-
-
-def test_is_sequence_named_objects_output(
-    fixture_estimator_instance, fixture_object_instance
-):
-    """Test is_sequence_named_objects returns expected value."""
-    # Correctly formatted iterables of (name, BaseObject instance) tuples
-    named_objects = [
-        ("Step 1", fixture_estimator_instance),
-        ("Step 2", fixture_object_instance),
-    ]
-    assert is_sequence_named_objects(named_objects) is True
-    assert is_sequence_named_objects(tuple(named_objects)) is True
-
-    # Test correct format, but duplicate names
-    named_objects = [
-        ("Step 1", fixture_estimator_instance),
-        ("Step 1", fixture_object_instance),
-    ]
-    assert is_sequence_named_objects(named_objects) is True
-    assert is_sequence_named_objects(tuple(named_objects)) is True
-    # Tests with correctly formatted dictionary
-    dict_named_objects = {
-        "Step 1": fixture_estimator_instance,
-        "Step 2": fixture_object_instance,
-    }
-    assert is_sequence_named_objects(dict_named_objects) is True
-    assert is_sequence_named_objects(dict_named_objects, allow_dict=False) is False
-
-    # Invalid format due to object names not being strings
-    incorrectly_named_objects = [
-        (1, fixture_estimator_instance),
-        (2, fixture_object_instance),
-    ]
-    assert is_sequence_named_objects(incorrectly_named_objects) is False
-
-    # Invalid format due to named items not being BaseObject instances
-    named_items = [("1", 7), ("2", 42)]
-    assert is_sequence_named_objects(named_items) is False
-    dict_named_objects = {"Step 1": 7, "Step 2": 42}
-    assert is_sequence_named_objects(dict_named_objects) is False
-
-    # Invalid because input is not a sequence
-    non_sequence = 7
-    assert is_sequence_named_objects(non_sequence) is False
-
-    # Generators are also invalid since they don't have length or ability
-    # to access individual elements, we don't includein the named object API
-    named_objects = [
-        ("Step 1", fixture_estimator_instance),
-        ("Step 2", fixture_object_instance),
-    ]
-    assert is_sequence_named_objects(c for c in named_objects) is False
-
-    # Validate use of object_type parameter
-    # Won't work because one named object is a BaseObject but not a BaseEstimator
-    assert is_sequence_named_objects(named_objects, object_type=BaseEstimator) is False
-
-    # Should work because we allow BaseObject or BaseEstimator types
-    named_objects = [("Step 1", BaseEstimator()), ("Step 2", BaseEstimator())]
-    assert (
-        is_sequence_named_objects(
-            named_objects, object_type=(BaseObject, BaseEstimator)
-        )
-        is True
-    )
-    assert is_sequence_named_objects(named_objects, object_type=BaseEstimator) is True
-
-
-def test_check_sequence_named_objects_output(
-    fixture_estimator_instance, fixture_object_instance
-):
-    """Test check_sequence_named_objects returns expected value."""
-    # Correctly formatted iterables of (name, BaseObject instance) tuples
-    named_objects = [
-        ("Step 1", fixture_estimator_instance),
-        ("Step 2", fixture_object_instance),
-    ]
-    assert check_sequence_named_objects(named_objects) == named_objects
-    assert check_sequence_named_objects(tuple(named_objects)) == tuple(named_objects)
-
-    # Tests with correctly formatted dictionary
-    dict_named_objects = {
-        "Step 1": fixture_estimator_instance,
-        "Step 2": fixture_object_instance,
-    }
-    assert check_sequence_named_objects(dict_named_objects) == dict_named_objects
-    # Raises an error if we don't allow dicts as part of named object API
-    with pytest.raises(ValueError):
-        check_sequence_named_objects(dict_named_objects, allow_dict=False)
-
-    # Invalid format due to object names not being strings
-    incorrectly_named_objects = [
-        (1, fixture_estimator_instance),
-        (2, fixture_object_instance),
-    ]
-    with pytest.raises(ValueError):
-        check_sequence_named_objects(incorrectly_named_objects)
-
-    # Invalid format due to named items not being BaseObject instances
-    named_items = [("1", 7), ("2", 42)]
-    with pytest.raises(ValueError):
-        check_sequence_named_objects(named_items)
-    dict_named_objects = {"Step 1": 7, "Step 2": 42}
-    with pytest.raises(ValueError):
-        check_sequence_named_objects(dict_named_objects)
-
-    # Invalid due to not being sequences
-    non_sequence = 7
-    with pytest.raises(ValueError):
-        check_sequence_named_objects(non_sequence)
-
-    # Generators are also invalid since they don't have length or ability
-    # to access individual elements, we don't includein the named object API
-    named_objects = [
-        ("Step 1", fixture_estimator_instance),
-        ("Step 2", fixture_object_instance),
-    ]
-    with pytest.raises(ValueError):
-        check_sequence_named_objects(c for c in named_objects)
-
-    # Validate use of object_type parameter
-    # Won't work because one named object is a BaseObject but not a BaseEstimator
-    with pytest.raises(ValueError):
-        check_sequence_named_objects(named_objects, object_type=BaseEstimator)
-
-    # Should work because we allow BaseObject or BaseEstimator types
-    named_objects = [("Step 1", BaseEstimator()), ("Step 2", BaseEstimator())]
-    assert (
-        check_sequence_named_objects(
-            named_objects, object_type=(BaseObject, BaseEstimator)
-        )
-        == named_objects
-    )
-    assert (
-        check_sequence_named_objects(named_objects, object_type=BaseEstimator)
-        == named_objects
-    )
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tests of the functionality for validating iterables of named objects.
+
+tests in this module include:
+
+- test_is_named_object_tuple_output
+- test_is_sequence_named_objects_output
+- test_check_sequence_named_objects_output
+"""
+
+__author__ = ["RNKuhns"]
+import pytest
+
+from skbase.base import BaseEstimator, BaseObject
+from skbase.validate import (
+    check_sequence_named_objects,
+    is_named_object_tuple,
+    is_sequence_named_objects,
+)
+
+
+@pytest.fixture
+def fixture_object_instance():
+    """Pytest fixture of BaseObject instance."""
+    return BaseObject()
+
+
+@pytest.fixture
+def fixture_estimator_instance():
+    """Pytest fixture of BaseEstimator instance."""
+    return BaseEstimator()
+
+
+def test_is_named_object_tuple_output(
+    fixture_estimator_instance, fixture_object_instance
+):
+    """Test is_named_object_tuple returns expected value."""
+    # Default checks for object to be an instance of BaseOBject
+    assert is_named_object_tuple(("Step 1", fixture_object_instance)) is True
+    assert is_named_object_tuple(("Step 2", fixture_estimator_instance)) is True
+
+    # If a different `object_type` is provided then it is used in the isinstance check
+
+    assert (
+        is_named_object_tuple(
+            ("Step 1", fixture_object_instance), object_type=BaseEstimator
+        )
+        is False
+    )
+    assert (
+        is_named_object_tuple(
+            ("Step 1", fixture_estimator_instance), object_type=BaseEstimator
+        )
+        is True
+    )
+
+    # If the input is does not follow named object tuple format then False is returned
+    # This checks for named object tuples, so dictionary input is not allowed
+    assert is_named_object_tuple({"Step 1": fixture_estimator_instance}) is False
+    # First element of tuple must be string
+    assert is_named_object_tuple((1, fixture_object_instance)) is False
+
+
+def test_is_sequence_named_objects_output(
+    fixture_estimator_instance, fixture_object_instance
+):
+    """Test is_sequence_named_objects returns expected value."""
+    # Correctly formatted iterables of (name, BaseObject instance) tuples
+    named_objects = [
+        ("Step 1", fixture_estimator_instance),
+        ("Step 2", fixture_object_instance),
+    ]
+    assert is_sequence_named_objects(named_objects) is True
+    assert is_sequence_named_objects(tuple(named_objects)) is True
+
+    # Test correct format, but duplicate names
+    named_objects = [
+        ("Step 1", fixture_estimator_instance),
+        ("Step 1", fixture_object_instance),
+    ]
+    assert is_sequence_named_objects(named_objects) is True
+    assert is_sequence_named_objects(tuple(named_objects)) is True
+    # Tests with correctly formatted dictionary
+    dict_named_objects = {
+        "Step 1": fixture_estimator_instance,
+        "Step 2": fixture_object_instance,
+    }
+    assert is_sequence_named_objects(dict_named_objects) is True
+    assert is_sequence_named_objects(dict_named_objects, allow_dict=False) is False
+
+    # Invalid format due to object names not being strings
+    incorrectly_named_objects = [
+        (1, fixture_estimator_instance),
+        (2, fixture_object_instance),
+    ]
+    assert is_sequence_named_objects(incorrectly_named_objects) is False
+
+    # Invalid format due to named items not being BaseObject instances
+    named_items = [("1", 7), ("2", 42)]
+    assert is_sequence_named_objects(named_items) is False
+    dict_named_objects = {"Step 1": 7, "Step 2": 42}
+    assert is_sequence_named_objects(dict_named_objects) is False
+
+    # Invalid because input is not a sequence
+    non_sequence = 7
+    assert is_sequence_named_objects(non_sequence) is False
+
+    # Generators are also invalid since they don't have length or ability
+    # to access individual elements, we don't includein the named object API
+    named_objects = [
+        ("Step 1", fixture_estimator_instance),
+        ("Step 2", fixture_object_instance),
+    ]
+    assert is_sequence_named_objects(c for c in named_objects) is False
+
+    # Validate use of object_type parameter
+    # Won't work because one named object is a BaseObject but not a BaseEstimator
+    assert is_sequence_named_objects(named_objects, object_type=BaseEstimator) is False
+
+    # Should work because we allow BaseObject or BaseEstimator types
+    named_objects = [("Step 1", BaseEstimator()), ("Step 2", BaseEstimator())]
+    assert (
+        is_sequence_named_objects(
+            named_objects, object_type=(BaseObject, BaseEstimator)
+        )
+        is True
+    )
+    assert is_sequence_named_objects(named_objects, object_type=BaseEstimator) is True
+
+
+def test_check_sequence_named_objects_output(
+    fixture_estimator_instance, fixture_object_instance
+):
+    """Test check_sequence_named_objects returns expected value."""
+    # Correctly formatted iterables of (name, BaseObject instance) tuples
+    named_objects = [
+        ("Step 1", fixture_estimator_instance),
+        ("Step 2", fixture_object_instance),
+    ]
+    assert check_sequence_named_objects(named_objects) == named_objects
+    assert check_sequence_named_objects(tuple(named_objects)) == tuple(named_objects)
+
+    # Tests with correctly formatted dictionary
+    dict_named_objects = {
+        "Step 1": fixture_estimator_instance,
+        "Step 2": fixture_object_instance,
+    }
+    assert check_sequence_named_objects(dict_named_objects) == dict_named_objects
+    # Raises an error if we don't allow dicts as part of named object API
+    with pytest.raises(ValueError):
+        check_sequence_named_objects(dict_named_objects, allow_dict=False)
+
+    # Invalid format due to object names not being strings
+    incorrectly_named_objects = [
+        (1, fixture_estimator_instance),
+        (2, fixture_object_instance),
+    ]
+    with pytest.raises(ValueError):
+        check_sequence_named_objects(incorrectly_named_objects)
+
+    # Invalid format due to named items not being BaseObject instances
+    named_items = [("1", 7), ("2", 42)]
+    with pytest.raises(ValueError):
+        check_sequence_named_objects(named_items)
+    dict_named_objects = {"Step 1": 7, "Step 2": 42}
+    with pytest.raises(ValueError):
+        check_sequence_named_objects(dict_named_objects)
+
+    # Invalid due to not being sequences
+    non_sequence = 7
+    with pytest.raises(ValueError):
+        check_sequence_named_objects(non_sequence)
+
+    # Generators are also invalid since they don't have length or ability
+    # to access individual elements, we don't includein the named object API
+    named_objects = [
+        ("Step 1", fixture_estimator_instance),
+        ("Step 2", fixture_object_instance),
+    ]
+    with pytest.raises(ValueError):
+        check_sequence_named_objects(c for c in named_objects)
+
+    # Validate use of object_type parameter
+    # Won't work because one named object is a BaseObject but not a BaseEstimator
+    with pytest.raises(ValueError):
+        check_sequence_named_objects(named_objects, object_type=BaseEstimator)
+
+    # Should work because we allow BaseObject or BaseEstimator types
+    named_objects = [("Step 1", BaseEstimator()), ("Step 2", BaseEstimator())]
+    assert (
+        check_sequence_named_objects(
+            named_objects, object_type=(BaseObject, BaseEstimator)
+        )
+        == named_objects
+    )
+    assert (
+        check_sequence_named_objects(named_objects, object_type=BaseEstimator)
+        == named_objects
+    )
```

### Comparing `skbase-0.4.5/skbase/validate/tests/test_type_validations.py` & `skbase-0.4.6/skbase/validate/tests/test_type_validations.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,370 +1,370 @@
-# -*- coding: utf-8 -*-
-# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
-"""Tests of the functionality for validating iterables of named objects.
-
-tests in this module include:
-
-- test_check_type_output
-- test_check_type_raises_error_if_expected_type_is_wrong_format
-- test_is_sequence_output
-- test_is_sequence_with_seq_of_class_and_instance_input
-- test_check_sequence_output
-- test_check_sequence_scalar_input_coercion
-- test_check_sequence_with_seq_of_class_and_instance_input
-- test_convert_scalar_seq_type_input_to_tuple_raises_error
-"""
-import collections
-
-import numpy as np
-import pytest
-
-from skbase.base import BaseEstimator, BaseObject
-from skbase.validate import check_sequence, check_type, is_sequence
-from skbase.validate._types import _convert_scalar_seq_type_input_to_tuple
-
-__author__ = ["RNKuhns"]
-
-
-@pytest.fixture
-def fixture_object_instance():
-    """Pytest fixture of BaseObject instance."""
-    return BaseObject()
-
-
-@pytest.fixture
-def fixture_estimator_instance():
-    """Pytest fixture of BaseObject instance."""
-    return BaseEstimator()
-
-
-def test_check_type_output(fixture_estimator_instance, fixture_object_instance):
-    """Test check type returns expected output."""
-    assert check_type(7, expected_type=int) == 7
-    assert check_type(7.2, expected_type=float) == 7.2
-    assert check_type(7.2, expected_type=(float, int)) == 7.2
-    assert check_type("something", expected_type=str) == "something"
-    assert check_type(None, expected_type=str, allow_none=True) is None
-    assert check_type(["a", 7, fixture_object_instance], expected_type=list) == [
-        "a",
-        7,
-        fixture_object_instance,
-    ]
-    assert (
-        check_type(fixture_estimator_instance, expected_type=BaseObject)
-        == fixture_estimator_instance
-    )
-    assert check_type(None, expected_type=int, allow_none=True) is None
-
-    with pytest.raises(TypeError, match=r"`input` should be type.*"):
-        check_type(7.2, expected_type=int)
-
-    with pytest.raises(TypeError, match=r"`input` should be type.*"):
-        check_type("something", expected_type=(int, float))
-
-    with pytest.raises(TypeError, match=r"`input` should be type.*"):
-        check_type(BaseEstimator, expected_type=BaseObject)
-
-    with pytest.raises(TypeError, match="^`input` should be.*"):
-        check_type("something", expected_type=int, allow_none=True)
-
-    # Verify optional use of issubclass instead of isinstance
-    assert (
-        check_type(BaseEstimator, expected_type=BaseObject, use_subclass=True)
-        == BaseEstimator
-    )
-
-
-def test_check_type_raises_error_if_expected_type_is_wrong_format():
-    """Test check_type raises an error if expected_type wrong format.
-
-    `expected_type` should be a type or tuple of types.
-    """
-    with pytest.raises(TypeError, match="^`expected_type` should be.*"):
-        check_type(7, expected_type=11)
-
-    with pytest.raises(TypeError, match="^`expected_type` should be.*"):
-        check_type(7, expected_type=[int])
-
-    with pytest.raises(TypeError, match="^`expected_type` should be.*"):
-        check_type(None, expected_type=[int])
-
-
-def test_is_sequence_output():
-    """Test is_sequence returns expected output.
-
-    This excludes test of class and class instance usage, which is included in
-    test_is_sequence_with_seq_of_class_and_instance_input.
-    """
-    # Test simple example with no constraints on sequence_type or element_type
-    # True for any sequence
-    assert is_sequence([1, 2, 3]) is True
-    # But false for generators, since they are iterable but not sequences
-    assert is_sequence((c for c in [1, 2, 3])) is False
-
-    # Test use of sequence_type restriction
-    assert is_sequence([1, 2, 3, 4], sequence_type=list) is True
-    assert is_sequence([1, 2, 3, 4], sequence_type=tuple) is False
-    assert is_sequence((1, 2, 3, 4), sequence_type=list) is False
-    assert is_sequence((1, 2, 3, 4), sequence_type=tuple) is True
-
-    # Test use of element_type restriction
-    assert is_sequence([1, 2, 3], element_type=int) is True
-    assert is_sequence([1, 2, 3], element_type=float) is False
-    assert is_sequence([1, 2, 3, 4], sequence_type=list, element_type=int) is True
-    assert is_sequence([1, 2, 3, 4], sequence_type=tuple, element_type=int) is False
-    assert is_sequence([1, 2, 3, 4], sequence_type=list, element_type=float) is False
-    assert is_sequence([1, 2, 3, 4], sequence_type=tuple, element_type=float) is False
-
-    # Tests using different types
-    assert is_sequence("abc") is True  # strings are iterable and sequences in Python
-    assert is_sequence([1, "something", 4.5]) is True
-    assert is_sequence([1, "something", 4.5], element_type=float) is False
-    assert (
-        is_sequence(
-            ("a string", "or another string"), sequence_type=tuple, element_type=str
-        )
-        is True
-    )
-
-    # Test with 3rd party types works in default way via exact type
-    assert is_sequence([1.2, 4.7], element_type=np.float_) is False
-    assert is_sequence([np.float_(1.2), np.float_(4.7)], element_type=np.float_) is True
-
-    # np.nan is float, not int or np.float_
-    assert is_sequence([np.nan, 4.8], element_type=float) is True
-    assert is_sequence([np.nan, 4], element_type=int) is False
-
-
-def test_is_sequence_with_seq_of_class_and_instance_input(
-    fixture_estimator_instance, fixture_object_instance
-):
-    """Test is_sequence returns expected value with sequence of classes as input."""
-    # Verify we can identify sequences of a given class type as valid sequences
-    input_seq = (fixture_estimator_instance, fixture_object_instance)
-    assert is_sequence(input_seq, element_type=BaseObject) is True
-    assert (
-        is_sequence(list(input_seq), sequence_type=list, element_type=BaseObject)
-        is True
-    )
-    # Verify we detect when list elements are not instances of valid class type
-    assert is_sequence([1, 2, 3], element_type=BaseObject) is False
-
-    # Verify we can identify sequences of class types as valid sequences of types
-    input_seq = (BaseObject, BaseEstimator)
-    assert is_sequence(input_seq, element_type=type) is True
-    assert is_sequence(list(input_seq), sequence_type=list, element_type=type) is True
-    # Verify we detect when list elements are not instances of valid types
-    assert is_sequence([1, 2, 3], element_type=BaseObject) is False
-
-
-def test_check_sequence_output():
-    """Test check_sequence returns expected output.
-
-    This excludes test of class and class instance usage, which is included in
-    test_check_sequence_with_seq_of_class_and_instance_input.
-    """
-    # Test simple example with no constraints on sequence_type or element_type
-    # True for any sequence
-    assert check_sequence([1, 2, 3]) == [1, 2, 3]
-    assert check_sequence([1, "a", 3.4, False]) == [1, "a", 3.4, False]
-    # But false for generators, since they are iterable but not sequences
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: Input sequence expected to be a a sequence.",
-    ):
-        assert check_sequence((c for c in [1, 2, 3]))
-
-    # Test use of sequence_type restriction
-    assert check_sequence([1, 2, 3, 4], sequence_type=list) == [1, 2, 3, 4]
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: Input sequence expected to be a tuple.",
-    ):
-        check_sequence([1, 2, 3, 4], sequence_type=tuple)
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: Input sequence expected to be a list.",
-    ):
-        check_sequence((1, 2, 3, 4), sequence_type=list)
-    assert check_sequence((1, 2, 3, 4), sequence_type=tuple) == (1, 2, 3, 4)
-    assert check_sequence((1, 2, 3, 4), sequence_type=(list, tuple)) == (1, 2, 3, 4)
-
-    # Test use of element_type restriction
-    assert check_sequence([1, 2, 3], element_type=int) == [1, 2, 3]
-    assert check_sequence([1, 2, 3], element_type=(float, int)) == [1, 2, 3]
-    assert check_sequence([1, 2, False, "a", 3], element_type=(bool, str, int)) == [
-        1,
-        2,
-        False,
-        "a",
-        3,
-    ]
-
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        check_sequence([1, 2, 3], element_type=float)
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        check_sequence([1, 2, 3, 4], sequence_type=tuple, element_type=int)
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        check_sequence([1, 2, 3, 4], sequence_type=list, element_type=float)
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        check_sequence([1, 2, 3, 4], sequence_type=tuple, element_type=float)
-
-    input_seq = [1, 2, 3, 4]
-    assert check_sequence(input_seq, sequence_type=list, element_type=int) == input_seq
-
-    # Tests using different types
-    # strings are iterable and sequences in Python
-    assert check_sequence("abc") == "abc"
-    assert check_sequence([1, "something", 4.5]) == [1, "something", 4.5]
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        check_sequence([1, "something", 4.5], element_type=float)
-
-    assert check_sequence(
-        ("a string", "or another string"), sequence_type=tuple, element_type=str
-    ) == ("a string", "or another string")
-
-    # Test with 3rd party types works in default way via exact type
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        check_sequence([1.2, 4.7], element_type=np.float_)
-    input_seq = [np.float_(1.2), np.float_(4.7)]
-    assert check_sequence(input_seq, element_type=np.float_) == input_seq
-
-    # np.nan is float, not int or np.float_
-    assert check_sequence([np.nan, 4.8], element_type=float) == [np.nan, 4.8]
-    assert check_sequence([np.nan, 4.8, 7], element_type=(float, int)) == [
-        np.nan,
-        4.8,
-        7,
-    ]
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        check_sequence([np.nan, 4], element_type=int)
-
-    # Check return type coercion to specified sequence type
-    input_seq = [1, 2, 3, 4]
-    assert check_sequence(
-        input_seq, sequence_type=list, element_type=int, coerce_output_type_to=tuple
-    ) == tuple(input_seq)
-
-
-def test_check_sequence_scalar_input_coercion():
-    """Test check_sequence coerces scalar inputs to sequences as expected."""
-    assert check_sequence(7, element_type=int, coerce_scalar_input=True) == (7,)
-    assert check_sequence(
-        7, element_type=int, coerce_output_type_to=list, coerce_scalar_input=True
-    ) == [7]
-
-    # Note that single strings treated as scalars for this purpose
-    assert check_sequence(
-        "some string", element_type=str, coerce_scalar_input=True
-    ) == ("some string",)
-
-    # coercion takes into account allowed sequence_types
-    assert check_sequence(
-        7, element_type=int, sequence_type=list, coerce_scalar_input=True
-    ) == [7]
-    # If more than one sequence_type allowed then the first is used for coercion
-    assert check_sequence(
-        7, element_type=int, sequence_type=(list, tuple), coerce_scalar_input=True
-    ) == [7]
-    # Output type conversion overrides input type coercion to specified sequence_type
-    assert check_sequence(
-        7,
-        element_type=int,
-        sequence_type=list,
-        coerce_output_type_to=tuple,
-        coerce_scalar_input=True,
-    ) == (7,)
-
-    # Still raise an error if element type is not expected
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        check_sequence(
-            7,
-            sequence_type=list,
-            element_type=float,
-            coerce_scalar_input=True,
-        )
-
-
-def test_check_sequence_with_seq_of_class_and_instance_input(
-    fixture_estimator_instance, fixture_object_instance
-):
-    """Test check_sequence returns expected value with sequence of classes as input."""
-    # Verify we can identify sequences of a given class type as valid sequences
-    input_seq = (fixture_estimator_instance, fixture_object_instance)
-    assert check_sequence(input_seq, element_type=BaseObject) == input_seq
-    assert check_sequence(
-        list(input_seq), sequence_type=list, element_type=BaseObject
-    ) == list(input_seq)
-
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        check_sequence(list(input_seq), sequence_type=tuple, element_type=BaseObject)
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        # Verify we detect when list elements are not instances of valid class type
-        check_sequence([1, 2, 3], element_type=BaseObject)
-
-    # Verify we can identify sequences of class types as valid sequences of types
-    input_seq = (BaseObject, BaseEstimator)
-    assert check_sequence(input_seq, element_type=type) == input_seq
-    assert check_sequence(
-        list(input_seq), sequence_type=list, element_type=type
-    ) == list(input_seq)
-    with pytest.raises(
-        TypeError,
-        match="Invalid sequence: .*",
-    ):
-        # Verify we detect when list elements are not instances of valid types
-        check_sequence([1, 2, 3], element_type=BaseObject)
-
-
-def test_convert_scalar_seq_type_input_to_tuple_raises_error():
-    """Test _convert_scalar_seq_type_input_to_tuple raises error."""
-    # Raises because 7 is not a type
-    with pytest.raises(
-        TypeError, match=r"`type_input` should be a type or tuple of types."
-    ):
-        _convert_scalar_seq_type_input_to_tuple(7)
-
-    # Test error message uses input_name
-    with pytest.raises(
-        TypeError, match=r"`some_input` should be a type or tuple of types."
-    ):
-        _convert_scalar_seq_type_input_to_tuple(7, input_name="some_input")
-
-    # Raises error because dict is a type but not a subclass of type_input_subclass
-    with pytest.raises(
-        TypeError, match=r"`type_input` should be a type or tuple of types."
-    ):
-        _convert_scalar_seq_type_input_to_tuple(
-            dict,
-            type_input_subclass=collections.abc.Sequence,
-        )
+# -*- coding: utf-8 -*-
+# copyright: skbase developers, BSD-3-Clause License (see LICENSE file)
+"""Tests of the functionality for validating iterables of named objects.
+
+tests in this module include:
+
+- test_check_type_output
+- test_check_type_raises_error_if_expected_type_is_wrong_format
+- test_is_sequence_output
+- test_is_sequence_with_seq_of_class_and_instance_input
+- test_check_sequence_output
+- test_check_sequence_scalar_input_coercion
+- test_check_sequence_with_seq_of_class_and_instance_input
+- test_convert_scalar_seq_type_input_to_tuple_raises_error
+"""
+import collections
+
+import numpy as np
+import pytest
+
+from skbase.base import BaseEstimator, BaseObject
+from skbase.validate import check_sequence, check_type, is_sequence
+from skbase.validate._types import _convert_scalar_seq_type_input_to_tuple
+
+__author__ = ["RNKuhns"]
+
+
+@pytest.fixture
+def fixture_object_instance():
+    """Pytest fixture of BaseObject instance."""
+    return BaseObject()
+
+
+@pytest.fixture
+def fixture_estimator_instance():
+    """Pytest fixture of BaseObject instance."""
+    return BaseEstimator()
+
+
+def test_check_type_output(fixture_estimator_instance, fixture_object_instance):
+    """Test check type returns expected output."""
+    assert check_type(7, expected_type=int) == 7
+    assert check_type(7.2, expected_type=float) == 7.2
+    assert check_type(7.2, expected_type=(float, int)) == 7.2
+    assert check_type("something", expected_type=str) == "something"
+    assert check_type(None, expected_type=str, allow_none=True) is None
+    assert check_type(["a", 7, fixture_object_instance], expected_type=list) == [
+        "a",
+        7,
+        fixture_object_instance,
+    ]
+    assert (
+        check_type(fixture_estimator_instance, expected_type=BaseObject)
+        == fixture_estimator_instance
+    )
+    assert check_type(None, expected_type=int, allow_none=True) is None
+
+    with pytest.raises(TypeError, match=r"`input` should be type.*"):
+        check_type(7.2, expected_type=int)
+
+    with pytest.raises(TypeError, match=r"`input` should be type.*"):
+        check_type("something", expected_type=(int, float))
+
+    with pytest.raises(TypeError, match=r"`input` should be type.*"):
+        check_type(BaseEstimator, expected_type=BaseObject)
+
+    with pytest.raises(TypeError, match="^`input` should be.*"):
+        check_type("something", expected_type=int, allow_none=True)
+
+    # Verify optional use of issubclass instead of isinstance
+    assert (
+        check_type(BaseEstimator, expected_type=BaseObject, use_subclass=True)
+        == BaseEstimator
+    )
+
+
+def test_check_type_raises_error_if_expected_type_is_wrong_format():
+    """Test check_type raises an error if expected_type wrong format.
+
+    `expected_type` should be a type or tuple of types.
+    """
+    with pytest.raises(TypeError, match="^`expected_type` should be.*"):
+        check_type(7, expected_type=11)
+
+    with pytest.raises(TypeError, match="^`expected_type` should be.*"):
+        check_type(7, expected_type=[int])
+
+    with pytest.raises(TypeError, match="^`expected_type` should be.*"):
+        check_type(None, expected_type=[int])
+
+
+def test_is_sequence_output():
+    """Test is_sequence returns expected output.
+
+    This excludes test of class and class instance usage, which is included in
+    test_is_sequence_with_seq_of_class_and_instance_input.
+    """
+    # Test simple example with no constraints on sequence_type or element_type
+    # True for any sequence
+    assert is_sequence([1, 2, 3]) is True
+    # But false for generators, since they are iterable but not sequences
+    assert is_sequence((c for c in [1, 2, 3])) is False
+
+    # Test use of sequence_type restriction
+    assert is_sequence([1, 2, 3, 4], sequence_type=list) is True
+    assert is_sequence([1, 2, 3, 4], sequence_type=tuple) is False
+    assert is_sequence((1, 2, 3, 4), sequence_type=list) is False
+    assert is_sequence((1, 2, 3, 4), sequence_type=tuple) is True
+
+    # Test use of element_type restriction
+    assert is_sequence([1, 2, 3], element_type=int) is True
+    assert is_sequence([1, 2, 3], element_type=float) is False
+    assert is_sequence([1, 2, 3, 4], sequence_type=list, element_type=int) is True
+    assert is_sequence([1, 2, 3, 4], sequence_type=tuple, element_type=int) is False
+    assert is_sequence([1, 2, 3, 4], sequence_type=list, element_type=float) is False
+    assert is_sequence([1, 2, 3, 4], sequence_type=tuple, element_type=float) is False
+
+    # Tests using different types
+    assert is_sequence("abc") is True  # strings are iterable and sequences in Python
+    assert is_sequence([1, "something", 4.5]) is True
+    assert is_sequence([1, "something", 4.5], element_type=float) is False
+    assert (
+        is_sequence(
+            ("a string", "or another string"), sequence_type=tuple, element_type=str
+        )
+        is True
+    )
+
+    # Test with 3rd party types works in default way via exact type
+    assert is_sequence([1.2, 4.7], element_type=np.float_) is False
+    assert is_sequence([np.float_(1.2), np.float_(4.7)], element_type=np.float_) is True
+
+    # np.nan is float, not int or np.float_
+    assert is_sequence([np.nan, 4.8], element_type=float) is True
+    assert is_sequence([np.nan, 4], element_type=int) is False
+
+
+def test_is_sequence_with_seq_of_class_and_instance_input(
+    fixture_estimator_instance, fixture_object_instance
+):
+    """Test is_sequence returns expected value with sequence of classes as input."""
+    # Verify we can identify sequences of a given class type as valid sequences
+    input_seq = (fixture_estimator_instance, fixture_object_instance)
+    assert is_sequence(input_seq, element_type=BaseObject) is True
+    assert (
+        is_sequence(list(input_seq), sequence_type=list, element_type=BaseObject)
+        is True
+    )
+    # Verify we detect when list elements are not instances of valid class type
+    assert is_sequence([1, 2, 3], element_type=BaseObject) is False
+
+    # Verify we can identify sequences of class types as valid sequences of types
+    input_seq = (BaseObject, BaseEstimator)
+    assert is_sequence(input_seq, element_type=type) is True
+    assert is_sequence(list(input_seq), sequence_type=list, element_type=type) is True
+    # Verify we detect when list elements are not instances of valid types
+    assert is_sequence([1, 2, 3], element_type=BaseObject) is False
+
+
+def test_check_sequence_output():
+    """Test check_sequence returns expected output.
+
+    This excludes test of class and class instance usage, which is included in
+    test_check_sequence_with_seq_of_class_and_instance_input.
+    """
+    # Test simple example with no constraints on sequence_type or element_type
+    # True for any sequence
+    assert check_sequence([1, 2, 3]) == [1, 2, 3]
+    assert check_sequence([1, "a", 3.4, False]) == [1, "a", 3.4, False]
+    # But false for generators, since they are iterable but not sequences
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: Input sequence expected to be a a sequence.",
+    ):
+        assert check_sequence((c for c in [1, 2, 3]))
+
+    # Test use of sequence_type restriction
+    assert check_sequence([1, 2, 3, 4], sequence_type=list) == [1, 2, 3, 4]
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: Input sequence expected to be a tuple.",
+    ):
+        check_sequence([1, 2, 3, 4], sequence_type=tuple)
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: Input sequence expected to be a list.",
+    ):
+        check_sequence((1, 2, 3, 4), sequence_type=list)
+    assert check_sequence((1, 2, 3, 4), sequence_type=tuple) == (1, 2, 3, 4)
+    assert check_sequence((1, 2, 3, 4), sequence_type=(list, tuple)) == (1, 2, 3, 4)
+
+    # Test use of element_type restriction
+    assert check_sequence([1, 2, 3], element_type=int) == [1, 2, 3]
+    assert check_sequence([1, 2, 3], element_type=(float, int)) == [1, 2, 3]
+    assert check_sequence([1, 2, False, "a", 3], element_type=(bool, str, int)) == [
+        1,
+        2,
+        False,
+        "a",
+        3,
+    ]
+
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        check_sequence([1, 2, 3], element_type=float)
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        check_sequence([1, 2, 3, 4], sequence_type=tuple, element_type=int)
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        check_sequence([1, 2, 3, 4], sequence_type=list, element_type=float)
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        check_sequence([1, 2, 3, 4], sequence_type=tuple, element_type=float)
+
+    input_seq = [1, 2, 3, 4]
+    assert check_sequence(input_seq, sequence_type=list, element_type=int) == input_seq
+
+    # Tests using different types
+    # strings are iterable and sequences in Python
+    assert check_sequence("abc") == "abc"
+    assert check_sequence([1, "something", 4.5]) == [1, "something", 4.5]
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        check_sequence([1, "something", 4.5], element_type=float)
+
+    assert check_sequence(
+        ("a string", "or another string"), sequence_type=tuple, element_type=str
+    ) == ("a string", "or another string")
+
+    # Test with 3rd party types works in default way via exact type
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        check_sequence([1.2, 4.7], element_type=np.float_)
+    input_seq = [np.float_(1.2), np.float_(4.7)]
+    assert check_sequence(input_seq, element_type=np.float_) == input_seq
+
+    # np.nan is float, not int or np.float_
+    assert check_sequence([np.nan, 4.8], element_type=float) == [np.nan, 4.8]
+    assert check_sequence([np.nan, 4.8, 7], element_type=(float, int)) == [
+        np.nan,
+        4.8,
+        7,
+    ]
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        check_sequence([np.nan, 4], element_type=int)
+
+    # Check return type coercion to specified sequence type
+    input_seq = [1, 2, 3, 4]
+    assert check_sequence(
+        input_seq, sequence_type=list, element_type=int, coerce_output_type_to=tuple
+    ) == tuple(input_seq)
+
+
+def test_check_sequence_scalar_input_coercion():
+    """Test check_sequence coerces scalar inputs to sequences as expected."""
+    assert check_sequence(7, element_type=int, coerce_scalar_input=True) == (7,)
+    assert check_sequence(
+        7, element_type=int, coerce_output_type_to=list, coerce_scalar_input=True
+    ) == [7]
+
+    # Note that single strings treated as scalars for this purpose
+    assert check_sequence(
+        "some string", element_type=str, coerce_scalar_input=True
+    ) == ("some string",)
+
+    # coercion takes into account allowed sequence_types
+    assert check_sequence(
+        7, element_type=int, sequence_type=list, coerce_scalar_input=True
+    ) == [7]
+    # If more than one sequence_type allowed then the first is used for coercion
+    assert check_sequence(
+        7, element_type=int, sequence_type=(list, tuple), coerce_scalar_input=True
+    ) == [7]
+    # Output type conversion overrides input type coercion to specified sequence_type
+    assert check_sequence(
+        7,
+        element_type=int,
+        sequence_type=list,
+        coerce_output_type_to=tuple,
+        coerce_scalar_input=True,
+    ) == (7,)
+
+    # Still raise an error if element type is not expected
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        check_sequence(
+            7,
+            sequence_type=list,
+            element_type=float,
+            coerce_scalar_input=True,
+        )
+
+
+def test_check_sequence_with_seq_of_class_and_instance_input(
+    fixture_estimator_instance, fixture_object_instance
+):
+    """Test check_sequence returns expected value with sequence of classes as input."""
+    # Verify we can identify sequences of a given class type as valid sequences
+    input_seq = (fixture_estimator_instance, fixture_object_instance)
+    assert check_sequence(input_seq, element_type=BaseObject) == input_seq
+    assert check_sequence(
+        list(input_seq), sequence_type=list, element_type=BaseObject
+    ) == list(input_seq)
+
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        check_sequence(list(input_seq), sequence_type=tuple, element_type=BaseObject)
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        # Verify we detect when list elements are not instances of valid class type
+        check_sequence([1, 2, 3], element_type=BaseObject)
+
+    # Verify we can identify sequences of class types as valid sequences of types
+    input_seq = (BaseObject, BaseEstimator)
+    assert check_sequence(input_seq, element_type=type) == input_seq
+    assert check_sequence(
+        list(input_seq), sequence_type=list, element_type=type
+    ) == list(input_seq)
+    with pytest.raises(
+        TypeError,
+        match="Invalid sequence: .*",
+    ):
+        # Verify we detect when list elements are not instances of valid types
+        check_sequence([1, 2, 3], element_type=BaseObject)
+
+
+def test_convert_scalar_seq_type_input_to_tuple_raises_error():
+    """Test _convert_scalar_seq_type_input_to_tuple raises error."""
+    # Raises because 7 is not a type
+    with pytest.raises(
+        TypeError, match=r"`type_input` should be a type or tuple of types."
+    ):
+        _convert_scalar_seq_type_input_to_tuple(7)
+
+    # Test error message uses input_name
+    with pytest.raises(
+        TypeError, match=r"`some_input` should be a type or tuple of types."
+    ):
+        _convert_scalar_seq_type_input_to_tuple(7, input_name="some_input")
+
+    # Raises error because dict is a type but not a subclass of type_input_subclass
+    with pytest.raises(
+        TypeError, match=r"`type_input` should be a type or tuple of types."
+    ):
+        _convert_scalar_seq_type_input_to_tuple(
+            dict,
+            type_input_subclass=collections.abc.Sequence,
+        )
```

### Comparing `skbase-0.4.5/skbase.egg-info/PKG-INFO` & `skbase-0.4.6/skbase.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,406 +1,426 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 736b 6261  : 2.1.Name: skba
-00000020: 7365 0a56 6572 7369 6f6e 3a20 302e 342e  se.Version: 0.4.
-00000030: 350a 5375 6d6d 6172 793a 2042 6173 6520  5.Summary: Base 
-00000040: 636c 6173 7365 7320 666f 7220 736b 6c65  classes for skle
-00000050: 6172 6e2d 6c69 6b65 2070 6172 616d 6574  arn-like paramet
-00000060: 7269 6320 6f62 6a65 6374 730a 4175 7468  ric objects.Auth
-00000070: 6f72 3a20 4672 616e 7a20 4b69 72c3 a16c  or: Franz Kir..l
-00000080: 792c 204d 6172 6b75 7320 4cc3 b66e 696e  y, Markus L..nin
-00000090: 672c 2052 7961 6e20 4b75 686e 730a 4d61  g, Ryan Kuhns.Ma
-000000a0: 696e 7461 696e 6572 2d65 6d61 696c 3a20  intainer-email: 
-000000b0: 4672 616e 7a20 4b69 7261 6c79 203c 662e  Franz Kiraly <f.
-000000c0: 6b69 7261 6c79 4075 636c 2e61 632e 756b  kiraly@ucl.ac.uk
-000000d0: 3e2c 2052 7961 6e20 4b75 686e 7320 3c72  >, Ryan Kuhns <r
-000000e0: 6b2e 736b 6261 7365 4067 6d61 696c 2e63  k.skbase@gmail.c
-000000f0: 6f6d 3e0a 4c69 6365 6e73 653a 2042 5344  om>.License: BSD
-00000100: 2033 2d43 6c61 7573 6520 4c69 6365 6e73   3-Clause Licens
-00000110: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
-00000120: 2020 2043 6f70 7972 6967 6874 2028 6329     Copyright (c)
-00000130: 2032 3032 322c 2073 6b62 6173 6520 4465   2022, skbase De
-00000140: 7665 6c6f 7065 7273 0a20 2020 2020 2020  velopers.       
-00000150: 2041 6c6c 2072 6967 6874 7320 7265 7365   All rights rese
-00000160: 7276 6564 2e0a 2020 2020 2020 2020 0a20  rved..        . 
-00000170: 2020 2020 2020 2052 6564 6973 7472 6962         Redistrib
-00000180: 7574 696f 6e20 616e 6420 7573 6520 696e  ution and use in
-00000190: 2073 6f75 7263 6520 616e 6420 6269 6e61   source and bina
-000001a0: 7279 2066 6f72 6d73 2c20 7769 7468 206f  ry forms, with o
-000001b0: 7220 7769 7468 6f75 740a 2020 2020 2020  r without.      
-000001c0: 2020 6d6f 6469 6669 6361 7469 6f6e 2c20    modification, 
-000001d0: 6172 6520 7065 726d 6974 7465 6420 7072  are permitted pr
-000001e0: 6f76 6964 6564 2074 6861 7420 7468 6520  ovided that the 
-000001f0: 666f 6c6c 6f77 696e 6720 636f 6e64 6974  following condit
-00000200: 696f 6e73 2061 7265 206d 6574 3a0a 2020  ions are met:.  
-00000210: 2020 2020 2020 0a20 2020 2020 2020 2031        .        1
-00000220: 2e20 5265 6469 7374 7269 6275 7469 6f6e  . Redistribution
-00000230: 7320 6f66 2073 6f75 7263 6520 636f 6465  s of source code
-00000240: 206d 7573 7420 7265 7461 696e 2074 6865   must retain the
-00000250: 2061 626f 7665 2063 6f70 7972 6967 6874   above copyright
-00000260: 206e 6f74 6963 652c 2074 6869 730a 2020   notice, this.  
-00000270: 2020 2020 2020 2020 206c 6973 7420 6f66           list of
-00000280: 2063 6f6e 6469 7469 6f6e 7320 616e 6420   conditions and 
-00000290: 7468 6520 666f 6c6c 6f77 696e 6720 6469  the following di
-000002a0: 7363 6c61 696d 6572 2e0a 2020 2020 2020  sclaimer..      
-000002b0: 2020 0a20 2020 2020 2020 2032 2e20 5265    .        2. Re
-000002c0: 6469 7374 7269 6275 7469 6f6e 7320 696e  distributions in
-000002d0: 2062 696e 6172 7920 666f 726d 206d 7573   binary form mus
-000002e0: 7420 7265 7072 6f64 7563 6520 7468 6520  t reproduce the 
-000002f0: 6162 6f76 6520 636f 7079 7269 6768 7420  above copyright 
-00000300: 6e6f 7469 6365 2c0a 2020 2020 2020 2020  notice,.        
-00000310: 2020 2074 6869 7320 6c69 7374 206f 6620     this list of 
-00000320: 636f 6e64 6974 696f 6e73 2061 6e64 2074  conditions and t
-00000330: 6865 2066 6f6c 6c6f 7769 6e67 2064 6973  he following dis
-00000340: 636c 6169 6d65 7220 696e 2074 6865 2064  claimer in the d
-00000350: 6f63 756d 656e 7461 7469 6f6e 0a20 2020  ocumentation.   
-00000360: 2020 2020 2020 2020 616e 642f 6f72 206f          and/or o
-00000370: 7468 6572 206d 6174 6572 6961 6c73 2070  ther materials p
-00000380: 726f 7669 6465 6420 7769 7468 2074 6865  rovided with the
-00000390: 2064 6973 7472 6962 7574 696f 6e2e 0a20   distribution.. 
-000003a0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000003b0: 332e 204e 6569 7468 6572 2074 6865 206e  3. Neither the n
-000003c0: 616d 6520 6f66 2074 6865 2063 6f70 7972  ame of the copyr
-000003d0: 6967 6874 2068 6f6c 6465 7220 6e6f 7220  ight holder nor 
-000003e0: 7468 6520 6e61 6d65 7320 6f66 2069 7473  the names of its
-000003f0: 0a20 2020 2020 2020 2020 2020 636f 6e74  .           cont
-00000400: 7269 6275 746f 7273 206d 6179 2062 6520  ributors may be 
-00000410: 7573 6564 2074 6f20 656e 646f 7273 6520  used to endorse 
-00000420: 6f72 2070 726f 6d6f 7465 2070 726f 6475  or promote produ
-00000430: 6374 7320 6465 7269 7665 6420 6672 6f6d  cts derived from
-00000440: 0a20 2020 2020 2020 2020 2020 7468 6973  .           this
-00000450: 2073 6f66 7477 6172 6520 7769 7468 6f75   software withou
-00000460: 7420 7370 6563 6966 6963 2070 7269 6f72  t specific prior
-00000470: 2077 7269 7474 656e 2070 6572 6d69 7373   written permiss
-00000480: 696f 6e2e 0a20 2020 2020 2020 200a 2020  ion..        .  
-00000490: 2020 2020 2020 5448 4953 2053 4f46 5457        THIS SOFTW
-000004a0: 4152 4520 4953 2050 524f 5649 4445 4420  ARE IS PROVIDED 
-000004b0: 4259 2054 4845 2043 4f50 5952 4947 4854  BY THE COPYRIGHT
-000004c0: 2048 4f4c 4445 5253 2041 4e44 2043 4f4e   HOLDERS AND CON
-000004d0: 5452 4942 5554 4f52 5320 2241 5320 4953  TRIBUTORS "AS IS
-000004e0: 220a 2020 2020 2020 2020 414e 4420 414e  ".        AND AN
-000004f0: 5920 4558 5052 4553 5320 4f52 2049 4d50  Y EXPRESS OR IMP
-00000500: 4c49 4544 2057 4152 5241 4e54 4945 532c  LIED WARRANTIES,
-00000510: 2049 4e43 4c55 4449 4e47 2c20 4255 5420   INCLUDING, BUT 
-00000520: 4e4f 5420 4c49 4d49 5445 4420 544f 2c20  NOT LIMITED TO, 
-00000530: 5448 450a 2020 2020 2020 2020 494d 504c  THE.        IMPL
-00000540: 4945 4420 5741 5252 414e 5449 4553 204f  IED WARRANTIES O
-00000550: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
-00000560: 5920 414e 4420 4649 544e 4553 5320 464f  Y AND FITNESS FO
-00000570: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
-00000580: 5552 504f 5345 2041 5245 0a20 2020 2020  URPOSE ARE.     
-00000590: 2020 2044 4953 434c 4149 4d45 442e 2049     DISCLAIMED. I
-000005a0: 4e20 4e4f 2045 5645 4e54 2053 4841 4c4c  N NO EVENT SHALL
-000005b0: 2054 4845 2043 4f50 5952 4947 4854 2048   THE COPYRIGHT H
-000005c0: 4f4c 4445 5220 4f52 2043 4f4e 5452 4942  OLDER OR CONTRIB
-000005d0: 5554 4f52 5320 4245 204c 4941 424c 450a  UTORS BE LIABLE.
-000005e0: 2020 2020 2020 2020 464f 5220 414e 5920          FOR ANY 
-000005f0: 4449 5245 4354 2c20 494e 4449 5245 4354  DIRECT, INDIRECT
-00000600: 2c20 494e 4349 4445 4e54 414c 2c20 5350  , INCIDENTAL, SP
-00000610: 4543 4941 4c2c 2045 5845 4d50 4c41 5259  ECIAL, EXEMPLARY
-00000620: 2c20 4f52 2043 4f4e 5345 5155 454e 5449  , OR CONSEQUENTI
-00000630: 414c 0a20 2020 2020 2020 2044 414d 4147  AL.        DAMAG
-00000640: 4553 2028 494e 434c 5544 494e 472c 2042  ES (INCLUDING, B
-00000650: 5554 204e 4f54 204c 494d 4954 4544 2054  UT NOT LIMITED T
-00000660: 4f2c 2050 524f 4355 5245 4d45 4e54 204f  O, PROCUREMENT O
-00000670: 4620 5355 4253 5449 5455 5445 2047 4f4f  F SUBSTITUTE GOO
-00000680: 4453 204f 520a 2020 2020 2020 2020 5345  DS OR.        SE
-00000690: 5256 4943 4553 3b20 4c4f 5353 204f 4620  RVICES; LOSS OF 
-000006a0: 5553 452c 2044 4154 412c 204f 5220 5052  USE, DATA, OR PR
-000006b0: 4f46 4954 533b 204f 5220 4255 5349 4e45  OFITS; OR BUSINE
-000006c0: 5353 2049 4e54 4552 5255 5054 494f 4e29  SS INTERRUPTION)
-000006d0: 2048 4f57 4556 4552 0a20 2020 2020 2020   HOWEVER.       
-000006e0: 2043 4155 5345 4420 414e 4420 4f4e 2041   CAUSED AND ON A
-000006f0: 4e59 2054 4845 4f52 5920 4f46 204c 4941  NY THEORY OF LIA
-00000700: 4249 4c49 5459 2c20 5748 4554 4845 5220  BILITY, WHETHER 
-00000710: 494e 2043 4f4e 5452 4143 542c 2053 5452  IN CONTRACT, STR
-00000720: 4943 5420 4c49 4142 494c 4954 592c 0a20  ICT LIABILITY,. 
-00000730: 2020 2020 2020 204f 5220 544f 5254 2028         OR TORT (
-00000740: 494e 434c 5544 494e 4720 4e45 474c 4947  INCLUDING NEGLIG
-00000750: 454e 4345 204f 5220 4f54 4845 5257 4953  ENCE OR OTHERWIS
-00000760: 4529 2041 5249 5349 4e47 2049 4e20 414e  E) ARISING IN AN
-00000770: 5920 5741 5920 4f55 5420 4f46 2054 4845  Y WAY OUT OF THE
-00000780: 2055 5345 0a20 2020 2020 2020 204f 4620   USE.        OF 
-00000790: 5448 4953 2053 4f46 5457 4152 452c 2045  THIS SOFTWARE, E
-000007a0: 5645 4e20 4946 2041 4456 4953 4544 204f  VEN IF ADVISED O
-000007b0: 4620 5448 4520 504f 5353 4942 494c 4954  F THE POSSIBILIT
-000007c0: 5920 4f46 2053 5543 4820 4441 4d41 4745  Y OF SUCH DAMAGE
-000007d0: 2e0a 2020 2020 2020 2020 0a50 726f 6a65  ..        .Proje
-000007e0: 6374 2d55 524c 3a20 686f 6d65 7061 6765  ct-URL: homepage
-000007f0: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000800: 2e63 6f6d 2f73 6b74 696d 652f 736b 6261  .com/sktime/skba
-00000810: 7365 0a50 726f 6a65 6374 2d55 524c 3a20  se.Project-URL: 
-00000820: 7265 706f 7369 746f 7279 2c20 6874 7470  repository, http
-00000830: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
-00000840: 6b74 696d 652f 736b 6261 7365 0a50 726f  ktime/skbase.Pro
-00000850: 6a65 6374 2d55 524c 3a20 646f 6375 6d65  ject-URL: docume
-00000860: 6e74 6174 696f 6e2c 2068 7474 7073 3a2f  ntation, https:/
-00000870: 2f67 6974 6875 622e 636f 6d2f 736b 7469  /github.com/skti
-00000880: 6d65 2f73 6b62 6173 650a 5072 6f6a 6563  me/skbase.Projec
-00000890: 742d 5552 4c3a 2064 6f77 6e6c 6f61 642c  t-URL: download,
-000008a0: 2068 7474 7073 3a2f 2f70 7970 692e 6f72   https://pypi.or
-000008b0: 672f 7072 6f6a 6563 742f 736b 6261 7365  g/project/skbase
-000008c0: 2f23 6669 6c65 730a 4b65 7977 6f72 6473  /#files.Keywords
-000008d0: 3a20 6461 7461 2d73 6369 656e 6365 2c6d  : data-science,m
-000008e0: 6163 6869 6e65 2d6c 6561 726e 696e 672c  achine-learning,
-000008f0: 7363 696b 6974 2d6c 6561 726e 0a43 6c61  scikit-learn.Cla
-00000900: 7373 6966 6965 723a 2049 6e74 656e 6465  ssifier: Intende
-00000910: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
-00000920: 6965 6e63 652f 5265 7365 6172 6368 0a43  ience/Research.C
-00000930: 6c61 7373 6966 6965 723a 2049 6e74 656e  lassifier: Inten
-00000940: 6465 6420 4175 6469 656e 6365 203a 3a20  ded Audience :: 
-00000950: 4465 7665 6c6f 7065 7273 0a43 6c61 7373  Developers.Class
-00000960: 6966 6965 723a 204c 6963 656e 7365 203a  ifier: License :
-00000970: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000980: 3a20 4253 4420 4c69 6365 6e73 650a 436c  : BSD License.Cl
-00000990: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-000009a0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000009b0: 3a20 5079 7468 6f6e 0a43 6c61 7373 6966  : Python.Classif
-000009c0: 6965 723a 2054 6f70 6963 203a 3a20 536f  ier: Topic :: So
-000009d0: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
-000009e0: 6e74 0a43 6c61 7373 6966 6965 723a 2054  nt.Classifier: T
-000009f0: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-00000a00: 6963 2f45 6e67 696e 6565 7269 6e67 0a43  ic/Engineering.C
-00000a10: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-00000a20: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
-00000a30: 6963 726f 736f 6674 203a 3a20 5769 6e64  icrosoft :: Wind
-00000a40: 6f77 730a 436c 6173 7369 6669 6572 3a20  ows.Classifier: 
-00000a50: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000a60: 203a 3a20 504f 5349 580a 436c 6173 7369   :: POSIX.Classi
-00000a70: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
-00000a80: 5379 7374 656d 203a 3a20 556e 6978 0a43  System :: Unix.C
-00000a90: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-00000aa0: 7469 6e67 2053 7973 7465 6d20 3a3a 204d  ting System :: M
-00000ab0: 6163 4f53 0a43 6c61 7373 6966 6965 723a  acOS.Classifier:
-00000ac0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-00000ad0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000ae0: 3a3a 2033 2e37 0a43 6c61 7373 6966 6965  :: 3.7.Classifie
-00000af0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000b00: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000b10: 6e20 3a3a 2033 2e38 0a43 6c61 7373 6966  n :: 3.8.Classif
-00000b20: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-00000b30: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-00000b40: 686f 6e20 3a3a 2033 2e39 0a43 6c61 7373  hon :: 3.9.Class
-00000b50: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-00000b60: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000b70: 7974 686f 6e20 3a3a 2033 2e31 300a 436c  ython :: 3.10.Cl
-00000b80: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000b90: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000ba0: 3a20 5079 7468 6f6e 203a 3a20 332e 3131  : Python :: 3.11
-00000bb0: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-00000bc0: 3a20 3c33 2e31 322c 3e3d 332e 370a 4465  : <3.12,>=3.7.De
-00000bd0: 7363 7269 7074 696f 6e2d 436f 6e74 656e  scription-Conten
-00000be0: 742d 5479 7065 3a20 7465 7874 2f6d 6172  t-Type: text/mar
-00000bf0: 6b64 6f77 6e0a 5072 6f76 6964 6573 2d45  kdown.Provides-E
-00000c00: 7874 7261 3a20 616c 6c5f 6578 7472 6173  xtra: all_extras
-00000c10: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00000c20: 2064 6576 0a50 726f 7669 6465 732d 4578   dev.Provides-Ex
-00000c30: 7472 613a 206c 696e 7465 7273 0a50 726f  tra: linters.Pro
-00000c40: 7669 6465 732d 4578 7472 613a 2062 696e  vides-Extra: bin
-00000c50: 6465 720a 5072 6f76 6964 6573 2d45 7874  der.Provides-Ext
-00000c60: 7261 3a20 646f 6373 0a50 726f 7669 6465  ra: docs.Provide
-00000c70: 732d 4578 7472 613a 2074 6573 740a 4c69  s-Extra: test.Li
-00000c80: 6365 6e73 652d 4669 6c65 3a20 4c49 4345  cense-File: LICE
-00000c90: 4e53 450a 0a0a 2320 5765 6c63 6f6d 6520  NSE...# Welcome 
-00000ca0: 746f 2073 6b62 6173 650a 0a3e 2041 2062  to skbase..> A b
-00000cb0: 6173 6520 636c 6173 7320 666f 7220 7363  ase class for sc
-00000cc0: 696b 6974 2d6c 6561 726e 2d6c 696b 6520  ikit-learn-like 
-00000cd0: 616e 6420 736b 7469 6d65 2d6c 696b 6520  and sktime-like 
-00000ce0: 7061 7261 6d65 7472 6963 206f 626a 6563  parametric objec
-00000cf0: 7473 0a0a 6073 6b62 6173 6560 2070 726f  ts..`skbase` pro
-00000d00: 7669 6465 7320 6261 7365 2063 6c61 7373  vides base class
-00000d10: 6573 2066 6f72 2063 7265 6174 696e 6720  es for creating 
-00000d20: 7363 696b 6974 2d6c 6561 726e 2d6c 696b  scikit-learn-lik
-00000d30: 6520 7061 7261 6d65 7472 6963 206f 626a  e parametric obj
-00000d40: 6563 7473 2c0a 616c 6f6e 6720 7769 7468  ects,.along with
-00000d50: 2074 6f6f 6c73 2074 6f20 6d61 6b65 2069   tools to make i
-00000d60: 7420 6561 7369 6572 2074 6f20 6275 696c  t easier to buil
-00000d70: 6420 796f 7572 206f 776e 2070 6163 6b61  d your own packa
-00000d80: 6765 7320 7468 6174 2066 6f6c 6c6f 7720  ges that follow 
-00000d90: 7468 6573 650a 6465 7369 676e 2070 6174  these.design pat
-00000da0: 7465 726e 732e 0a0a 3a72 6f63 6b65 743a  terns...:rocket:
-00000db0: 2056 6572 7369 6f6e 2030 2e34 2e35 2069   Version 0.4.5 i
-00000dc0: 7320 6e6f 7720 6176 6169 6c61 626c 652e  s now available.
-00000dd0: 2043 6865 636b 6f75 7420 6f75 720a 5b72   Checkout our.[r
-00000de0: 656c 6561 7365 206e 6f74 6573 5d28 6874  elease notes](ht
-00000df0: 7470 733a 2f2f 736b 6261 7365 2e72 6561  tps://skbase.rea
-00000e00: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00000e10: 6174 6573 742f 6368 616e 6765 6c6f 672e  atest/changelog.
-00000e20: 6874 6d6c 292e 0a0a 7c20 4f76 6572 7669  html)...| Overvi
-00000e30: 6577 207c 207c 0a7c 2d2d 2d7c 2d2d 2d7c  ew | |.|---|---|
-00000e40: 0a7c 202a 2a43 492f 4344 2a2a 207c 205b  .| **CI/CD** | [
-00000e50: 215b 5465 7374 735d 2868 7474 7073 3a2f  ![Tests](https:/
-00000e60: 2f67 6974 6875 622e 636f 6d2f 736b 7469  /github.com/skti
-00000e70: 6d65 2f73 6b62 6173 652f 6163 7469 6f6e  me/skbase/action
-00000e80: 732f 776f 726b 666c 6f77 732f 7465 7374  s/workflows/test
-00000e90: 2e79 6d6c 2f62 6164 6765 2e73 7667 3f62  .yml/badge.svg?b
-00000ea0: 7261 6e63 683d 6d61 696e 295d 2868 7474  ranch=main)](htt
-00000eb0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000ec0: 736b 7469 6d65 2f73 6b62 6173 652f 6163  sktime/skbase/ac
-00000ed0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-00000ee0: 7465 7374 2e79 6d6c 2920 5b21 5b63 6f64  test.yml) [![cod
-00000ef0: 6563 6f76 5d28 6874 7470 733a 2f2f 636f  ecov](https://co
-00000f00: 6465 636f 762e 696f 2f67 682f 736b 7469  decov.io/gh/skti
-00000f10: 6d65 2f73 6b62 6173 652f 6272 616e 6368  me/skbase/branch
-00000f20: 2f6d 6169 6e2f 6772 6170 682f 6261 6467  /main/graph/badg
-00000f30: 652e 7376 673f 746f 6b65 6e3d 324a 3432  e.svg?token=2J42
-00000f40: 344e 4c4f 3832 295d 2868 7474 7073 3a2f  4NLO82)](https:/
-00000f50: 2f63 6f64 6563 6f76 2e69 6f2f 6768 2f73  /codecov.io/gh/s
-00000f60: 6b74 696d 652f 736b 6261 7365 2920 5b21  ktime/skbase) [!
-00000f70: 5b44 6f63 756d 656e 7461 7469 6f6e 2053  [Documentation S
-00000f80: 7461 7475 735d 2868 7474 7073 3a2f 2f72  tatus](https://r
-00000f90: 6561 6474 6865 646f 6373 2e6f 7267 2f70  eadthedocs.org/p
-00000fa0: 726f 6a65 6374 732f 736b 6261 7365 2f62  rojects/skbase/b
-00000fb0: 6164 6765 2f3f 7665 7273 696f 6e3d 6c61  adge/?version=la
-00000fc0: 7465 7374 295d 2868 7474 7073 3a2f 2f73  test)](https://s
-00000fd0: 6b62 6173 652e 7265 6164 7468 6564 6f63  kbase.readthedoc
-00000fe0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f3f  s.io/en/latest/?
-00000ff0: 6261 6467 653d 6c61 7465 7374 2920 5b21  badge=latest) [!
-00001000: 5b70 7265 2d63 6f6d 6d69 742e 6369 2073  [pre-commit.ci s
-00001010: 7461 7475 735d 2868 7474 7073 3a2f 2f72  tatus](https://r
-00001020: 6573 756c 7473 2e70 7265 2d63 6f6d 6d69  esults.pre-commi
-00001030: 742e 6369 2f62 6164 6765 2f67 6974 6875  t.ci/badge/githu
-00001040: 622f 736b 7469 6d65 2f73 6b62 6173 652f  b/sktime/skbase/
-00001050: 6d61 696e 2e73 7667 295d 2868 7474 7073  main.svg)](https
-00001060: 3a2f 2f72 6573 756c 7473 2e70 7265 2d63  ://results.pre-c
-00001070: 6f6d 6d69 742e 6369 2f6c 6174 6573 742f  ommit.ci/latest/
-00001080: 6769 7468 7562 2f73 6b74 696d 652f 736b  github/sktime/sk
-00001090: 6261 7365 2f6d 6169 6e29 207c 0a7c 202a  base/main) |.| *
-000010a0: 2a43 6f64 652a 2a20 7c20 205b 215b 2170  *Code** |  [![!p
-000010b0: 7970 695d 2868 7474 7073 3a2f 2f69 6d67  ypi](https://img
-000010c0: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
-000010d0: 2f76 2f73 6369 6b69 742d 6261 7365 3f63  /v/scikit-base?c
-000010e0: 6f6c 6f72 3d6f 7261 6e67 6529 5d28 6874  olor=orange)](ht
-000010f0: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
-00001100: 726f 6a65 6374 2f73 6b62 6173 652f 2920  roject/skbase/) 
-00001110: 205b 215b 2170 7974 686f 6e2d 7665 7273   [![!python-vers
-00001120: 696f 6e73 5d28 6874 7470 733a 2f2f 696d  ions](https://im
-00001130: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-00001140: 692f 7079 7665 7273 696f 6e73 2f73 6369  i/pyversions/sci
-00001150: 6b69 742d 6261 7365 295d 2868 7474 7073  kit-base)](https
-00001160: 3a2f 2f77 7777 2e70 7974 686f 6e2e 6f72  ://www.python.or
-00001170: 672f 2920 5b21 5b21 626c 6163 6b5d 2868  g/) [![!black](h
-00001180: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00001190: 6473 2e69 6f2f 6261 6467 652f 636f 6465  ds.io/badge/code
-000011a0: 2532 3073 7479 6c65 2d62 6c61 636b 2d30  %20style-black-0
-000011b0: 3030 3030 302e 7376 6729 5d28 6874 7470  00000.svg)](http
-000011c0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f70  s://github.com/p
-000011d0: 7366 2f62 6c61 636b 2920 5b21 5b73 6563  sf/black) [![sec
-000011e0: 7572 6974 793a 2062 616e 6469 745d 2868  urity: bandit](h
-000011f0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00001200: 6473 2e69 6f2f 6261 6467 652f 7365 6375  ds.io/badge/secu
-00001210: 7269 7479 2d62 616e 6469 742d 7965 6c6c  rity-bandit-yell
-00001220: 6f77 2e73 7667 295d 2868 7474 7073 3a2f  ow.svg)](https:/
-00001230: 2f67 6974 6875 622e 636f 6d2f 5079 4351  /github.com/PyCQ
-00001240: 412f 6261 6e64 6974 2920 7c0a 7c20 2a2a  A/bandit) |.| **
-00001250: 446f 776e 6c6f 6164 732a 2a7c 205b 215b  Downloads**| [![
-00001260: 446f 776e 6c6f 6164 735d 2868 7474 7073  Downloads](https
-00001270: 3a2f 2f73 7461 7469 632e 7065 7079 2e74  ://static.pepy.t
-00001280: 6563 682f 7065 7273 6f6e 616c 697a 6564  ech/personalized
-00001290: 2d62 6164 6765 2f73 6369 6b69 742d 6261  -badge/scikit-ba
-000012a0: 7365 3f70 6572 696f 643d 7765 656b 2675  se?period=week&u
-000012b0: 6e69 7473 3d69 6e74 6572 6e61 7469 6f6e  nits=internation
-000012c0: 616c 5f73 7973 7465 6d26 6c65 6674 5f63  al_system&left_c
-000012d0: 6f6c 6f72 3d67 7265 7926 7269 6768 745f  olor=grey&right_
-000012e0: 636f 6c6f 723d 626c 7565 266c 6566 745f  color=blue&left_
-000012f0: 7465 7874 3d77 6565 6b6c 7925 3230 2870  text=weekly%20(p
-00001300: 7970 6929 295d 2868 7474 7073 3a2f 2f70  ypi))](https://p
-00001310: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
-00001320: 2f73 6369 6b69 742d 6261 7365 2920 5b21  /scikit-base) [!
-00001330: 5b44 6f77 6e6c 6f61 6473 5d28 6874 7470  [Downloads](http
-00001340: 733a 2f2f 7374 6174 6963 2e70 6570 792e  s://static.pepy.
-00001350: 7465 6368 2f70 6572 736f 6e61 6c69 7a65  tech/personalize
-00001360: 642d 6261 6467 652f 7363 696b 6974 2d62  d-badge/scikit-b
-00001370: 6173 653f 7065 7269 6f64 3d6d 6f6e 7468  ase?period=month
-00001380: 2675 6e69 7473 3d69 6e74 6572 6e61 7469  &units=internati
-00001390: 6f6e 616c 5f73 7973 7465 6d26 6c65 6674  onal_system&left
-000013a0: 5f63 6f6c 6f72 3d67 7265 7926 7269 6768  _color=grey&righ
-000013b0: 745f 636f 6c6f 723d 626c 7565 266c 6566  t_color=blue&lef
-000013c0: 745f 7465 7874 3d6d 6f6e 7468 6c79 2532  t_text=monthly%2
-000013d0: 3028 7079 7069 2929 5d28 6874 7470 733a  0(pypi))](https:
-000013e0: 2f2f 7065 7079 2e74 6563 682f 7072 6f6a  //pepy.tech/proj
-000013f0: 6563 742f 7363 696b 6974 2d62 6173 6529  ect/scikit-base)
-00001400: 205b 215b 446f 776e 6c6f 6164 735d 2868   [![Downloads](h
-00001410: 7474 7073 3a2f 2f73 7461 7469 632e 7065  ttps://static.pe
-00001420: 7079 2e74 6563 682f 7065 7273 6f6e 616c  py.tech/personal
-00001430: 697a 6564 2d62 6164 6765 2f73 6369 6b69  ized-badge/sciki
-00001440: 742d 6261 7365 3f70 6572 696f 643d 746f  t-base?period=to
-00001450: 7461 6c26 756e 6974 733d 696e 7465 726e  tal&units=intern
-00001460: 6174 696f 6e61 6c5f 7379 7374 656d 266c  ational_system&l
-00001470: 6566 745f 636f 6c6f 723d 6772 6579 2672  eft_color=grey&r
-00001480: 6967 6874 5f63 6f6c 6f72 3d62 6c75 6526  ight_color=blue&
-00001490: 6c65 6674 5f74 6578 743d 6375 6d75 6c61  left_text=cumula
-000014a0: 7469 7665 2532 3028 7079 7069 2929 5d28  tive%20(pypi))](
-000014b0: 6874 7470 733a 2f2f 7065 7079 2e74 6563  https://pepy.tec
-000014c0: 682f 7072 6f6a 6563 742f 7363 696b 6974  h/project/scikit
-000014d0: 2d62 6173 6529 207c 0a0a 3c21 2d2d 2041  -base) |..<!-- A
-000014e0: 4c4c 2d43 4f4e 5452 4942 5554 4f52 532d  LL-CONTRIBUTORS-
-000014f0: 4241 4447 453a 5354 4152 5420 2d20 446f  BADGE:START - Do
-00001500: 206e 6f74 2072 656d 6f76 6520 6f72 206d   not remove or m
-00001510: 6f64 6966 7920 7468 6973 2073 6563 7469  odify this secti
-00001520: 6f6e 202d 2d3e 0a5b 215b 416c 6c20 436f  on -->.[![All Co
-00001530: 6e74 7269 6275 746f 7273 5d28 6874 7470  ntributors](http
-00001540: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00001550: 696f 2f62 6164 6765 2f61 6c6c 5f63 6f6e  io/badge/all_con
-00001560: 7472 6962 7574 6f72 732d 3133 2d6f 7261  tributors-13-ora
-00001570: 6e67 652e 7376 673f 7374 796c 653d 666c  nge.svg?style=fl
-00001580: 6174 2d73 7175 6172 6529 5d28 2363 6f6e  at-square)](#con
-00001590: 7472 6962 7574 6f72 7329 0a3c 212d 2d20  tributors).<!-- 
-000015a0: 414c 4c2d 434f 4e54 5249 4255 544f 5253  ALL-CONTRIBUTORS
-000015b0: 2d42 4144 4745 3a45 4e44 202d 2d3e 0a0a  -BADGE:END -->..
-000015c0: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
-000015d0: 0a0a 546f 206c 6561 726e 206d 6f72 6520  ..To learn more 
-000015e0: 6162 6f75 7420 7468 6520 7061 636b 6167  about the packag
-000015f0: 6520 6368 6563 6b6f 7574 206f 7572 205b  e checkout our [
-00001600: 646f 6375 6d65 6e74 6174 696f 6e5d 2868  documentation](h
-00001610: 7474 7073 3a2f 2f73 6b62 6173 652e 7265  ttps://skbase.re
-00001620: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00001630: 6c61 7465 7374 2f29 2e0a 0a23 2320 3a68  latest/)...## :h
-00001640: 6f75 7267 6c61 7373 5f66 6c6f 7769 6e67  ourglass_flowing
-00001650: 5f73 616e 643a 2049 6e73 7461 6c6c 2073  _sand: Install s
-00001660: 6b62 6173 650a 466f 7220 7472 6f75 626c  kbase.For troubl
-00001670: 6520 7368 6f6f 7469 6e67 206f 7220 6d6f  e shooting or mo
-00001680: 7265 2069 6e66 6f72 6d61 7469 6f6e 2c20  re information, 
-00001690: 7365 6520 6f75 720a 5b64 6574 6169 6c65  see our.[detaile
-000016a0: 6420 696e 7374 616c 6c61 7469 6f6e 2069  d installation i
-000016b0: 6e73 7472 7563 7469 6f6e 735d 2868 7474  nstructions](htt
-000016c0: 7073 3a2f 2f73 6b62 6173 652e 7265 6164  ps://skbase.read
-000016d0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
-000016e0: 7465 7374 2f75 7365 725f 646f 6375 6d65  test/user_docume
-000016f0: 6e74 6174 696f 6e2f 696e 7374 616c 6c61  ntation/installa
-00001700: 7469 6f6e 2e68 746d 6c29 2e0a 0a2d 202a  tion.html)...- *
-00001710: 2a4f 7065 7261 7469 6e67 2073 7973 7465  *Operating syste
-00001720: 6d2a 2a3a 206d 6163 4f53 2058 20c2 b720  m**: macOS X .. 
-00001730: 4c69 6e75 7820 c2b7 2057 696e 646f 7773  Linux .. Windows
-00001740: 2038 2e31 206f 7220 6869 6768 6572 0a2d   8.1 or higher.-
-00001750: 202a 2a50 7974 686f 6e20 7665 7273 696f   **Python versio
-00001760: 6e2a 2a3a 2050 7974 686f 6e20 332e 372c  n**: Python 3.7,
-00001770: 2033 2e38 2c20 332e 392c 2033 2e31 3020   3.8, 3.9, 3.10 
-00001780: 616e 6420 332e 3131 0a2d 202a 2a50 6163  and 3.11.- **Pac
-00001790: 6b61 6765 206d 616e 6167 6572 732a 2a3a  kage managers**:
-000017a0: 205b 7069 705d 0a0a 5b70 6970 5d3a 2068   [pip]..[pip]: h
-000017b0: 7474 7073 3a2f 2f70 6970 2e70 7970 612e  ttps://pip.pypa.
-000017c0: 696f 2f65 6e2f 7374 6162 6c65 2f0a 0a23  io/en/stable/..#
-000017d0: 2323 2070 6970 0a73 6b62 6173 6520 7265  ## pip.skbase re
-000017e0: 6c65 6173 6573 2061 7265 2061 7661 696c  leases are avail
-000017f0: 6162 6c65 2061 7320 736f 7572 6365 2070  able as source p
-00001800: 6163 6b61 6765 7320 616e 6420 6269 6e61  ackages and bina
-00001810: 7279 2077 6865 656c 7320 7669 6120 5079  ry wheels via Py
-00001820: 5049 0a61 6e64 2063 616e 2062 6520 696e  PI.and can be in
-00001830: 7374 616c 6c65 6420 7573 696e 6720 7069  stalled using pi
-00001840: 702e 2043 6865 636b 6f75 7420 7468 6520  p. Checkout the 
-00001850: 6675 6c6c 206c 6973 7420 6f66 2070 7265  full list of pre
-00001860: 2d63 6f6d 7069 6c65 6420 5b77 6865 656c  -compiled [wheel
-00001870: 7320 6f6e 2050 7950 695d 2868 7474 7073  s on PyPi](https
-00001880: 3a2f 2f70 7970 692e 6f72 672f 7369 6d70  ://pypi.org/simp
-00001890: 6c65 2f73 6b62 6173 652f 292e 0a0a 546f  le/skbase/)...To
-000018a0: 2069 6e73 7461 6c6c 2074 6865 2063 6f72   install the cor
-000018b0: 6520 7061 636b 6167 6520 7573 653a 0a0a  e package use:..
-000018c0: 6060 6062 6173 680a 7069 7020 696e 7374  ```bash.pip inst
-000018d0: 616c 6c20 7363 696b 6974 2d62 6173 650a  all scikit-base.
-000018e0: 6060 600a 0a6f 722c 2069 6620 796f 7520  ```..or, if you 
-000018f0: 7761 6e74 2074 6f20 696e 7374 616c 6c20  want to install 
-00001900: 7769 7468 2074 6865 206d 6178 696d 756d  with the maximum
-00001910: 2073 6574 206f 6620 6465 7065 6e64 656e   set of dependen
-00001920: 6369 6573 2c20 7573 653a 0a0a 6060 6062  cies, use:..```b
-00001930: 6173 680a 7069 7020 696e 7374 616c 6c20  ash.pip install 
-00001940: 7363 696b 6974 2d62 6173 655b 616c 6c5f  scikit-base[all_
-00001950: 6578 7472 6173 5d0a 6060 600a            extras].```.
+00000010: 3a20 322e 310d 0a4e 616d 653a 2073 6b62  : 2.1..Name: skb
+00000020: 6173 650d 0a56 6572 7369 6f6e 3a20 302e  ase..Version: 0.
+00000030: 342e 360d 0a53 756d 6d61 7279 3a20 4261  4.6..Summary: Ba
+00000040: 7365 2063 6c61 7373 6573 2066 6f72 2073  se classes for s
+00000050: 6b6c 6561 726e 2d6c 696b 6520 7061 7261  klearn-like para
+00000060: 6d65 7472 6963 206f 626a 6563 7473 0d0a  metric objects..
+00000070: 4175 7468 6f72 2d65 6d61 696c 3a20 736b  Author-email: sk
+00000080: 7469 6d65 2064 6576 656c 6f70 6572 7320  time developers 
+00000090: 3c73 6b74 696d 652e 746f 6f6c 626f 7840  <sktime.toolbox@
+000000a0: 676d 6169 6c2e 636f 6d3e 0d0a 4d61 696e  gmail.com>..Main
+000000b0: 7461 696e 6572 3a20 4672 616e 7a20 4b69  tainer: Franz Ki
+000000c0: 72c3 a16c 790d 0a4d 6169 6e74 6169 6e65  r..ly..Maintaine
+000000d0: 722d 656d 6169 6c3a 2073 6b74 696d 6520  r-email: sktime 
+000000e0: 6465 7665 6c6f 7065 7273 203c 736b 7469  developers <skti
+000000f0: 6d65 2e74 6f6f 6c62 6f78 4067 6d61 696c  me.toolbox@gmail
+00000100: 2e63 6f6d 3e0d 0a4c 6963 656e 7365 3a20  .com>..License: 
+00000110: 4253 4420 332d 436c 6175 7365 204c 6963  BSD 3-Clause Lic
+00000120: 656e 7365 0d0a 2020 2020 2020 2020 0d0a  ense..        ..
+00000130: 2020 2020 2020 2020 436f 7079 7269 6768          Copyrigh
+00000140: 7420 2863 2920 3230 3232 2c20 736b 6261  t (c) 2022, skba
+00000150: 7365 2044 6576 656c 6f70 6572 730d 0a20  se Developers.. 
+00000160: 2020 2020 2020 2041 6c6c 2072 6967 6874         All right
+00000170: 7320 7265 7365 7276 6564 2e0d 0a20 2020  s reserved...   
+00000180: 2020 2020 200d 0a20 2020 2020 2020 2052       ..        R
+00000190: 6564 6973 7472 6962 7574 696f 6e20 616e  edistribution an
+000001a0: 6420 7573 6520 696e 2073 6f75 7263 6520  d use in source 
+000001b0: 616e 6420 6269 6e61 7279 2066 6f72 6d73  and binary forms
+000001c0: 2c20 7769 7468 206f 7220 7769 7468 6f75  , with or withou
+000001d0: 740d 0a20 2020 2020 2020 206d 6f64 6966  t..        modif
+000001e0: 6963 6174 696f 6e2c 2061 7265 2070 6572  ication, are per
+000001f0: 6d69 7474 6564 2070 726f 7669 6465 6420  mitted provided 
+00000200: 7468 6174 2074 6865 2066 6f6c 6c6f 7769  that the followi
+00000210: 6e67 2063 6f6e 6469 7469 6f6e 7320 6172  ng conditions ar
+00000220: 6520 6d65 743a 0d0a 2020 2020 2020 2020  e met:..        
+00000230: 0d0a 2020 2020 2020 2020 312e 2052 6564  ..        1. Red
+00000240: 6973 7472 6962 7574 696f 6e73 206f 6620  istributions of 
+00000250: 736f 7572 6365 2063 6f64 6520 6d75 7374  source code must
+00000260: 2072 6574 6169 6e20 7468 6520 6162 6f76   retain the abov
+00000270: 6520 636f 7079 7269 6768 7420 6e6f 7469  e copyright noti
+00000280: 6365 2c20 7468 6973 0d0a 2020 2020 2020  ce, this..      
+00000290: 2020 2020 206c 6973 7420 6f66 2063 6f6e       list of con
+000002a0: 6469 7469 6f6e 7320 616e 6420 7468 6520  ditions and the 
+000002b0: 666f 6c6c 6f77 696e 6720 6469 7363 6c61  following discla
+000002c0: 696d 6572 2e0d 0a20 2020 2020 2020 200d  imer...        .
+000002d0: 0a20 2020 2020 2020 2032 2e20 5265 6469  .        2. Redi
+000002e0: 7374 7269 6275 7469 6f6e 7320 696e 2062  stributions in b
+000002f0: 696e 6172 7920 666f 726d 206d 7573 7420  inary form must 
+00000300: 7265 7072 6f64 7563 6520 7468 6520 6162  reproduce the ab
+00000310: 6f76 6520 636f 7079 7269 6768 7420 6e6f  ove copyright no
+00000320: 7469 6365 2c0d 0a20 2020 2020 2020 2020  tice,..         
+00000330: 2020 7468 6973 206c 6973 7420 6f66 2063    this list of c
+00000340: 6f6e 6469 7469 6f6e 7320 616e 6420 7468  onditions and th
+00000350: 6520 666f 6c6c 6f77 696e 6720 6469 7363  e following disc
+00000360: 6c61 696d 6572 2069 6e20 7468 6520 646f  laimer in the do
+00000370: 6375 6d65 6e74 6174 696f 6e0d 0a20 2020  cumentation..   
+00000380: 2020 2020 2020 2020 616e 642f 6f72 206f          and/or o
+00000390: 7468 6572 206d 6174 6572 6961 6c73 2070  ther materials p
+000003a0: 726f 7669 6465 6420 7769 7468 2074 6865  rovided with the
+000003b0: 2064 6973 7472 6962 7574 696f 6e2e 0d0a   distribution...
+000003c0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000003d0: 2020 332e 204e 6569 7468 6572 2074 6865    3. Neither the
+000003e0: 206e 616d 6520 6f66 2074 6865 2063 6f70   name of the cop
+000003f0: 7972 6967 6874 2068 6f6c 6465 7220 6e6f  yright holder no
+00000400: 7220 7468 6520 6e61 6d65 7320 6f66 2069  r the names of i
+00000410: 7473 0d0a 2020 2020 2020 2020 2020 2063  ts..           c
+00000420: 6f6e 7472 6962 7574 6f72 7320 6d61 7920  ontributors may 
+00000430: 6265 2075 7365 6420 746f 2065 6e64 6f72  be used to endor
+00000440: 7365 206f 7220 7072 6f6d 6f74 6520 7072  se or promote pr
+00000450: 6f64 7563 7473 2064 6572 6976 6564 2066  oducts derived f
+00000460: 726f 6d0d 0a20 2020 2020 2020 2020 2020  rom..           
+00000470: 7468 6973 2073 6f66 7477 6172 6520 7769  this software wi
+00000480: 7468 6f75 7420 7370 6563 6966 6963 2070  thout specific p
+00000490: 7269 6f72 2077 7269 7474 656e 2070 6572  rior written per
+000004a0: 6d69 7373 696f 6e2e 0d0a 2020 2020 2020  mission...      
+000004b0: 2020 0d0a 2020 2020 2020 2020 5448 4953    ..        THIS
+000004c0: 2053 4f46 5457 4152 4520 4953 2050 524f   SOFTWARE IS PRO
+000004d0: 5649 4445 4420 4259 2054 4845 2043 4f50  VIDED BY THE COP
+000004e0: 5952 4947 4854 2048 4f4c 4445 5253 2041  YRIGHT HOLDERS A
+000004f0: 4e44 2043 4f4e 5452 4942 5554 4f52 5320  ND CONTRIBUTORS 
+00000500: 2241 5320 4953 220d 0a20 2020 2020 2020  "AS IS"..       
+00000510: 2041 4e44 2041 4e59 2045 5850 5245 5353   AND ANY EXPRESS
+00000520: 204f 5220 494d 504c 4945 4420 5741 5252   OR IMPLIED WARR
+00000530: 414e 5449 4553 2c20 494e 434c 5544 494e  ANTIES, INCLUDIN
+00000540: 472c 2042 5554 204e 4f54 204c 494d 4954  G, BUT NOT LIMIT
+00000550: 4544 2054 4f2c 2054 4845 0d0a 2020 2020  ED TO, THE..    
+00000560: 2020 2020 494d 504c 4945 4420 5741 5252      IMPLIED WARR
+00000570: 414e 5449 4553 204f 4620 4d45 5243 4841  ANTIES OF MERCHA
+00000580: 4e54 4142 494c 4954 5920 414e 4420 4649  NTABILITY AND FI
+00000590: 544e 4553 5320 464f 5220 4120 5041 5254  TNESS FOR A PART
+000005a0: 4943 554c 4152 2050 5552 504f 5345 2041  ICULAR PURPOSE A
+000005b0: 5245 0d0a 2020 2020 2020 2020 4449 5343  RE..        DISC
+000005c0: 4c41 494d 4544 2e20 494e 204e 4f20 4556  LAIMED. IN NO EV
+000005d0: 454e 5420 5348 414c 4c20 5448 4520 434f  ENT SHALL THE CO
+000005e0: 5059 5249 4748 5420 484f 4c44 4552 204f  PYRIGHT HOLDER O
+000005f0: 5220 434f 4e54 5249 4255 544f 5253 2042  R CONTRIBUTORS B
+00000600: 4520 4c49 4142 4c45 0d0a 2020 2020 2020  E LIABLE..      
+00000610: 2020 464f 5220 414e 5920 4449 5245 4354    FOR ANY DIRECT
+00000620: 2c20 494e 4449 5245 4354 2c20 494e 4349  , INDIRECT, INCI
+00000630: 4445 4e54 414c 2c20 5350 4543 4941 4c2c  DENTAL, SPECIAL,
+00000640: 2045 5845 4d50 4c41 5259 2c20 4f52 2043   EXEMPLARY, OR C
+00000650: 4f4e 5345 5155 454e 5449 414c 0d0a 2020  ONSEQUENTIAL..  
+00000660: 2020 2020 2020 4441 4d41 4745 5320 2849        DAMAGES (I
+00000670: 4e43 4c55 4449 4e47 2c20 4255 5420 4e4f  NCLUDING, BUT NO
+00000680: 5420 4c49 4d49 5445 4420 544f 2c20 5052  T LIMITED TO, PR
+00000690: 4f43 5552 454d 454e 5420 4f46 2053 5542  OCUREMENT OF SUB
+000006a0: 5354 4954 5554 4520 474f 4f44 5320 4f52  STITUTE GOODS OR
+000006b0: 0d0a 2020 2020 2020 2020 5345 5256 4943  ..        SERVIC
+000006c0: 4553 3b20 4c4f 5353 204f 4620 5553 452c  ES; LOSS OF USE,
+000006d0: 2044 4154 412c 204f 5220 5052 4f46 4954   DATA, OR PROFIT
+000006e0: 533b 204f 5220 4255 5349 4e45 5353 2049  S; OR BUSINESS I
+000006f0: 4e54 4552 5255 5054 494f 4e29 2048 4f57  NTERRUPTION) HOW
+00000700: 4556 4552 0d0a 2020 2020 2020 2020 4341  EVER..        CA
+00000710: 5553 4544 2041 4e44 204f 4e20 414e 5920  USED AND ON ANY 
+00000720: 5448 454f 5259 204f 4620 4c49 4142 494c  THEORY OF LIABIL
+00000730: 4954 592c 2057 4845 5448 4552 2049 4e20  ITY, WHETHER IN 
+00000740: 434f 4e54 5241 4354 2c20 5354 5249 4354  CONTRACT, STRICT
+00000750: 204c 4941 4249 4c49 5459 2c0d 0a20 2020   LIABILITY,..   
+00000760: 2020 2020 204f 5220 544f 5254 2028 494e       OR TORT (IN
+00000770: 434c 5544 494e 4720 4e45 474c 4947 454e  CLUDING NEGLIGEN
+00000780: 4345 204f 5220 4f54 4845 5257 4953 4529  CE OR OTHERWISE)
+00000790: 2041 5249 5349 4e47 2049 4e20 414e 5920   ARISING IN ANY 
+000007a0: 5741 5920 4f55 5420 4f46 2054 4845 2055  WAY OUT OF THE U
+000007b0: 5345 0d0a 2020 2020 2020 2020 4f46 2054  SE..        OF T
+000007c0: 4849 5320 534f 4654 5741 5245 2c20 4556  HIS SOFTWARE, EV
+000007d0: 454e 2049 4620 4144 5649 5345 4420 4f46  EN IF ADVISED OF
+000007e0: 2054 4845 2050 4f53 5349 4249 4c49 5459   THE POSSIBILITY
+000007f0: 204f 4620 5355 4348 2044 414d 4147 452e   OF SUCH DAMAGE.
+00000800: 0d0a 2020 2020 2020 2020 0d0a 5072 6f6a  ..        ..Proj
+00000810: 6563 742d 5552 4c3a 2068 6f6d 6570 6167  ect-URL: homepag
+00000820: 652c 2068 7474 7073 3a2f 2f67 6974 6875  e, https://githu
+00000830: 622e 636f 6d2f 736b 7469 6d65 2f73 6b62  b.com/sktime/skb
+00000840: 6173 650d 0a50 726f 6a65 6374 2d55 524c  ase..Project-URL
+00000850: 3a20 7265 706f 7369 746f 7279 2c20 6874  : repository, ht
+00000860: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000870: 2f73 6b74 696d 652f 736b 6261 7365 0d0a  /sktime/skbase..
+00000880: 5072 6f6a 6563 742d 5552 4c3a 2064 6f63  Project-URL: doc
+00000890: 756d 656e 7461 7469 6f6e 2c20 6874 7470  umentation, http
+000008a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+000008b0: 6b74 696d 652f 736b 6261 7365 0d0a 5072  ktime/skbase..Pr
+000008c0: 6f6a 6563 742d 5552 4c3a 2064 6f77 6e6c  oject-URL: downl
+000008d0: 6f61 642c 2068 7474 7073 3a2f 2f70 7970  oad, https://pyp
+000008e0: 692e 6f72 672f 7072 6f6a 6563 742f 736b  i.org/project/sk
+000008f0: 6261 7365 2f23 6669 6c65 730d 0a4b 6579  base/#files..Key
+00000900: 776f 7264 733a 2064 6174 612d 7363 6965  words: data-scie
+00000910: 6e63 652c 6d61 6368 696e 652d 6c65 6172  nce,machine-lear
+00000920: 6e69 6e67 2c73 6369 6b69 742d 6c65 6172  ning,scikit-lear
+00000930: 6e0d 0a43 6c61 7373 6966 6965 723a 2049  n..Classifier: I
+00000940: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000950: 203a 3a20 5363 6965 6e63 652f 5265 7365   :: Science/Rese
+00000960: 6172 6368 0d0a 436c 6173 7369 6669 6572  arch..Classifier
+00000970: 3a20 496e 7465 6e64 6564 2041 7564 6965  : Intended Audie
+00000980: 6e63 6520 3a3a 2044 6576 656c 6f70 6572  nce :: Developer
+00000990: 730d 0a43 6c61 7373 6966 6965 723a 204c  s..Classifier: L
+000009a0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000009b0: 7072 6f76 6564 203a 3a20 4253 4420 4c69  proved :: BSD Li
+000009c0: 6365 6e73 650d 0a43 6c61 7373 6966 6965  cense..Classifie
+000009d0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+000009e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+000009f0: 6e0d 0a43 6c61 7373 6966 6965 723a 2054  n..Classifier: T
+00000a00: 6f70 6963 203a 3a20 536f 6674 7761 7265  opic :: Software
+00000a10: 2044 6576 656c 6f70 6d65 6e74 0d0a 436c   Development..Cl
+00000a20: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
+00000a30: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
+00000a40: 6769 6e65 6572 696e 670d 0a43 6c61 7373  gineering..Class
+00000a50: 6966 6965 723a 204f 7065 7261 7469 6e67  ifier: Operating
+00000a60: 2053 7973 7465 6d20 3a3a 204d 6963 726f   System :: Micro
+00000a70: 736f 6674 203a 3a20 5769 6e64 6f77 730d  soft :: Windows.
+00000a80: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+00000a90: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000aa0: 2050 4f53 4958 0d0a 436c 6173 7369 6669   POSIX..Classifi
+00000ab0: 6572 3a20 4f70 6572 6174 696e 6720 5379  er: Operating Sy
+00000ac0: 7374 656d 203a 3a20 556e 6978 0d0a 436c  stem :: Unix..Cl
+00000ad0: 6173 7369 6669 6572 3a20 4f70 6572 6174  assifier: Operat
+00000ae0: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
+00000af0: 634f 530d 0a43 6c61 7373 6966 6965 723a  cOS..Classifier:
+00000b00: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000b10: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000b20: 3a3a 2033 2e37 0d0a 436c 6173 7369 6669  :: 3.7..Classifi
+00000b30: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+00000b40: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000b50: 6f6e 203a 3a20 332e 380d 0a43 6c61 7373  on :: 3.8..Class
+00000b60: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000b70: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000b80: 7974 686f 6e20 3a3a 2033 2e39 0d0a 436c  ython :: 3.9..Cl
+00000b90: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000ba0: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000bb0: 3a20 5079 7468 6f6e 203a 3a20 332e 3130  : Python :: 3.10
+00000bc0: 0d0a 436c 6173 7369 6669 6572 3a20 5072  ..Classifier: Pr
+00000bd0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000be0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000bf0: 332e 3131 0d0a 5265 7175 6972 6573 2d50  3.11..Requires-P
+00000c00: 7974 686f 6e3a 203c 332e 3132 2c3e 3d33  ython: <3.12,>=3
+00000c10: 2e37 0d0a 4465 7363 7269 7074 696f 6e2d  .7..Description-
+00000c20: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
+00000c30: 7874 2f6d 6172 6b64 6f77 6e0d 0a50 726f  xt/markdown..Pro
+00000c40: 7669 6465 732d 4578 7472 613a 2061 6c6c  vides-Extra: all
+00000c50: 5f65 7874 7261 730d 0a50 726f 7669 6465  _extras..Provide
+00000c60: 732d 4578 7472 613a 2064 6576 0d0a 5072  s-Extra: dev..Pr
+00000c70: 6f76 6964 6573 2d45 7874 7261 3a20 6c69  ovides-Extra: li
+00000c80: 6e74 6572 730d 0a50 726f 7669 6465 732d  nters..Provides-
+00000c90: 4578 7472 613a 2062 696e 6465 720d 0a50  Extra: binder..P
+00000ca0: 726f 7669 6465 732d 4578 7472 613a 2064  rovides-Extra: d
+00000cb0: 6f63 730d 0a50 726f 7669 6465 732d 4578  ocs..Provides-Ex
+00000cc0: 7472 613a 2074 6573 740d 0a4c 6963 656e  tra: test..Licen
+00000cd0: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+00000ce0: 0d0a 0d0a 3c61 2068 7265 663d 2268 7474  ....<a href="htt
+00000cf0: 7073 3a2f 2f73 6b62 6173 652e 7265 6164  ps://skbase.read
+00000d00: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+00000d10: 7465 7374 2f22 3e3c 696d 6720 7372 633d  test/"><img src=
+00000d20: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000d30: 636f 6d2f 736b 7469 6d65 2f73 6b62 6173  com/sktime/skbas
+00000d40: 652f 626c 6f62 2f6d 6169 6e2f 646f 6373  e/blob/main/docs
+00000d50: 2f73 6f75 7263 652f 696d 6167 6573 2f73  /source/images/s
+00000d60: 6b62 6173 652d 6c6f 676f 2d77 6974 682d  kbase-logo-with-
+00000d70: 6e61 6d65 2e70 6e67 2220 7769 6474 683d  name.png" width=
+00000d80: 2231 3735 2220 616c 6967 6e3d 2272 6967  "175" align="rig
+00000d90: 6874 2220 2f3e 3c2f 613e 0d0a 0d0a 2320  ht" /></a>....# 
+00000da0: 5765 6c63 6f6d 6520 746f 2073 6b62 6173  Welcome to skbas
+00000db0: 650d 0a0d 0a3e 2041 2062 6173 6520 636c  e....> A base cl
+00000dc0: 6173 7320 666f 7220 7363 696b 6974 2d6c  ass for scikit-l
+00000dd0: 6561 726e 2d6c 696b 6520 616e 6420 736b  earn-like and sk
+00000de0: 7469 6d65 2d6c 696b 6520 7061 7261 6d65  time-like parame
+00000df0: 7472 6963 206f 626a 6563 7473 0d0a 0d0a  tric objects....
+00000e00: 6073 6b62 6173 6560 2070 726f 7669 6465  `skbase` provide
+00000e10: 7320 6261 7365 2063 6c61 7373 6573 2066  s base classes f
+00000e20: 6f72 2063 7265 6174 696e 6720 7363 696b  or creating scik
+00000e30: 6974 2d6c 6561 726e 2d6c 696b 6520 7061  it-learn-like pa
+00000e40: 7261 6d65 7472 6963 206f 626a 6563 7473  rametric objects
+00000e50: 2c0d 0a61 6c6f 6e67 2077 6974 6820 746f  ,..along with to
+00000e60: 6f6c 7320 746f 206d 616b 6520 6974 2065  ols to make it e
+00000e70: 6173 6965 7220 746f 2062 7569 6c64 2079  asier to build y
+00000e80: 6f75 7220 6f77 6e20 7061 636b 6167 6573  our own packages
+00000e90: 2074 6861 7420 666f 6c6c 6f77 2074 6865   that follow the
+00000ea0: 7365 0d0a 6465 7369 676e 2070 6174 7465  se..design patte
+00000eb0: 726e 732e 0d0a 0d0a 3a72 6f63 6b65 743a  rns.....:rocket:
+00000ec0: 2056 6572 7369 6f6e 2030 2e34 2e36 2069   Version 0.4.6 i
+00000ed0: 7320 6e6f 7720 6176 6169 6c61 626c 652e  s now available.
+00000ee0: 2043 6865 636b 6f75 7420 6f75 720d 0a5b   Checkout our..[
+00000ef0: 7265 6c65 6173 6520 6e6f 7465 735d 2868  release notes](h
+00000f00: 7474 7073 3a2f 2f73 6b62 6173 652e 7265  ttps://skbase.re
+00000f10: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00000f20: 6c61 7465 7374 2f63 6861 6e67 656c 6f67  latest/changelog
+00000f30: 2e68 746d 6c29 2e0d 0a0d 0a7c 204f 7665  .html).....| Ove
+00000f40: 7276 6965 7720 7c20 7c0d 0a7c 2d2d 2d7c  rview | |..|---|
+00000f50: 2d2d 2d7c 0d0a 7c20 2a2a 4349 2f43 442a  ---|..| **CI/CD*
+00000f60: 2a20 7c20 5b21 5b54 6573 7473 5d28 6874  * | [![Tests](ht
+00000f70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000f80: 2f73 6b74 696d 652f 736b 6261 7365 2f61  /sktime/skbase/a
+00000f90: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+00000fa0: 2f74 6573 742e 796d 6c2f 6261 6467 652e  /test.yml/badge.
+00000fb0: 7376 673f 6272 616e 6368 3d6d 6169 6e29  svg?branch=main)
+00000fc0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000fd0: 2e63 6f6d 2f73 6b74 696d 652f 736b 6261  .com/sktime/skba
+00000fe0: 7365 2f61 6374 696f 6e73 2f77 6f72 6b66  se/actions/workf
+00000ff0: 6c6f 7773 2f74 6573 742e 796d 6c29 205b  lows/test.yml) [
+00001000: 215b 636f 6465 636f 765d 2868 7474 7073  ![codecov](https
+00001010: 3a2f 2f63 6f64 6563 6f76 2e69 6f2f 6768  ://codecov.io/gh
+00001020: 2f73 6b74 696d 652f 736b 6261 7365 2f62  /sktime/skbase/b
+00001030: 7261 6e63 682f 6d61 696e 2f67 7261 7068  ranch/main/graph
+00001040: 2f62 6164 6765 2e73 7667 3f74 6f6b 656e  /badge.svg?token
+00001050: 3d32 4a34 3234 4e4c 4f38 3229 5d28 6874  =2J424NLO82)](ht
+00001060: 7470 733a 2f2f 636f 6465 636f 762e 696f  tps://codecov.io
+00001070: 2f67 682f 736b 7469 6d65 2f73 6b62 6173  /gh/sktime/skbas
+00001080: 6529 205b 215b 446f 6375 6d65 6e74 6174  e) [![Documentat
+00001090: 696f 6e20 5374 6174 7573 5d28 6874 7470  ion Status](http
+000010a0: 733a 2f2f 7265 6164 7468 6564 6f63 732e  s://readthedocs.
+000010b0: 6f72 672f 7072 6f6a 6563 7473 2f73 6b62  org/projects/skb
+000010c0: 6173 652f 6261 6467 652f 3f76 6572 7369  ase/badge/?versi
+000010d0: 6f6e 3d6c 6174 6573 7429 5d28 6874 7470  on=latest)](http
+000010e0: 733a 2f2f 736b 6261 7365 2e72 6561 6474  s://skbase.readt
+000010f0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001100: 6573 742f 3f62 6164 6765 3d6c 6174 6573  est/?badge=lates
+00001110: 7429 205b 215b 7072 652d 636f 6d6d 6974  t) [![pre-commit
+00001120: 2e63 6920 7374 6174 7573 5d28 6874 7470  .ci status](http
+00001130: 733a 2f2f 7265 7375 6c74 732e 7072 652d  s://results.pre-
+00001140: 636f 6d6d 6974 2e63 692f 6261 6467 652f  commit.ci/badge/
+00001150: 6769 7468 7562 2f73 6b74 696d 652f 736b  github/sktime/sk
+00001160: 6261 7365 2f6d 6169 6e2e 7376 6729 5d28  base/main.svg)](
+00001170: 6874 7470 733a 2f2f 7265 7375 6c74 732e  https://results.
+00001180: 7072 652d 636f 6d6d 6974 2e63 692f 6c61  pre-commit.ci/la
+00001190: 7465 7374 2f67 6974 6875 622f 736b 7469  test/github/skti
+000011a0: 6d65 2f73 6b62 6173 652f 6d61 696e 2920  me/skbase/main) 
+000011b0: 7c0d 0a7c 202a 2a43 6f64 652a 2a20 7c20  |..| **Code** | 
+000011c0: 205b 215b 2170 7970 695d 2868 7474 7073   [![!pypi](https
+000011d0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000011e0: 6f2f 7079 7069 2f76 2f73 6369 6b69 742d  o/pypi/v/scikit-
+000011f0: 6261 7365 3f63 6f6c 6f72 3d6f 7261 6e67  base?color=orang
+00001200: 6529 5d28 6874 7470 733a 2f2f 7079 7069  e)](https://pypi
+00001210: 2e6f 7267 2f70 726f 6a65 6374 2f73 6b62  .org/project/skb
+00001220: 6173 652f 2920 205b 215b 2170 7974 686f  ase/)  [![!pytho
+00001230: 6e2d 7665 7273 696f 6e73 5d28 6874 7470  n-versions](http
+00001240: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00001250: 696f 2f70 7970 692f 7079 7665 7273 696f  io/pypi/pyversio
+00001260: 6e73 2f73 6369 6b69 742d 6261 7365 295d  ns/scikit-base)]
+00001270: 2868 7474 7073 3a2f 2f77 7777 2e70 7974  (https://www.pyt
+00001280: 686f 6e2e 6f72 672f 2920 5b21 5b21 626c  hon.org/) [![!bl
+00001290: 6163 6b5d 2868 7474 7073 3a2f 2f69 6d67  ack](https://img
+000012a0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000012b0: 652f 636f 6465 2532 3073 7479 6c65 2d62  e/code%20style-b
+000012c0: 6c61 636b 2d30 3030 3030 302e 7376 6729  lack-000000.svg)
+000012d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000012e0: 2e63 6f6d 2f70 7366 2f62 6c61 636b 2920  .com/psf/black) 
+000012f0: 5b21 5b73 6563 7572 6974 793a 2062 616e  [![security: ban
+00001300: 6469 745d 2868 7474 7073 3a2f 2f69 6d67  dit](https://img
+00001310: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00001320: 652f 7365 6375 7269 7479 2d62 616e 6469  e/security-bandi
+00001330: 742d 7965 6c6c 6f77 2e73 7667 295d 2868  t-yellow.svg)](h
+00001340: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001350: 6d2f 5079 4351 412f 6261 6e64 6974 2920  m/PyCQA/bandit) 
+00001360: 7c0d 0a7c 202a 2a44 6f77 6e6c 6f61 6473  |..| **Downloads
+00001370: 2a2a 7c20 5b21 5b44 6f77 6e6c 6f61 6473  **| [![Downloads
+00001380: 5d28 6874 7470 733a 2f2f 7374 6174 6963  ](https://static
+00001390: 2e70 6570 792e 7465 6368 2f70 6572 736f  .pepy.tech/perso
+000013a0: 6e61 6c69 7a65 642d 6261 6467 652f 7363  nalized-badge/sc
+000013b0: 696b 6974 2d62 6173 653f 7065 7269 6f64  ikit-base?period
+000013c0: 3d77 6565 6b26 756e 6974 733d 696e 7465  =week&units=inte
+000013d0: 726e 6174 696f 6e61 6c5f 7379 7374 656d  rnational_system
+000013e0: 266c 6566 745f 636f 6c6f 723d 6772 6579  &left_color=grey
+000013f0: 2672 6967 6874 5f63 6f6c 6f72 3d62 6c75  &right_color=blu
+00001400: 6526 6c65 6674 5f74 6578 743d 7765 656b  e&left_text=week
+00001410: 6c79 2532 3028 7079 7069 2929 5d28 6874  ly%20(pypi))](ht
+00001420: 7470 733a 2f2f 7065 7079 2e74 6563 682f  tps://pepy.tech/
+00001430: 7072 6f6a 6563 742f 7363 696b 6974 2d62  project/scikit-b
+00001440: 6173 6529 205b 215b 446f 776e 6c6f 6164  ase) [![Download
+00001450: 735d 2868 7474 7073 3a2f 2f73 7461 7469  s](https://stati
+00001460: 632e 7065 7079 2e74 6563 682f 7065 7273  c.pepy.tech/pers
+00001470: 6f6e 616c 697a 6564 2d62 6164 6765 2f73  onalized-badge/s
+00001480: 6369 6b69 742d 6261 7365 3f70 6572 696f  cikit-base?perio
+00001490: 643d 6d6f 6e74 6826 756e 6974 733d 696e  d=month&units=in
+000014a0: 7465 726e 6174 696f 6e61 6c5f 7379 7374  ternational_syst
+000014b0: 656d 266c 6566 745f 636f 6c6f 723d 6772  em&left_color=gr
+000014c0: 6579 2672 6967 6874 5f63 6f6c 6f72 3d62  ey&right_color=b
+000014d0: 6c75 6526 6c65 6674 5f74 6578 743d 6d6f  lue&left_text=mo
+000014e0: 6e74 686c 7925 3230 2870 7970 6929 295d  nthly%20(pypi))]
+000014f0: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
+00001500: 6368 2f70 726f 6a65 6374 2f73 6369 6b69  ch/project/sciki
+00001510: 742d 6261 7365 2920 5b21 5b44 6f77 6e6c  t-base) [![Downl
+00001520: 6f61 6473 5d28 6874 7470 733a 2f2f 7374  oads](https://st
+00001530: 6174 6963 2e70 6570 792e 7465 6368 2f70  atic.pepy.tech/p
+00001540: 6572 736f 6e61 6c69 7a65 642d 6261 6467  ersonalized-badg
+00001550: 652f 7363 696b 6974 2d62 6173 653f 7065  e/scikit-base?pe
+00001560: 7269 6f64 3d74 6f74 616c 2675 6e69 7473  riod=total&units
+00001570: 3d69 6e74 6572 6e61 7469 6f6e 616c 5f73  =international_s
+00001580: 7973 7465 6d26 6c65 6674 5f63 6f6c 6f72  ystem&left_color
+00001590: 3d67 7265 7926 7269 6768 745f 636f 6c6f  =grey&right_colo
+000015a0: 723d 626c 7565 266c 6566 745f 7465 7874  r=blue&left_text
+000015b0: 3d63 756d 756c 6174 6976 6525 3230 2870  =cumulative%20(p
+000015c0: 7970 6929 295d 2868 7474 7073 3a2f 2f70  ypi))](https://p
+000015d0: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+000015e0: 2f73 6369 6b69 742d 6261 7365 2920 7c0d  /scikit-base) |.
+000015f0: 0a0d 0a3c 212d 2d20 414c 4c2d 434f 4e54  ...<!-- ALL-CONT
+00001600: 5249 4255 544f 5253 2d42 4144 4745 3a53  RIBUTORS-BADGE:S
+00001610: 5441 5254 202d 2044 6f20 6e6f 7420 7265  TART - Do not re
+00001620: 6d6f 7665 206f 7220 6d6f 6469 6679 2074  move or modify t
+00001630: 6869 7320 7365 6374 696f 6e20 2d2d 3e0d  his section -->.
+00001640: 0a5b 215b 416c 6c20 436f 6e74 7269 6275  .[![All Contribu
+00001650: 746f 7273 5d28 6874 7470 733a 2f2f 696d  tors](https://im
+00001660: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+00001670: 6765 2f61 6c6c 5f63 6f6e 7472 6962 7574  ge/all_contribut
+00001680: 6f72 732d 3133 2d6f 7261 6e67 652e 7376  ors-13-orange.sv
+00001690: 673f 7374 796c 653d 666c 6174 2d73 7175  g?style=flat-squ
+000016a0: 6172 6529 5d28 2363 6f6e 7472 6962 7574  are)](#contribut
+000016b0: 6f72 7329 0d0a 3c21 2d2d 2041 4c4c 2d43  ors)..<!-- ALL-C
+000016c0: 4f4e 5452 4942 5554 4f52 532d 4241 4447  ONTRIBUTORS-BADG
+000016d0: 453a 454e 4420 2d2d 3e0d 0a0d 0a23 2320  E:END -->....## 
+000016e0: 446f 6375 6d65 6e74 6174 696f 6e0d 0a0d  Documentation...
+000016f0: 0a54 6f20 6c65 6172 6e20 6d6f 7265 2061  .To learn more a
+00001700: 626f 7574 2074 6865 2070 6163 6b61 6765  bout the package
+00001710: 2063 6865 636b 6f75 7420 6f75 7220 5b64   checkout our [d
+00001720: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00001730: 7470 733a 2f2f 736b 6261 7365 2e72 6561  tps://skbase.rea
+00001740: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00001750: 6174 6573 742f 292e 0d0a 0d0a 2323 203a  atest/).....## :
+00001760: 686f 7572 676c 6173 735f 666c 6f77 696e  hourglass_flowin
+00001770: 675f 7361 6e64 3a20 496e 7374 616c 6c20  g_sand: Install 
+00001780: 736b 6261 7365 0d0a 466f 7220 7472 6f75  skbase..For trou
+00001790: 626c 6520 7368 6f6f 7469 6e67 206f 7220  ble shooting or 
+000017a0: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+000017b0: 2c20 7365 6520 6f75 720d 0a5b 6465 7461  , see our..[deta
+000017c0: 696c 6564 2069 6e73 7461 6c6c 6174 696f  iled installatio
+000017d0: 6e20 696e 7374 7275 6374 696f 6e73 5d28  n instructions](
+000017e0: 6874 7470 733a 2f2f 736b 6261 7365 2e72  https://skbase.r
+000017f0: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
+00001800: 2f6c 6174 6573 742f 7573 6572 5f64 6f63  /latest/user_doc
+00001810: 756d 656e 7461 7469 6f6e 2f69 6e73 7461  umentation/insta
+00001820: 6c6c 6174 696f 6e2e 6874 6d6c 292e 0d0a  llation.html)...
+00001830: 0d0a 2d20 2a2a 4f70 6572 6174 696e 6720  ..- **Operating 
+00001840: 7379 7374 656d 2a2a 3a20 6d61 634f 5320  system**: macOS 
+00001850: 5820 c2b7 204c 696e 7578 20c2 b720 5769  X .. Linux .. Wi
+00001860: 6e64 6f77 7320 382e 3120 6f72 2068 6967  ndows 8.1 or hig
+00001870: 6865 720d 0a2d 202a 2a50 7974 686f 6e20  her..- **Python 
+00001880: 7665 7273 696f 6e2a 2a3a 2050 7974 686f  version**: Pytho
+00001890: 6e20 332e 372c 2033 2e38 2c20 332e 392c  n 3.7, 3.8, 3.9,
+000018a0: 2033 2e31 3020 616e 6420 332e 3131 0d0a   3.10 and 3.11..
+000018b0: 2d20 2a2a 5061 636b 6167 6520 6d61 6e61  - **Package mana
+000018c0: 6765 7273 2a2a 3a20 5b70 6970 5d0d 0a0d  gers**: [pip]...
+000018d0: 0a5b 7069 705d 3a20 6874 7470 733a 2f2f  .[pip]: https://
+000018e0: 7069 702e 7079 7061 2e69 6f2f 656e 2f73  pip.pypa.io/en/s
+000018f0: 7461 626c 652f 0d0a 0d0a 2323 2320 7069  table/....### pi
+00001900: 700d 0a73 6b62 6173 6520 7265 6c65 6173  p..skbase releas
+00001910: 6573 2061 7265 2061 7661 696c 6162 6c65  es are available
+00001920: 2061 7320 736f 7572 6365 2070 6163 6b61   as source packa
+00001930: 6765 7320 616e 6420 6269 6e61 7279 2077  ges and binary w
+00001940: 6865 656c 7320 7669 6120 5079 5049 0d0a  heels via PyPI..
+00001950: 616e 6420 6361 6e20 6265 2069 6e73 7461  and can be insta
+00001960: 6c6c 6564 2075 7369 6e67 2070 6970 2e20  lled using pip. 
+00001970: 4368 6563 6b6f 7574 2074 6865 2066 756c  Checkout the ful
+00001980: 6c20 6c69 7374 206f 6620 7072 652d 636f  l list of pre-co
+00001990: 6d70 696c 6564 205b 7768 6565 6c73 206f  mpiled [wheels o
+000019a0: 6e20 5079 5069 5d28 6874 7470 733a 2f2f  n PyPi](https://
+000019b0: 7079 7069 2e6f 7267 2f73 696d 706c 652f  pypi.org/simple/
+000019c0: 736b 6261 7365 2f29 2e0d 0a0d 0a54 6f20  skbase/).....To 
+000019d0: 696e 7374 616c 6c20 7468 6520 636f 7265  install the core
+000019e0: 2070 6163 6b61 6765 2075 7365 3a0d 0a0d   package use:...
+000019f0: 0a60 6060 6261 7368 0d0a 7069 7020 696e  .```bash..pip in
+00001a00: 7374 616c 6c20 7363 696b 6974 2d62 6173  stall scikit-bas
+00001a10: 650d 0a60 6060 0d0a 0d0a 6f72 2c20 6966  e..```....or, if
+00001a20: 2079 6f75 2077 616e 7420 746f 2069 6e73   you want to ins
+00001a30: 7461 6c6c 2077 6974 6820 7468 6520 6d61  tall with the ma
+00001a40: 7869 6d75 6d20 7365 7420 6f66 2064 6570  ximum set of dep
+00001a50: 656e 6465 6e63 6965 732c 2075 7365 3a0d  endencies, use:.
+00001a60: 0a0d 0a60 6060 6261 7368 0d0a 7069 7020  ...```bash..pip 
+00001a70: 696e 7374 616c 6c20 7363 696b 6974 2d62  install scikit-b
+00001a80: 6173 655b 616c 6c5f 6578 7472 6173 5d0d  ase[all_extras].
+00001a90: 0a60 6060 0d0a                           .```..
```

### Comparing `skbase-0.4.5/skbase.egg-info/SOURCES.txt` & `skbase-0.4.6/skbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skbase-0.4.5/skbase.egg-info/requires.txt` & `skbase-0.4.6/skbase.egg-info/requires.txt`

 * *Files identical despite different names*

