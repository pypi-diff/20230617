# Comparing `tmp/kaxi-0.1.0.tar.gz` & `tmp/kaxi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaxi-0.1.0.tar", max compression
+gzip compressed data, was "kaxi-0.1.1.tar", max compression
```

## Comparing `kaxi-0.1.0.tar` & `kaxi-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        6 2023-06-17 02:15:27.801508 kaxi-0.1.0/README.md
--rw-r--r--   0        0        0       74 2023-06-17 02:14:17.955100 kaxi-0.1.0/kaxi/__init__.py
--rw-r--r--   0        0        0      807 2023-06-17 02:14:19.910175 kaxi-0.1.0/kaxi/log.py
--rw-r--r--   0        0        0      282 2023-06-17 01:50:25.535522 kaxi-0.1.0/kaxi/main.py
--rw-r--r--   0        0        0     3666 2023-06-17 02:14:19.938326 kaxi-0.1.0/kaxi/runner.py
--rw-r--r--   0        0        0     1264 2023-06-17 02:20:26.460166 kaxi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 kaxi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-17 03:12:52.103273 kaxi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2190 2023-06-17 03:12:52.103273 kaxi-0.1.1/README.md
+-rw-r--r--   0        0        0       74 2023-06-17 03:12:52.103273 kaxi-0.1.1/kaxi/__init__.py
+-rw-r--r--   0        0        0      807 2023-06-17 03:12:52.103273 kaxi-0.1.1/kaxi/log.py
+-rw-r--r--   0        0        0      282 2023-06-17 03:12:52.103273 kaxi-0.1.1/kaxi/main.py
+-rw-r--r--   0        0        0     3666 2023-06-17 03:12:52.103273 kaxi-0.1.1/kaxi/runner.py
+-rw-r--r--   0        0        0     1334 2023-06-17 03:12:52.103273 kaxi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2963 1970-01-01 00:00:00.000000 kaxi-0.1.1/PKG-INFO
```

### Comparing `kaxi-0.1.0/kaxi/log.py` & `kaxi-0.1.1/kaxi/log.py`

 * *Files identical despite different names*

### Comparing `kaxi-0.1.0/kaxi/runner.py` & `kaxi-0.1.1/kaxi/runner.py`

 * *Files identical despite different names*

### Comparing `kaxi-0.1.0/pyproject.toml` & `kaxi-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 [tool.poetry]
 name = "kaxi"
-version = "0.1.0"
+version = "0.1.1"
 description = "Run pipelines similar to github actions"
 authors = ["Gabriel Guarisa <gabrielguarisa@gmail.com>"]
 readme = "README.md"
+license = "MIT"
+repository = "https://github.com/gabrielguarisa/kaxi"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyyaml = "^6.0"
 typer = "^0.9.0"
 colorlog = "^6.7.0"
```

