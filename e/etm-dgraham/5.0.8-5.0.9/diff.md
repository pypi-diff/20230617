# Comparing `tmp/etm-dgraham-5.0.8.tar.gz` & `tmp/etm-dgraham-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.0.8.tar", last modified: Wed Jun 14 00:21:08 2023, max compression
+gzip compressed data, was "etm-dgraham-5.0.9.tar", last modified: Thu Jun 15 14:14:47 2023, max compression
```

## Comparing `etm-dgraham-5.0.8.tar` & `etm-dgraham-5.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.526338 etm-dgraham-5.0.8/
--rw-r--r--   0 dag        (501) staff       (20)     2463 2023-06-14 00:17:51.000000 etm-dgraham-5.0.8/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   129624 2023-06-14 00:21:08.526166 etm-dgraham-5.0.8/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   128712 2023-06-08 20:23:17.000000 etm-dgraham-5.0.8/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.8/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.8/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.518404 etm-dgraham-5.0.8/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.522472 etm-dgraham-5.0.8/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.0.8/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-14 00:17:51.000000 etm-dgraham-5.0.8/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.8/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.8/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.8/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   282318 2023-06-14 00:17:51.000000 etm-dgraham-5.0.8/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37350 2023-06-08 15:18:02.000000 etm-dgraham-5.0.8/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.8/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)    98133 2023-06-14 00:17:51.000000 etm-dgraham-5.0.8/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.524513 etm-dgraham-5.0.8/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   129624 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-14 00:21:08.000000 etm-dgraham-5.0.8/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.8/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.8/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.8/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-14 00:21:08.526380 etm-dgraham-5.0.8/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.8/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.524608 etm-dgraham-5.0.8/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.8/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-14 00:21:08.525551 etm-dgraham-5.0.8/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.8/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.8/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.8/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.8/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.048062 etm-dgraham-5.0.9/
+-rw-r--r--   0 dag        (501) staff       (20)     2463 2023-06-15 14:14:22.000000 etm-dgraham-5.0.9/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   129624 2023-06-15 14:14:47.047914 etm-dgraham-5.0.9/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   128712 2023-06-14 16:35:47.000000 etm-dgraham-5.0.9/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.9/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.9/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.039799 etm-dgraham-5.0.9/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.043736 etm-dgraham-5.0.9/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-13 20:00:03.000000 etm-dgraham-5.0.9/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-15 14:14:22.000000 etm-dgraham-5.0.9/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.9/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.9/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.9/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   283305 2023-06-15 14:14:22.000000 etm-dgraham-5.0.9/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37350 2023-06-14 16:35:47.000000 etm-dgraham-5.0.9/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.9/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    98989 2023-06-15 12:36:09.000000 etm-dgraham-5.0.9/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.046348 etm-dgraham-5.0.9/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   129624 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-15 14:14:47.000000 etm-dgraham-5.0.9/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.9/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.9/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.9/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-15 14:14:47.048094 etm-dgraham-5.0.9/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.9/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.046451 etm-dgraham-5.0.9/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.9/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-15 14:14:47.047422 etm-dgraham-5.0.9/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.9/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.9/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.9/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.9/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.0.8/CHANGES.txt` & `etm-dgraham-5.0.9/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-Recent tagged changes as of 2023-06-13T20:17:48.417919-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.0.8) Daniel Graham
+Recent tagged changes as of 2023-06-15T10:14:19.986207-04:00:
+- 1 second ago (HEAD -> working, tag: 5.0.9) Daniel Graham
+    7f30e8b 2023-06-15 10:14:19 -0400
+    Tagged version 5.0.9.
+
+- 2 days ago (tag: 5.0.8) Daniel Graham
     1f587d1 2023-06-13 20:17:48 -0400
     Tagged version 5.0.8. Only display and allow completion of jthe
     jobs of the oldest unfinished instance of a repeating task.
 
-- 6 days ago (tag: 5.0.7) Daniel Graham
+- 7 days ago (tag: 5.0.7) Daniel Graham
     b9eccc6 2023-06-08 08:38:27 -0400
     Tagged version 5.0.7.
 
-- 8 days ago (tag: 5.0.6) Daniel Graham
+- 10 days ago (tag: 5.0.6) Daniel Graham
     345ca4e 2023-06-05 12:41:31 -0400
     Tagged version 5.0.6.
 
-- 9 days ago (tag: 5.0.5) Daniel Graham
+- 10 days ago (tag: 5.0.5) Daniel Graham
     9273685 2023-06-05 06:28:25 -0400
     Tagged version 5.0.5.
 
-- 9 days ago (tag: 5.0.4) Daniel Graham
+- 10 days ago (tag: 5.0.4) Daniel Graham
     ea199ac 2023-06-05 06:02:56 -0400
     Tagged version 5.0.4.
 
-- 9 days ago (tag: 5.0.3) Daniel Graham
+- 11 days ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
-- 9 days ago (tag: 5.0.2) Daniel Graham
+- 11 days ago (tag: 5.0.2) Daniel Graham
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
 
-- 9 days ago (tag: 5.0.1) Daniel Graham
+- 11 days ago (tag: 5.0.1) Daniel Graham
     b30f0ed 2023-06-04 12:47:15 -0400
     Tagged version 5.0.1.
 
-- 11 days ago (tag: 5.0.0) Daniel Graham
+- 12 days ago (tag: 5.0.0) Daniel Graham
     7bc8090 2023-06-03 07:21:38 -0400
     Tagged version 5.0.0. Use pendulum periods for f and elements of h
     instead of datetimes.
 
-- 2 weeks ago (tag: 4.12.9) Daniel Graham
+- 3 weeks ago (tag: 4.12.9) Daniel Graham
     b8fbc47 2023-05-27 13:45:19 -0400
     Tagged version 4.12.9.
 
 - 3 weeks ago (tag: 4.12.8) Daniel Graham
     b0316d5 2023-05-26 13:50:15 -0400
     Tagged version 4.12.8.
 
@@ -49,19 +53,19 @@
     442ff98 2023-05-25 13:53:52 -0400
     Tagged version 4.12.7.
 
 - 3 weeks ago (tag: 4.12.6) Daniel Graham
     3da7332 2023-05-23 14:01:37 -0400
     Tagged version 4.12.6.
 
-- 3 weeks ago (tag: 4.12.5) Daniel Graham
+- 4 weeks ago (tag: 4.12.5) Daniel Graham
     f0c24d8 2023-05-21 15:08:06 -0400
     Tagged version 4.12.5.
 
-- 3 weeks ago (tag: 4.12.4) Daniel Graham
+- 4 weeks ago (tag: 4.12.4) Daniel Graham
     15b3333 2023-05-20 14:33:40 -0400
     Tagged version 4.12.4.
 
 - 4 weeks ago (tag: 4.12.3) Daniel Graham
     dd49fda 2023-05-17 12:24:12 -0400
     Tagged version 4.12.3.
 
@@ -70,14 +74,10 @@
     Tagged version 4.12.2.
 
 - 4 weeks ago (tag: 4.12.1) Daniel Graham
     68005b7 2023-05-15 14:20:25 -0400
     Tagged version 4.12.1. Added display for all-day events to busy
     view
 
-- 4 weeks ago (tag: 4.12.0) Daniel Graham
+- 5 weeks ago (tag: 4.12.0) Daniel Graham
     ce2ab09 2023-05-13 12:46:39 -0400
     Tagged version 4.12.0. Added engaged view
-
-- 5 weeks ago (tag: 4.11.18) Daniel Graham
-    cd5482a 2023-05-11 12:20:48 -0400
-    Tagged version 4.11.18.
```

### Comparing `etm-dgraham-5.0.8/PKG-INFO` & `etm-dgraham-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.8
+Version: 5.0.9
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.0.8/README.md` & `etm-dgraham-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/bump.py` & `etm-dgraham-5.0.9/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/docs/index_konnections.md` & `etm-dgraham-5.0.9/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/docs/index_usedtime.md` & `etm-dgraham-5.0.9/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/docs/multiple_timers.md` & `etm-dgraham-5.0.9/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etm/__main__.py` & `etm-dgraham-5.0.9/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etm/data.py` & `etm-dgraham-5.0.9/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etm/ical.py` & `etm-dgraham-5.0.9/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etm/make_examples.py` & `etm-dgraham-5.0.9/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etm/model.py` & `etm-dgraham-5.0.9/etm/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
                 '-': ["exclude", "list of datetimes to exclude", self.do_datetimes],
                 'a': ["alerts", "list of alerts", do_alert],
                 'b': ["beginby", "number of days for beginby notices", do_beginby],
                 'c': ["calendar", "calendar", do_string],
                 'd': ["description", "item details", do_paragraph],
                 'e': ["extent", "timeperiod", do_duration],
                 'w': ["wrap", "list of two timeperiods", do_two_periods],
-                'f': ["finish", "completion datetime", self.do_completion],
+                'f': ["finish", "completion done -> due", self.do_completion],
                 'g': ["goto", "url or filepath", do_string],
                 'h': ["completions", "list of completion datetimes", self.do_completions],
                 'i': ["index", "forward slash delimited string", do_string],
                 'k': ["konnection", "document id", do_konnection],
                 'l': ["location", "location or context, e.g., home, office, errands", do_string],
                 'm': ["mask", "string to be masked", do_mask],
                 'n': ["attendee", "name <email address>", do_string],
@@ -537,19 +537,19 @@
                 'rW': ["week numbers", "list of integers in 1, ... 53", do_weeknumbers],
                 'rc': ["count", "integer number of repetitions", do_count],
                 'ru': ["until", "datetime", self.do_until],
                 'rs': ["set positions", "integer", do_setpositions],
                 'r?': ["repetition &-key", "enter &-key", self.do_ampr],
 
                 'jj': ["summary", "job summary. Append an '&' to add a job option.", do_string],
-                'ja': ["alert", "list of timeperiod before job is scheduled followed by a colon and a list of command", do_alert],
+                'ja': ["alert", "list of timeperiods before job is scheduled followed by a colon and a list of commands", do_alert],
                 'jb': ["beginby", " integer number of days", do_beginby],
                 'jd': ["description", " string", do_paragraph],
                 'je': ["extent", " timeperiod", do_duration],
-                'jf': ["finish", " datetime", self.do_completion],
+                'jf': ["finish", " completion done -> due", self.do_completion],
                 'ji': ["unique id", " integer or string", do_string],
                 'jl': ["location", " string", do_string],
                 'jm': ["mask", "string to be masked", do_mask],
                 'jp': ["prerequisite ids", "list of ids of immediate prereqs", do_stringlist],
                 'js': ["scheduled", "timeperiod before task scheduled when job is scheduled", do_duration],
                 'ju': ["used time", "timeperiod: datetime", do_usedtime],
                 'j?': ["job &-key", "enter &-key", self.do_ampj],
@@ -833,14 +833,17 @@
                         if self.doc_id in active_tasks:
                             del active_tasks[self.doc_id]
 
                         save_item = True
                     else:  # finished last instance
                         self.item_hsh['f'] = completion_entry
                         save_item = True
+                # else:
+                #     # FIXME This is the undated task with jobs branch
+                #     save_item = True
 
         else:
             # no jobs
             if 's' in self.item_hsh:
                 if 'r' in self.item_hsh:
                     nxt = get_next_due(self.item_hsh, completed_datetime, completion_entry.end)
                     if nxt:
@@ -966,14 +969,16 @@
 
     def update_keyval(self, kv):
         """
         TODO: add return status
         """
         key, val = kv
 
+        condition = 'f' in key
+
         if key in self.keys:
             a, r, do = self.keys[key]
             ask = a
             msg = self.check_allowed(key)
             if msg:
                 obj = None
                 reply = msg
@@ -982,15 +987,15 @@
                 if msg:
                     obj = None
                     reply = msg
                 else:
                     # call the appropriate do for the key
                     obj, rep = do(val)
                     reply = rep if rep else r
-                    if obj:
+                    if obj is not None:
                         self.object_hsh[kv] = obj
                     else:
                         if kv in self.object_hsh:
                             del self.object_hsh[kv]
             self.askreply[kv] = (ask, reply)
         else:
             display_key = f"@{key}" if len(key) == 1 else f"&{key[-1]}"
@@ -1001,17 +1006,18 @@
         created = self.item_hsh.get('created', None)
         self.item_hsh = {'created': created}
         cur_hsh = {}
         cur_key = None
         msg = []
         for pos, (k, v) in self.pos_hsh.items():
             obj = self.object_hsh.get((k, v))
-            if not obj:
+            if obj is None:
                 msg.append(f"bad entry for {k}: {v}")
-                continue
+                return msg
+                # continue
             elif k in ['a', 'u', 'n', 't', 'k']:
                 self.item_hsh.setdefault(k, []).append(obj)
             elif k in ['rr', 'jj']:
                 if cur_hsh:
                     # starting new rrule or job - append the old
                     self.item_hsh.setdefault(cur_key, []).append(cur_hsh)
                 cur_key = k[0]
@@ -1333,26 +1339,26 @@
         if bad_lst:
             rep += f"\nincomplete or invalid completions: {', '.join(bad_lst)}"
 
         return obj, rep
 
 
     def do_completion(self, arg):
-        obj = None
+        # obj = None
         tz = self.item_hsh.get('z', None)
         args = [x.strip() for x in arg.split('->')]
         obj, rep = self.do_datetimes(args)
         parts = [date_to_datetime(x) for x in obj] if obj else []
         if len(parts) > 1:
             start_dt, end_dt = parts[:2]
-            obj = pendulum.period(parts[0], parts[1])
+            obj = pendulum.period(start_dt, end_dt)
             rep = f"{format_datetime(start_dt, short=True)[1]} -> {format_datetime(end_dt, short=True)[1]}"
         else:
             obj = None
-            rep = f"\nincomplete or invalid completion: {rep}"
+            rep = f"\nincomplete or invalid completion: {arg}"
         return obj, rep
 
 
     def do_timezone(self, arg=None):
         """
         >>> item = Item("")
         >>> item.do_timezone()
@@ -5231,26 +5237,26 @@
     for i in ids:
         if last_completion:
             # remove all completions if repeating
             # last_completion will be returned to set @s for the next instance or @f if there are none
             del id2hsh[i]['f']
         else:
             # remove finished jobs from the requirements
-            if id2hsh[i].get('f', None):
+            if id2hsh[i].get('f', None) is not None:
                 # i is finished so remove it from the requirements for any
                 # other jobs
                 for j in ids:
                     if i in req[j]:
                         # since i is finished, remove it from j's requirements
                         req[j].remove(i)
 
     awf = [0, 0, 0]
     # set the job status for each job - f) finished, a) available or w) waiting
     for i in ids:
-        if id2hsh[i].get('f', None): # i is finished
+        if id2hsh[i].get('f', None) is not None: # i is finished
             id2hsh[i]['status'] = FINISHED_CHAR
             awf[2] += 1
         elif req[i]: # there are unfinished requirements for i
             id2hsh[i]['status'] = '+'
             awf[1] += 1
         else: # there are no unfinished requirements for i
             id2hsh[i]['status'] = '-'
@@ -5260,14 +5266,15 @@
         id2hsh[i]['summary'] = "{} {}: {}".format(summary, "/".join([str(x) for x in awf]), id2hsh[i]['j'])
         id2hsh[i]['req'] = req[i]
         id2hsh[i]['i'] = i
 
     if msg:
         logger.warning(f"{msg}")
         return False, msg, None
+    # logger.debug(f"returning True, {[id2hsh[i] for i in ids]}, {last_completion}")
     return True, [id2hsh[i] for i in ids], last_completion
 
 #######################
 ### end jobs setup ####
 #######################
 
 
@@ -5689,15 +5696,16 @@
                     else: # k or p
                         relevant = rset.after(today, inc=True)
                         already_done = [x.end for x in item.get('h', [])]
                         # relevant will be the first instance after 12am today
                         # it will be the @s entry for the updated repeating item
                         # these are @s entries for the instances to be preserved
                         between = rset.between(dtstart, today-ONEMIN, inc=True)
-                        remaining = [x for x in between if x not in already_done and x != dtstart]
+                        # remaining = [x for x in between if x not in already_done and x != dtstart]
+                        remaining = [x for x in between if x not in already_done]
                         # once instances have been created, between will be empty until
                         # the current date falls after item['s'] and relevant is reset
                         num_remaining = f"({len(remaining)})" if remaining else ""
                         sum_abbr = item['summary'][:summary_width]
                         summary = f"{sum_abbr} {num_remaining}"
                         if dtstart.date() < today.date() and 'j' not in item:
                             pastdue.append([(dtstart.date() - today.date()).days, summary, item.doc_id, None, None])
@@ -6243,15 +6251,15 @@
         flags = get_flags(doc_id, link_list, konnect_list, pinned_list, timers)
         if 'j' in item:
             task_location = item.get('l', '~')
             priority = int(item.get('p', 0))
             sort_priority = 4 - int(priority)
             show_priority = str(priority) if priority > 0 else ""
             for job in item['j']:
-                if job.get('f'):
+                if job.get('f', None) is not None:
                     # show completed jobs only in completed view
                     continue
                 location = job.get('l', task_location)
                 extent = job.get('e', '')
                 extent = format_duration(extent) if extent else ''
                 status = 0 if job.get('status') == '-' else 1
                 # status 1 -> waiting, status 0 -> available
@@ -6776,29 +6784,27 @@
     engaged_hsh = {}
     engaged2id_hsh = {}     # yw -> row2id
     week2day2engaged = {}   # year, week -> dayofweek -> period total for day
     week2day2heading = {}
     weeks = set([])
     rows = []
     done = []
+    completed = []
     engaged = []
     # busy = []
 
     #XXX year, week -> dayofweek -> list of [time interval, summary, period]
     busy_details = {}
     week2day2busy = {}
     week2day2allday = {}
 
     #XXX main loop begins
     todayYMD = now.format("YYYYMMDD")
     tomorrowYMD = (now + 1*DAY).format("YYYYMMDD")
 
-    # Only display one active instance of a repeating task with jobs
-    repeating_with_jobs_ids = []
-
     for item in db:
         if item.get('itemtype', None) == None:
             logger.error(f"itemtype missing from {item}")
             continue
         if item['itemtype'] in "!?":
             continue
 
@@ -6869,26 +6875,34 @@
                             ],
                         }
                     )
 
 
         if itemtype == '-':
             d = [] # d for done
+            # c = [] # c for completed
             if isinstance(finished, pendulum.Period):
                 # finished will be false if the period is ZERO
+                # we need details of when completed (start and end) for completed view
                 d.append([finished.start, summary, doc_id, format_date(finished.end)[1]])
+                # to skip completed instances we only need the completed (end) instance
+                completed.append(finished.end)
+                # ditto below for history
             if history:
                 for dt in history:
                     d.append([dt.start, summary, doc_id, format_date(dt.end)[1]])
+                    completed.append(dt.end)
             if jobs:
                 for job in jobs:
                     job_summary = job.get('summary', '')
                     if 'f' in job:
                         # FIXME
-                        d.append([job['f'].start, job_summary, doc_id, job['i']])
+                        # d.append([job['f'].start, job_summary, doc_id, format_date(job['f'].end)[1]])
+                        d.append([job['f'].start, job_summary, doc_id, ""])
+                        completed.append(job['f'].end)
             if d:
                 for row in d:
                     dt = row[0]
                     if isinstance(dt, pendulum.Date) and not isinstance(dt, pendulum.DateTime):
                         # dt = pendulum.parse(dt.format("YYYYMMDD"), tz='local')
                         dt = pendulum.datetime(dt.year, dt.month, dt.day, tz='local')
                         # dt.set(hour=23, minute=59, second=59)
@@ -6914,15 +6928,16 @@
                                     flags,
                                     rhc,
                                     (row[2], None, row[3])
                                     ],
                             }
                             )
 
-        if not start or finished is not None:
+        startdt = date_to_datetime(start)
+        if not start or finished is not None or startdt in completed:
             continue
 
         # XXX INSTANCES
 
         # keep these for reference for this item
         end_dt = None
 
@@ -6953,23 +6968,24 @@
             if 'r' in item:
                 freq = item['r'][0].get('r', 'y')
             else:
                 freq = 'y'
 
             instance = dt if '+' in item or 'r' in item else None
 
+            if instance in completed:
+                continue
+
             if 'j' in item:
 
                 # repeating task with jobs
 
                 if instance:
                     if doc_id in active_tasks and active_tasks[doc_id] != instance:
                             continue
-
-
                     else:
                         active_tasks[doc_id] = instance
 
 
                 for job in item['j']:
                     if 'f' in job:
                         continue
```

### Comparing `etm-dgraham-5.0.8/etm/options.py` & `etm-dgraham-5.0.9/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etm/report.py` & `etm-dgraham-5.0.9/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etm/view.py` & `etm-dgraham-5.0.9/etm/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -2144,22 +2144,53 @@
     timer_warning = " and\nits associated timer" if has_timer else ""
     repeating = 'r' in hsh or '+' in hsh
 
     between = []
     due = ""
 
     title = "Finish"
-    if instance and instance != model.date_to_datetime(hsh['s']):
+
+    if job:
+        # only a completion date needed - either undated or finishing the oldest instance
+        need = 1
+        between = [hsh.get('s', None)]
+        entry =  "now"
+        # due = hsh.get('s', "")
+        start = f"\nDue: {format_datetime(hsh['s'])[1]}" if 's' in hsh else ""
+
+        text= f"""\
+Selected: {hsh['itemtype']} {hsh['summary']}\nJob: {job}{start}
+
+Enter <completion datetime>
+        """
+
+
+    elif instance and instance == model.date_to_datetime(hsh['s']):
+        # the oldest instance is selected
+        need = 1
+        between = [hsh.get('s', None)]
+        entry =  "now"
+        # due = hsh.get('s', "")
+        start = f"\nDue: {format_datetime(hsh['s'])[1]}" if 's' in hsh else ""
+
+        text= f"""\
+Selected: {hsh['itemtype']} {hsh['summary']}{start}
+
+Enter <completion datetime>
+        """
+
+    elif instance:
+        # either the instance or the oldest
         need = 2
         between = [hsh['s'], instance]
-        if instance != hsh['s']:
-            values = [
-                f"{format_datetime(hsh['s'])[1]} (oldest)",
-                f"{format_datetime(instance)[1]} (selected)",
-                ]
+        # if instance != hsh['s']:
+        values = [
+            f"{format_datetime(hsh['s'])[1]} (oldest)",
+            f"{format_datetime(instance)[1]} (selected)",
+            ]
 
         values_list = []
         count = -1
         for x in values:
             count += 1
             values_list.append(f"    {count}: {x}")
 
@@ -2173,16 +2204,16 @@
 The number of the instance to finish and
 the completion datetime to use?
 number : datetime\
         """
         entry = "1 : now"
         due = ""
 
-
-    elif repeating and between:
+    elif repeating:
+        # must be selected from today's pastdue
         already_done = [x.end for x in hsh.get('h', [])]
         need = 2
         between = [x[0] for x in model.item_instances(hsh, model.date_to_datetime(hsh['s']), pendulum.now().replace(hour=0, minute=0, second=0, microsecond=0)) if x[0] not in already_done]
         values_list = []
         # values.append( (0, format_datetime(between[0][0])[1]) )
         count = -1
         for x in between:
```

### Comparing `etm-dgraham-5.0.8/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.0.9/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.8
+Version: 5.0.9
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.0.8/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.0.9/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.0.9/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etmlogo.png` & `etm-dgraham-5.0.9/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etmlogo_small.png` & `etm-dgraham-5.0.9/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/etmview_agenda.png` & `etm-dgraham-5.0.9/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/namedcolors.py` & `etm-dgraham-5.0.9/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/new.png` & `etm-dgraham-5.0.9/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/setup.py` & `etm-dgraham-5.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/test/test_parser.py` & `etm-dgraham-5.0.9/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/utilities/colons_to_slashes.py` & `etm-dgraham-5.0.9/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/utilities/etm_in` & `etm-dgraham-5.0.9/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/utilities/inbasket` & `etm-dgraham-5.0.9/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.8/utilities/open_in_mutt` & `etm-dgraham-5.0.9/utilities/open_in_mutt`

 * *Files identical despite different names*

