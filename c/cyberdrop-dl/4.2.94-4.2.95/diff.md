# Comparing `tmp/cyberdrop-dl-4.2.94.tar.gz` & `tmp/cyberdrop-dl-4.2.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.94.tar", last modified: Sat Jun 10 15:14:17 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.95.tar", last modified: Sat Jun 17 02:01:17 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.94.tar` & `cyberdrop-dl-4.2.95.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:17.423178 cyberdrop-dl-4.2.94/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-10 15:14:17.423178 cyberdrop-dl-4.2.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:17.419178 cyberdrop-dl-4.2.94/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:17.419178 cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:17.419178 cyberdrop-dl-4.2.94/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:17.423178 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:17.423178 cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:17.423178 cyberdrop-dl-4.2.94/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 15:14:17.419178 cyberdrop-dl-4.2.94/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-10 15:14:17.000000 cyberdrop-dl-4.2.94/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-10 15:14:17.000000 cyberdrop-dl-4.2.94/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 15:14:17.000000 cyberdrop-dl-4.2.94/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-10 15:14:17.000000 cyberdrop-dl-4.2.94/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-10 15:14:17.000000 cyberdrop-dl-4.2.94/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-10 15:14:17.000000 cyberdrop-dl-4.2.94/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-10 15:14:17.423178 cyberdrop-dl-4.2.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 15:14:08.000000 cyberdrop-dl-4.2.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:17.807838 cyberdrop-dl-4.2.95/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-17 02:01:17.807838 cyberdrop-dl-4.2.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:17.787838 cyberdrop-dl-4.2.95/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:17.795838 cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:17.795838 cyberdrop-dl-4.2.95/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:17.799838 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:17.807838 cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23724 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:17.807838 cyberdrop-dl-4.2.95/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20933 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 02:01:17.791838 cyberdrop-dl-4.2.95/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-17 02:01:17.000000 cyberdrop-dl-4.2.95/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-17 02:01:17.000000 cyberdrop-dl-4.2.95/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 02:01:17.000000 cyberdrop-dl-4.2.95/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-17 02:01:17.000000 cyberdrop-dl-4.2.95/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-17 02:01:17.000000 cyberdrop-dl-4.2.95/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-17 02:01:17.000000 cyberdrop-dl-4.2.95/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-17 02:01:17.807838 cyberdrop-dl-4.2.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 02:01:05.000000 cyberdrop-dl-4.2.95/setup.py
```

### Comparing `cyberdrop-dl-4.2.94/LICENSE` & `cyberdrop-dl-4.2.95/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/PKG-INFO` & `cyberdrop-dl-4.2.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.94
+Version: 4.2.95
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.94 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.95 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.94/README.md` & `cyberdrop-dl-4.2.95/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 import asyncio
 import csv
 import io
 import logging
 import os
 import re
-from typing import TYPE_CHECKING, Tuple
+from typing import TYPE_CHECKING, Any, Tuple
 
 import aiofiles
 import rich
+import yaml
 
 from cyberdrop_dl.base_functions.data_classes import MediaItem
 from cyberdrop_dl.base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
     from pathlib import Path
 
@@ -115,14 +116,46 @@
 async def create_media_item(url: URL, referer: URL, sql_helper: SQLHelper, domain: str) -> MediaItem:
     """Returns the MediaItem of a given url, throws NoExtensionFailure if url.name doesn't have extension"""
     filename, ext = await get_filename_and_ext(url.name)
     complete = await sql_helper.check_complete_singular(domain, url)
     return MediaItem(url, referer, complete, filename, ext, filename)
 
 
+class CacheManager:
+    def __init__(self, cache_file: Path):
+        self.cache_file = cache_file
+        self.cache = {}
+
+    async def load(self):
+        if not self.cache_file.exists():
+            return
+
+        async with aiofiles.open(self.cache_file, 'r') as cache_file:
+            cache = yaml.load(await cache_file.read(), Loader=yaml.FullLoader)
+        if cache:
+            self.cache = cache
+
+    async def get(self, key: str) -> Any:
+        return self.cache.get(key, None)
+
+    async def save(self, key: str, value: Any):
+        self.cache[key] = value
+        await self._save()
+
+    async def remove(self, key: str):
+        if key in self.cache:
+            del self.cache[key]
+            await self._save()
+
+    async def _save(self):
+        cache = yaml.dump(self.cache)
+        async with aiofiles.open(self.cache_file, 'w') as cache_file:
+            await cache_file.write(cache)
+
+
 class ErrorFileWriter:
     """Writes errors to a file"""
     def __init__(self, output_errored: bool, output_unsupported: bool, output_last_post: bool, errored_scrapes: Path,
                  errored_downloads: Path, unsupported: Path, last_post: Path):
         self.output_errored = output_errored
         self.output_unsupported = output_unsupported
         self.output_last_post = output_last_post
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
             "simpcity_password": "",
             "socialmediagirls_username": "",
             "socialmediagirls_password": "",
             "xbunker_username": "",
             "xbunker_password": "",
         },
         "Files": {
+            "variable_cache_file": "internal_variable_cache.yaml",
             "db_file": "download_history.sqlite",
             "errored_download_urls_file": "Errored_Download_URLs.csv",
             "errored_scrape_urls_file": "Errored_Scrape_URLs.csv",
             "input_file": "URLs.txt",
             "log_file": "downloader.log",
             "output_folder": "Downloads",
             "output_last_forum_post_file": "URLs_last_post.txt",
@@ -61,14 +62,15 @@
             "visible_rows_threads": 2,
             "visible_rows_domains": 2,
             "visible_rows_albums": 2,
             "visible_rows_files": 10,
         },
         "Ratelimiting": {
             "connection_timeout": 15,
+            "read_timeout": 300,
             "ratelimit": 50,
             "throttle": 0.5,
         },
         "Runtime": {
             "allow_insecure_connections": False,
             "attempts": 10,
             "block_sub_folders": False,
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import asyncio
-import contextlib
 import functools
 import json
 import logging
 import ssl
 import time
 from http import HTTPStatus
 from typing import TYPE_CHECKING, Any, Callable, Coroutine, Dict, Optional, Tuple
@@ -40,16 +39,18 @@
                 return await func(self, *args, **kwargs)
 
     return wrapper
 
 
 class Client:
     """Creates a 'client' that can be referenced by scraping or download sessions"""
-    def __init__(self, ratelimit: int, throttle: float, secure: bool, connect_timeout: int, user_agent: str):
+    def __init__(self, ratelimit: int, throttle: float, secure: bool, connect_timeout: int, read_timeout: int,
+                 user_agent: str):
         self.connect_timeout = connect_timeout
+        self.read_timeout = read_timeout
         self.ratelimit = ratelimit
         self.throttle = throttle
         self.simultaneous_session_limit = asyncio.Semaphore(50)
         self.user_agent = user_agent
         self.verify_ssl = secure
         self.ssl_context = ssl.create_default_context(cafile=certifi.where()) if secure else False
         self.cookies = aiohttp.CookieJar(quote_cookie=False)
@@ -116,15 +117,16 @@
 
 
 class DownloadSession:
     """AIOHTTP operations for downloading"""
     def __init__(self, client: Client):
         self.client = client
         self.headers = {"user-agent": client.user_agent}
-        self.timeouts = aiohttp.ClientTimeout(total=None, connect=self.client.connect_timeout, sock_read=None)
+        self.timeouts = aiohttp.ClientTimeout(total=self.client.read_timeout + self.client.connect_timeout,
+                                              connect=self.client.connect_timeout, sock_read=self.client.read_timeout)
         self.client_session = aiohttp.ClientSession(headers=self.headers, raise_for_status=True,
                                                     cookie_jar=self.client.cookies, timeout=self.timeouts)
         self.throttle_times: Dict[str, float] = {}
         self.bunkr_maintenance = [URL("https://bnkr.b-cdn.net/maintenance-vid.mp4"), URL("https://bnkr.b-cdn.net/maintenance.mp4")]
 
     async def _append_content(self, file: Path, content: aiohttp.StreamReader,
                               update_progress: functools.partial | Callable[[int], Optional[bool]]) -> None:
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 
 import http
 import re
 from typing import TYPE_CHECKING, Dict, List, Union
 
+import aiohttp.client_exceptions
 from aiolimiter import AsyncLimiter
 from yarl import URL
 
 from ..base_functions.base_functions import get_filename_and_ext, log, logger, make_title_safe
 from ..base_functions.data_classes import DomainItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
-    from ..base_functions.base_functions import ErrorFileWriter
+    from ..base_functions.base_functions import CacheManager, ErrorFileWriter
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
 class GoFileCrawler:
-    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter):
+    def __init__(self, quiet: bool, SQL_Helper: SQLHelper, error_writer: ErrorFileWriter,
+                 cache_manager: CacheManager):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.limiter = AsyncLimiter(1, 1)
 
+        self.cache_manager = cache_manager
         self.error_writer = error_writer
 
         self.api_address = URL("https://api.gofile.io")
         self.js_address = URL("https://gofile.io/dist/js/alljs.js")
         self.token = ""
         self.websiteToken = ""
 
@@ -54,22 +57,26 @@
             logger.debug(e)
 
     async def get_website_token(self, session: ScrapeSession, website_token: str = None):
         """Creates an anon gofile account to use."""
         if self.websiteToken:
             return
 
+        if not website_token:
+            website_token = await self.cache_manager.get("gofile_website_token")
+
         if website_token:
             self.websiteToken = website_token
             return
 
         try:
             async with self.limiter:
                 js_obj = await session.get_text(self.js_address)
             self.websiteToken = re.search(r'fetchData\.websiteToken\s*=\s*"(.*?)"', js_obj).group(1)
+            await self.cache_manager.save("gofile_website_token", self.websiteToken)
         except Exception as e:
             logger.debug("Error encountered while getting GoFile websiteToken", exc_info=True)
             log("Error: Couldn't generate GoFile websiteToken", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def set_cookie(self, session: ScrapeSession):
         """Sets the given token as a cookie into the session (and client)"""
@@ -102,16 +109,25 @@
         results: List[List] = []
         params = {
             "token": self.token,
             "contentId": content_id,
             "websiteToken": self.websiteToken,
         }
 
-        async with self.limiter:
-            content = await session.get_json(self.api_address / "getContent", params)
+        try:
+            async with self.limiter:
+                content = await session.get_json(self.api_address / "getContent", params)
+        except aiohttp.client_exceptions.ClientResponseError as e:
+            if e.code == http.HTTPStatus.UNAUTHORIZED:
+                self.websiteToken = ""
+                await self.cache_manager.remove("gofile_website_token")
+                await self.get_website_token(session)
+                params["websiteToken"] = self.websiteToken
+                async with self.limiter:
+                    content = await session.get_json(self.api_address / "getContent", params)
 
         if content["status"] != "ok":
             await self.error_writer.write_errored_scrape(url, Exception("Does Not Exist"), self.quiet)
             return results
 
         content = content['data']
         if title:
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,10 +76,11 @@
                 url_path = args[2]
                 if not self.can_retry(url_path):
                     logger.debug('Skipping %s...', media.url, exc_info=True)
                     await self.handle_failed(media, e)
                     return None
                 logger.debug(e.message)
                 logger.debug(f'Retrying ({self.current_attempt[url_path]}) {media.url}...')
-                self.current_attempt[url_path] += 1
+                if e.code != 999:
+                    self.current_attempt[url_path] += 1
 
     return wrapper
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,15 @@
     def __init__(self, domain: str, CDL_Helper: CDLHelper, Progress_Master: ProgressMaster):
         self.domain = domain
         self.throttle = CDL_Helper.get_throttle(domain)
 
         max_workers = get_threads_number(CDL_Helper.args, domain)
         self._semaphore = asyncio.Semaphore(max_workers)
         self.current_attempt: Dict[str, int] = {}
+        self.current_attempt_filesize: Dict[str, int] = {}
 
         self.download_session = DownloadSession(CDL_Helper.client)
 
         self.CDL_Helper = CDL_Helper
         self.Progress_Master = Progress_Master
 
     async def download(self, album: str, media: MediaItem, url_path: str, album_task: TaskID) -> None:
@@ -242,18 +243,37 @@
                 await self.CDL_Helper.files.add_completed()
             await self.Progress_Master.FileProgress.mark_file_completed(file_task)
 
             log(f"Completed Download: {media.filename} from {media.referer}", quiet=True)
             await self.CDL_Helper.File_Lock.remove_lock(filename)
             return
 
+        except (aiohttp.client_exceptions.ServerDisconnectedError, asyncio.TimeoutError,
+                aiohttp.client_exceptions.ServerTimeoutError) as e:
+            if await self.CDL_Helper.File_Lock.check_lock(filename):
+                await self.CDL_Helper.File_Lock.remove_lock(filename)
+
+            with contextlib.suppress(Exception):
+                await self.Progress_Master.FileProgress.remove_file(file_task)
+
+            if partial_file.is_file():
+                size = partial_file.stat().st_size
+                if partial_file.name not in self.current_attempt_filesize:
+                    self.current_attempt_filesize[filename] = size
+                elif self.current_attempt_filesize[filename] > size:
+                    self.current_attempt_filesize[filename] = size
+                else:
+                    raise DownloadFailure(code=getattr(e, "code", 1), message="Download timeout reached, retrying")
+                raise DownloadFailure(code=999, message="Download timeout reached, retrying")
+
+            raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
+
         except (aiohttp.client_exceptions.ClientPayloadError, aiohttp.client_exceptions.ClientOSError,
-                aiohttp.client_exceptions.ServerDisconnectedError, asyncio.TimeoutError,
-                aiohttp.client_exceptions.ClientResponseError, aiohttp.client_exceptions.ServerTimeoutError,
-                DownloadFailure, FileNotFoundError, PermissionError) as e:
+                aiohttp.client_exceptions.ClientResponseError, DownloadFailure, FileNotFoundError,
+                PermissionError) as e:
             if await self.CDL_Helper.File_Lock.check_lock(filename):
                 await self.CDL_Helper.File_Lock.remove_lock(filename)
 
             with contextlib.suppress(Exception):
                 await self.Progress_Master.FileProgress.remove_file(file_task)
 
             if hasattr(e, "message"):
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import argparse
 import asyncio
 import atexit
 import contextlib
 import logging
 import re
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Tuple
 
 import aiofiles
 import aiorun as aiorun
 from yarl import URL
 
-from cyberdrop_dl.base_functions.base_functions import ErrorFileWriter, clear, log, purge_dir
+from cyberdrop_dl.base_functions.base_functions import (
+    CacheManager,
+    ErrorFileWriter,
+    clear,
+    log,
+    purge_dir,
+)
 from cyberdrop_dl.base_functions.config_manager import document_args, run_args
 from cyberdrop_dl.base_functions.config_schema import config_default
 from cyberdrop_dl.base_functions.sorting_functions import Sorter
 from cyberdrop_dl.base_functions.sql_helper import SQLHelper
 from cyberdrop_dl.client.client import Client, ScrapeSession
 from cyberdrop_dl.downloader.downloader_utils import check_free_space
 from cyberdrop_dl.downloader.downloaders import DownloadDirector
@@ -36,14 +42,15 @@
     # Path options
     config_group = config_data["Files"]
     path_opts = parser.add_argument_group("Path options")
     path_opts.add_argument("-i", "--input-file", type=Path, help="file containing links to download (default: %(default)s)", default=config_group["input_file"])
     path_opts.add_argument("-o", "--output-folder", type=Path, help="folder to download files to (default: %(default)s)", default=config_group["output_folder"])
 
     path_opts.add_argument("--config-file", type=Path, help="config file to read arguments from (default: %(default)s)", default="config.yaml")
+    path_opts.add_argument("--variable-cache-file", type=Path, help="internal variable cache file to read from and write to (default: %(default)s)", default=config_group["variable_cache_file"])
     path_opts.add_argument("--db-file", type=Path, help="history database file to write to (default: %(default)s)", default=config_group["db_file"])
     path_opts.add_argument("--errored-download-urls-file", type=Path, default=config_group["errored_download_urls_file"], help="csv file to write failed download information to (default: %(default)s)")
     path_opts.add_argument("--errored-scrape-urls-file", type=Path, default=config_group["errored_scrape_urls_file"], help="csv file to write failed scrape information to (default: %(default)s)")
     path_opts.add_argument("--log-file", type=Path, help="log file to write to (default: %(default)s)", default=config_group["log_file"])
     path_opts.add_argument("--output-last-forum-post-file", type=Path, default=config_group["output_last_forum_post_file"], help="the text file to output last scraped post from a forum thread for re-feeding into CDL (default: %(default)s)")
     path_opts.add_argument("--unsupported-urls-file", type=Path, default=config_group["unsupported_urls_file"], help="the csv file to output unsupported links into (default: %(default)s)")
 
@@ -95,14 +102,15 @@
     sort_opts.add_argument("--sorted-others", help="schema to sort other (default: %(default)s)", default=config_group["sorted_others"])
     sort_opts.add_argument("--sorted-videos", help="schema to sort videos (default: %(default)s)", default=config_group["sorted_videos"])
 
     # Ratelimiting
     config_group = config_data["Ratelimiting"]
     ratelimit_opts = parser.add_argument_group("Ratelimiting options")
     ratelimit_opts.add_argument("--connection-timeout", type=int, default=config_group["connection_timeout"], help="number of seconds to wait attempting to connect to a URL during the downloading phase (default: %(default)s)")
+    ratelimit_opts.add_argument("--read-timeout", type=int, default=config_group["read_timeout"], help="number of seconds to wait attempting to read all file data during the downloading phase (default: %(default)s)")
     ratelimit_opts.add_argument("--ratelimit", type=int, default=config_group["ratelimit"], help="this applies to requests made in the program during scraping, the number you provide is in requests/seconds (default: %(default)s)")
     ratelimit_opts.add_argument("--throttle", type=int, default=config_group["throttle"], help="this is a throttle between requests during the downloading phase, the number is in seconds (default: %(default)s)")
 
     # Forum Options
     forum_opts = parser.add_argument_group("Forum options")
     forum_opts.add_argument("--output-last-forum-post", help="outputs the last post of a forum scrape to use as a starting point for future runs", action="store_true")
     forum_opts.add_argument("--separate-posts", help="separates forum scraping into folders by post number", action="store_true")
@@ -148,15 +156,15 @@
     progress_opts.add_argument("--visible-rows-files", type=int, help="number of visiblerows to use for the files table (default: %(default)s)", default=config_group["visible_rows_files"])
 
     # Links
     parser.add_argument("links", metavar="link", nargs="*", help="link to content to download (passing multiple links is supported)", default=[])
     return parser.parse_args()
 
 
-async def file_management(args: Dict, links: List) -> ErrorFileWriter:
+async def file_management(args: Dict, links: List) -> Tuple[ErrorFileWriter, CacheManager]:
     """We handle file defaults here (resetting and creation)"""
     input_file = args['Files']['input_file']
     if not input_file.is_file() and not links:
         input_file.touch()
 
     Path(args['Files']['output_folder']).mkdir(parents=True, exist_ok=True)
 
@@ -187,15 +195,18 @@
 
         errored_urls = args['Files']['errored_scrape_urls_file']
         if errored_urls.exists():
             errored_urls.unlink()
         errored_urls.touch()
         await error_writer.write_errored_scrape_header()
 
-    return error_writer
+    cache_manager = CacheManager(args['Files']['variable_cache_file'])
+    await cache_manager.load()
+
+    return error_writer, cache_manager
 
 
 async def regex_links(urls: List) -> List:
     """Regex grab the links from the URLs.txt file"""
     """This allows code blocks or full paragraphs to be copy and pasted into the URLs.txt"""
     yarl_links = []
     for line in urls:
@@ -258,26 +269,26 @@
 
 
 async def director(args: Dict, links: List) -> None:
     """This is the overarching director coordinator for CDL."""
     await clear()
     await document_args(args)
     log(f"We are running version {VERSION} of Cyberdrop Downloader")
-    error_writer = await file_management(args, links)
+    error_writer, cache_manager = await file_management(args, links)
 
     if not await check_free_space(args['Runtime']['required_free_space'], args['Files']['output_folder']):
         log("Not enough free space to continue. You can change the required space required using --required-free-space.", style="red")
         exit(1)
 
     links = await consolidate_links(args, links)
     client = Client(args['Ratelimiting']['ratelimit'], args['Ratelimiting']['throttle'],
                     args['Runtime']['allow_insecure_connections'], args["Ratelimiting"]["connection_timeout"],
-                    args['Runtime']['user_agent'])
+                    args["Ratelimiting"]["read_timeout"], args['Runtime']['user_agent'])
     SQL_Helper = SQLHelper(args['Ignore']['ignore_history'], args['Ignore']['ignore_cache'], args['Files']['db_file'])
-    Scraper = ScrapeMapper(args, client, SQL_Helper, False, error_writer)
+    Scraper = ScrapeMapper(args, client, SQL_Helper, False, error_writer, cache_manager)
 
     await SQL_Helper.sql_initialize()
 
     if links:
         Forums = await scrape_links(Scraper, links)
         await asyncio.sleep(5)
         await clear()
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         try:
             if not self.jdownloader_username or not self.jdownloader_password or not self.jdownloader_device:
                 raise JDownloaderFailure("jdownloader credentials were not provided.")
             jd = myjdapi.Myjdapi()
             jd.set_app_key("CYBERDROP-DL")
             jd.connect(self.jdownloader_username, self.jdownloader_password)
             return jd.get_device(self.jdownloader_device)
-        except JDownloaderFailure:
+        except (myjdapi.MYJDApiException, JDownloaderFailure) as e:
             log("Failed JDownloader setup", quiet=self.quiet, style="red")
             self.jdownloader_enable = False
             return None
 
     async def direct_unsupported_to_jdownloader(self, url: URL, title: str) -> None:
         """Sends links to JDownloader"""
         if self.jdownloader_enable:
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.95/cyberdrop_dl/scraper/Scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,29 +28,31 @@
 from cyberdrop_dl.crawlers.Saint_Spider import SaintCrawler
 from cyberdrop_dl.crawlers.ShareX_Spider import ShareXCrawler
 from cyberdrop_dl.crawlers.XBunkr_Spider import XBunkrCrawler
 from cyberdrop_dl.crawlers.Xenforo_Spider import XenforoCrawler
 from cyberdrop_dl.scraper.JDownloader_Integration import JDownloader
 
 if TYPE_CHECKING:
-    from cyberdrop_dl.base_functions.base_functions import ErrorFileWriter
+    from cyberdrop_dl.base_functions.base_functions import CacheManager, ErrorFileWriter
     from cyberdrop_dl.base_functions.sql_helper import SQLHelper
 
 
 class ScrapeMapper:
     """This class maps links to their respective handlers, or JDownloader if they are unsupported"""
-    def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper, quiet: bool, error_writer: ErrorFileWriter):
+    def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper, quiet: bool, error_writer: ErrorFileWriter,
+                 cache_manager: CacheManager):
         self.args = args
         self.client = client
         self.SQL_Helper = SQL_Helper
         self.Cascade = CascadeItem({})
         self.Forums = ForumItem({})
         self.skip_data = SkipData(args['Ignore']['skip_hosts'])
         self.only_data = SkipData(args['Ignore']['only_hosts'])
 
+        self.cache_manager = cache_manager
         self.error_writer = error_writer
 
         self.anonfiles_crawler: Optional[AnonfilesCrawler] = None
         self.bunkr_crawler: Optional[BunkrCrawler] = None
         self.cyberdrop_crawler: Optional[CyberdropCrawler] = None
         self.coomeno_crawler: Optional[CoomenoCrawler] = None
         self.cyberfile_crawler: Optional[CyberFileCrawler] = None
@@ -186,15 +188,15 @@
         await self._handle_album_additions("gfycat", album_obj, title)
         await gfycat_session.exit_handler()
 
     async def GoFile(self, url, title=None):
         gofile_session = ScrapeSession(self.client)
         if not self.gofile_crawler:
             self.gofile_crawler = GoFileCrawler(quiet=self.quiet, SQL_Helper=self.SQL_Helper,
-                                                error_writer=self.error_writer)
+                                                error_writer=self.error_writer, cache_manager=self.cache_manager)
 
         async with self.gofile_semaphore:
             await self.gofile_crawler.get_acct_token(session=gofile_session,
                                                      api_token=self.args['Authentication']['gofile_api_key'])
             await self.gofile_crawler.get_website_token(session=gofile_session,
                                                         website_token=self.args['Authentication']['gofile_website_token'])
         domain_obj = await self.gofile_crawler.fetch(gofile_session, url)
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.95/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.94
+Version: 4.2.95
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.94 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.95 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.94/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.95/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.94/setup.cfg` & `cyberdrop-dl-4.2.95/setup.cfg`

 * *Files identical despite different names*

