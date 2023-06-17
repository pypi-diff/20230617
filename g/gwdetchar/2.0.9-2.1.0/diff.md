# Comparing `tmp/gwdetchar-2.0.9.tar.gz` & `tmp/gwdetchar-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdetchar-2.0.9.tar", last modified: Thu Apr 27 00:58:43 2023, max compression
+gzip compressed data, was "gwdetchar-2.1.0.tar", last modified: Sat Jun 17 00:03:06 2023, max compression
```

## Comparing `gwdetchar-2.0.9.tar` & `gwdetchar-2.1.0.tar`

### file list

```diff
@@ -1,103 +1,141 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.224574 gwdetchar-2.0.9/
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)      100 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-27 00:58:43.224785 gwdetchar-2.0.9/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.226881 gwdetchar-2.0.9/gwdetchar/
--rw-r--r--   0 egoetz     (501) staff       (20)     1113 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/gwdetchar/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      471 2023-04-27 00:58:43.227017 gwdetchar-2.0.9/gwdetchar/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4716 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.0.9/gwdetchar/condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/conftest.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3044 2023-04-25 15:49:41.000000 gwdetchar-2.0.9/gwdetchar/const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/daq.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.152453 gwdetchar-2.0.9/gwdetchar/io/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7367 2023-02-28 19:11:25.000000 gwdetchar-2.0.9/gwdetchar/io/datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    41524 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/gwdetchar/io/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3749 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.156779 gwdetchar-2.0.9/gwdetchar/io/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/tests/test_datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    24193 2023-04-25 22:58:28.000000 gwdetchar-2.0.9/gwdetchar/io/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2455 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/io/tests/test_ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.165821 gwdetchar-2.0.9/gwdetchar/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    35157 2022-10-03 17:36:21.000000 gwdetchar-2.0.9/gwdetchar/lasso/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.0.9/gwdetchar/lasso/old.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.169632 gwdetchar-2.0.9/gwdetchar/lasso/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.0.9/gwdetchar/lasso/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/lasso/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/mct.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.173014 gwdetchar-2.0.9/gwdetchar/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.180972 gwdetchar-2.0.9/gwdetchar/nagios/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/nagios/tests/test_main.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.194792 gwdetchar-2.0.9/gwdetchar/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13880 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12666 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/config.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.200650 gwdetchar-2.0.9/gwdetchar/omega/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13619 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/omega/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/overflow.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.203482 gwdetchar-2.0.9/gwdetchar/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.204832 gwdetchar-2.0.9/gwdetchar/saturation/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/saturation/tests/test_saturation.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.209764 gwdetchar-2.0.9/gwdetchar/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.216016 gwdetchar-2.0.9/gwdetchar/scattering/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/scattering/tests/test_simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.223958 gwdetchar-2.0.9/gwdetchar/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.0.9/gwdetchar/tests/test_condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_daq.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.0.9/gwdetchar/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-04-27 00:58:43.148599 gwdetchar-2.0.9/gwdetchar.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     3615 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2419 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2022-12-02 22:06:25.000000 gwdetchar-2.0.9/gwdetchar.egg-info/not-zip-safe
--rw-r--r--   0 egoetz     (501) staff       (20)      292 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-04-27 00:58:43.000000 gwdetchar-2.0.9/gwdetchar.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     3000 2023-04-27 00:58:43.226296 gwdetchar-2.0.9/setup.cfg
--rw-r--r--   0 egoetz     (501) staff       (20)     1205 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/setup.py
--rw-r--r--   0 egoetz     (501) staff       (20)    65747 2023-04-24 20:03:47.000000 gwdetchar-2.0.9/versioneer.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.672925 gwdetchar-2.1.0/
+-rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/.codecov.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)       35 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/.gitattributes
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.567351 gwdetchar-2.1.0/.github/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.582700 gwdetchar-2.1.0/.github/workflows/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.github/workflows/build.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/.github/workflows/docs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1084 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.github/workflows/lint.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.gitignore
+-rw-r--r--   0 egoetz     (501) staff       (20)      577 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/.readthedocs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-06-17 00:03:06.672402 gwdetchar-2.1.0/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.583376 gwdetchar-2.1.0/ci/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/ci/test-cli.sh
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.585552 gwdetchar-2.1.0/docs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/Makefile
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.568003 gwdetchar-2.1.0/docs/_static/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.586437 gwdetchar-2.1.0/docs/_static/css/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/_static/css/custom.css
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.587096 gwdetchar-2.1.0/docs/api/
+-rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/api/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/conf.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.587750 gwdetchar-2.1.0/docs/conlog/
+-rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/conlog/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.588637 gwdetchar-2.1.0/docs/daq/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/daq/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.589270 gwdetchar-2.1.0/docs/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/data/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.589989 gwdetchar-2.1.0/docs/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/html/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.590628 gwdetchar-2.1.0/docs/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/lasso/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.591228 gwdetchar-2.1.0/docs/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/docs/nagios/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.591877 gwdetchar-2.1.0/docs/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/omega/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.592499 gwdetchar-2.1.0/docs/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/saturation/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.593367 gwdetchar-2.1.0/docs/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/docs/scattering/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.604874 gwdetchar-2.1.0/gwdetchar/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      160 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.1.0/gwdetchar/cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.1.0/gwdetchar/condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/conftest.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.1.0/gwdetchar/const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/daq.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.612968 gwdetchar-2.1.0/gwdetchar/io/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7522 2023-06-17 00:02:41.000000 gwdetchar-2.1.0/gwdetchar/io/datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    41413 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/io/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3749 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.616185 gwdetchar-2.1.0/gwdetchar/io/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/tests/test_datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    24146 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/io/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2455 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/io/tests/test_ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.621633 gwdetchar-2.1.0/gwdetchar/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    35568 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/lasso/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.1.0/gwdetchar/lasso/old.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.629730 gwdetchar-2.1.0/gwdetchar/lasso/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.1.0/gwdetchar/lasso/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/lasso/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/mct.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.638209 gwdetchar-2.1.0/gwdetchar/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.639984 gwdetchar-2.1.0/gwdetchar/nagios/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/nagios/tests/test_main.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.651116 gwdetchar-2.1.0/gwdetchar/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13880 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12682 2023-05-16 23:56:26.000000 gwdetchar-2.1.0/gwdetchar/omega/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.655049 gwdetchar-2.1.0/gwdetchar/omega/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13502 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/omega/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/overflow.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.657251 gwdetchar-2.1.0/gwdetchar/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.658443 gwdetchar-2.1.0/gwdetchar/saturation/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/saturation/tests/test_saturation.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.661821 gwdetchar-2.1.0/gwdetchar/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.665006 gwdetchar-2.1.0/gwdetchar/scattering/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/scattering/tests/test_simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.671489 gwdetchar-2.1.0/gwdetchar/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.1.0/gwdetchar/tests/test_condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_daq.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.1.0/gwdetchar/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-06-17 00:03:06.608977 gwdetchar-2.1.0/gwdetchar.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2832 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      353 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-06-17 00:03:06.000000 gwdetchar-2.1.0/gwdetchar.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     3462 2023-06-16 22:43:20.000000 gwdetchar-2.1.0/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2023-06-17 00:03:06.673062 gwdetchar-2.1.0/setup.cfg
```

### Comparing `gwdetchar-2.0.9/LICENSE` & `gwdetchar-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/PKG-INFO` & `gwdetchar-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.0.9
+Version: 2.1.0
 Summary: A python package for gravitational-wave detector characterisation
-Home-page: https://github.com/gwdetchar/gwdetchar/
-Author: Alex Urban, Duncan Macleod
-Author-email: alexander.urban@ligo.org
+Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
+Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
-Keywords: physics,astronomy,gravitational-waves,ligo
+Project-URL: Documentation, https://gwdetchar.readthedocs.io
+Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
+Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
+Project-URL: Discussion Forum, https://gwdetchar.slack.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 ############################################
 Gravitational-wave Detector Characterisation
 ############################################
```

### Comparing `gwdetchar-2.0.9/README.rst` & `gwdetchar-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/__init__.py` & `gwdetchar-2.1.0/gwdetchar/omega/tests/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright (C) Duncan Macleod (2015)
+# Copyright (C) Alex Urban (2019)
 #
 # This file is part of the GW DetChar python package.
 #
 # GW DetChar is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,20 +12,11 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with GW DetChar.  If not, see <http://www.gnu.org/licenses/>.
 
-"""The GW DetChar package (`gwdetchar`) provides python utilies for
-Gravitational-wave detector characterisation.
-
-This package extends the GWpy package for gravitational-wave
-data processing (https://gwpy.github.io).
+"""Tests for :mod:`gwdetchar.omega`
 """
 
-from ._version import get_versions
-
-__version__ = get_versions()['version']
-__author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
-
-del get_versions
+__author__ = 'Alex Urban <alexander.urban@ligo.org>'
```

### Comparing `gwdetchar-2.0.9/gwdetchar/cds.py` & `gwdetchar-2.1.0/gwdetchar/cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/cli.py` & `gwdetchar-2.1.0/gwdetchar/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     'levelname': {'color': 39},
     'asctime': {'color': 27},
     'name': {'color': 12},
 }
 
 NOW = datetime.datetime.now()
 TIMEZONE = reference.LocalTimezone().tzname(NOW)
+NOW_GPS = to_gps(NOW)
 
 DATEFMT = '%Y-%m-%d %H:%M:%S {}'.format(TIMEZONE)
 FMT = '%(name)s %(asctime)s %(levelname)+8s: %(message)s'
 
 # disable matplotlib logging
 logging.getLogger("matplotlib").setLevel(logging.CRITICAL)
```

### Comparing `gwdetchar-2.0.9/gwdetchar/condor.py` & `gwdetchar-2.1.0/gwdetchar/condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/conftest.py` & `gwdetchar-2.1.0/gwdetchar/conftest.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/conlog.py` & `gwdetchar-2.1.0/gwdetchar/conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/const.py` & `gwdetchar-2.1.0/gwdetchar/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,15 @@
     ('ER7', Segment(1117400416, 1118329216)),
     ('ER8', Segment(1123858817, 1126623617)),
     ('O1', Segment(1126623617, 1136649617)),
     ('ER9', Segment(1152136817, 1152255617)),
     ('ER10', Segment(1161907217, 1164499217)),
     ('O2', Segment(1164499217, 1187733618)),
     ('O3', Segment(1187733618, 1366556418)),
-    ('ER15', Segment(1366556418, 1368975618)),
-    ('O4', Segment(1368975618, 2000000000)),
+    ('O4', Segment(1366556418, 2000000000)),
 ])
 
 
 def latest_epoch():
     """Returns the name of the latest known epoch
     """
     epochs = sorted(EPOCH.items(), key=lambda x: x[1][0])
```

### Comparing `gwdetchar-2.0.9/gwdetchar/daq.py` & `gwdetchar-2.1.0/gwdetchar/daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/io/__init__.py` & `gwdetchar-2.1.0/gwdetchar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/io/datafind.py` & `gwdetchar-2.1.0/gwdetchar/io/datafind.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,16 +145,16 @@
     nproc : `int`, optional
         number of parallel processes to use, uses serial process by default
 
     verbose : `bool`, optional
         print verbose output about NDS progress, default: False
 
     **kwargs : `dict`, optional
-        additional keyword arguments to `~gwpy.timeseries.TimeSeries.read`
-        or `~gwpy.timeseries.TimeSeries.get`
+        additional keyword arguments to `~gwpy.timeseries.TimeSeries.read`,
+        `~gwpy.timeseries.TimeSeries.get`, or `~gwpy.io.datafind.find_urls`
 
     Returns
     -------
     data : `~gwpy.timeseries.TimeSeries` or `~gwpy.timeseries.TimeSeriesDict`
         collection of data for the requested channels in the requested time
         range
 
@@ -187,15 +187,17 @@
     else:
         series_class = TimeSeries
 
     if frametype is not None:
         try:  # locate frame files
             ifo = re.search('[A-Z]1', frametype).group(0)
             obs = ifo[0]
-            source = io_datafind.find_urls(obs, frametype, start, end)
+            on_gaps = kwargs.get('on_gaps', 'error')
+            source = io_datafind.find_urls(obs, frametype, start, end,
+                                           on_gaps=on_gaps, **kwargs)
         except AttributeError:
             raise AttributeError(
                 'Could not determine observatory from frametype')
         except (HTTPError, JSONDecodeError):  # frame files not found
             pass
     if source and (isinstance(source, list) and
                    isinstance(channel, (list, tuple))):
```

### Comparing `gwdetchar-2.0.9/gwdetchar/io/html.py` & `gwdetchar-2.1.0/gwdetchar/io/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 from pygments import highlight
 from pygments.formatters import HtmlFormatter
 from pygments.lexers import get_lexer_by_name
 
 from gwpy.time import from_gps
 
 from ..plot import plot_segments
-from .._version import get_versions
+from .._version import __version__
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 __credit__ = 'Alex Urban <alexander.urban@ligo.org>'
 
 # -- give context for ifo names
 
 OBSERVATORY_MAP = {
@@ -1181,18 +1181,16 @@
         the markup object containing the footer HTML
     """
     page = markup.page()
     page.twotags.append('footer')
     markup.element('footer', case=page.case, parent=page)(class_='footer')
     page.div(class_='container')
     if link is None:
-        version = get_versions()['version']
-        commit = get_versions()['full-revisionid']
-        package = 'gwdetchar-%s' % version
-        source = 'https://github.com/gwdetchar/gwdetchar/tree/%s' % commit
+        package = f'gwdetchar-{__version__}'
+        source = 'https://github.com/gwdetchar/gwdetchar'
         host = 'GitHub'
     elif isinstance(link, (tuple, list)):
         package, source, host = link
     else:
         raise ValueError("'link' argument must be either None or a tuple of "
                          "package name, URL, and host name")
     # format various links
```

### Comparing `gwdetchar-2.0.9/gwdetchar/io/ligolw.py` & `gwdetchar-2.1.0/gwdetchar/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/io/tests/__init__.py` & `gwdetchar-2.1.0/gwdetchar/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/io/tests/test_datafind.py` & `gwdetchar-2.1.0/gwdetchar/io/tests/test_datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/io/tests/test_html.py` & `gwdetchar-2.1.0/gwdetchar/io/tests/test_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,27 +30,26 @@
 from pygments import __version__ as pygments_version
 from pytz import reference
 from unittest import mock
 
 from gwpy.segments import (Segment, DataQualityFlag)
 
 from .. import html
-from ..._version import get_versions
+from ..._version import __version__ as gwdetchar_version
 from ...utils import parse_html
 
 from matplotlib import use
 use('Agg')
 
 __author__ = 'Alex Urban <alexander.urban@ligo.org>'
 
 
 # global test objects
 
-VERSION = get_versions()['version']
-COMMIT = get_versions()['full-revisionid']
+VERSION = gwdetchar_version
 
 STYLESHEETS = '\n'.join([
     '<link href="{}" rel="stylesheet" media="all" />'.format(css)
     for css in html.CSS_FILES])
 SCRIPTS = '\n'.join([
     '<script src="{}" type="text/javascript"></script>'.format(js)
     for js in html.JS_FILES])
@@ -147,26 +146,26 @@
 </div>
 </div>"""  # noqa: E501
 
 HTML_FOOTER = """<footer class="footer">
 <div class="container">
 <div class="row">
 <div class="col-sm-3 icon-bar">
-<a href="https://github.com/gwdetchar/gwdetchar/tree/%s" title="View gwdetchar-%s on GitHub" target="_blank"><i class="fas fa-code"></i></a>
+<a href="https://github.com/gwdetchar/gwdetchar" title="View gwdetchar-%s on GitHub" target="_blank"><i class="fas fa-code"></i></a>
 <a href="https://github.com/gwdetchar/gwdetchar/issues" title="Open an issue ticket" target="_blank"><i class="fas fa-ticket-alt"></i></a>
 <a href="about" title="How was this page generated?"><i class="fas fa-info-circle"></i></a>
 <a href="external" title="View this page&quot;s external source"><i class="fas fa-external-link-alt"></i></a>
 <a href="https://apod.nasa.gov/apod/astropix.html" title="Take a break from science" target="_blank"><i class="fas fa-heartbeat"></i></a>
 </div>
 <div class="col-sm-6">
 <p>Created by {user} at {date}</p>
 </div>
 </div>
 </div>
-</footer>""" % (COMMIT, VERSION)  # noqa: E501
+</footer>""" % (VERSION)  # noqa: E501
 
 HTML_CLOSE = """</div>
 %s
 </body>
 </html>""" % HTML_FOOTER
 
 FLAG_CONTENT = """<div class="card border-warning mb-1 shadow-sm">
```

#### html2text {}

```diff
@@ -9,18 +9,18 @@
 received a copy of the GNU General Public License # along with gwdetchar. If
 not, see
 www.gnu.org/licenses/>. """Tests for `gwdetchar.io.html` """ import datetime
 import os import pytest import shutil import sys from getpass import getuser
 from MarkupPy import markup from pygments import __version__ as
 pygments_version from pytz import reference from unittest import mock from
 gwpy.segments import (Segment, DataQualityFlag) from .. import html from
-..._version import get_versions from ...utils import parse_html from matplotlib
-import use use('Agg') __author__ = 'Alex Urban
-urban@ligo.org>' # global test objects VERSION = get_versions()['version']
-COMMIT = get_versions()['full-revisionid'] STYLESHEETS = '\n'.join([ '
+..._version import __version__ as gwdetchar_version from ...utils import
+parse_html from matplotlib import use use('Agg') __author__ = 'Alex Urban
+urban@ligo.org>' # global test objects VERSION = gwdetchar_version STYLESHEETS
+= '\n'.join([ '
 '.format(css) for css in html.CSS_FILES]) SCRIPTS = '\n'.join([ '
 '.format(js) for js in html.JS_FILES]) NEW_BOOTSTRAP_PAGE = """
 
 
 
  %s %s
 """ % (STYLESHEETS, SCRIPTS) TEST_CONFIGURATION = """[section] key = value"""
@@ -66,15 +66,15 @@
 Name      Version
 gwdetchar 1.2.3
 gwpy      1.0.0
 Export to CSV
 """ # noqa: E501 HTML_FOOTER = """
 
 Created by {user} at {date}
-""" % (COMMIT, VERSION) # noqa: E501 HTML_CLOSE = """
+""" % (VERSION) # noqa: E501 HTML_CLOSE = """
 %s
 """ % HTML_FOOTER FLAG_CONTENT = """
 X1:TEST_FLAG
 {plots} {content}
 """ # noqa: E501 FLAG_HTML = FLAG_CONTENT.format(content="""
 # seg\tstart\tstop\tduration
 0\t0\t66\t66.0
```

### Comparing `gwdetchar-2.0.9/gwdetchar/io/tests/test_ligolw.py` & `gwdetchar-2.1.0/gwdetchar/io/tests/test_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/lasso/__init__.py` & `gwdetchar-2.1.0/gwdetchar/lasso/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/lasso/__main__.py` & `gwdetchar-2.1.0/gwdetchar/lasso/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,17 @@
 import numpy
 
 from MarkupPy import markup
 
 from astropy.table import Table
 
 from sklearn import linear_model
-from sklearn.preprocessing import scale
+from sklearn.preprocessing import StandardScaler, scale
 
 from pandas import set_option
-
 from gwpy.detector import ChannelList
 from gwpy.io import nds2 as io_nds2
 
 from .. import (cli, lasso as gwlasso)
 from ..io.datafind import get_data
 from ..io import html as htmlio
 
@@ -112,15 +111,16 @@
 
             ncluster = min(len(cluster), max_correlated_channels)
             colors2 = [cmap(i) for i in numpy.linspace(0, 1, ncluster+1)]
 
             # plot
             fig = Plot(figsize=(12, 4))
             fig.subplots_adjust(*p7)
-            ax = fig.gca(xscale='auto-gps')
+            ax = fig.gca()
+            ax.set_xscale('auto-gps')
             ax.plot(
                 times, scale(currentts.value)*numpy.sign(input_[1][1]),
                 label=texify(currentchan), linewidth=line_size_aux,
                 color=colors[0])
 
             for i in range(0, ncluster):
                 this = cluster[i]
@@ -210,15 +210,18 @@
 
         # create scaled, sign-corrected, and overlayed timeseries
         tsscaled = scale(ts.value)
         if lassocoef < 0:
             tsscaled = numpy.negative(tsscaled)
         fig = Plot(figsize=(12, 4))
         fig.subplots_adjust(*p1)
-        ax = fig.gca(xscale='auto-gps', epoch=start, xlim=xlim)
+        ax = fig.gca()
+        ax.set_xscale('auto-gps')
+        ax.set_epoch(start)
+        ax.set_xlim(xlim)
         ax.plot(times, _descaler(target), label=texify(primary),
                 color='black', linewidth=line_size_primary)
         ax.plot(times, _descaler(tsscaled), label=texify(chan),
                 linewidth=line_size_aux)
         if range_is_primary:
             ax.set_ylabel('Sensitive range [Mpc]')
         else:
@@ -586,33 +589,38 @@
         frametype = '%s_T' % args.ifo  # for second trends
 
     # read aux channels
     auxdata = get_data(
         channels, start, end, verbose='Reading:'.rjust(30),
         frametype=frametype, nproc=args.nproc, pad=0).crop(start, end)
 
+    # re-order aux channels to the same order as channel list
+
+    [auxdata.move_to_end(key=ch) for ch in channels if ch]
+
     # -- removes flat data to be re-introdused later
 
     LOGGER.info('-- Pre-processing auxiliary channel data')
-
     auxdata = gwlasso.remove_flat(auxdata)
     flatable = Table(data=(list(set(channels) - set(auxdata.keys())),),
                      names=('Channels',))
     LOGGER.debug('Removed {0} channels with flat data'.format(len(flatable)))
     LOGGER.debug('{0} channels remaining'.format(len(auxdata)))
 
     # -- remove bad data
 
     LOGGER.info("Removing any channels with bad data...")
     nbefore = len(auxdata)
     auxdata = gwlasso.remove_bad(auxdata)
     nafter = len(auxdata)
     LOGGER.debug('Removed {0} channels with bad data'.format(nbefore - nafter))
     LOGGER.debug('{0} channels remaining'.format(nafter))
-    data = numpy.array([scale(ts.value) for ts in auxdata.values()]).T
+    data = numpy.array([ts.value for ts in auxdata.values()]).T
+    scaler = StandardScaler()
+    data = scaler.fit_transform(data)
 
     # -- perform lasso regression -------------------
 
     # create model
     LOGGER.info('-- Fitting data to target')
     target = scale(primaryts.value)
     model = gwlasso.fit(data, target, alpha=args.alpha)
@@ -636,15 +644,15 @@
     # print results
     LOGGER.info('Found {} channels with |Lasso coefficient| >= {}:\n\n'.format(
                 len(results), threshold))
     print(results)
     print('\n\n')
 
     # convert to pandas
-    set_option('max_colwidth', -1)
+    set_option('max_colwidth', None)
     df = results.to_pandas()
     df.index += 1
 
     # write results to files
     gpsstub = '%d-%d' % (start, end-start)
     resultsfile = '%s-LASSO_RESULTS-%s.csv' % (args.ifo, gpsstub)
     results.write(resultsfile, format='csv', overwrite=True)
@@ -663,15 +671,18 @@
     times = primaryts.times.value
     xlim = primaryts.span
     cmap = get_cmap('tab20')
     colors = [cmap(i) for i in numpy.linspace(0, 1, len(nonzerodata)+1)]
 
     plot = Plot(figsize=(12, 4))
     plot.subplots_adjust(*p1)
-    ax = plot.gca(xscale='auto-gps', epoch=start, xlim=xlim)
+    ax = plot.gca()
+    ax.set_xscale('auto-gps')
+    ax.set_epoch(start)
+    ax.set_xlim(xlim)
     ax.plot(times, _descaler(target), label=texify(primary),
             color='black', linewidth=line_size_primary)
     ax.plot(times, _descaler(modelFit), label='Lasso model',
             linewidth=line_size_aux)
     if range_is_primary:
         ax.set_ylabel('Sensitive range [Mpc]')
         ax.set_title('Lasso Model of Range')
@@ -682,15 +693,18 @@
     plot1 = gwplot.save_figure(
          plot, '%s-LASSO_MODEL-%s.png' % (args.ifo, gpsstub),
          bbox_inches='tight')
 
     # summed contributions
     plot = Plot(figsize=(12, 4))
     plot.subplots_adjust(*p1)
-    ax = plot.gca(xscale='auto-gps', epoch=start, xlim=xlim)
+    ax = plot.gca()
+    ax.set_xscale('auto-gps')
+    ax.set_epoch(start)
+    ax.set_xlim(xlim)
     ax.plot(times, _descaler(target), label=texify(primary),
             color='black', linewidth=line_size_primary)
     summed = 0
     for i, name in enumerate(results['Channel']):
         summed += scale(nonzerodata[name].value) * nonzerocoef[name]
         if i:
             label = 'Channels 1-{0}'.format(i+1)
@@ -707,15 +721,18 @@
     plot2 = gwplot.save_figure(
         plot, '%s-LASSO_CHANNEL_SUMMATION-%s.png' % (args.ifo, gpsstub),
         bbox_inches='tight')
 
     # individual contributions
     plot = Plot(figsize=(12, 4))
     plot.subplots_adjust(*p1)
-    ax = plot.gca(xscale='auto-gps', epoch=start, xlim=xlim)
+    ax = plot.gca()
+    ax.set_xscale('auto-gps')
+    ax.set_epoch(start)
+    ax.set_xlim(xlim)
     ax.plot(times, _descaler(target), label=texify(primary),
             color='black', linewidth=line_size_primary)
     for i, name in enumerate(results['Channel']):
         this = _descaler(scale(nonzerodata[name].value) * nonzerocoef[name])
         if i:
             label = 'Channels 1-{0}'.format(i+1)
         else:
@@ -737,23 +754,25 @@
     LOGGER.info("-- Processing channels")
     counter = multiprocessing.Value('i', 0)
 
     # process channels
     pool = multiprocessing.Pool(nprocplot)
     results = pool.map(_process_channel, enumerate(list(nonzerodata.items())))
     results = sorted(results, key=lambda x: abs(x[1]), reverse=True)
+    pool.close()
 
     #  generate clustered time series plots
     counter = multiprocessing.Value('i', 0)
     max_correlated_channels = 20
 
     if args.no_cluster is False:
         LOGGER.info("-- Generating clusters")
         pool = multiprocessing.Pool(nprocplot)
         clusters = pool.map(_generate_cluster, enumerate(results))
+        pool.close()
 
     channelsfile = '%s-CHANNELS-%s.csv' % (args.ifo, gpsstub)
     numpy.savetxt(channelsfile, channels, delimiter=',', fmt='%s')
 
     # write html
     trange = '%d-%d' % (start, end)
     title = '%s Lasso Correlation: %s' % (args.ifo, trange)
```

### Comparing `gwdetchar-2.0.9/gwdetchar/lasso/core.py` & `gwdetchar-2.1.0/gwdetchar/lasso/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/lasso/old.py` & `gwdetchar-2.1.0/gwdetchar/lasso/old.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/lasso/plot.py` & `gwdetchar-2.1.0/gwdetchar/lasso/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/lasso/tests/__init__.py` & `gwdetchar-2.1.0/gwdetchar/lasso/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/lasso/tests/test_core.py` & `gwdetchar-2.1.0/gwdetchar/lasso/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/lasso/tests/test_main.py` & `gwdetchar-2.1.0/gwdetchar/lasso/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/lasso/tests/test_plot.py` & `gwdetchar-2.1.0/gwdetchar/lasso/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/mct.py` & `gwdetchar-2.1.0/gwdetchar/mct.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/nagios/__init__.py` & `gwdetchar-2.1.0/gwdetchar/nagios/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/nagios/__main__.py` & `gwdetchar-2.1.0/gwdetchar/nagios/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/nagios/core.py` & `gwdetchar-2.1.0/gwdetchar/nagios/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/nagios/tests/__init__.py` & `gwdetchar-2.1.0/gwdetchar/nagios/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/nagios/tests/test_main.py` & `gwdetchar-2.1.0/gwdetchar/nagios/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/__init__.py` & `gwdetchar-2.1.0/gwdetchar/omega/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/__main__.py` & `gwdetchar-2.1.0/gwdetchar/omega/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/batch.py` & `gwdetchar-2.1.0/gwdetchar/omega/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 import subprocess
 import sys
 
 from getpass import getuser
 from pycondor import (Dagman, Job)
 
 from .. import (cli, condor)
+from ..cli import NOW_GPS
 
 # authorship credits
 __author__ = 'Alex Urban <alexander.urban@ligo.org>'
 __credits__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 # set CLI docstring
 CLI_DOCSTRING = """Batch-generate a series of Omega scans
@@ -110,27 +111,27 @@
     if ignore_state_flags:
         flags.append("--ignore-state-flags")
     return flags
 
 
 def get_condor_arguments(accounting_group=ACCOUNTING_GROUP,
                          accounting_group_user=ACCOUNTING_GROUP_USER,
-                         timeout=0, extra_commands=[], gps=0):
+                         timeout=0, extra_commands=[], gps=NOW_GPS):
     """Get a list of arguments for Condor processing
     """
     # get reference epoch
     if '{epoch}' in accounting_group:
         epoch = condor.accounting_epoch(gps)
         accounting_group = accounting_group.format(epoch=epoch.lower())
     # validate accounting tag
     condor.is_valid(accounting_group)
     # determine condor arguments
     condorcmds = [
-        "accounting_group = {}".format(accounting_group),
-        "accounting_group_user = {}".format(accounting_group_user),
+        f"accounting_group = {accounting_group}",
+        f"accounting_group_user = {accounting_group_user}",
     ]
     if timeout:
         condorcmds.append("periodic_remove = {}".format(
             'CurrentTime-EnteredCurrentStatus > {}'.format(
                 3600 * timeout),
         ))
     condorcmds.extend(extra_commands)
```

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/config.py` & `gwdetchar-2.1.0/gwdetchar/omega/config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/core.py` & `gwdetchar-2.1.0/gwdetchar/omega/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/html.py` & `gwdetchar-2.1.0/gwdetchar/omega/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/plot.py` & `gwdetchar-2.1.0/gwdetchar/omega/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/tests/__init__.py` & `gwdetchar-2.1.0/gwdetchar/tests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright (C) Alex Urban (2019)
+# Copyright (C) Duncan Macleod (2015)
 #
 # This file is part of the GW DetChar python package.
 #
 # GW DetChar is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,11 +12,11 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with GW DetChar.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Tests for :mod:`gwdetchar.omega`
+"""Tests for `gwdetchar`
 """
 
-__author__ = 'Alex Urban <alexander.urban@ligo.org>'
+__author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
```

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/tests/test_batch.py` & `gwdetchar-2.1.0/gwdetchar/omega/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/tests/test_config.py` & `gwdetchar-2.1.0/gwdetchar/omega/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/tests/test_core.py` & `gwdetchar-2.1.0/gwdetchar/omega/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/tests/test_html.py` & `gwdetchar-2.1.0/gwdetchar/omega/tests/test_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,22 @@
 """
 
 import os
 import shutil
 from io import StringIO
 
 from .. import (config, html)
-from ..._version import get_versions
 from ...utils import parse_html
 
 __author__ = 'Alex Urban <alexander.urban@ligo.org>'
 __credits__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 
 
 # global test objects
 
-VERSION = get_versions()['version']
-COMMIT = get_versions()['full-revisionid']
-
 HTML_HEADER = """<nav class="navbar fixed-top navbar-expand-md navbar-{ifo} shadow-sm">
 <div class="container-fluid">
 <div class="navbar-brand border border-white rounded">{IFO} &Omega;-scan</div>
 <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target=".navbar-collapse">
 <span class="navbar-toggler-icon"></span>
 </button>
 <div class="collapse navbar-collapse justify-content-between">
```

#### html2text {}

```diff
@@ -6,19 +6,17 @@
 in the hope that it will be useful, # but WITHOUT ANY WARRANTY; without even
 the implied warranty of # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 See the # GNU General Public License for more details. # # You should have
 received a copy of the GNU General Public License # along with gwdetchar. If
 not, see
 www.gnu.org/licenses/>. """Tests for `gwdetchar.omega.html` """ import os
 import shutil from io import StringIO from .. import (config, html) from
-..._version import get_versions from ...utils import parse_html __author__ =
-'Alex Urban
+...utils import parse_html __author__ = 'Alex Urban
 urban@ligo.org>' __credits__ = 'Duncan Macleod
-macleod@ligo.org>' # global test objects VERSION = get_versions()['version']
-COMMIT = get_versions()['full-revisionid'] HTML_HEADER = """
+macleod@ligo.org>' # global test objects HTML_HEADER = """
 {IFO} Ω-scan
 
     * 0
     * Summary
     * GW
       * Gravitational-Wave Strain *
       X1:TEST-AUX
```

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/tests/test_main.py` & `gwdetchar-2.1.0/gwdetchar/omega/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/omega/tests/test_plot.py` & `gwdetchar-2.1.0/gwdetchar/omega/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/overflow.py` & `gwdetchar-2.1.0/gwdetchar/overflow.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/plot.py` & `gwdetchar-2.1.0/gwdetchar/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/saturation/__init__.py` & `gwdetchar-2.1.0/gwdetchar/saturation/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/saturation/__main__.py` & `gwdetchar-2.1.0/gwdetchar/saturation/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/saturation/core.py` & `gwdetchar-2.1.0/gwdetchar/saturation/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/saturation/tests/__init__.py` & `gwdetchar-2.1.0/gwdetchar/saturation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/saturation/tests/test_saturation.py` & `gwdetchar-2.1.0/gwdetchar/saturation/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/__init__.py` & `gwdetchar-2.1.0/gwdetchar/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/__main__.py` & `gwdetchar-2.1.0/gwdetchar/scattering/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/core.py` & `gwdetchar-2.1.0/gwdetchar/scattering/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/plot.py` & `gwdetchar-2.1.0/gwdetchar/scattering/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/simple.py` & `gwdetchar-2.1.0/gwdetchar/scattering/simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/tests/__init__.py` & `gwdetchar-2.1.0/gwdetchar/scattering/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/tests/test_core.py` & `gwdetchar-2.1.0/gwdetchar/scattering/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/tests/test_main.py` & `gwdetchar-2.1.0/gwdetchar/scattering/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/tests/test_plot.py` & `gwdetchar-2.1.0/gwdetchar/scattering/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/scattering/tests/test_simple.py` & `gwdetchar-2.1.0/gwdetchar/scattering/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/tests/test_cds.py` & `gwdetchar-2.1.0/gwdetchar/tests/test_cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/tests/test_cli.py` & `gwdetchar-2.1.0/gwdetchar/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/tests/test_condor.py` & `gwdetchar-2.1.0/gwdetchar/tests/test_condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/tests/test_conlog.py` & `gwdetchar-2.1.0/gwdetchar/tests/test_conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/tests/test_const.py` & `gwdetchar-2.1.0/gwdetchar/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/tests/test_daq.py` & `gwdetchar-2.1.0/gwdetchar/tests/test_daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/tests/test_plot.py` & `gwdetchar-2.1.0/gwdetchar/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/tests/test_utils.py` & `gwdetchar-2.1.0/gwdetchar/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar/utils.py` & `gwdetchar-2.1.0/gwdetchar/utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.0.9/gwdetchar.egg-info/PKG-INFO` & `gwdetchar-2.1.0/gwdetchar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.0.9
+Version: 2.1.0
 Summary: A python package for gravitational-wave detector characterisation
-Home-page: https://github.com/gwdetchar/gwdetchar/
-Author: Alex Urban, Duncan Macleod
-Author-email: alexander.urban@ligo.org
+Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
+Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
-Keywords: physics,astronomy,gravitational-waves,ligo
+Project-URL: Documentation, https://gwdetchar.readthedocs.io
+Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
+Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
+Project-URL: Discussion Forum, https://gwdetchar.slack.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE
 
 ############################################
 Gravitational-wave Detector Characterisation
 ############################################
```

### Comparing `gwdetchar-2.0.9/gwdetchar.egg-info/entry_points.txt` & `gwdetchar-2.1.0/gwdetchar.egg-info/entry_points.txt`

 * *Files identical despite different names*

