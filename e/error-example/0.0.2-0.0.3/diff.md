# Comparing `tmp/error-example-0.0.2.tar.gz` & `tmp/error-example-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-example-0.0.2.tar", last modified: Fri Jun 16 05:09:32 2023, max compression
+gzip compressed data, was "error-example-0.0.3.tar", last modified: Sat Jun 17 15:04:47 2023, max compression
```

## Comparing `error-example-0.0.2.tar` & `error-example-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 05:09:32.800335 error-example-0.0.2/
--rw-rw-rw-   0        0        0      151 2023-06-16 05:09:32.795489 error-example-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-06-15 17:54:13.000000 error-example-0.0.2/README.md
--rw-rw-rw-   0        0        0      256 2023-06-16 05:09:06.000000 error-example-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 05:09:32.800335 error-example-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 05:09:32.759983 error-example-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 05:09:32.778781 error-example-0.0.2/src/error_example/
--rw-rw-rw-   0        0        0       15 2023-06-15 17:52:48.000000 error-example-0.0.2/src/error_example/main.py
-drwxrwxrwx   0        0        0        0 2023-06-16 05:09:32.795489 error-example-0.0.2/src/error_example.egg-info/
--rw-rw-rw-   0        0        0      151 2023-06-16 05:09:32.000000 error-example-0.0.2/src/error_example.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-06-16 05:09:32.000000 error-example-0.0.2/src/error_example.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 05:09:32.000000 error-example-0.0.2/src/error_example.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-16 05:09:32.000000 error-example-0.0.2/src/error_example.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 15:04:47.592464 error-example-0.0.3/
+-rw-rw-rw-   0        0        0       98 2023-06-17 15:04:47.589954 error-example-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-06-15 17:54:13.000000 error-example-0.0.3/README.txt
+-rw-rw-rw-   0        0        0      250 2023-06-17 15:03:39.000000 error-example-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-17 15:04:47.593463 error-example-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-17 15:04:47.561690 error-example-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-17 15:04:47.572242 error-example-0.0.3/src/error_example/
+-rw-rw-rw-   0        0        0       15 2023-06-15 17:52:48.000000 error-example-0.0.3/src/error_example/main.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:04:47.586562 error-example-0.0.3/src/error_example.egg-info/
+-rw-rw-rw-   0        0        0       98 2023-06-17 15:04:47.000000 error-example-0.0.3/src/error_example.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      215 2023-06-17 15:04:47.000000 error-example-0.0.3/src/error_example.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 15:04:47.000000 error-example-0.0.3/src/error_example.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-17 15:04:47.000000 error-example-0.0.3/src/error_example.egg-info/top_level.txt
```

