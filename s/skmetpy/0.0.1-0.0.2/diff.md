# Comparing `tmp/skmetpy-0.0.1.tar.gz` & `tmp/skmetpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skmetpy-0.0.1.tar", last modified: Sat Jun 17 10:33:53 2023, max compression
+gzip compressed data, was "skmetpy-0.0.2.tar", last modified: Sat Jun 17 10:44:55 2023, max compression
```

## Comparing `skmetpy-0.0.1.tar` & `skmetpy-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 10:33:53.052795 skmetpy-0.0.1/
--rw-rw-rw-   0        0        0      259 2023-06-17 10:33:53.052795 skmetpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-17 10:33:53.052795 skmetpy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      324 2023-06-17 10:33:45.000000 skmetpy-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 10:33:53.051826 skmetpy-0.0.1/skmetpy.egg-info/
--rw-rw-rw-   0        0        0      259 2023-06-17 10:33:53.000000 skmetpy-0.0.1/skmetpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      132 2023-06-17 10:33:53.000000 skmetpy-0.0.1/skmetpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 10:33:53.000000 skmetpy-0.0.1/skmetpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 10:33:53.000000 skmetpy-0.0.1/skmetpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 10:44:55.366897 skmetpy-0.0.2/
+-rw-rw-rw-   0        0        0      259 2023-06-17 10:44:55.366897 skmetpy-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-17 10:44:55.361737 skmetpy-0.0.2/nunpy/
+-rw-rw-rw-   0        0        0       34 2023-06-17 10:44:27.000000 skmetpy-0.0.2/nunpy/__init__.py
+-rw-rw-rw-   0        0        0       37 2023-06-17 10:43:49.000000 skmetpy-0.0.2/nunpy/rechape.py
+-rw-rw-rw-   0        0        0       42 2023-06-17 10:44:55.366897 skmetpy-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      324 2023-06-17 10:44:42.000000 skmetpy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 10:44:55.365895 skmetpy-0.0.2/skmetpy.egg-info/
+-rw-rw-rw-   0        0        0      259 2023-06-17 10:44:55.000000 skmetpy-0.0.2/skmetpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-17 10:44:55.000000 skmetpy-0.0.2/skmetpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 10:44:55.000000 skmetpy-0.0.2/skmetpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 10:44:55.000000 skmetpy-0.0.2/skmetpy.egg-info/top_level.txt
```

