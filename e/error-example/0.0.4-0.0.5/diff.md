# Comparing `tmp/error-example-0.0.4.tar.gz` & `tmp/error-example-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-example-0.0.4.tar", last modified: Sat Jun 17 15:06:50 2023, max compression
+gzip compressed data, was "error-example-0.0.5.tar", last modified: Sat Jun 17 15:16:01 2023, max compression
```

## Comparing `error-example-0.0.4.tar` & `error-example-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 15:06:50.353485 error-example-0.0.4/
--rw-rw-rw-   0        0        0      148 2023-06-17 15:06:50.348026 error-example-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-06-15 17:54:13.000000 error-example-0.0.4/README.txt
--rw-rw-rw-   0        0        0      254 2023-06-17 15:06:25.000000 error-example-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-17 15:06:50.353825 error-example-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-17 15:06:50.315157 error-example-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-17 15:06:50.327171 error-example-0.0.4/src/error_example/
--rw-rw-rw-   0        0        0       15 2023-06-15 17:52:48.000000 error-example-0.0.4/src/error_example/main.py
-drwxrwxrwx   0        0        0        0 2023-06-17 15:06:50.344707 error-example-0.0.4/src/error_example.egg-info/
--rw-rw-rw-   0        0        0      148 2023-06-17 15:06:50.000000 error-example-0.0.4/src/error_example.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-06-17 15:06:50.000000 error-example-0.0.4/src/error_example.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 15:06:50.000000 error-example-0.0.4/src/error_example.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-17 15:06:50.000000 error-example-0.0.4/src/error_example.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 15:16:01.171900 error-example-0.0.5/
+-rw-rw-rw-   0        0        0      148 2023-06-17 15:16:01.169355 error-example-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-06-15 17:54:13.000000 error-example-0.0.5/README.txt
+-rw-rw-rw-   0        0        0      225 2023-06-17 15:15:29.000000 error-example-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-17 15:16:01.172667 error-example-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-17 15:16:01.134120 error-example-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-06-17 15:16:01.141386 error-example-0.0.5/src/error_example/
+-rw-rw-rw-   0        0        0       15 2023-06-15 17:52:48.000000 error-example-0.0.5/src/error_example/main.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:16:01.164046 error-example-0.0.5/src/error_example.egg-info/
+-rw-rw-rw-   0        0        0      148 2023-06-17 15:16:01.000000 error-example-0.0.5/src/error_example.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-06-17 15:16:01.000000 error-example-0.0.5/src/error_example.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 15:16:01.000000 error-example-0.0.5/src/error_example.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-17 15:16:01.000000 error-example-0.0.5/src/error_example.egg-info/top_level.txt
```

