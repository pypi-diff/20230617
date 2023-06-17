# Comparing `tmp/callbackin-0.1.0.tar.gz` & `tmp/callbackin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callbackin-0.1.0.tar", max compression
+gzip compressed data, was "callbackin-0.2.0.tar", max compression
```

## Comparing `callbackin-0.1.0.tar` & `callbackin-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2023-06-17 10:49:27.040450 callbackin-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-17 10:49:27.040416 callbackin-0.1.0/callbackin/__init__.py
--rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.1.0/callbackin/__main__.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.1.0/callbackin/handler/__init__.py
--rw-r--r--   0        0        0      186 2023-06-17 10:59:07.385500 callbackin-0.1.0/callbackin/handler/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3811 2023-06-17 11:10:35.718296 callbackin-0.1.0/callbackin/handler/__pycache__/callback.cpython-311.pyc
--rw-r--r--   0        0        0     4190 2023-06-17 10:59:07.804434 callbackin-0.1.0/callbackin/handler/__pycache__/login.cpython-311.pyc
--rw-r--r--   0        0        0     2029 2023-06-17 11:10:29.612392 callbackin-0.1.0/callbackin/handler/callback.py
--rw-r--r--   0        0        0     1895 2023-06-17 10:58:12.979780 callbackin-0.1.0/callbackin/handler/login.py
--rw-r--r--   0        0        0     4750 2023-06-17 11:27:39.911051 callbackin-0.1.0/callbackin/main.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.1.0/callbackin/schemas/__init__.py
--rw-r--r--   0        0        0      186 2023-06-17 10:59:07.414431 callbackin-0.1.0/callbackin/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      775 2023-06-17 10:59:07.414882 callbackin-0.1.0/callbackin/schemas/__pycache__/callback.cpython-311.pyc
--rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.1.0/callbackin/schemas/callback.py
--rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.1.0/callbackin/utils/__init__.py
--rw-r--r--   0        0        0      184 2023-06-17 10:59:07.808986 callbackin-0.1.0/callbackin/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2563 2023-06-17 11:10:35.734748 callbackin-0.1.0/callbackin/utils/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     2608 2023-06-17 11:32:05.763460 callbackin-0.1.0/callbackin/utils/__pycache__/request.cpython-311.pyc
--rw-r--r--   0        0        0     1322 2023-06-17 11:08:57.376439 callbackin-0.1.0/callbackin/utils/config.py
--rw-r--r--   0        0        0     1493 2023-06-17 11:32:01.695647 callbackin-0.1.0/callbackin/utils/request.py
--rw-r--r--   0        0        0      440 2023-06-17 11:23:38.528337 callbackin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 callbackin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-06-17 11:36:46.832824 callbackin-0.2.0/README.md
+-rw-r--r--   0        0        0       21 2023-06-17 11:37:22.884692 callbackin-0.2.0/callbackin/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-17 11:29:59.539358 callbackin-0.2.0/callbackin/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.295912 callbackin-0.2.0/callbackin/handler/__init__.py
+-rw-r--r--   0        0        0      186 2023-06-17 10:59:07.385500 callbackin-0.2.0/callbackin/handler/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3811 2023-06-17 11:10:35.718296 callbackin-0.2.0/callbackin/handler/__pycache__/callback.cpython-311.pyc
+-rw-r--r--   0        0        0     4190 2023-06-17 10:59:07.804434 callbackin-0.2.0/callbackin/handler/__pycache__/login.cpython-311.pyc
+-rw-r--r--   0        0        0     2029 2023-06-17 11:10:29.612392 callbackin-0.2.0/callbackin/handler/callback.py
+-rw-r--r--   0        0        0     1895 2023-06-17 10:58:12.979780 callbackin-0.2.0/callbackin/handler/login.py
+-rw-r--r--   0        0        0     4750 2023-06-17 11:27:39.911051 callbackin-0.2.0/callbackin/main.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.286706 callbackin-0.2.0/callbackin/schemas/__init__.py
+-rw-r--r--   0        0        0      186 2023-06-17 10:59:07.414431 callbackin-0.2.0/callbackin/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      775 2023-06-17 10:59:07.414882 callbackin-0.2.0/callbackin/schemas/__pycache__/callback.cpython-311.pyc
+-rw-r--r--   0        0        0      210 2023-06-17 10:51:29.288644 callbackin-0.2.0/callbackin/schemas/callback.py
+-rw-r--r--   0        0        0        0 2023-06-17 10:51:29.261151 callbackin-0.2.0/callbackin/utils/__init__.py
+-rw-r--r--   0        0        0      184 2023-06-17 10:59:07.808986 callbackin-0.2.0/callbackin/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2563 2023-06-17 11:10:35.734748 callbackin-0.2.0/callbackin/utils/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     2608 2023-06-17 11:32:05.763460 callbackin-0.2.0/callbackin/utils/__pycache__/request.cpython-311.pyc
+-rw-r--r--   0        0        0     1322 2023-06-17 11:08:57.376439 callbackin-0.2.0/callbackin/utils/config.py
+-rw-r--r--   0        0        0     1493 2023-06-17 11:32:01.695647 callbackin-0.2.0/callbackin/utils/request.py
+-rw-r--r--   0        0        0      440 2023-06-17 11:36:55.966211 callbackin-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 callbackin-0.2.0/PKG-INFO
```

### Comparing `callbackin-0.1.0/callbackin/handler/__pycache__/callback.cpython-311.pyc` & `callbackin-0.2.0/callbackin/handler/__pycache__/callback.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `callbackin-0.1.0/callbackin/handler/__pycache__/login.cpython-311.pyc` & `callbackin-0.2.0/callbackin/handler/__pycache__/login.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `callbackin-0.1.0/callbackin/handler/callback.py` & `callbackin-0.2.0/callbackin/handler/callback.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.1.0/callbackin/handler/login.py` & `callbackin-0.2.0/callbackin/handler/login.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.1.0/callbackin/main.py` & `callbackin-0.2.0/callbackin/main.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.1.0/callbackin/schemas/__pycache__/callback.cpython-311.pyc` & `callbackin-0.2.0/callbackin/schemas/__pycache__/callback.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `callbackin-0.1.0/callbackin/utils/__pycache__/config.cpython-311.pyc` & `callbackin-0.2.0/callbackin/utils/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `callbackin-0.1.0/callbackin/utils/__pycache__/request.cpython-311.pyc` & `callbackin-0.2.0/callbackin/utils/__pycache__/request.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `callbackin-0.1.0/callbackin/utils/config.py` & `callbackin-0.2.0/callbackin/utils/config.py`

 * *Files identical despite different names*

### Comparing `callbackin-0.1.0/callbackin/utils/request.py` & `callbackin-0.2.0/callbackin/utils/request.py`

 * *Files identical despite different names*

