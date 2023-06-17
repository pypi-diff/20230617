# Comparing `tmp/telegram-upload-0.6.0.tar.gz` & `tmp/telegram-upload-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram-upload-0.6.0.tar", last modified: Thu Jun 15 21:02:09 2023, max compression
+gzip compressed data, was "telegram-upload-0.6.1.tar", last modified: Sat Jun 17 14:15:51 2023, max compression
```

## Comparing `telegram-upload-0.6.0.tar` & `telegram-upload-0.6.1.tar`

### file list

```diff
@@ -1,69 +1,56 @@
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-06-15 21:02:09.311202 telegram-upload-0.6.0/
--rw-r--r--   0 nekmo     (1000) users      (100)      152 2020-09-11 13:53:01.000000 telegram-upload-0.6.0/AUTHORS.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     3321 2018-03-26 15:24:08.000000 telegram-upload-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     3817 2023-06-15 20:45:42.000000 telegram-upload-0.6.0/HISTORY.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     1065 2018-03-26 15:24:08.000000 telegram-upload-0.6.0/LICENSE
--rw-r--r--   0 nekmo     (1000) users      (100)      407 2019-03-15 19:00:45.000000 telegram-upload-0.6.0/MANIFEST.in
--rw-r--r--   0 nekmo     (1000) users      (100)     5669 2023-06-15 21:02:09.311202 telegram-upload-0.6.0/PKG-INFO
--rw-r--r--   0 nekmo     (1000) users      (100)     4660 2023-06-14 11:35:47.000000 telegram-upload-0.6.0/README.rst
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-06-15 21:02:09.297869 telegram-upload-0.6.0/docs/
--rw-r--r--   0 nekmo     (1000) users      (100)     7452 2020-05-06 23:30:09.000000 telegram-upload-0.6.0/docs/Makefile
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-06-15 21:02:09.291202 telegram-upload-0.6.0/docs/_build/
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-06-15 21:02:09.291202 telegram-upload-0.6.0/docs/_build/html/
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-06-15 21:02:09.301202 telegram-upload-0.6.0/docs/_build/html/_static/
--rw-r--r--   0 nekmo     (1000) users      (100)    19192 2020-04-19 22:56:18.000000 telegram-upload-0.6.0/docs/_build/html/_static/a462d4fca3dc794db2.gif
--rw-r--r--   0 nekmo     (1000) users      (100)      286 2020-10-04 02:14:24.000000 telegram-upload-0.6.0/docs/_build/html/_static/file.png
--rw-r--r--   0 nekmo     (1000) users      (100)    49610 2020-04-19 23:03:56.000000 telegram-upload-0.6.0/docs/_build/html/_static/logo.png
--rw-r--r--   0 nekmo     (1000) users      (100)       90 2020-10-04 02:14:24.000000 telegram-upload-0.6.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 nekmo     (1000) users      (100)       90 2020-10-04 02:14:24.000000 telegram-upload-0.6.0/docs/_build/html/_static/plus.png
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-06-15 21:02:09.301202 telegram-upload-0.6.0/docs/_static/
--rw-r--r--   0 nekmo     (1000) users      (100)    19192 2020-04-19 22:56:18.000000 telegram-upload-0.6.0/docs/_static/a462d4fca3dc794db2.gif
--rw-r--r--   0 nekmo     (1000) users      (100)    49610 2020-04-19 23:03:56.000000 telegram-upload-0.6.0/docs/_static/logo.png
--rw-r--r--   0 nekmo     (1000) users      (100)       28 2018-05-06 00:43:04.000000 telegram-upload-0.6.0/docs/authors.rst
--rwxr-xr-x   0 nekmo     (1000) users      (100)     9637 2020-12-28 22:50:49.000000 telegram-upload-0.6.0/docs/conf.py
--rw-r--r--   0 nekmo     (1000) users      (100)       33 2018-05-06 00:43:04.000000 telegram-upload-0.6.0/docs/contributing.rst
--rw-r--r--   0 nekmo     (1000) users      (100)       28 2018-05-06 00:43:04.000000 telegram-upload-0.6.0/docs/history.rst
--rw-r--r--   0 nekmo     (1000) users      (100)      553 2020-12-28 22:50:49.000000 telegram-upload-0.6.0/docs/index.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     1815 2021-09-08 23:36:33.000000 telegram-upload-0.6.0/docs/installation.rst
--rw-r--r--   0 nekmo     (1000) users      (100)      112 2020-04-19 15:44:37.000000 telegram-upload-0.6.0/docs/modules.rst
--rw-r--r--   0 nekmo     (1000) users      (100)       27 2020-04-19 23:17:30.000000 telegram-upload-0.6.0/docs/readme.rst
--rw-r--r--   0 nekmo     (1000) users      (100)      103 2020-04-19 15:44:37.000000 telegram-upload-0.6.0/docs/setup.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     1154 2020-04-19 15:44:37.000000 telegram-upload-0.6.0/docs/telegram_upload.rst
--rw-r--r--   0 nekmo     (1000) users      (100)      143 2020-04-19 15:44:37.000000 telegram-upload-0.6.0/docs/travis_pypi_setup.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     2341 2020-12-28 22:50:49.000000 telegram-upload-0.6.0/docs/troubleshooting.rst
--rw-r--r--   0 nekmo     (1000) users      (100)     5893 2023-06-14 17:51:52.000000 telegram-upload-0.6.0/docs/usage.rst
--rw-r--r--   0 nekmo     (1000) users      (100)       80 2021-09-11 01:48:21.000000 telegram-upload-0.6.0/requirements.txt
--rw-r--r--   0 nekmo     (1000) users      (100)      398 2023-06-15 21:02:09.311202 telegram-upload-0.6.0/setup.cfg
--rw-r--r--   0 nekmo     (1000) users      (100)     4669 2023-06-15 20:12:20.000000 telegram-upload-0.6.0/setup.py
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-06-15 21:02:09.304536 telegram-upload-0.6.0/telegram_upload/
--rw-r--r--   0 nekmo     (1000) users      (100)      151 2023-06-15 20:56:12.000000 telegram-upload-0.6.0/telegram_upload/__init__.py
--rw-r--r--   0 nekmo     (1000) users      (100)       86 2020-05-06 22:38:42.000000 telegram-upload-0.6.0/telegram_upload/_compat.py
--rw-r--r--   0 nekmo     (1000) users      (100)     5001 2022-05-12 23:00:37.000000 telegram-upload-0.6.0/telegram_upload/cli.py
--rw-r--r--   0 nekmo     (1000) users      (100)    10835 2023-06-14 17:31:18.000000 telegram-upload-0.6.0/telegram_upload/client.py
--rw-r--r--   0 nekmo     (1000) users      (100)      830 2021-09-04 02:28:03.000000 telegram-upload-0.6.0/telegram_upload/config.py
--rw-r--r--   0 nekmo     (1000) users      (100)     8052 2023-06-14 17:30:54.000000 telegram-upload-0.6.0/telegram_upload/download_files.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1639 2021-09-04 00:43:12.000000 telegram-upload-0.6.0/telegram_upload/exceptions.py
--rw-r--r--   0 nekmo     (1000) users      (100)    11840 2023-06-14 18:24:38.000000 telegram-upload-0.6.0/telegram_upload/management.py
--rw-r--r--   0 nekmo     (1000) users      (100)     7478 2023-06-14 01:35:41.000000 telegram-upload-0.6.0/telegram_upload/upload_files.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1570 2022-02-27 03:32:42.000000 telegram-upload-0.6.0/telegram_upload/utils.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1972 2022-05-12 22:38:59.000000 telegram-upload-0.6.0/telegram_upload/video.py
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-06-15 21:02:09.307869 telegram-upload-0.6.0/telegram_upload.egg-info/
--rw-r--r--   0 nekmo     (1000) users      (100)     5669 2023-06-15 21:02:09.000000 telegram-upload-0.6.0/telegram_upload.egg-info/PKG-INFO
--rw-r--r--   0 nekmo     (1000) users      (100)     1424 2023-06-15 21:02:09.000000 telegram-upload-0.6.0/telegram_upload.egg-info/SOURCES.txt
--rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-06-15 21:02:09.000000 telegram-upload-0.6.0/telegram_upload.egg-info/dependency_links.txt
--rw-r--r--   0 nekmo     (1000) users      (100)      134 2023-06-15 21:02:09.000000 telegram-upload-0.6.0/telegram_upload.egg-info/entry_points.txt
--rw-r--r--   0 nekmo     (1000) users      (100)        1 2023-06-15 21:02:09.000000 telegram-upload-0.6.0/telegram_upload.egg-info/not-zip-safe
--rw-r--r--   0 nekmo     (1000) users      (100)       85 2023-06-15 21:02:09.000000 telegram-upload-0.6.0/telegram_upload.egg-info/requires.txt
--rw-r--r--   0 nekmo     (1000) users      (100)       22 2023-06-15 21:02:09.000000 telegram-upload-0.6.0/telegram_upload.egg-info/top_level.txt
-drwxr-xr-x   0 nekmo     (1000) users      (100)        0 2023-06-15 21:02:09.311202 telegram-upload-0.6.0/tests/
--rw-r--r--   0 nekmo     (1000) users      (100)        0 2020-12-28 22:50:49.000000 telegram-upload-0.6.0/tests/__init__.py
--rw-r--r--   0 nekmo     (1000) users      (100)       88 2020-12-30 23:03:14.000000 telegram-upload-0.6.0/tests/_compat.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1524 2022-02-27 04:26:40.000000 telegram-upload-0.6.0/tests/test_cli.py
--rw-r--r--   0 nekmo     (1000) users      (100)     3837 2023-06-13 22:53:00.000000 telegram-upload-0.6.0/tests/test_client.py
--rw-r--r--   0 nekmo     (1000) users      (100)      901 2021-03-01 23:27:00.000000 telegram-upload-0.6.0/tests/test_config.py
--rw-r--r--   0 nekmo     (1000) users      (100)    10678 2023-06-14 00:25:07.000000 telegram-upload-0.6.0/tests/test_download_files.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1128 2020-12-30 23:04:05.000000 telegram-upload-0.6.0/tests/test_exceptions.py
--rw-r--r--   0 nekmo     (1000) users      (100)     4134 2023-06-12 01:38:59.000000 telegram-upload-0.6.0/tests/test_files.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1444 2021-03-04 01:48:06.000000 telegram-upload-0.6.0/tests/test_management.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1217 2020-12-28 22:50:49.000000 telegram-upload-0.6.0/tests/test_utils.py
--rw-r--r--   0 nekmo     (1000) users      (100)     1345 2020-12-28 22:50:49.000000 telegram-upload-0.6.0/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    49610 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9637 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-17 14:15:51.858001 telegram-upload-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/telegram_upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/upload_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/telegram_upload/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/telegram_upload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 14:15:51.000000 telegram-upload-0.6.1/telegram_upload.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:51.854001 telegram-upload-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_download_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-17 14:15:29.000000 telegram-upload-0.6.1/tests/test_video.py
```

### Comparing `telegram-upload-0.6.0/CONTRIBUTING.rst` & `telegram-upload-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/HISTORY.rst` & `telegram-upload-0.6.1/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =======
 History
 =======
 
+0.6.1 (2023-06-17)
+------------------
+
+* Issue #197: if to.lstrip("-+").isdigit(): AttributeError: 'int' object has no attribute 'lstrip'
+
 0.6.0 (2023-06-15)
 ------------------
 
 * Issue #99: Combine split files when downloading
 * Issue #118: Feature Request - Choose channel by ID
 * Issue #113: Numbered files are uploaded in weird order
 * Issue #111: telethon.errors.rpcerrorlist.FloodWaitError: A wait of 819 seconds is required (caused by CheckChatInviteRequest)
```

### Comparing `telegram-upload-0.6.0/LICENSE` & `telegram-upload-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/PKG-INFO` & `telegram-upload-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: telegram-upload
-Version: 0.6.0
+Version: 0.6.1
 Summary: Upload (and download) files to Telegram up to 2 GiB using your account 
 Home-page: https://github.com/Nekmo/telegram-upload/
 Download-URL: https://github.com/Nekmo/telegram-upload/archive/master.zip
 Author: Nekmo
 Author-email: contacto@nekmo.com
 Keywords: telegram-upload,telegram,upload,video
 Platform: linux
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
-Provides: telegram_upload
 Provides: tests
+Provides: telegram_upload
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 
 .. image:: https://raw.githubusercontent.com/Nekmo/telegram-upload/master/logo.png
     :width: 100%
```

### Comparing `telegram-upload-0.6.0/README.rst` & `telegram-upload-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/docs/Makefile` & `telegram-upload-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/docs/_build/html/_static/logo.png` & `telegram-upload-0.6.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/docs/conf.py` & `telegram-upload-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/docs/index.rst` & `telegram-upload-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/docs/installation.rst` & `telegram-upload-0.6.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/docs/troubleshooting.rst` & `telegram-upload-0.6.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/docs/usage.rst` & `telegram-upload-0.6.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/setup.py` & `telegram-upload-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/telegram_upload/cli.py` & `telegram-upload-0.6.1/telegram_upload/cli.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/telegram_upload/client.py` & `telegram-upload-0.6.1/telegram_upload/client.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/telegram_upload/config.py` & `telegram-upload-0.6.1/telegram_upload/config.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/telegram_upload/download_files.py` & `telegram-upload-0.6.1/telegram_upload/download_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/telegram_upload/exceptions.py` & `telegram-upload-0.6.1/telegram_upload/exceptions.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/telegram_upload/management.py` & `telegram-upload-0.6.1/telegram_upload/management.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,15 +175,15 @@
     else:
         thumbnail = None
     files_cls = LARGE_FILE_MODES[large_files]
     files = files_cls(files, caption=caption, thumbnail=thumbnail, force_file=force_file)
     if large_files == 'fail':
         # Validate now
         files = list(files)
-    if to.lstrip("-+").isdigit():
+    if isinstance(to, str) and to.lstrip("-+").isdigit():
         to = int(to)
     if sort and natsorted:
         files = natsorted(files, key=lambda x: x.name)
     elif sort:
         files = sorted(files, key=lambda x: x.name)
     if album:
         client.send_files_as_album(to, files, delete_on_success, print_file_id, forward)
@@ -210,15 +210,15 @@
     "saved messages" and use parameter ``--delete-on-success``. Forwarded messages will
     be removed from the chat after downloading, such as a download queue.
     """
     client = Client(config or default_config(), proxy=proxy)
     client.start()
     if not interactive and not from_:
         from_ = 'me'
-    elif not interactive and from_.lstrip("-+").isdigit():
+    elif isinstance(from_, str)  and from_.lstrip("-+").isdigit():
         from_ = int(from_)
     elif interactive and not from_:
         click.echo('Select the dialog of the files to download:')
         click.echo('[SPACE] Select dialog [ENTER] Next step')
         from_ = async_to_sync(interactive_select_dialog(client))
     if interactive:
         click.echo('Select all files to download:')
```

### Comparing `telegram-upload-0.6.0/telegram_upload/upload_files.py` & `telegram-upload-0.6.1/telegram_upload/upload_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/telegram_upload/utils.py` & `telegram-upload-0.6.1/telegram_upload/utils.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/telegram_upload/video.py` & `telegram-upload-0.6.1/telegram_upload/video.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/telegram_upload.egg-info/PKG-INFO` & `telegram-upload-0.6.1/telegram_upload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: telegram-upload
-Version: 0.6.0
+Version: 0.6.1
 Summary: Upload (and download) files to Telegram up to 2 GiB using your account 
 Home-page: https://github.com/Nekmo/telegram-upload/
 Download-URL: https://github.com/Nekmo/telegram-upload/archive/master.zip
 Author: Nekmo
 Author-email: contacto@nekmo.com
 Keywords: telegram-upload,telegram,upload,video
 Platform: linux
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Natural Language :: English
 Classifier: Development Status :: 5 - Production/Stable
-Provides: telegram_upload
 Provides: tests
+Provides: telegram_upload
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 
 .. image:: https://raw.githubusercontent.com/Nekmo/telegram-upload/master/logo.png
     :width: 100%
```

### Comparing `telegram-upload-0.6.0/tests/test_cli.py` & `telegram-upload-0.6.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/tests/test_client.py` & `telegram-upload-0.6.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/tests/test_config.py` & `telegram-upload-0.6.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/tests/test_download_files.py` & `telegram-upload-0.6.1/tests/test_download_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/tests/test_exceptions.py` & `telegram-upload-0.6.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/tests/test_files.py` & `telegram-upload-0.6.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/tests/test_management.py` & `telegram-upload-0.6.1/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/tests/test_utils.py` & `telegram-upload-0.6.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `telegram-upload-0.6.0/tests/test_video.py` & `telegram-upload-0.6.1/tests/test_video.py`

 * *Files identical despite different names*

