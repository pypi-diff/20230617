# Comparing `tmp/bdfrx-1.0.8.tar.gz` & `tmp/bdfrx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdfrx-1.0.8.tar", last modified: Wed Jun  7 00:23:08 2023, max compression
+gzip compressed data, was "bdfrx-1.0.9.tar", last modified: Sat Jun 17 21:17:38 2023, max compression
```

## Comparing `bdfrx-1.0.8.tar` & `bdfrx-1.0.9.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.599015 bdfrx-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-06-07 00:22:55.000000 bdfrx-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-06-07 00:23:08.599015 bdfrx-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-06-07 00:22:55.000000 bdfrx-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.595015 bdfrx-1.0.8/bdfrx/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6880 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/bdfrx.db
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/default_config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_authenticator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.599015 bdfrx-1.0.8/bdfrx/site_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/base_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/catbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/delay_for_reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/download_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/erome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.599015 bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/gallery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/gfycat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/imgchest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/imgur.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/pornhub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/redgifs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/self_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/vidble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/vreddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-07 00:22:55.000000 bdfrx-1.0.8/bdfrx/site_downloaders/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.595015 bdfrx-1.0.8/bdfrx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    68901 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 00:23:08.000000 bdfrx-1.0.8/bdfrx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-07 00:22:55.000000 bdfrx-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 00:23:08.599015 bdfrx-1.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:23:08.599015 bdfrx-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_download_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_file_name_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-07 00:22:55.000000 bdfrx-1.0.8/tests/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:17:38.217058 bdfrx-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-06-17 21:17:23.000000 bdfrx-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    69626 2023-06-17 21:17:38.217058 bdfrx-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28085 2023-06-17 21:17:23.000000 bdfrx-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:17:38.213058 bdfrx-1.0.9/bdfrx/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6880 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36864 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/bdfrx.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/default_config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10728 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_authenticator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:17:38.213058 bdfrx-1.0.9/bdfrx/site_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/base_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/catbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/delay_for_reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/download_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/erome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:17:38.217058 bdfrx-1.0.9/bdfrx/site_downloaders/fallback_downloaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/fallback_downloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/fallback_downloaders/fallback_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/flickr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/gfycat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/imgchest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/imgur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/nsfw_pics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/pornhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/redgifs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/self_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/vidble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/vreddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-17 21:17:23.000000 bdfrx-1.0.9/bdfrx/site_downloaders/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:17:38.213058 bdfrx-1.0.9/bdfrx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    69626 2023-06-17 21:17:38.000000 bdfrx-1.0.9/bdfrx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-17 21:17:38.000000 bdfrx-1.0.9/bdfrx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 21:17:38.000000 bdfrx-1.0.9/bdfrx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-17 21:17:38.000000 bdfrx-1.0.9/bdfrx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-17 21:17:38.000000 bdfrx-1.0.9/bdfrx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 21:17:38.000000 bdfrx-1.0.9/bdfrx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-17 21:17:23.000000 bdfrx-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 21:17:38.217058 bdfrx-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 21:17:38.217058 bdfrx-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-17 21:17:23.000000 bdfrx-1.0.9/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-17 21:17:23.000000 bdfrx-1.0.9/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-06-17 21:17:23.000000 bdfrx-1.0.9/tests/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-17 21:17:23.000000 bdfrx-1.0.9/tests/test_download_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-17 21:17:23.000000 bdfrx-1.0.9/tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18454 2023-06-17 21:17:23.000000 bdfrx-1.0.9/tests/test_file_name_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-17 21:17:23.000000 bdfrx-1.0.9/tests/test_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-17 21:17:23.000000 bdfrx-1.0.9/tests/test_resource.py
```

### Comparing `bdfrx-1.0.8/LICENSE` & `bdfrx-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/PKG-INFO` & `bdfrx-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.8
+Version: 1.0.9
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,15 +696,15 @@
 License-File: LICENSE
 
 # Bulk Downloader for Reddit x
 
 [![PyPI Status](https://img.shields.io/pypi/status/bdfrx?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![PyPI version](https://img.shields.io/pypi/v/bdfrx.svg?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![Python Test](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml)
-[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&label=linting)](https://github.com/charliermarsh/ruff)
+[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&label=linting)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=Python)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 This is a tool to download submissions from Reddit. BDFRx is flexible and can be used in scripts if needed through an extensive command-line interface. [List of currently supported sources](#list-of-currently-supported-sources)
 
 If you wish to open an issue, please read [the guide on opening issues](docs/CONTRIBUTING.md#opening-an-issue) to ensure that your issue is clear and contains everything it needs to for the developers to investigate.
 
@@ -738,16 +738,23 @@
 
 ## **Differences from [BDFR](https://github.com/aliparlakci/bulk-downloader-for-reddit)**
 
 BDFRx differs from the base BDFR in a few ways:
 
 - Does not contain the Archive and Clone modes (If you require these modes you can try v0.9.1, provided *as is* or use the base [BDFR](https://github.com/aliparlakci/bulk-downloader-for-reddit) project)
 - Option to use an Sqlite3 database to store hashes, links and post ID's to be filtered in future runs
-- Uses the `bdfrx` config directory by default as well as a different client_id which does not require the use of the client_secret
-    - You will not be able to use the BDFR id/secret/token, you will need to authorize with the new client_id
+- Uses the `bdfrx` config directory by default
+
+## Reddit API Changes
+
+Starting July 1st 2023 ([along with the other changes](https://reddit.com/12qwagm)) rate limits will be [applied ***per client id*** rather than by client id/user combination](https://reddit.com/13wsiks). Therefore it is no longer tenable to ship BDFRx with an installed client id as it will cause rate limiting for all users. **The shipped client id will no longer be valid after the changes.**
+
+To create your own for use with BDFRx go [here](https://old.reddit.com/prefs/apps/) and click "create an app". It's recommended to choose "Installed App" and use "http://localhost:7634" as the redirect url. <!-- markdownlint-disable-line MD034 -->
+
+Once you have your personal client id add it to your [config.cfg](bdfrx/default_config.cfg) at the location in the [configuration](#configuration) section.
 
 ## Usage
 
 BDFRx works by taking submissions from a variety of "sources" from Reddit and then parsing them to download. These sources might be a subreddit, multireddit, a user list, or individual links. These sources are combined and downloaded to disk, according to a naming and organisational scheme defined by the user.
 
 The sole mode of BDFRx is download. The `download` command will download the resource linked in the Reddit submission, such as the images, video, etc.
 
@@ -1031,14 +1038,18 @@
 ### Configuration File
 
 The `config.cfg` is the file that supplies BDFRx with the configuration to use. At the moment, the following keys **must** be included in the configuration file supplied.
 
 - `client_id`
 - `scopes`
 
+The following key may be required depending on the type of client id you created.
+
+- `client_secret`
+
 The following keys are optional, and defaults will be used if they cannot be found.
 
 - `backup_log_count`
 - `max_wait_time`
 - `time_format`
 - `disabled_modules`
 - `filename-restriction-scheme`
```

### Comparing `bdfrx-1.0.8/README.md` & `bdfrx-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Bulk Downloader for Reddit x
 
 [![PyPI Status](https://img.shields.io/pypi/status/bdfrx?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![PyPI version](https://img.shields.io/pypi/v/bdfrx.svg?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![Python Test](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml)
-[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&label=linting)](https://github.com/charliermarsh/ruff)
+[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&label=linting)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=Python)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 This is a tool to download submissions from Reddit. BDFRx is flexible and can be used in scripts if needed through an extensive command-line interface. [List of currently supported sources](#list-of-currently-supported-sources)
 
 If you wish to open an issue, please read [the guide on opening issues](docs/CONTRIBUTING.md#opening-an-issue) to ensure that your issue is clear and contains everything it needs to for the developers to investigate.
 
@@ -41,16 +41,23 @@
 
 ## **Differences from [BDFR](https://github.com/aliparlakci/bulk-downloader-for-reddit)**
 
 BDFRx differs from the base BDFR in a few ways:
 
 - Does not contain the Archive and Clone modes (If you require these modes you can try v0.9.1, provided *as is* or use the base [BDFR](https://github.com/aliparlakci/bulk-downloader-for-reddit) project)
 - Option to use an Sqlite3 database to store hashes, links and post ID's to be filtered in future runs
-- Uses the `bdfrx` config directory by default as well as a different client_id which does not require the use of the client_secret
-    - You will not be able to use the BDFR id/secret/token, you will need to authorize with the new client_id
+- Uses the `bdfrx` config directory by default
+
+## Reddit API Changes
+
+Starting July 1st 2023 ([along with the other changes](https://reddit.com/12qwagm)) rate limits will be [applied ***per client id*** rather than by client id/user combination](https://reddit.com/13wsiks). Therefore it is no longer tenable to ship BDFRx with an installed client id as it will cause rate limiting for all users. **The shipped client id will no longer be valid after the changes.**
+
+To create your own for use with BDFRx go [here](https://old.reddit.com/prefs/apps/) and click "create an app". It's recommended to choose "Installed App" and use "http://localhost:7634" as the redirect url. <!-- markdownlint-disable-line MD034 -->
+
+Once you have your personal client id add it to your [config.cfg](bdfrx/default_config.cfg) at the location in the [configuration](#configuration) section.
 
 ## Usage
 
 BDFRx works by taking submissions from a variety of "sources" from Reddit and then parsing them to download. These sources might be a subreddit, multireddit, a user list, or individual links. These sources are combined and downloaded to disk, according to a naming and organisational scheme defined by the user.
 
 The sole mode of BDFRx is download. The `download` command will download the resource linked in the Reddit submission, such as the images, video, etc.
 
@@ -334,14 +341,18 @@
 ### Configuration File
 
 The `config.cfg` is the file that supplies BDFRx with the configuration to use. At the moment, the following keys **must** be included in the configuration file supplied.
 
 - `client_id`
 - `scopes`
 
+The following key may be required depending on the type of client id you created.
+
+- `client_secret`
+
 The following keys are optional, and defaults will be used if they cannot be found.
 
 - `backup_log_count`
 - `max_wait_time`
 - `time_format`
 - `disabled_modules`
 - `filename-restriction-scheme`
```

### Comparing `bdfrx-1.0.8/bdfrx/__main__.py` & `bdfrx-1.0.9/bdfrx/__main__.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/bdfrx.db` & `bdfrx-1.0.9/bdfrx/bdfrx.db`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/completion.py` & `bdfrx-1.0.9/bdfrx/completion.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/configuration.py` & `bdfrx-1.0.9/bdfrx/configuration.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/connector.py` & `bdfrx-1.0.9/bdfrx/connector.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/download_filter.py` & `bdfrx-1.0.9/bdfrx/download_filter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/downloader.py` & `bdfrx-1.0.9/bdfrx/downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/file_name_formatter.py` & `bdfrx-1.0.9/bdfrx/file_name_formatter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/oauth2.py` & `bdfrx-1.0.9/bdfrx/oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/resource.py` & `bdfrx-1.0.9/bdfrx/resource.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/base_downloader.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/base_downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/catbox.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/catbox.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/delay_for_reddit.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/delay_for_reddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/direct.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/direct.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/download_factory.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/download_factory.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from bdfrx.exceptions import NotADownloadableLinkError
 from bdfrx.site_downloaders.base_downloader import BaseDownloader
 from bdfrx.site_downloaders.catbox import Catbox
 from bdfrx.site_downloaders.delay_for_reddit import DelayForReddit
 from bdfrx.site_downloaders.direct import Direct
 from bdfrx.site_downloaders.erome import Erome
 from bdfrx.site_downloaders.fallback_downloaders.ytdlp_fallback import YtdlpFallback
+from bdfrx.site_downloaders.flickr import Flickr
 from bdfrx.site_downloaders.gallery import Gallery
 from bdfrx.site_downloaders.gfycat import Gfycat
 from bdfrx.site_downloaders.imgchest import Imgchest
 from bdfrx.site_downloaders.imgur import Imgur
+from bdfrx.site_downloaders.nsfw_pics import NsfwPics
 from bdfrx.site_downloaders.pornhub import PornHub
 from bdfrx.site_downloaders.redgifs import Redgifs
 from bdfrx.site_downloaders.self_post import SelfPost
 from bdfrx.site_downloaders.vidble import Vidble
 from bdfrx.site_downloaders.vreddit import VReddit
 from bdfrx.site_downloaders.youtube import Youtube
 
@@ -38,18 +40,22 @@
             return Direct
         if re.match(r"erome\.com.*", sanitised_url):
             return Erome
         if re.match(r"catbox\.moe", sanitised_url):
             return Catbox
         if re.match(r"delayforreddit\.com", sanitised_url):
             return DelayForReddit
+        if re.match(r"flickr\.com", sanitised_url) or re.match(r"flic\.kr", sanitised_url):
+            return Flickr
         if re.match(r"reddit\.com/gallery/.*", sanitised_url) or re.match(r"patreon\.com.*", sanitised_url):
             return Gallery
         if re.match(r"imgchest\.com/p/", sanitised_url):
             return Imgchest
+        if re.match(r"nsfw\.pics", sanitised_url):
+            return NsfwPics
         if re.match(r"reddit\.com/r/", sanitised_url):
             return SelfPost
         if re.match(r"(m\.)?youtu\.?be", sanitised_url):
             return Youtube
         if re.match(r"i\.redd\.it.*", sanitised_url):
             return Direct
         if re.match(r"v\.redd\.it.*", sanitised_url):
```

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/erome.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/erome.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/fallback_downloaders/ytdlp_fallback.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/gallery.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/gallery.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/gfycat.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/gfycat.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/imgchest.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/imgchest.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/imgur.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/imgur.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/pornhub.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/pornhub.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/redgifs.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/redgifs.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/self_post.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/self_post.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/vidble.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/vidble.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/vreddit.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/vreddit.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx/site_downloaders/youtube.py` & `bdfrx-1.0.9/bdfrx/site_downloaders/youtube.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/bdfrx.egg-info/PKG-INFO` & `bdfrx-1.0.9/bdfrx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdfrx
-Version: 1.0.8
+Version: 1.0.9
 Summary: Downloads and archives content from reddit
 Author-email: OMEGARAZER <bdfrx.python@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -696,15 +696,15 @@
 License-File: LICENSE
 
 # Bulk Downloader for Reddit x
 
 [![PyPI Status](https://img.shields.io/pypi/status/bdfrx?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![PyPI version](https://img.shields.io/pypi/v/bdfrx.svg?logo=PyPI)](https://pypi.python.org/pypi/bdfrx)
 [![Python Test](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/actions/workflows/test.yml)
-[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&label=linting)](https://github.com/charliermarsh/ruff)
+[![linting: Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&label=linting)](https://github.com/astral-sh/ruff)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?logo=Python)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 
 This is a tool to download submissions from Reddit. BDFRx is flexible and can be used in scripts if needed through an extensive command-line interface. [List of currently supported sources](#list-of-currently-supported-sources)
 
 If you wish to open an issue, please read [the guide on opening issues](docs/CONTRIBUTING.md#opening-an-issue) to ensure that your issue is clear and contains everything it needs to for the developers to investigate.
 
@@ -738,16 +738,23 @@
 
 ## **Differences from [BDFR](https://github.com/aliparlakci/bulk-downloader-for-reddit)**
 
 BDFRx differs from the base BDFR in a few ways:
 
 - Does not contain the Archive and Clone modes (If you require these modes you can try v0.9.1, provided *as is* or use the base [BDFR](https://github.com/aliparlakci/bulk-downloader-for-reddit) project)
 - Option to use an Sqlite3 database to store hashes, links and post ID's to be filtered in future runs
-- Uses the `bdfrx` config directory by default as well as a different client_id which does not require the use of the client_secret
-    - You will not be able to use the BDFR id/secret/token, you will need to authorize with the new client_id
+- Uses the `bdfrx` config directory by default
+
+## Reddit API Changes
+
+Starting July 1st 2023 ([along with the other changes](https://reddit.com/12qwagm)) rate limits will be [applied ***per client id*** rather than by client id/user combination](https://reddit.com/13wsiks). Therefore it is no longer tenable to ship BDFRx with an installed client id as it will cause rate limiting for all users. **The shipped client id will no longer be valid after the changes.**
+
+To create your own for use with BDFRx go [here](https://old.reddit.com/prefs/apps/) and click "create an app". It's recommended to choose "Installed App" and use "http://localhost:7634" as the redirect url. <!-- markdownlint-disable-line MD034 -->
+
+Once you have your personal client id add it to your [config.cfg](bdfrx/default_config.cfg) at the location in the [configuration](#configuration) section.
 
 ## Usage
 
 BDFRx works by taking submissions from a variety of "sources" from Reddit and then parsing them to download. These sources might be a subreddit, multireddit, a user list, or individual links. These sources are combined and downloaded to disk, according to a naming and organisational scheme defined by the user.
 
 The sole mode of BDFRx is download. The `download` command will download the resource linked in the Reddit submission, such as the images, video, etc.
 
@@ -1031,14 +1038,18 @@
 ### Configuration File
 
 The `config.cfg` is the file that supplies BDFRx with the configuration to use. At the moment, the following keys **must** be included in the configuration file supplied.
 
 - `client_id`
 - `scopes`
 
+The following key may be required depending on the type of client id you created.
+
+- `client_secret`
+
 The following keys are optional, and defaults will be used if they cannot be found.
 
 - `backup_log_count`
 - `max_wait_time`
 - `time_format`
 - `disabled_modules`
 - `filename-restriction-scheme`
```

### Comparing `bdfrx-1.0.8/bdfrx.egg-info/SOURCES.txt` & `bdfrx-1.0.9/bdfrx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,20 @@
 bdfrx/site_downloaders/__init__.py
 bdfrx/site_downloaders/base_downloader.py
 bdfrx/site_downloaders/catbox.py
 bdfrx/site_downloaders/delay_for_reddit.py
 bdfrx/site_downloaders/direct.py
 bdfrx/site_downloaders/download_factory.py
 bdfrx/site_downloaders/erome.py
+bdfrx/site_downloaders/flickr.py
 bdfrx/site_downloaders/gallery.py
 bdfrx/site_downloaders/gfycat.py
 bdfrx/site_downloaders/imgchest.py
 bdfrx/site_downloaders/imgur.py
+bdfrx/site_downloaders/nsfw_pics.py
 bdfrx/site_downloaders/pornhub.py
 bdfrx/site_downloaders/redgifs.py
 bdfrx/site_downloaders/self_post.py
 bdfrx/site_downloaders/vidble.py
 bdfrx/site_downloaders/vreddit.py
 bdfrx/site_downloaders/youtube.py
 bdfrx/site_downloaders/fallback_downloaders/__init__.py
```

### Comparing `bdfrx-1.0.8/pyproject.toml` & `bdfrx-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 package-data = {"bdfrx" = ["default_config.cfg", "bdfrx.db",]}
 
 [project.optional-dependencies]
 dev = [
     "black>=23.3.0",
     "pre-commit>=3.3.1",
     "pytest>=7.3.1",
-    "ruff>=0.0.264",
+    "ruff>=0.0.272",
 ]
 
 [project.urls]
 "Homepage" = "https://omegarazer.github.io/bulk-downloader-for-reddit-x"
 "Source" = "https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x"
 "Bug Reports" = "https://github.com/OMEGARAZER/bulk-downloader-for-reddit-x/issues"
```

### Comparing `bdfrx-1.0.8/tests/test_completion.py` & `bdfrx-1.0.9/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/tests/test_configuration.py` & `bdfrx-1.0.9/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/tests/test_connector.py` & `bdfrx-1.0.9/tests/test_connector.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/tests/test_download_filter.py` & `bdfrx-1.0.9/tests/test_download_filter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/tests/test_downloader.py` & `bdfrx-1.0.9/tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/tests/test_file_name_formatter.py` & `bdfrx-1.0.9/tests/test_file_name_formatter.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/tests/test_oauth2.py` & `bdfrx-1.0.9/tests/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `bdfrx-1.0.8/tests/test_resource.py` & `bdfrx-1.0.9/tests/test_resource.py`

 * *Files identical despite different names*

