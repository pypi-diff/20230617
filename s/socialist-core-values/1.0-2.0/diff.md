# Comparing `tmp/socialist_core_values-1.0.tar.gz` & `tmp/socialist_core_values-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialist_core_values-1.0.tar", last modified: Sat Jun 17 08:31:56 2023, max compression
+gzip compressed data, was "socialist_core_values-2.0.tar", last modified: Sat Jun 17 08:50:38 2023, max compression
```

## Comparing `socialist_core_values-1.0.tar` & `socialist_core_values-2.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 08:31:55.996212 socialist_core_values-1.0/
--rw-rw-rw-   0        0        0    35823 2023-06-17 08:26:19.000000 socialist_core_values-1.0/LICENSE
--rw-rw-rw-   0        0        0      261 2023-06-17 08:31:55.995207 socialist_core_values-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-06-17 08:26:19.000000 socialist_core_values-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 08:31:55.996212 socialist_core_values-1.0/setup.cfg
--rw-rw-rw-   0        0        0      461 2023-06-17 08:30:37.000000 socialist_core_values-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 08:31:55.994201 socialist_core_values-1.0/socialist_core_values.egg-info/
--rw-rw-rw-   0        0        0      261 2023-06-17 08:31:55.000000 socialist_core_values-1.0/socialist_core_values.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-06-17 08:31:55.000000 socialist_core_values-1.0/socialist_core_values.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 08:31:55.000000 socialist_core_values-1.0/socialist_core_values.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 08:31:55.000000 socialist_core_values-1.0/socialist_core_values.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 08:50:38.860479 socialist_core_values-2.0/
+-rw-rw-rw-   0        0        0    35823 2023-06-17 08:26:19.000000 socialist_core_values-2.0/LICENSE
+-rw-rw-rw-   0        0        0      261 2023-06-17 08:50:38.859357 socialist_core_values-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-06-17 08:26:19.000000 socialist_core_values-2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 08:50:38.860479 socialist_core_values-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      461 2023-06-17 08:50:28.000000 socialist_core_values-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:50:38.850239 socialist_core_values-2.0/socialist_core_values/
+-rw-rw-rw-   0        0        0      105 2023-03-10 06:19:10.000000 socialist_core_values-2.0/socialist_core_values/__init__.py
+-rw-rw-rw-   0        0        0     2114 2023-06-17 08:24:43.000000 socialist_core_values-2.0/socialist_core_values/main.py
+drwxrwxrwx   0        0        0        0 2023-06-17 08:50:38.858350 socialist_core_values-2.0/socialist_core_values.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-06-17 08:50:38.000000 socialist_core_values-2.0/socialist_core_values.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-17 08:50:38.000000 socialist_core_values-2.0/socialist_core_values.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 08:50:38.000000 socialist_core_values-2.0/socialist_core_values.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-06-17 08:50:38.000000 socialist_core_values-2.0/socialist_core_values.egg-info/top_level.txt
```

### Comparing `socialist_core_values-1.0/LICENSE` & `socialist_core_values-2.0/LICENSE`

 * *Files identical despite different names*

