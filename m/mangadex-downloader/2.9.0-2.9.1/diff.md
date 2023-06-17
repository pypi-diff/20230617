# Comparing `tmp/mangadex-downloader-2.9.0.tar.gz` & `tmp/mangadex-downloader-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mangadex-downloader-2.9.0.tar", last modified: Mon May  1 13:06:26 2023, max compression
+gzip compressed data, was "mangadex-downloader-2.9.1.tar", last modified: Wed May 17 05:56:57 2023, max compression
```

## Comparing `mangadex-downloader-2.9.0.tar` & `mangadex-downloader-2.9.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.660271 mangadex-downloader-2.9.0/mangadex_downloader/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/artist_and_author.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.660271 mangadex-downloader-2.9.0/mangadex_downloader/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/auth/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/auth/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/auth/oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/chapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.660271 mangadex-downloader-2.9.0/mangadex_downloader/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/args_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.664271 mangadex-downloader-2.9.0/mangadex_downloader/config/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/auth_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.656271 mangadex-downloader-2.9.0/mangadex_downloader/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.664271 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/CREDITS
--rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.664271 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/
--rw-r--r--   0 runner    (1001) docker     (123)   856800 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSans.otf
--rw-r--r--   0 runner    (1001) docker     (123)   305436 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBold.otf
--rw-r--r--   0 runner    (1001) docker     (123)   233476 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBoldOblique.otf
--rw-r--r--   0 runner    (1001) docker     (123)   473976 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansOblique.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.668271 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/
--rw-r--r--   0 runner    (1001) docker     (123)  1563256 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   416128 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   342488 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   763696 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansOblique.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/format/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22098 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/chinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/comic_book.py
--rw-r--r--   0 runner    (1001) docker     (123)    16899 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/sevenzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/tachiyomi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/format/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/forums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/images/
--rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/images/mangadex-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/json_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/manga.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/mdlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/tracker/
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_ch_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_file_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_img_info.sql
--rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/tracker/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/mangadex_downloader/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:06:26.660271 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-01 13:06:26.000000 mangadex-downloader-2.9.0/mangadex_downloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/requirements-optional.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:06:26.672271 mangadex-downloader-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-01 13:06:12.000000 mangadex-downloader-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.446139 mangadex-downloader-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-17 05:56:57.446139 mangadex-downloader-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.430139 mangadex-downloader-2.9.1/mangadex_downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/artist_and_author.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.434139 mangadex-downloader-2.9.1/mangadex_downloader/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/auth/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/auth/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11511 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/auth/oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20378 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/chapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.434139 mangadex-downloader-2.9.1/mangadex_downloader/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15912 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cli/args_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cli/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cli/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cli/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.434139 mangadex-downloader-2.9.1/mangadex_downloader/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/config/auth_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/config/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.422139 mangadex-downloader-2.9.1/mangadex_downloader/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.434139 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    23240 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/CREDITS
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.438139 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/otf/
+-rw-r--r--   0 runner    (1001) docker     (123)   856800 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSans.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   305436 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBold.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   233476 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBoldOblique.otf
+-rw-r--r--   0 runner    (1001) docker     (123)   473976 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansOblique.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.442139 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/ttf/
+-rw-r--r--   0 runner    (1001) docker     (123)  1563256 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   416128 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   342488 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   763696 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansOblique.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.442139 mangadex-downloader-2.9.1/mangadex_downloader/format/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22172 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/chinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10771 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/comic_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16899 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12039 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/sevenzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/tachiyomi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10507 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/format/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/forums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.442139 mangadex-downloader-2.9.1/mangadex_downloader/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    49604 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/images/mangadex-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16190 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/json_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9846 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/manga.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/mdlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.442139 mangadex-downloader-2.9.1/mangadex_downloader/tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.442139 mangadex-downloader-2.9.1/mangadex_downloader/tracker/info_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/info_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/info_data/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/info_data/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11127 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.442139 mangadex-downloader-2.9.1/mangadex_downloader/tracker/sql_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/sql_files/create_ch_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/sql_files/create_file_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/sql_files/create_img_info.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    10322 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/tracker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/mangadex_downloader/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:56:57.430139 mangadex-downloader-2.9.1/mangadex_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6959 2023-05-17 05:56:57.000000 mangadex-downloader-2.9.1/mangadex_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-05-17 05:56:57.000000 mangadex-downloader-2.9.1/mangadex_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:56:57.000000 mangadex-downloader-2.9.1/mangadex_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-17 05:56:57.000000 mangadex-downloader-2.9.1/mangadex_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-17 05:56:57.000000 mangadex-downloader-2.9.1/mangadex_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-17 05:56:57.000000 mangadex-downloader-2.9.1/mangadex_downloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/requirements-optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 05:56:57.446139 mangadex-downloader-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-17 05:56:43.000000 mangadex-downloader-2.9.1/setup.py
```

### Comparing `mangadex-downloader-2.9.0/LICENSE` & `mangadex-downloader-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/PKG-INFO` & `mangadex-downloader-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangadex-downloader
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Command-line tool to download manga from MangaDex, written in Python
 Home-page: https://github.com/mansuf/mangadex-downloader
 Download-URL: https://github.com/mansuf/mangadex-downloader/releases
 Author: Rahman Yusuf
 Author-email: danipart4@gmail.com
 License: MIT
 Keywords: mangadex
```

### Comparing `mangadex-downloader-2.9.0/README.md` & `mangadex-downloader-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/__main__.py` & `mangadex-downloader-2.9.1/mangadex_downloader/__main__.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/artist_and_author.py` & `mangadex-downloader-2.9.1/mangadex_downloader/artist_and_author.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/auth/base.py` & `mangadex-downloader-2.9.1/mangadex_downloader/auth/base.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/auth/legacy.py` & `mangadex-downloader-2.9.1/mangadex_downloader/auth/legacy.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/auth/oauth2.py` & `mangadex-downloader-2.9.1/mangadex_downloader/auth/oauth2.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/chapter.py` & `mangadex-downloader-2.9.1/mangadex_downloader/chapter.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cli/__init__.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cli/args_parser.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cli/args_parser.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cli/auth.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cli/auth.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cli/command.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cli/command.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cli/config.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cli/config.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cli/download.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cli/download.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cli/update.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cli/update.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cli/url.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cli/url.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cli/utils.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cli/utils.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/config/auth_cache.py` & `mangadex-downloader-2.9.1/mangadex_downloader/config/auth_cache.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/config/config.py` & `mangadex-downloader-2.9.1/mangadex_downloader/config/config.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/config/env.py` & `mangadex-downloader-2.9.1/mangadex_downloader/config/env.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/config/utils.py` & `mangadex-downloader-2.9.1/mangadex_downloader/config/utils.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/cover.py` & `mangadex-downloader-2.9.1/mangadex_downloader/cover.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/downloader.py` & `mangadex-downloader-2.9.1/mangadex_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/errors.py` & `mangadex-downloader-2.9.1/mangadex_downloader/errors.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fetcher.py` & `mangadex-downloader-2.9.1/mangadex_downloader/fetcher.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/filters.py` & `mangadex-downloader-2.9.1/mangadex_downloader/filters.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/AUTHORS` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/AUTHORS`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/COPYING` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/COPYING`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/CREDITS` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/CREDITS`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/README` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/README`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSans.otf` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSans.otf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBold.otf` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBold.otf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBoldOblique.otf` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansBoldOblique.otf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansOblique.otf` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/otf/FreeSansOblique.otf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSans.ttf` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSans.ttf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBold.ttf` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBold.ttf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBoldOblique.ttf` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansBoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansOblique.ttf` & `mangadex-downloader-2.9.1/mangadex_downloader/fonts/GNU FreeFont/ttf/FreeSansOblique.ttf`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/__init__.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/__init__.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/base.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,14 +486,16 @@
         # - Check for new chapters.
         # - Re-download the volume that has new chapters (if available)
         # - Verify downloaded volumes
 
         # Steps for new (not downloaded) volumes:
         # - Download all of them, yes
 
+        self.write_tachiyomi_info()
+
         cache = self.get_fmt_volume_cache(manga)
 
         # There is not existing (downloaded) volumes
         # Download all of them
         if tracker.disabled or tracker.empty:
             self.download_volumes(worker, cache)
 
@@ -589,14 +591,16 @@
         # - Check for new chapters.
         # - Re-download the entire file (if there is new chapters)
         # - Verify downloaded file
 
         # Steps for new (not downloaded) file (single format):
         # - Download all of them, yes
 
+        self.write_tachiyomi_info()
+
         cache, total, merged_name = result_cache
 
         # There is no existing (downloaded) file
         # Download all of them
         if tracker.disabled or tracker.empty:
             self.download_single(worker, total, merged_name, cache)
```

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/chinfo.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/chinfo.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/comic_book.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/comic_book.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/epub.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/epub.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/pdf.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/pdf.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/raw.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 
 class RawVolume(BaseFormat):
     def main(self):
         base_path = self.path
         manga = self.manga
         tracker = manga.tracker
         file_info = None
+        self.write_tachiyomi_info()
 
         # Recreate DownloadTracker JSON file if --replace is present
         if self.replace:
             manga.tracker.recreate()
 
         cache = self.get_fmt_volume_cache(manga)
 
@@ -223,14 +224,15 @@
     def main(self):
         base_path = self.path
         manga = self.manga
         tracker = manga.tracker
         file_info = None
         success_images = {}
         failed_images = []
+        self.write_tachiyomi_info()
 
         # Recreate DownloadTracker JSON file if --replace is present
         if self.replace:
             manga.tracker.recreate()
 
         result_cache = self.get_fmt_single_cache(manga)
```

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/sevenzip.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/sevenzip.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/tachiyomi.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/tachiyomi.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/format/utils.py` & `mangadex-downloader-2.9.1/mangadex_downloader/format/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,16 +245,16 @@
         "1 = Ongoing",
         "2 = Completed",
         "3 = Licensed",
         "4 = Publishing finished",
         "5 = Cancelled",
         "6 = On hiatus"
     ]
-    with open(path, 'w') as writer:
-        writer.write(json_op.dumps(data))
+    with open(path, 'wb') as writer:
+        writer.write(json_op.dumps(data, convert_str=False))
 
 class QueueWorkerReadMarker(threading.Thread):
     """A queue-based worker run in another thread for ChapterReadMarker
     
     This class will mark chapter as read for every 20 chapters
     and will be done asynchronously (in another thread)
     """
```

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/forums.py` & `mangadex-downloader-2.9.1/mangadex_downloader/forums.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/group.py` & `mangadex-downloader-2.9.1/mangadex_downloader/group.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/images/mangadex-logo.png` & `mangadex-downloader-2.9.1/mangadex_downloader/images/mangadex-logo.png`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/iterator.py` & `mangadex-downloader-2.9.1/mangadex_downloader/iterator.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/json_op.py` & `mangadex-downloader-2.9.1/mangadex_downloader/json_op.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/language.py` & `mangadex-downloader-2.9.1/mangadex_downloader/language.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/main.py` & `mangadex-downloader-2.9.1/mangadex_downloader/main.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/manga.py` & `mangadex-downloader-2.9.1/mangadex_downloader/manga.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/mdlist.py` & `mangadex-downloader-2.9.1/mangadex_downloader/mdlist.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/network.py` & `mangadex-downloader-2.9.1/mangadex_downloader/network.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/range.py` & `mangadex-downloader-2.9.1/mangadex_downloader/range.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/tag.py` & `mangadex-downloader-2.9.1/mangadex_downloader/tag.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/tracker/__init__.py` & `mangadex-downloader-2.9.1/mangadex_downloader/tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/legacy.py` & `mangadex-downloader-2.9.1/mangadex_downloader/tracker/info_data/legacy.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/tracker/info_data/sqlite.py` & `mangadex-downloader-2.9.1/mangadex_downloader/tracker/info_data/sqlite.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/tracker/legacy.py` & `mangadex-downloader-2.9.1/mangadex_downloader/tracker/legacy.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_ch_info.sql` & `mangadex-downloader-2.9.1/mangadex_downloader/tracker/sql_files/create_ch_info.sql`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_file_info.sql` & `mangadex-downloader-2.9.1/mangadex_downloader/tracker/sql_files/create_file_info.sql`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/tracker/sql_files/create_img_info.sql` & `mangadex-downloader-2.9.1/mangadex_downloader/tracker/sql_files/create_img_info.sql`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/tracker/sqlite.py` & `mangadex-downloader-2.9.1/mangadex_downloader/tracker/sqlite.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/update.py` & `mangadex-downloader-2.9.1/mangadex_downloader/update.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/user.py` & `mangadex-downloader-2.9.1/mangadex_downloader/user.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader/utils.py` & `mangadex-downloader-2.9.1/mangadex_downloader/utils.py`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader.egg-info/PKG-INFO` & `mangadex-downloader-2.9.1/mangadex_downloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mangadex-downloader
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Command-line tool to download manga from MangaDex, written in Python
 Home-page: https://github.com/mansuf/mangadex-downloader
 Download-URL: https://github.com/mansuf/mangadex-downloader/releases
 Author: Rahman Yusuf
 Author-email: danipart4@gmail.com
 License: MIT
 Keywords: mangadex
```

### Comparing `mangadex-downloader-2.9.0/mangadex_downloader.egg-info/SOURCES.txt` & `mangadex-downloader-2.9.1/mangadex_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mangadex-downloader-2.9.0/setup.py` & `mangadex-downloader-2.9.1/setup.py`

 * *Files identical despite different names*

