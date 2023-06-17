# Comparing `tmp/swmmtoolbox-4.0.6.tar.gz` & `tmp/swmmtoolbox-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swmmtoolbox-4.0.6.tar", last modified: Tue Feb 14 02:35:28 2023, max compression
+gzip compressed data, was "swmmtoolbox-4.0.7.tar", last modified: Sat Jun 17 04:16:25 2023, max compression
```

## Comparing `swmmtoolbox-4.0.6.tar` & `swmmtoolbox-4.0.7.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 02:35:28.973460 swmmtoolbox-4.0.6/
--rw-rw-r--   0 tim       (1000) tim       (1000)      102 2023-02-12 05:11:36.000000 swmmtoolbox-4.0.6/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 02:35:28.953460 swmmtoolbox-4.0.6/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 02:35:28.957460 swmmtoolbox-4.0.6/.github/workflows/
--rw-rw-r--   0 tim       (1000) tim       (1000)      505 2023-02-12 05:11:36.000000 swmmtoolbox-4.0.6/.github/workflows/clean-workflow-runs.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-02-12 05:11:36.000000 swmmtoolbox-4.0.6/.github/workflows/python-package.yml
--rw-r--r--   0 tim       (1000) tim       (1000)      290 2021-08-07 16:03:06.000000 swmmtoolbox-4.0.6/.gitignore
--rw-r--r--   0 tim       (1000) tim       (1000)       85 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.6/.hgignore
--rw-r--r--   0 tim       (1000) tim       (1000)     2787 2023-02-14 02:07:47.000000 swmmtoolbox-4.0.6/.pre-commit-config.yaml
--rw-r--r--   0 tim       (1000) tim       (1000)       31 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.6/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1038 2022-09-28 02:50:14.000000 swmmtoolbox-4.0.6/BADGES.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     1250 2023-02-14 02:12:14.000000 swmmtoolbox-4.0.6/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3094 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.6/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1488 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.6/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     2859 2023-02-14 02:35:28.973460 swmmtoolbox-4.0.6/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     1385 2022-12-11 04:23:26.000000 swmmtoolbox-4.0.6/README.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)        6 2023-02-14 02:12:14.000000 swmmtoolbox-4.0.6/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 02:35:28.957460 swmmtoolbox-4.0.6/docs/
--rw-r--r--   0 tim       (1000) tim       (1000)     5580 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.6/docs/Makefile
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.6/docs/authors.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      648 2023-01-08 06:36:30.000000 swmmtoolbox-4.0.6/docs/command_line.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     8034 2023-01-22 03:38:20.000000 swmmtoolbox-4.0.6/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.6/docs/contributing.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      401 2023-01-02 07:22:50.000000 swmmtoolbox-4.0.6/docs/function_summary.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      498 2023-01-02 05:48:31.000000 swmmtoolbox-4.0.6/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.6/docs/license.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2021-12-16 19:04:32.000000 swmmtoolbox-4.0.6/docs/make.bat
--rw-r--r--   0 tim       (1000) tim       (1000)       27 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.6/docs/readme.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      574 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.6/docs/usage.rst
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 02:35:28.965460 swmmtoolbox-4.0.6/interfacing_guide/
--rw-r--r--   0 tim       (1000) tim       (1000)    40220 2020-02-20 11:55:02.000000 swmmtoolbox-4.0.6/interfacing_guide/Interfacing.chm
--rw-r--r--   0 tim       (1000) tim       (1000)      787 2022-06-18 22:56:24.000000 swmmtoolbox-4.0.6/interfacing_guide/readme.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      809 2020-02-20 11:55:02.000000 swmmtoolbox-4.0.6/interfacing_guide/swmm5.bas
--rw-r--r--   0 tim       (1000) tim       (1000)     1583 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.6/interfacing_guide/swmm5.h
--rw-r--r--   0 tim       (1000) tim       (1000)     4860 2020-02-20 11:55:02.000000 swmmtoolbox-4.0.6/interfacing_guide/swmm5.lib
--rw-r--r--   0 tim       (1000) tim       (1000)      959 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.6/interfacing_guide/swmm5.pas
--rw-r--r--   0 tim       (1000) tim       (1000)    10858 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.6/interfacing_guide/swmm5_iface.bas
--rw-r--r--   0 tim       (1000) tim       (1000)     8838 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.6/interfacing_guide/swmm5_iface.c
--rw-r--r--   0 tim       (1000) tim       (1000)      998 2020-02-20 11:55:02.000000 swmmtoolbox-4.0.6/interfacing_guide/swmm5_iface.h
--rw-r--r--   0 tim       (1000) tim       (1000)     8564 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.6/interfacing_guide/swmm5_iface.pas
--rw-r--r--   0 tim       (1000) tim       (1000)     1800 2022-06-18 22:56:24.000000 swmmtoolbox-4.0.6/interfacing_guide/test.c
--rw-rw-r--   0 tim       (1000) tim       (1000)     2788 2023-02-14 02:12:15.000000 swmmtoolbox-4.0.6/pyproject.toml
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-02-14 02:35:28.973460 swmmtoolbox-4.0.6/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)      490 2023-01-22 03:38:20.000000 swmmtoolbox-4.0.6/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 02:35:28.953460 swmmtoolbox-4.0.6/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 02:35:28.965460 swmmtoolbox-4.0.6/src/swmmtoolbox/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:20.000000 swmmtoolbox-4.0.6/src/swmmtoolbox/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    26266 2023-02-14 02:08:28.000000 swmmtoolbox-4.0.6/src/swmmtoolbox/swmmtoolbox.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 02:35:28.965460 swmmtoolbox-4.0.6/src/swmmtoolbox.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)     2859 2023-02-14 02:35:28.000000 swmmtoolbox-4.0.6/src/swmmtoolbox.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     1226 2023-02-14 02:35:28.000000 swmmtoolbox-4.0.6/src/swmmtoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2023-02-14 02:35:28.000000 swmmtoolbox-4.0.6/src/swmmtoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       61 2023-02-14 02:35:28.000000 swmmtoolbox-4.0.6/src/swmmtoolbox.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      258 2023-02-14 02:35:28.000000 swmmtoolbox-4.0.6/src/swmmtoolbox.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       12 2023-02-14 02:35:28.000000 swmmtoolbox-4.0.6/src/swmmtoolbox.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-02-14 02:35:28.973460 swmmtoolbox-4.0.6/tests/
--rw-rw-r--   0 tim       (1000) tim       (1000)     3642 2021-12-10 12:27:28.000000 swmmtoolbox-4.0.6/tests/extract_link.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)     3258 2021-12-10 12:30:01.000000 swmmtoolbox-4.0.6/tests/extract_node.csv
--rw-r--r--   0 tim       (1000) tim       (1000)  2493442 2020-02-20 11:55:08.000000 swmmtoolbox-4.0.6/tests/frutal.out
--rw-r--r--   0 tim       (1000) tim       (1000)     8667 2020-02-20 11:55:08.000000 swmmtoolbox-4.0.6/tests/listdetail_link.csv
--rw-r--r--   0 tim       (1000) tim       (1000)     6228 2020-02-20 11:55:06.000000 swmmtoolbox-4.0.6/tests/listdetail_node.csv
--rw-rw-r--   0 tim       (1000) tim       (1000)     4363 2023-01-22 03:38:20.000000 swmmtoolbox-4.0.6/tests/test_extract.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1451 2023-02-14 02:11:03.000000 swmmtoolbox-4.0.6/tests/test_listdetail.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-17 04:16:25.644079 swmmtoolbox-4.0.7/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      102 2023-06-10 22:19:08.000000 swmmtoolbox-4.0.7/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-17 04:16:25.620079 swmmtoolbox-4.0.7/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-17 04:16:25.624079 swmmtoolbox-4.0.7/.github/workflows/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      501 2023-06-17 04:11:21.000000 swmmtoolbox-4.0.7/.github/workflows/clean-workflow-runs.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-06-10 22:19:08.000000 swmmtoolbox-4.0.7/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      298 2023-03-05 18:50:14.000000 swmmtoolbox-4.0.7/.gitignore
+-rw-r--r--   0 tim       (1000) tim       (1000)       85 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.7/.hgignore
+-rw-r--r--   0 tim       (1000) tim       (1000)     2651 2023-06-17 04:11:21.000000 swmmtoolbox-4.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 tim       (1000) tim       (1000)       31 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.7/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1038 2022-09-28 02:50:14.000000 swmmtoolbox-4.0.7/BADGES.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1352 2023-06-17 04:15:10.000000 swmmtoolbox-4.0.7/CHANGELOG.md
+-rw-r--r--   0 tim       (1000) tim       (1000)     3094 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.7/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1488 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.7/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4035 2023-06-17 04:16:25.644079 swmmtoolbox-4.0.7/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     2561 2023-06-17 01:14:34.000000 swmmtoolbox-4.0.7/README.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)        6 2023-06-17 04:15:10.000000 swmmtoolbox-4.0.7/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-17 04:16:25.628079 swmmtoolbox-4.0.7/docs/
+-rw-r--r--   0 tim       (1000) tim       (1000)     5580 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.7/docs/Makefile
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.7/docs/authors.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      648 2023-05-13 04:19:59.000000 swmmtoolbox-4.0.7/docs/command_line.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     8034 2023-01-22 03:38:20.000000 swmmtoolbox-4.0.7/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.7/docs/contributing.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      317 2023-06-17 00:16:25.000000 swmmtoolbox-4.0.7/docs/function_summary.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      498 2023-01-02 05:48:31.000000 swmmtoolbox-4.0.7/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.7/docs/license.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5104 2021-12-16 19:04:32.000000 swmmtoolbox-4.0.7/docs/make.bat
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2020-02-20 11:55:00.000000 swmmtoolbox-4.0.7/docs/readme.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      574 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.7/docs/usage.rst
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-17 04:16:25.636079 swmmtoolbox-4.0.7/interfacing_guide/
+-rw-r--r--   0 tim       (1000) tim       (1000)    40220 2020-02-20 11:55:02.000000 swmmtoolbox-4.0.7/interfacing_guide/Interfacing.chm
+-rw-r--r--   0 tim       (1000) tim       (1000)      787 2022-06-18 22:56:24.000000 swmmtoolbox-4.0.7/interfacing_guide/readme.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      809 2020-02-20 11:55:02.000000 swmmtoolbox-4.0.7/interfacing_guide/swmm5.bas
+-rw-r--r--   0 tim       (1000) tim       (1000)     1583 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.7/interfacing_guide/swmm5.h
+-rw-r--r--   0 tim       (1000) tim       (1000)     4860 2020-02-20 11:55:02.000000 swmmtoolbox-4.0.7/interfacing_guide/swmm5.lib
+-rw-r--r--   0 tim       (1000) tim       (1000)      959 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.7/interfacing_guide/swmm5.pas
+-rw-r--r--   0 tim       (1000) tim       (1000)    10858 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.7/interfacing_guide/swmm5_iface.bas
+-rw-r--r--   0 tim       (1000) tim       (1000)     8838 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.7/interfacing_guide/swmm5_iface.c
+-rw-r--r--   0 tim       (1000) tim       (1000)      998 2020-02-20 11:55:02.000000 swmmtoolbox-4.0.7/interfacing_guide/swmm5_iface.h
+-rw-r--r--   0 tim       (1000) tim       (1000)     8564 2021-06-20 02:30:44.000000 swmmtoolbox-4.0.7/interfacing_guide/swmm5_iface.pas
+-rw-r--r--   0 tim       (1000) tim       (1000)     1800 2022-06-18 22:56:24.000000 swmmtoolbox-4.0.7/interfacing_guide/test.c
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2788 2023-06-17 04:15:11.000000 swmmtoolbox-4.0.7/pyproject.toml
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-06-17 04:16:25.644079 swmmtoolbox-4.0.7/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)      515 2023-03-01 21:51:19.000000 swmmtoolbox-4.0.7/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-17 04:16:25.624079 swmmtoolbox-4.0.7/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-17 04:16:25.636079 swmmtoolbox-4.0.7/src/swmmtoolbox/
+-rw-r--r--   0 tim       (1000) tim       (1000)       27 2023-06-17 01:14:35.000000 swmmtoolbox-4.0.7/src/swmmtoolbox/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    25250 2023-06-17 00:06:18.000000 swmmtoolbox-4.0.7/src/swmmtoolbox/swmmtoolbox.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-17 04:16:25.636079 swmmtoolbox-4.0.7/src/swmmtoolbox.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)     4035 2023-06-17 04:16:25.000000 swmmtoolbox-4.0.7/src/swmmtoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     1226 2023-06-17 04:16:25.000000 swmmtoolbox-4.0.7/src/swmmtoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2023-06-17 04:16:25.000000 swmmtoolbox-4.0.7/src/swmmtoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       61 2023-06-17 04:16:25.000000 swmmtoolbox-4.0.7/src/swmmtoolbox.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      258 2023-06-17 04:16:25.000000 swmmtoolbox-4.0.7/src/swmmtoolbox.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       12 2023-06-17 04:16:25.000000 swmmtoolbox-4.0.7/src/swmmtoolbox.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-17 04:16:25.644079 swmmtoolbox-4.0.7/tests/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3642 2021-12-10 12:27:28.000000 swmmtoolbox-4.0.7/tests/extract_link.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3258 2021-12-10 12:30:01.000000 swmmtoolbox-4.0.7/tests/extract_node.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)  2493442 2020-02-20 11:55:08.000000 swmmtoolbox-4.0.7/tests/frutal.out
+-rw-r--r--   0 tim       (1000) tim       (1000)     8667 2020-02-20 11:55:08.000000 swmmtoolbox-4.0.7/tests/listdetail_link.csv
+-rw-r--r--   0 tim       (1000) tim       (1000)     6228 2020-02-20 11:55:06.000000 swmmtoolbox-4.0.7/tests/listdetail_node.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4358 2023-05-13 06:04:56.000000 swmmtoolbox-4.0.7/tests/test_extract.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1446 2023-05-13 06:05:03.000000 swmmtoolbox-4.0.7/tests/test_listdetail.py
```

### Comparing `swmmtoolbox-4.0.6/.github/workflows/python-package.yml` & `swmmtoolbox-4.0.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/.pre-commit-config.yaml` & `swmmtoolbox-4.0.7/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 ---
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 
-default_language_version:
-    python: python3.8
-
 repos:
     - repo: https://github.com/pre-commit/pre-commit-hooks
       rev: v4.4.0
       hooks:
           - id: check-case-conflict
           - id: check-docstring-first
           - id: check-executables-have-shebangs
@@ -22,27 +19,27 @@
           - id: fix-encoding-pragma
             args: [--remove]
           - id: mixed-line-ending
           - id: trailing-whitespace
             exclude: notebooks/tstoolbox_plot_bash.sh
 
     - repo: https://github.com/pappasam/toml-sort
-      rev: v0.22.3
+      rev: v0.23.1
       hooks:
           - id: toml-sort-fix
             args: [--in-place, --spaces-indent-inline-array, '4']
 
     - repo: https://github.com/adrienverge/yamllint.git
-      rev: v1.29.0
+      rev: v1.32.0
       hooks:
           - id: yamllint
             args: [--format, parsable, --strict]
 
     - repo: https://github.com/jumanjihouse/pre-commit-hook-yamlfmt
-      rev: 0.2.2
+      rev: 0.2.3
       hooks:
           - id: yamlfmt
 
     - repo: https://github.com/jumanjihouse/pre-commit-hooks
       rev: 3.0.0
       hooks:
           - id: shellcheck
@@ -51,17 +48,18 @@
     - repo: https://github.com/lovesegfault/beautysh
       rev: v6.2.1
       hooks:
           - id: beautysh
             args: [--indent-size, '4']
 
     - repo: https://github.com/psf/black
-      rev: 23.1.0
+      rev: 23.3.0
       hooks:
           - id: black
+          - id: black-jupyter
 
     - repo: https://github.com/pycqa/isort
       rev: 5.12.0
       hooks:
           - id: isort
             name: isort (python)
             args: [--profile, black, --filter-files]
@@ -70,33 +68,28 @@
             types: [cython]
             args: [--profile, black, --filter-files]
           - id: isort
             name: isort (pyi)
             types: [pyi]
             args: [--profile, black, --filter-files]
 
-    - repo: https://github.com/dfm/black_nbconvert
-      rev: v0.4.0
-      hooks:
-          - id: black_nbconvert
-
     - repo: https://github.com/asottile/blacken-docs
       rev: 1.13.0
       hooks:
           - id: blacken-docs
 
     - repo: https://github.com/asottile/pyupgrade
-      rev: v3.3.1
+      rev: v3.6.0
       hooks:
           - id: pyupgrade
 
     - repo: https://github.com/commitizen-tools/commitizen
-      rev: v2.41.0
+      rev: 3.2.2
       hooks:
           - id: commitizen
             stages: [commit-msg]
 
     - repo: https://github.com/mwouts/jupytext
-      rev: v1.14.4
+      rev: v1.14.6
       hooks:
           - id: jupytext
             args: [--from, ipynb, --to, auto:percent, --sync]
```

### Comparing `swmmtoolbox-4.0.6/BADGES.rst` & `swmmtoolbox-4.0.7/BADGES.rst`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/CHANGELOG.md` & `swmmtoolbox-4.0.7/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v4.0.7 (2023-06-17)
+
+### Refactor
+
+- moved all command line functions into main and improved docs
+
 ## v4.0.6 (2023-02-13)
 
 ### Refactor
 
 - small refactors
 
 ## v4.0.5 (2023-01-16)
```

### Comparing `swmmtoolbox-4.0.6/CONTRIBUTING.rst` & `swmmtoolbox-4.0.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/LICENSE.txt` & `swmmtoolbox-4.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/docs/Makefile` & `swmmtoolbox-4.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/docs/command_line.rst` & `swmmtoolbox-4.0.7/docs/command_line.rst`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/docs/conf.py` & `swmmtoolbox-4.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/docs/make.bat` & `swmmtoolbox-4.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/docs/usage.rst` & `swmmtoolbox-4.0.7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/Interfacing.chm` & `swmmtoolbox-4.0.7/interfacing_guide/Interfacing.chm`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/readme.txt` & `swmmtoolbox-4.0.7/interfacing_guide/readme.txt`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/swmm5.bas` & `swmmtoolbox-4.0.7/interfacing_guide/swmm5.bas`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/swmm5.h` & `swmmtoolbox-4.0.7/interfacing_guide/swmm5.h`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/swmm5.lib` & `swmmtoolbox-4.0.7/interfacing_guide/swmm5.lib`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/swmm5.pas` & `swmmtoolbox-4.0.7/interfacing_guide/swmm5.pas`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/swmm5_iface.bas` & `swmmtoolbox-4.0.7/interfacing_guide/swmm5_iface.bas`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/swmm5_iface.c` & `swmmtoolbox-4.0.7/interfacing_guide/swmm5_iface.c`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/swmm5_iface.h` & `swmmtoolbox-4.0.7/interfacing_guide/swmm5_iface.h`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/swmm5_iface.pas` & `swmmtoolbox-4.0.7/interfacing_guide/swmm5_iface.pas`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/interfacing_guide/test.c` & `swmmtoolbox-4.0.7/interfacing_guide/test.c`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/pyproject.toml` & `swmmtoolbox-4.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     ".ipynb_checkpoints/*"
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "4.0.6"
+version = "4.0.7"
 version_files = ["VERSION"]
 
 [tool.isort]
 profile = "black"
 
 [tool.setuptools]
 license-files = ["LICENSE.txt"]
```

### Comparing `swmmtoolbox-4.0.6/src/swmmtoolbox/swmmtoolbox.py` & `swmmtoolbox-4.0.7/src/swmmtoolbox/swmmtoolbox.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,20 @@
 
 import copy
 import csv
 import datetime
 import os
 import struct
 import sys
-import warnings
 from contextlib import suppress
 
-import numpy as np
 import pandas as pd
-from cltoolbox import Program
-from cltoolbox.rst_text_formatter import RSTHelpFormatter
 from toolbox_utils import tsutils
 
-program = Program("swmmtoolbox", 0.0)
+__all__ = ["catalog", "listdetail", "listvariables", "stdtoswmm5", "extract"]
 
 PROPCODE = {
     0: {1: "Area"},
     1: {0: "Type", 2: "Inv_elev", 3: "Max_depth"},
     2: {0: "Type", 4: "Inv_offset", 3: "Max_depth", 5: "Length"},
 }
 
@@ -399,14 +395,15 @@
             + self.swmm_nsubcatch * self.swmm_nsubcatchvars
             + self.swmm_nnodes * self.nnodevars
             + self.swmm_nlinks * self.nlinkvars
             + self.nsystemvars
         )
 
     def type_check(self, itemtype):
+        """Type check the itemtype argument."""
         if itemtype in (0, 1, 2, 3, 4):
             return itemtype
 
         try:
             typenumber = self.itemlist.index(itemtype)
         except ValueError as exc:
             raise ValueError(
@@ -416,28 +413,30 @@
                     "{list(range(5)) + self.itemlist}".
                     """
                 )
             ) from exc
         return typenumber
 
     def name_check(self, itemtype, itemname):
+        """Check that the itemname is in the itemtype list."""
         self.itemtype = self.type_check(itemtype)
         try:
             itemindex = self.names[self.itemtype].index(str(itemname))
         except (ValueError, KeyError) as exc:
             raise ValueError(
                 tsutils.error_wrapper(
                     f"""
                     {itemname} was not found in "{itemtype}" list.
                     """
                 )
             ) from exc
         return (itemname, itemindex)
 
     def get_swmm_results(self, itemtype, name, variableindex, period):
+        """Get the SWMM results for the given itemtype, name, variableindex, and period."""
         if itemtype not in (0, 1, 2, 4):
             raise ValueError(
                 tsutils.error_wrapper(
                     f"""
                     Type must be one of subcatchment (0), node (1). link (2),
                     or system (4). You gave "{itemtype}".
                     """
@@ -477,44 +476,28 @@
         offset = offset + self.record_size * variableindex
 
         self.fpb.seek(offset, 0)
         value = struct.unpack("f", self.fpb.read(self.record_size))[0]
         return (date, value)
 
 
-@program.command()
-def about():
-    """Display version number and system information."""
-    tsutils.about(__name__)
-
-
-@program.command("catalog", formatter_class=RSTHelpFormatter)
 @tsutils.doc(_LOCAL_DOCSTRINGS)
-def catalog_cli(filename, itemtype="", tablefmt="csv_nos", header="default"):
+def catalog(filename, itemtype=""):
     """List the catalog of objects in output file.
 
     This catalog list is all of the labels that can be used in the extract
     routine.
 
     Parameters
     ----------
     ${filename}
     ${itemtype}
     ${tablefmt}
     ${header}
     """
-    if header == "default":
-        header = ["TYPE", "NAME", "VARIABLE"]
-    tsutils.printiso(
-        catalog(filename, itemtype=itemtype), headers=header, tablefmt=tablefmt
-    )
-
-
-def catalog(filename, itemtype=""):
-    """List the catalog of objects in output file."""
     obj = SwmmExtract(filename)
     if itemtype:
         typenumber = obj.type_check(itemtype)
         plist = [typenumber]
     else:
         plist = list(range(len(obj.itemlist)))
     collect = []
@@ -527,17 +510,16 @@
                 collect.append(["system", oname, oname])
                 continue
             for j in obj.vars[typenumber]:
                 collect.append([obj.itemlist[i], oname, obj.varcode[typenumber][j]])
     return collect
 
 
-@program.command("listdetail", formatter_class=RSTHelpFormatter)
 @tsutils.doc(_LOCAL_DOCSTRINGS)
-def listdetail_cli(filename, itemtype, name="", tablefmt="simple", header="default"):
+def listdetail(filename, itemtype, name="", header="default"):
     """List nodes and metadata in output file.
 
     Parameters
     ----------
     ${filename}
 
     ${itemtype}
@@ -548,21 +530,14 @@
         Specific name to print only that entry.  This can be
         looked up using 'listvariables'.
 
     ${tablefmt}
 
     ${header}
     """
-    tsutils.printiso(
-        listdetail(filename, itemtype, name=name, header=header), tablefmt=tablefmt
-    )
-
-
-def listdetail(filename, itemtype, name="", header="default"):
-    """List nodes and metadata in output file."""
     obj = SwmmExtract(filename)
     typenumber = obj.type_check(itemtype)
     if name:
         objectlist = [obj.name_check(itemtype, name)[0]]
     else:
         objectlist = obj.names[typenumber]
 
@@ -590,33 +565,26 @@
         else:
             cnt = cheader.count(head)
             cheader.append(f"{head}.{cnt}")
     dfc.columns = cheader
     return dfc
 
 
-@program.command("listvariables", formatter_class=RSTHelpFormatter)
 @tsutils.doc(_LOCAL_DOCSTRINGS)
-def listvariables_cli(filename, tablefmt="csv_nos", header="default"):
+def listvariables(filename, header="default"):
     """List variables available for each type.
 
     The type are "subcatchment", "node", "link", "pollutant", "system".
 
     Parameters
     ----------
     ${filename}
     ${tablefmt}
     ${header}
     """
-
-    tsutils.printiso(listvariables(filename, header=header), tablefmt=tablefmt)
-
-
-def listvariables(filename, header="default"):
-    """List variables available for each type."""
     obj = SwmmExtract(filename)
     if header == "default":
         header = ["TYPE", "DESCRIPTION", "VARINDEX"]
     # 'pollutant' really isn't it's own itemtype
     # but part of subcatchment, node, and link...
     collect = []
     for itemtype in ("subcatchment", "node", "link", "system"):
@@ -626,17 +594,16 @@
             try:
                 collect.append([itemtype, obj.varcode[typenumber][i].decode(), i])
             except (TypeError, AttributeError):
                 collect.append([itemtype, str(obj.varcode[typenumber][i]), str(i)])
     return collect
 
 
-@program.command("stdtoswmm5", formatter_class=RSTHelpFormatter)
 @tsutils.doc(_LOCAL_DOCSTRINGS)
-def stdtoswmm5_cli(start_date=None, end_date=None, input_ts="-"):
+def stdtoswmm5(start_date=None, end_date=None, input_ts="-"):
     """Take the toolbox standard format and return SWMM5 format.
 
     Toolbox standard::
 
        Datetime, Column_Name
        2000-01-01 00:00:00 ,  45.6
        2000-01-01 01:00:00 ,  45.2
@@ -651,21 +618,14 @@
 
     Parameters
     ----------
     ${input_ts}
     ${start_date}
     ${end_date}
     """
-    tsutils.printiso(
-        stdtoswmm5(start_date=start_date, end_date=end_date, input_ts=input_ts)
-    )
-
-
-def stdtoswmm5(start_date=None, end_date=None, input_ts="-"):
-    """Take the toolbox standard format and return SWMM5 format."""
     sys.tracebacklimit = 1000
     tsd = tsutils.read_iso_ts(input_ts)[start_date:end_date]
     try:
         # Header
         print(";Datetime,", ", ".join(str(i) for i in tsd.columns))
 
         # Data
@@ -685,37 +645,24 @@
             sep=" ",
             quoting=csv.QUOTE_NONE,
         )
     except OSError:
         return
 
 
-@program.command(formatter_class=RSTHelpFormatter)
-@tsutils.doc(_LOCAL_DOCSTRINGS)
-def getdata(filename, *labels):
-    """DEPRECATED: Use 'extract' instead."""
-    return extract(filename, *labels)
-
-
-@program.command("extract", formatter_class=RSTHelpFormatter)
 @tsutils.doc(_LOCAL_DOCSTRINGS)
-def extract_cli(filename, *labels):
+def extract(filename, *labels):
     """Get the time series data for a particular object and variable.
 
     Parameters
     ----------
     ${filename}
     ${labels}
 
     """
-    tsutils.printiso(extract(filename, *labels))
-
-
-def extract(filename, *labels):
-    """Get the time series data for a particular object and variable."""
     obj = SwmmExtract(filename)
     nlabels = []
 
     # Don't look at the following code. It's just a hack to get the
     # labels to work with the old syntax.
     labels = tsutils.make_list(labels, sep=" ", flat=True)
     plabels = []
@@ -776,61 +723,66 @@
                 columns=[f"{itemtype}_{name}_{obj.varcode[typenumber][variableindex]}"],
             )
         )
     result = pd.concat(jtsd, axis=1).reindex(jtsd[0].index)
     return result
 
 
-@tsutils.doc(_LOCAL_DOCSTRINGS)
-def extract_arr(filename, *labels):
-    """DEPRECATED: Extract and return the raw numpy array.
-
-    DEPRECATED: Will be removed in future version. Instead use the following.
-
-    >>> from swmmtoolbox import swmmtoolbox
-    >>> na = swmmtoolbox.extract("filename.out", "link,41a,Flow_rate")[0].to_array()
-
-    The `extract_arr` function will return the numpy array for the last entry
-    in "*labels".
-
-    Parameters
-    ----------
-    ${filename}
-    ${labels}
+def main():
+    """Command line interface."""
 
-    """
-    warnings.warn(
-        tsutils.error_wrapper(
-            """
-            DEPRECATED: Will be removed in future version. Instead use the
-            following.
+    import cltoolbox
+    from cltoolbox.rst_text_formatter import RSTHelpFormatter
 
-            >>> from swmmtoolbox import swmmtoolbox
+    if not os.path.exists("debug_swmmtoolbox"):
+        sys.tracebacklimit = 0
 
-            >>> na = swmmtoolbox.extract("filename.out", "link,41a,Flow_rate")[0].to_array()
-            """
+    @cltoolbox.command()
+    def about():
+        """Display version number and system information."""
+        tsutils.about(__name__)
+
+    @cltoolbox.command("catalog", formatter_class=RSTHelpFormatter)
+    @tsutils.copy_doc(catalog)
+    def catalog_cli(filename, itemtype="", tablefmt="csv_nos", header="default"):
+        """List the catalog in a SWMM5 file."""
+        if header == "default":
+            header = ["TYPE", "NAME", "VARIABLE"]
+        tsutils.printiso(
+            catalog(filename, itemtype=itemtype), headers=header, tablefmt=tablefmt
+        )
+
+    @cltoolbox.command("extract", formatter_class=RSTHelpFormatter)
+    @tsutils.copy_doc(extract)
+    def extract_cli(filename, *labels):
+        """Get the time series data for a particular object and variable."""
+        tsutils.printiso(extract(filename, *labels))
+
+    @cltoolbox.command("listdetail", formatter_class=RSTHelpFormatter)
+    @tsutils.copy_doc(listdetail)
+    def listdetail_cli(
+        filename, itemtype, name="", tablefmt="simple", header="default"
+    ):
+        """List the variables in a SWMM5 file."""
+        tsutils.printiso(
+            listdetail(filename, itemtype, name=name, header=header), tablefmt=tablefmt
+        )
+
+    @cltoolbox.command("listvariables", formatter_class=RSTHelpFormatter)
+    @tsutils.copy_doc(listvariables)
+    def listvariables_cli(filename, tablefmt="csv_nos", header="default"):
+        """List the variables in a SWMM5 file."""
+        tsutils.printiso(listvariables(filename, header=header), tablefmt=tablefmt)
+
+    @cltoolbox.command("stdtoswmm5", formatter_class=RSTHelpFormatter)
+    @tsutils.copy_doc(stdtoswmm5)
+    def stdtoswmm5_cli(start_date=None, end_date=None, input_ts="-"):
+        """Convert standard time series to SWMM5 time series."""
+        tsutils.printiso(
+            stdtoswmm5(start_date=start_date, end_date=end_date, input_ts=input_ts)
         )
-    )
-    obj = SwmmExtract(filename)
-    for label in labels:
-        itemtype, name, variableindex = tsutils.make_list(label, n=3)
-        typenumber = obj.type_check(itemtype)
-        if itemtype != "system":
-            name = obj.name_check(itemtype, name)[0]
-
-        data = np.zeros(len(list(range(obj.swmm_nperiods))))
-
-        for time in range(obj.swmm_nperiods):
-            _, value = obj.get_swmm_results(typenumber, name, int(variableindex), time)
-            data[time] = value
-
-    return data
-
 
-def main():
-    if not os.path.exists("debug_swmmtoolbox"):
-        sys.tracebacklimit = 0
-    program()
+    cltoolbox.main()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `swmmtoolbox-4.0.6/src/swmmtoolbox.egg-info/SOURCES.txt` & `swmmtoolbox-4.0.7/src/swmmtoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/tests/extract_link.csv` & `swmmtoolbox-4.0.7/tests/extract_link.csv`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/tests/extract_node.csv` & `swmmtoolbox-4.0.7/tests/extract_node.csv`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/tests/frutal.out` & `swmmtoolbox-4.0.7/tests/frutal.out`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/tests/listdetail_link.csv` & `swmmtoolbox-4.0.7/tests/listdetail_link.csv`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/tests/listdetail_node.csv` & `swmmtoolbox-4.0.7/tests/listdetail_node.csv`

 * *Files identical despite different names*

### Comparing `swmmtoolbox-4.0.6/tests/test_extract.py` & `swmmtoolbox-4.0.7/tests/test_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Tests for `swmmtoolbox` module.
 """
 import os
 import sys
 from unittest import TestCase
 
-from pandas.util.testing import assert_frame_equal
+from pandas.testing import assert_frame_equal
 
 try:
     from cStringIO import StringIO
 except:
     from io import StringIO
 
 import pandas as pd
```

### Comparing `swmmtoolbox-4.0.6/tests/test_listdetail.py` & `swmmtoolbox-4.0.7/tests/test_listdetail.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Tests for `swmmtoolbox` module.
 """
 import os
 import sys
 from unittest import TestCase
 
-from pandas.util.testing import assert_frame_equal
+from pandas.testing import assert_frame_equal
 
 try:
     from cStringIO import StringIO
 except:
     from io import StringIO
 
 import pandas as pd
```

