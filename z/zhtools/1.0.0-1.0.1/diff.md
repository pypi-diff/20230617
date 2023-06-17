# Comparing `tmp/zhtools-1.0.0.tar.gz` & `tmp/zhtools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhtools-1.0.0.tar", last modified: Sat Jun 17 08:26:00 2023, max compression
+gzip compressed data, was "zhtools-1.0.1.tar", last modified: Sat Jun 17 09:29:04 2023, max compression
```

## Comparing `zhtools-1.0.0.tar` & `zhtools-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.258435 zhtools-1.0.0/
--rw-r--r--   0 ziipin     (501) staff       (20)     1065 2023-06-17 07:25:35.000000 zhtools-1.0.0/LICENSE
--rw-r--r--   0 ziipin     (501) staff       (20)     2723 2023-06-17 08:26:00.258180 zhtools-1.0.0/PKG-INFO
--rw-r--r--   0 ziipin     (501) staff       (20)     2283 2023-06-17 07:54:00.000000 zhtools-1.0.0/README.md
--rw-r--r--   0 ziipin     (501) staff       (20)      624 2023-06-17 08:25:02.000000 zhtools-1.0.0/pyproject.toml
--rw-r--r--   0 ziipin     (501) staff       (20)       38 2023-06-17 08:26:00.258512 zhtools-1.0.0/setup.cfg
-drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.241637 zhtools-1.0.0/tests/
--rw-r--r--   0 ziipin     (501) staff       (20)     2700 2023-06-17 07:28:23.000000 zhtools-1.0.0/tests/test_cache.py
--rw-r--r--   0 ziipin     (501) staff       (20)     2420 2023-06-17 07:26:17.000000 zhtools-1.0.0/tests/test_signals.py
-drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.250506 zhtools-1.0.0/zhtools/
--rw-r--r--   0 ziipin     (501) staff       (20)        0 2023-06-16 06:56:33.000000 zhtools-1.0.0/zhtools/__init__.py
--rw-r--r--   0 ziipin     (501) staff       (20)     5246 2023-06-17 08:13:34.000000 zhtools-1.0.0/zhtools/api_service.py
--rw-r--r--   0 ziipin     (501) staff       (20)      751 2023-06-16 10:34:45.000000 zhtools-1.0.0/zhtools/async_tools.py
-drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.254127 zhtools-1.0.0/zhtools/cache/
--rw-r--r--   0 ziipin     (501) staff       (20)      170 2023-06-17 07:28:23.000000 zhtools-1.0.0/zhtools/cache/__init__.py
--rw-r--r--   0 ziipin     (501) staff       (20)     3923 2023-06-17 07:29:27.000000 zhtools-1.0.0/zhtools/cache/decorators.py
--rw-r--r--   0 ziipin     (501) staff       (20)     3067 2023-06-17 07:24:39.000000 zhtools-1.0.0/zhtools/cache/storages.py
--rw-r--r--   0 ziipin     (501) staff       (20)      482 2023-06-16 09:43:15.000000 zhtools-1.0.0/zhtools/calculation.py
--rw-r--r--   0 ziipin     (501) staff       (20)     2011 2023-06-17 08:25:02.000000 zhtools-1.0.0/zhtools/cli.py
--rw-r--r--   0 ziipin     (501) staff       (20)     3694 2023-06-17 06:09:04.000000 zhtools-1.0.0/zhtools/concurrents.py
--rw-r--r--   0 ziipin     (501) staff       (20)     1564 2023-06-17 07:24:39.000000 zhtools-1.0.0/zhtools/config.py
--rw-r--r--   0 ziipin     (501) staff       (20)      220 2023-06-16 09:35:06.000000 zhtools-1.0.0/zhtools/context_manager.py
-drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.256896 zhtools-1.0.0/zhtools/data_structs/
--rw-r--r--   0 ziipin     (501) staff       (20)        0 2023-06-17 06:41:31.000000 zhtools-1.0.0/zhtools/data_structs/__init__.py
--rw-r--r--   0 ziipin     (501) staff       (20)     2159 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/data_structs/convertors.py
--rw-r--r--   0 ziipin     (501) staff       (20)      998 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/data_structs/dataclass.py
--rw-r--r--   0 ziipin     (501) staff       (20)      880 2023-06-17 06:36:44.000000 zhtools-1.0.0/zhtools/data_structs/enum.py
--rw-r--r--   0 ziipin     (501) staff       (20)     1509 2023-06-17 07:00:08.000000 zhtools-1.0.0/zhtools/data_structs/pydantic.py
--rw-r--r--   0 ziipin     (501) staff       (20)     1240 2023-06-17 03:38:24.000000 zhtools-1.0.0/zhtools/decorators.py
--rw-r--r--   0 ziipin     (501) staff       (20)      380 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/exceptions.py
--rw-r--r--   0 ziipin     (501) staff       (20)     1023 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/random.py
-drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.257722 zhtools-1.0.0/zhtools/security/
--rw-r--r--   0 ziipin     (501) staff       (20)        0 2023-06-17 06:50:08.000000 zhtools-1.0.0/zhtools/security/__init__.py
--rw-r--r--   0 ziipin     (501) staff       (20)     1439 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/security/aes.py
--rw-r--r--   0 ziipin     (501) staff       (20)     2060 2023-06-16 10:27:21.000000 zhtools-1.0.0/zhtools/signals.py
--rw-r--r--   0 ziipin     (501) staff       (20)     4903 2023-06-16 09:35:06.000000 zhtools-1.0.0/zhtools/timetools.py
--rw-r--r--   0 ziipin     (501) staff       (20)     1042 2023-06-17 03:59:38.000000 zhtools-1.0.0/zhtools/typing.py
-drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.252597 zhtools-1.0.0/zhtools.egg-info/
--rw-r--r--   0 ziipin     (501) staff       (20)     2723 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/PKG-INFO
--rw-r--r--   0 ziipin     (501) staff       (20)      851 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/SOURCES.txt
--rw-r--r--   0 ziipin     (501) staff       (20)        1 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/dependency_links.txt
--rw-r--r--   0 ziipin     (501) staff       (20)       37 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/entry_points.txt
--rw-r--r--   0 ziipin     (501) staff       (20)       86 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/requires.txt
--rw-r--r--   0 ziipin     (501) staff       (20)        8 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/top_level.txt
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 09:29:04.627127 zhtools-1.0.1/
+-rw-r--r--   0 ziipin     (501) staff       (20)     1065 2023-06-17 07:25:35.000000 zhtools-1.0.1/LICENSE
+-rw-r--r--   0 ziipin     (501) staff       (20)     2723 2023-06-17 09:29:04.626876 zhtools-1.0.1/PKG-INFO
+-rw-r--r--   0 ziipin     (501) staff       (20)     2283 2023-06-17 07:54:00.000000 zhtools-1.0.1/README.md
+-rw-r--r--   0 ziipin     (501) staff       (20)      624 2023-06-17 09:28:56.000000 zhtools-1.0.1/pyproject.toml
+-rw-r--r--   0 ziipin     (501) staff       (20)       38 2023-06-17 09:29:04.627227 zhtools-1.0.1/setup.cfg
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 09:29:04.612928 zhtools-1.0.1/tests/
+-rw-r--r--   0 ziipin     (501) staff       (20)     2700 2023-06-17 07:28:23.000000 zhtools-1.0.1/tests/test_cache.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     2420 2023-06-17 07:26:17.000000 zhtools-1.0.1/tests/test_signals.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 09:29:04.620917 zhtools-1.0.1/zhtools/
+-rw-r--r--   0 ziipin     (501) staff       (20)        0 2023-06-16 06:56:33.000000 zhtools-1.0.1/zhtools/__init__.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     5246 2023-06-17 08:13:34.000000 zhtools-1.0.1/zhtools/api_service.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      751 2023-06-16 10:34:45.000000 zhtools-1.0.1/zhtools/async_tools.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 09:29:04.623955 zhtools-1.0.1/zhtools/cache/
+-rw-r--r--   0 ziipin     (501) staff       (20)      170 2023-06-17 07:28:23.000000 zhtools-1.0.1/zhtools/cache/__init__.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     3923 2023-06-17 07:29:27.000000 zhtools-1.0.1/zhtools/cache/decorators.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     3067 2023-06-17 07:24:39.000000 zhtools-1.0.1/zhtools/cache/storages.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      482 2023-06-16 09:43:15.000000 zhtools-1.0.1/zhtools/calculation.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     2011 2023-06-17 08:25:02.000000 zhtools-1.0.1/zhtools/cli.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     3694 2023-06-17 06:09:04.000000 zhtools-1.0.1/zhtools/concurrents.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1564 2023-06-17 07:24:39.000000 zhtools-1.0.1/zhtools/config.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      220 2023-06-16 09:35:06.000000 zhtools-1.0.1/zhtools/context_manager.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 09:29:04.625708 zhtools-1.0.1/zhtools/data_structs/
+-rw-r--r--   0 ziipin     (501) staff       (20)        0 2023-06-17 06:41:31.000000 zhtools-1.0.1/zhtools/data_structs/__init__.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     2159 2023-06-17 06:52:29.000000 zhtools-1.0.1/zhtools/data_structs/convertors.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      998 2023-06-17 06:52:29.000000 zhtools-1.0.1/zhtools/data_structs/dataclass.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1640 2023-06-17 09:23:26.000000 zhtools-1.0.1/zhtools/data_structs/enum.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1509 2023-06-17 07:00:08.000000 zhtools-1.0.1/zhtools/data_structs/pydantic.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1240 2023-06-17 03:38:24.000000 zhtools-1.0.1/zhtools/decorators.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      380 2023-06-17 06:52:29.000000 zhtools-1.0.1/zhtools/exceptions.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1023 2023-06-17 06:52:29.000000 zhtools-1.0.1/zhtools/random.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 09:29:04.626489 zhtools-1.0.1/zhtools/security/
+-rw-r--r--   0 ziipin     (501) staff       (20)        0 2023-06-17 06:50:08.000000 zhtools-1.0.1/zhtools/security/__init__.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1439 2023-06-17 06:52:29.000000 zhtools-1.0.1/zhtools/security/aes.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     2060 2023-06-16 10:27:21.000000 zhtools-1.0.1/zhtools/signals.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     4903 2023-06-16 09:35:06.000000 zhtools-1.0.1/zhtools/timetools.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1042 2023-06-17 03:59:38.000000 zhtools-1.0.1/zhtools/typing.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 09:29:04.622753 zhtools-1.0.1/zhtools.egg-info/
+-rw-r--r--   0 ziipin     (501) staff       (20)     2723 2023-06-17 09:29:04.000000 zhtools-1.0.1/zhtools.egg-info/PKG-INFO
+-rw-r--r--   0 ziipin     (501) staff       (20)      851 2023-06-17 09:29:04.000000 zhtools-1.0.1/zhtools.egg-info/SOURCES.txt
+-rw-r--r--   0 ziipin     (501) staff       (20)        1 2023-06-17 09:29:04.000000 zhtools-1.0.1/zhtools.egg-info/dependency_links.txt
+-rw-r--r--   0 ziipin     (501) staff       (20)       37 2023-06-17 09:29:04.000000 zhtools-1.0.1/zhtools.egg-info/entry_points.txt
+-rw-r--r--   0 ziipin     (501) staff       (20)       86 2023-06-17 09:29:04.000000 zhtools-1.0.1/zhtools.egg-info/requires.txt
+-rw-r--r--   0 ziipin     (501) staff       (20)        8 2023-06-17 09:29:04.000000 zhtools-1.0.1/zhtools.egg-info/top_level.txt
```

### Comparing `zhtools-1.0.0/LICENSE` & `zhtools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/PKG-INFO` & `zhtools-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhtools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Some simple tool methods like cache, timetools and so on.
 Author-email: zhyipeng <zhyipeng@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: httpx
```

### Comparing `zhtools-1.0.0/README.md` & `zhtools-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/pyproject.toml` & `zhtools-1.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zhtools"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="zhyipeng", email="zhyipeng@outlook.com" },
 ]
 description = "Some simple tool methods like cache, timetools and so on."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `zhtools-1.0.0/tests/test_cache.py` & `zhtools-1.0.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/tests/test_signals.py` & `zhtools-1.0.1/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/api_service.py` & `zhtools-1.0.1/zhtools/api_service.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/async_tools.py` & `zhtools-1.0.1/zhtools/async_tools.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/cache/decorators.py` & `zhtools-1.0.1/zhtools/cache/decorators.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/cache/storages.py` & `zhtools-1.0.1/zhtools/cache/storages.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/cli.py` & `zhtools-1.0.1/zhtools/cli.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/concurrents.py` & `zhtools-1.0.1/zhtools/concurrents.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/config.py` & `zhtools-1.0.1/zhtools/config.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/data_structs/convertors.py` & `zhtools-1.0.1/zhtools/data_structs/convertors.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/data_structs/dataclass.py` & `zhtools-1.0.1/zhtools/data_structs/dataclass.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/data_structs/pydantic.py` & `zhtools-1.0.1/zhtools/data_structs/pydantic.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/decorators.py` & `zhtools-1.0.1/zhtools/decorators.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/random.py` & `zhtools-1.0.1/zhtools/random.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/security/aes.py` & `zhtools-1.0.1/zhtools/security/aes.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/signals.py` & `zhtools-1.0.1/zhtools/signals.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/timetools.py` & `zhtools-1.0.1/zhtools/timetools.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools/typing.py` & `zhtools-1.0.1/zhtools/typing.py`

 * *Files identical despite different names*

### Comparing `zhtools-1.0.0/zhtools.egg-info/PKG-INFO` & `zhtools-1.0.1/zhtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhtools
-Version: 1.0.0
+Version: 1.0.1
 Summary: Some simple tool methods like cache, timetools and so on.
 Author-email: zhyipeng <zhyipeng@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: httpx
```

### Comparing `zhtools-1.0.0/zhtools.egg-info/SOURCES.txt` & `zhtools-1.0.1/zhtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

