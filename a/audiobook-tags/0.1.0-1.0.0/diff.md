# Comparing `tmp/audiobook-tags-0.1.0.tar.gz` & `tmp/audiobook-tags-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiobook-tags-0.1.0.tar", last modified: Fri Jun 16 06:22:43 2023, max compression
+gzip compressed data, was "audiobook-tags-1.0.0.tar", last modified: Sat Jun 17 04:48:08 2023, max compression
```

## Comparing `audiobook-tags-0.1.0.tar` & `audiobook-tags-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:43.168458 audiobook-tags-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-16 06:22:30.000000 audiobook-tags-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-16 06:22:30.000000 audiobook-tags-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-16 06:22:43.168458 audiobook-tags-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-16 06:22:30.000000 audiobook-tags-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 06:22:43.168458 audiobook-tags-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-16 06:22:30.000000 audiobook-tags-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:43.164458 audiobook-tags-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 06:22:43.168458 audiobook-tags-0.1.0/src/audiobook_tags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-16 06:22:43.000000 audiobook-tags-0.1.0/src/audiobook_tags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-16 06:22:43.000000 audiobook-tags-0.1.0/src/audiobook_tags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:22:43.000000 audiobook-tags-0.1.0/src/audiobook_tags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 06:22:43.000000 audiobook-tags-0.1.0/src/audiobook_tags.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 06:22:43.000000 audiobook-tags-0.1.0/src/audiobook_tags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 06:22:43.000000 audiobook-tags-0.1.0/src/audiobook_tags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:48:08.619668 audiobook-tags-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-17 04:47:59.000000 audiobook-tags-1.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 04:47:59.000000 audiobook-tags-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-17 04:48:08.619668 audiobook-tags-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-17 04:47:59.000000 audiobook-tags-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-17 04:48:08.619668 audiobook-tags-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-17 04:47:59.000000 audiobook-tags-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:48:08.615668 audiobook-tags-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 04:48:08.619668 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 04:48:08.000000 audiobook-tags-1.0.0/src/audiobook_tags.egg-info/top_level.txt
```

### Comparing `audiobook-tags-0.1.0/LICENSE.txt` & `audiobook-tags-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `audiobook-tags-0.1.0/setup.py` & `audiobook-tags-1.0.0/setup.py`

 * *Files identical despite different names*

