# Comparing `tmp/zhtools-0.3.1.tar.gz` & `tmp/zhtools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhtools-0.3.1.tar", last modified: Thu Jul 21 04:54:16 2022, max compression
+gzip compressed data, was "zhtools-1.0.0.tar", last modified: Sat Jun 17 08:26:00 2023, max compression
```

## Comparing `zhtools-0.3.1.tar` & `zhtools-1.0.0.tar`

### file list

```diff
@@ -1,72 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-07-21 04:54:09.000000 zhtools-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-07-21 04:54:16.819325 zhtools-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1969 2022-07-21 04:54:09.000000 zhtools-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-21 04:54:16.823325 zhtools-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-07-21 04:54:09.000000 zhtools-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.815325 zhtools-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:09.000000 zhtools-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-21 04:54:09.000000 zhtools-0.3.1/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.815325 zhtools-0.3.1/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:09.000000 zhtools-0.3.1/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-07-21 04:54:09.000000 zhtools-0.3.1/tests/readers/test_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-07-21 04:54:09.000000 zhtools-0.3.1/tests/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.815325 zhtools-0.3.1/tests/test_code_generator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:09.000000 zhtools-0.3.1/tests/test_code_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2726 2022-07-21 04:54:09.000000 zhtools-0.3.1/tests/test_code_generator/test_json2model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-07-21 04:54:09.000000 zhtools-0.3.1/tests/test_defer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2022-07-21 04:54:09.000000 zhtools-0.3.1/tests/test_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/
--rw-r--r--   0 runner    (1001) docker     (121)     2512 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6214 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/api_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/async_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/cache/
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3276 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/cache/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3071 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/cache/storages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2320 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/code_generator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/code_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/code_generator/json2model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/code_generator/orms/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/code_generator/orms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4261 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/code_generator/orms/generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/code_generator/orms/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/code_generator/orms/tortoise.py
--rw-r--r--   0 runner    (1001) docker     (121)     1984 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/concurrents.py
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1736 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/ctx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/data_structs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/data_structs/convertors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/data_structs/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/data_structs/lazy.py
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/exporters/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2690 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/exporters/xlsx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/io_tools/
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/io_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/io_tools/readers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/io_tools/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/io_tools/readers/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     2260 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/io_tools/readers/xlsx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/log.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/random.py
--rw-r--r--   0 runner    (1001) docker     (121)     2178 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/redis_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/security/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/security/aes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools/third_parties/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/third_parties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/third_parties/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/timetools.py
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-07-21 04:54:09.000000 zhtools-0.3.1/zhtools/type_hint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-21 04:54:16.819325 zhtools-0.3.1/zhtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2458 2022-07-21 04:54:16.000000 zhtools-0.3.1/zhtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-07-21 04:54:16.000000 zhtools-0.3.1/zhtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-21 04:54:16.000000 zhtools-0.3.1/zhtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       67 2022-07-21 04:54:16.000000 zhtools-0.3.1/zhtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-21 04:54:16.000000 zhtools-0.3.1/zhtools.egg-info/top_level.txt
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.258435 zhtools-1.0.0/
+-rw-r--r--   0 ziipin     (501) staff       (20)     1065 2023-06-17 07:25:35.000000 zhtools-1.0.0/LICENSE
+-rw-r--r--   0 ziipin     (501) staff       (20)     2723 2023-06-17 08:26:00.258180 zhtools-1.0.0/PKG-INFO
+-rw-r--r--   0 ziipin     (501) staff       (20)     2283 2023-06-17 07:54:00.000000 zhtools-1.0.0/README.md
+-rw-r--r--   0 ziipin     (501) staff       (20)      624 2023-06-17 08:25:02.000000 zhtools-1.0.0/pyproject.toml
+-rw-r--r--   0 ziipin     (501) staff       (20)       38 2023-06-17 08:26:00.258512 zhtools-1.0.0/setup.cfg
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.241637 zhtools-1.0.0/tests/
+-rw-r--r--   0 ziipin     (501) staff       (20)     2700 2023-06-17 07:28:23.000000 zhtools-1.0.0/tests/test_cache.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     2420 2023-06-17 07:26:17.000000 zhtools-1.0.0/tests/test_signals.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.250506 zhtools-1.0.0/zhtools/
+-rw-r--r--   0 ziipin     (501) staff       (20)        0 2023-06-16 06:56:33.000000 zhtools-1.0.0/zhtools/__init__.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     5246 2023-06-17 08:13:34.000000 zhtools-1.0.0/zhtools/api_service.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      751 2023-06-16 10:34:45.000000 zhtools-1.0.0/zhtools/async_tools.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.254127 zhtools-1.0.0/zhtools/cache/
+-rw-r--r--   0 ziipin     (501) staff       (20)      170 2023-06-17 07:28:23.000000 zhtools-1.0.0/zhtools/cache/__init__.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     3923 2023-06-17 07:29:27.000000 zhtools-1.0.0/zhtools/cache/decorators.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     3067 2023-06-17 07:24:39.000000 zhtools-1.0.0/zhtools/cache/storages.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      482 2023-06-16 09:43:15.000000 zhtools-1.0.0/zhtools/calculation.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     2011 2023-06-17 08:25:02.000000 zhtools-1.0.0/zhtools/cli.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     3694 2023-06-17 06:09:04.000000 zhtools-1.0.0/zhtools/concurrents.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1564 2023-06-17 07:24:39.000000 zhtools-1.0.0/zhtools/config.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      220 2023-06-16 09:35:06.000000 zhtools-1.0.0/zhtools/context_manager.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.256896 zhtools-1.0.0/zhtools/data_structs/
+-rw-r--r--   0 ziipin     (501) staff       (20)        0 2023-06-17 06:41:31.000000 zhtools-1.0.0/zhtools/data_structs/__init__.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     2159 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/data_structs/convertors.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      998 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/data_structs/dataclass.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      880 2023-06-17 06:36:44.000000 zhtools-1.0.0/zhtools/data_structs/enum.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1509 2023-06-17 07:00:08.000000 zhtools-1.0.0/zhtools/data_structs/pydantic.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1240 2023-06-17 03:38:24.000000 zhtools-1.0.0/zhtools/decorators.py
+-rw-r--r--   0 ziipin     (501) staff       (20)      380 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/exceptions.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1023 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/random.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.257722 zhtools-1.0.0/zhtools/security/
+-rw-r--r--   0 ziipin     (501) staff       (20)        0 2023-06-17 06:50:08.000000 zhtools-1.0.0/zhtools/security/__init__.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1439 2023-06-17 06:52:29.000000 zhtools-1.0.0/zhtools/security/aes.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     2060 2023-06-16 10:27:21.000000 zhtools-1.0.0/zhtools/signals.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     4903 2023-06-16 09:35:06.000000 zhtools-1.0.0/zhtools/timetools.py
+-rw-r--r--   0 ziipin     (501) staff       (20)     1042 2023-06-17 03:59:38.000000 zhtools-1.0.0/zhtools/typing.py
+drwxr-xr-x   0 ziipin     (501) staff       (20)        0 2023-06-17 08:26:00.252597 zhtools-1.0.0/zhtools.egg-info/
+-rw-r--r--   0 ziipin     (501) staff       (20)     2723 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/PKG-INFO
+-rw-r--r--   0 ziipin     (501) staff       (20)      851 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/SOURCES.txt
+-rw-r--r--   0 ziipin     (501) staff       (20)        1 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/dependency_links.txt
+-rw-r--r--   0 ziipin     (501) staff       (20)       37 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/entry_points.txt
+-rw-r--r--   0 ziipin     (501) staff       (20)       86 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/requires.txt
+-rw-r--r--   0 ziipin     (501) staff       (20)        8 2023-06-17 08:26:00.000000 zhtools-1.0.0/zhtools.egg-info/top_level.txt
```

### Comparing `zhtools-0.3.1/LICENSE` & `zhtools-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zhtools-0.3.1/PKG-INFO` & `zhtools-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 Metadata-Version: 2.1
 Name: zhtools
-Version: 0.3.1
-Summary: Some simple tool methods like cache, exporter and so on.
-Home-page: https://github.com/zhyipeng/zhtools
-Author: zhyipeng
-Author-email: zhyipeng@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
+Version: 1.0.0
+Summary: Some simple tool methods like cache, timetools and so on.
+Author-email: zhyipeng <zhyipeng@outlook.com>
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: httpx
+Provides-Extra: pydantic
+Provides-Extra: redis
+Provides-Extra: aioredis
 License-File: LICENSE
 
 # Zhtools
-Some simple tool methods like cache, exporter and so on.
+Some simple tool methods like cache, timetools and so on.
 
 
 ## Modules
 - cache: A simple cache decorator.
-- code_generator: 
-  - json2model: Generate pydantic model from json string.
-  - orms: Generate model code from create table sql.
-- exporters: Export data to a file like .xlsx and etc.
-- io_tools: Some io tool methods.
-  - readers: Simple method to read data from a file like .xlsx and etc.
 - data_structs: Some data structs implements and tools.
-- random: Uuid, random string and so on.
-- redis_helper: Some tools base on redis.
-- timetools: Some date/time/timezone tools.
-- type_hint: Common type hints.
+- security: some simple security methods.
 - api_service: Simple way to define an api client.
-- enum: More practical enum.
-- concurrents: Some tools for concurrent base on multi process/thread/coroutine.
-- ctx: Some context tools.
 - async_tools: about python async/await.
-- security: some simple security methods.
-- log: simple logging config tools.
+- calculation: Math calculation methods.
+- cli: Command-line tools.
+- concurrents: Some tools for concurrent base on multi process/thread/coroutine.
+- config: Global config by this tool.
+- context_manager: Common context manager.
+- decorators: Common decorators.
+- exceptions: Common exceptions by this tool.
+- random: Random methods.
 - signals: simple signal dispatcher.
-- \_\_init\_\_: Unclassified tools.
+- timetools: Some date/time/timezone tools.
+- typing: Common type hints.
 
 
 ## Update logs
+- **1.0.0** 2023-06-17:
+  - Refactored code to used more type hint. Now only support python 3.11+.
+  - Because of the ChatGPT, remove the `code_generator` module.
+  - Remove `data_structs.lazy` module, recommend to use `lazy-object-proxy` instead.
+  - Remove `exporters` module.
+  - Remove `io_tools` module.
+  - Remove `redis_helper` module.
+  - Remove `log` module.
+  - Move `enum` to `data_structs.enum`.
+  - Move `third_parties.pydantic` to `data_structs.pydantic`.
+  - Move `type_hint` to `typing`.
+  - Change `requests` and `aiohttp` requirement to `httpx`.
 - **0.3.0** 2022-07-21:
   - Refactored cache.
   - Add signal dispatcher.
 - **0.2.3** 2022-04-08: 
   - Fix & add cli command.
   - Add log module.
 - **0.2.2** 2022-01-08:
@@ -70,9 +76,7 @@
   - Add orm code generators.
 - **0.0.6** 2021-04-25:
   - Add enum module.
 - **0.0.5** 2021-04-19: 
   - Added api service.
   - Optimized the performance of XlsxReader.
   - Added progress bar to XlsxExporter (supported by [tqdm](https://github.com/tqdm/tqdm)).
-
-
```

### Comparing `zhtools-0.3.1/README.md` & `zhtools-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 # Zhtools
-Some simple tool methods like cache, exporter and so on.
+Some simple tool methods like cache, timetools and so on.
 
 
 ## Modules
 - cache: A simple cache decorator.
-- code_generator: 
-  - json2model: Generate pydantic model from json string.
-  - orms: Generate model code from create table sql.
-- exporters: Export data to a file like .xlsx and etc.
-- io_tools: Some io tool methods.
-  - readers: Simple method to read data from a file like .xlsx and etc.
 - data_structs: Some data structs implements and tools.
-- random: Uuid, random string and so on.
-- redis_helper: Some tools base on redis.
-- timetools: Some date/time/timezone tools.
-- type_hint: Common type hints.
+- security: some simple security methods.
 - api_service: Simple way to define an api client.
-- enum: More practical enum.
-- concurrents: Some tools for concurrent base on multi process/thread/coroutine.
-- ctx: Some context tools.
 - async_tools: about python async/await.
-- security: some simple security methods.
-- log: simple logging config tools.
+- calculation: Math calculation methods.
+- cli: Command-line tools.
+- concurrents: Some tools for concurrent base on multi process/thread/coroutine.
+- config: Global config by this tool.
+- context_manager: Common context manager.
+- decorators: Common decorators.
+- exceptions: Common exceptions by this tool.
+- random: Random methods.
 - signals: simple signal dispatcher.
-- \_\_init\_\_: Unclassified tools.
+- timetools: Some date/time/timezone tools.
+- typing: Common type hints.
 
 
 ## Update logs
+- **1.0.0** 2023-06-17:
+  - Refactored code to used more type hint. Now only support python 3.11+.
+  - Because of the ChatGPT, remove the `code_generator` module.
+  - Remove `data_structs.lazy` module, recommend to use `lazy-object-proxy` instead.
+  - Remove `exporters` module.
+  - Remove `io_tools` module.
+  - Remove `redis_helper` module.
+  - Remove `log` module.
+  - Move `enum` to `data_structs.enum`.
+  - Move `third_parties.pydantic` to `data_structs.pydantic`.
+  - Move `type_hint` to `typing`.
+  - Change `requests` and `aiohttp` requirement to `httpx`.
 - **0.3.0** 2022-07-21:
   - Refactored cache.
   - Add signal dispatcher.
 - **0.2.3** 2022-04-08: 
   - Fix & add cli command.
   - Add log module.
 - **0.2.2** 2022-01-08:
```

### Comparing `zhtools-0.3.1/tests/test_cache.py` & `zhtools-1.0.0/tests/test_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import time
 
-from zhtools.cache import Empty, MemoryStorage, cache, get_func_name
+from zhtools.cache import Empty, MemoryStorage, cache
+from zhtools.cache.decorators import get_func_name
 from zhtools.config import config
 
 
 def test_get_func_name():
     def func1():
         pass
```

### Comparing `zhtools-0.3.1/tests/test_signals.py` & `zhtools-1.0.0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `zhtools-0.3.1/zhtools/cache/decorators.py` & `zhtools-1.0.0/zhtools/cache/decorators.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,110 +1,125 @@
 import asyncio
 import functools
 import inspect
-from typing import Any, Callable
+from collections.abc import Callable
+from typing import Any, AnyStr, overload
 
 import wrapt
 
-from zhtools.cache.storages import Empty, MemoryStorage
 from zhtools.config import config
-from zhtools.type_hint import MakeCacheKeyFunc, Wrapped
+from zhtools.typing import (AsyncWrapped, AsyncWrapper, CommonWrapped,
+                            CommonWrapper, P)
+from .storages import Empty
 
-storage = MemoryStorage()
 
-
-def is_async(func: Wrapped):
+def _is_async(func: Callable):
     if isinstance(func, classmethod):
         func = func.__wrapped__
     return inspect.iscoroutinefunction(func)
 
 
-def get_func_name(func: Wrapped) -> str:
+MakeCacheKeyFunc = Callable[[CommonWrapped, P], AnyStr]
+
+
+def get_func_name(func: Callable) -> str:
     if inspect.isfunction(func) or inspect.ismethod(func):
         return func.__name__
     return func.__class__.__name__
 
 
-def make_cache_key(func: Wrapped, *args, **kwargs) -> str:
+def make_cache_key(func: CommonWrapped, *args, **kwargs) -> str:
     return f'{get_func_name(func)}:{(args, kwargs)}'
 
 
 class cache:
     """
-    common cache decorator.
-    >>> from zhtools.config import config
-    >>> from zhtools.cache import cache, MemoryStorage, RedisStorage
+    >>> from zhtools.cache.storages import RedisStorage
     >>> config.storage = RedisStorage()
     >>> @cache
-    >>> def foo():
-            ...
+    >>> def foo(a: int, b: int) -> int:
+    ...
+    >>> @cache(key=lambda a, b: f'{a}:{b}')
+    >>> def foo1(a: int, b: int) -> int:
+    ...
     """
 
     def __new__(cls,
-                func: Wrapped = None,
-                /,
-                key: MakeCacheKeyFunc = make_cache_key):
+                func: CommonWrapped = None,
+                *,
+                key: MakeCacheKeyFunc = make_cache_key,
+                expire: int = None):
         obj = super().__new__(cls)
         cls.__init__(obj, key=key)
-        if func is not None:
+        if func is not None and (callable(func) or isinstance(func, classmethod)):
             obj = obj.__call__(func)
+
         return obj
 
-    def __init__(self, key: MakeCacheKeyFunc = make_cache_key):
+    def __init__(self, *, key: MakeCacheKeyFunc = make_cache_key, expire: int = None):
         self.key = key
+        self.expire = expire or config.default_expire
 
-    def get_cache_key(self, func: Wrapped, instance: Any, args, kwargs) -> str:
+    def get_key(self, func: CommonWrapped, instance: Any, args: P.args, kwargs: P.kwargs) -> str:
         if instance is not None and not inspect.isclass(instance):
             return self.key(func, instance, *args, **kwargs)
         else:
             return self.key(func, *args, **kwargs)
 
     @wrapt.decorator
-    def wrapper(self, func: Wrapped, instance: Any, args, kwargs) -> Wrapped:
-        cache_key = self.get_cache_key(func, instance, args, kwargs)
-        cache_result = config.storage.get(cache_key)
+    def wrapper(self, func: CommonWrapped, instance: Any, args: P.args, kwargs: P.kwargs) -> CommonWrapper:
+        _key = self.get_key(func, instance, args, kwargs)
+        cache_result = config.storage.get(_key)
         if cache_result is not Empty:
             return cache_result
 
         result = func(*args, **kwargs)
-
-        config.storage.setex(cache_key, result, config.default_expire)
+        config.storage.setex(_key, result, self.expire)
         return result
 
     @wrapt.decorator
-    async def async_wrapper(self, func: Wrapped, instance: Any, args, kwargs) -> Wrapped:
-        cache_key = self.get_cache_key(func, instance, args, kwargs)
-        cache_result = await config.storage.get(cache_key)
+    async def async_wrapper(self,
+                            func: AsyncWrapped,
+                            instance: Any,
+                            args: P.args,
+                            kwargs: P.kwargs) -> AsyncWrapper:
+        _key = self.get_key(func, instance, args, kwargs)
+        cache_result = await config.storage.get(_key)
         if cache_result is not Empty:
             return cache_result
 
         result = await func(*args, **kwargs)
-
-        asyncio.create_task(
-            config.storage.setex(cache_key, result, config.default_expire)
-        )
+        asyncio.create_task(config.storage.setex(_key, result, self.expire))
         return result
 
-    def __call__(self, func: Wrapped):
-        if is_async(func):
+    @overload
+    def __call__(self, func: AsyncWrapped) -> AsyncWrapper:
+        ...
+
+    def __call__(self, func: CommonWrapped) -> CommonWrapper:
+        if _is_async(func):
             return self.async_wrapper(func)
         return self.wrapper(func)
 
 
 class cond_lru_cache:
     """use functools.lru_cache when use_cache return True"""
 
     def __init__(self,
-                 use_cache: Callable[[...], bool],
+                 use_cache: Callable[P, bool],
                  maxsize: int = 128,
                  typed: bool = False):
         self.use_cache = use_cache
         self.maxsize = maxsize
         self.typed = typed
 
     @wrapt.decorator
-    def __call__(self, func, instance, args, kwargs):
+    def __call__(self,
+                 func: CommonWrapped,
+                 instance: Any,
+                 args: P.args,
+                 kwargs: P.kwargs) -> CommonWrapper:
         deco_func = functools.lru_cache(self.maxsize, self.typed)(func)
         if self.use_cache(*args, **kwargs):
             return deco_func(*args, **kwargs)
 
         return func(*args, **kwargs)
```

### Comparing `zhtools-0.3.1/zhtools/cache/storages.py` & `zhtools-1.0.0/zhtools/cache/storages.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,92 @@
 import abc
 import logging
 import pickle
 import time
 import typing
-from typing import Any
 
 if typing.TYPE_CHECKING:
     from redis import Redis
     from aioredis import Redis as AsyncRedis
 
+
+T = typing.TypeVar('T')
+
 Empty = object()
 
 
-class Storage(metaclass=abc.ABCMeta):
+class Storage(typing.Generic[T], metaclass=abc.ABCMeta):
 
     @abc.abstractmethod
-    def get(self, key: str) -> Any:
+    def get(self, key: str) -> T:
         pass
 
-    def set(self, key: str, value: Any):
+    def set(self, key: str, value: T):
         self.setex(key, value, float('inf'))
 
     @abc.abstractmethod
-    def setex(self, key: str, value: Any, expire: float):
+    def setex(self, key: str, value: T, expire: float):
         pass
 
 
 class AsyncStorage(Storage, metaclass=abc.ABCMeta):
 
     @abc.abstractmethod
-    async def get(self, key: str) -> Any:
+    async def get(self, key: str) -> T:
         pass
 
-    async def set(self, key: str, value: Any):
+    async def set(self, key: str, value: T):
         await self.setex(key, value, float('inf'))
 
     @abc.abstractmethod
-    async def setex(self, key: str, value: Any, expire: float):
+    async def setex(self, key: str, value: T, expire: float):
         pass
 
 
 class MemoryStorage(Storage):
 
     def __init__(self):
-        self.data: dict[str, tuple[Any, float]] = {}
+        self.data: dict[str, tuple[T, float]] = {}
 
-    def get(self, key: str) -> Any:
+    def get(self, key: str) -> T:
         val, expire = self.data.get(key, (Empty, 0))
         if val is Empty:
             return val
 
         if expire < time.time():
             del self.data[key]
             return Empty
         return val
 
-    def setex(self, key: str, value: Any, expire: float):
+    def setex(self, key: str, value: T, expire: float):
         if expire is None:
             expire = float('inf')
         expire_at = time.time() + expire
         self.data[key] = (value, expire_at)
 
 
 class RedisStorage(Storage):
 
     def __init__(self, redis_cli: 'Redis'):
         self.redis_cli = redis_cli
 
-    def get(self, key: str) -> Any:
+    def get(self, key: str) -> T:
         ret = self.redis_cli.get(key)
         if ret is None:
             return Empty
 
         if isinstance(ret, bytes):
             try:
                 ret = pickle.loads(ret)
             except pickle.UnpicklingError:
                 pass
 
         return ret
 
-    def setex(self, key: str, value: Any, expire: float):
+    def setex(self, key: str, value: T, expire: float):
         try:
             value = pickle.dumps(value)
         except pickle.PickleError:
             logging.error(f'cache value {value} can not pickle.')
             return
 
         if expire is None or expire == float('inf'):
@@ -94,28 +96,28 @@
 
 
 class AsyncRedisStorage(AsyncStorage):
 
     def __init__(self, redis_cli: 'AsyncRedis'):
         self.redis_cli = redis_cli
 
-    async def get(self, key: str) -> Any:
+    async def get(self, key: str) -> T:
         ret = await self.redis_cli.get(key)
         if ret is None:
             return Empty
 
         if isinstance(ret, bytes):
             try:
                 ret = pickle.loads(ret)
             except pickle.UnpicklingError:
                 pass
 
         return ret
 
-    async def setex(self, key: str, value: Any, expire: float):
+    async def setex(self, key: str, value: T, expire: float):
         try:
             value = pickle.dumps(value)
         except pickle.PickleError:
             logging.error(f'cache value {value} can not pickle.')
             return
 
         if expire is None or expire == float('inf'):
```

### Comparing `zhtools-0.3.1/zhtools/cli.py` & `zhtools-1.0.0/zhtools/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,13 @@
 import os.path
 import string
 import sys
 from pathlib import Path
 from typing import Optional
 
-from zhtools.code_generator.orms import tortoise_orm, sqlalchemy_orm
-
-
-ormers = {
-    'tortoise': tortoise_orm,
-    'sqlalchemy': sqlalchemy_orm,
-}
-
-
-def orm(sql: str, mode: str = 'sqlalchemy'):
-    """create table sql to orm model code."""
-    assert mode in ormers, f'mode is only in ({", ".join(ormers.keys())})'
-    ormers[mode](sql)
-
 
 def sort_requirements(requirements: str, newline: str = None):
     p = Path(requirements)
     if not p.is_absolute():
         p = Path.cwd() / Path(requirements)
 
     items = []
@@ -72,15 +58,14 @@
     for cmd, func in commands.items():
         print(cmd.ljust(10, ' ') + func.__doc__)
 
 
 commands = {
     '-h': help_info,
     '--help': help_info,
-    'orm': orm,
     'i': install,
     'install': install,
 }
 
 
 def execute_from_command_line(argv: Optional[list[str]] = None) -> None:
     if not argv:
@@ -96,9 +81,13 @@
             cmd(*argv[2:])
         else:
             cmd()
     except KeyboardInterrupt:
         pass
 
 
+def main():
+    execute_from_command_line()
+
+
 if __name__ == '__main__':
     execute_from_command_line()
```

### Comparing `zhtools-0.3.1/zhtools/data_structs/convertors.py` & `zhtools-1.0.0/zhtools/data_structs/convertors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
-from typing import Any
+from typing import TypeVar
+
 
 def underline_to_camel_case(v: str) -> str:
     return v.replace('_', ' ').title().replace(' ', '')
 
 
 def underline_to_small_camel_case(v: str) -> str:
     v = underline_to_camel_case(v)
@@ -58,12 +59,31 @@
 
     for k in d:
         if isinstance(d[k], defaultdict):
             d[k] = deconstruct_defaultdict(d[k])
     return d
 
 
-def transpose_dict(data: dict) -> dict[Any, set]:
+K = TypeVar('K')
+V = TypeVar('V')
+
+
+def transpose_dict(data: dict[K, V]) -> dict[V, set[K]]:
     ret = defaultdict(set)
     for k, v in data.items():
         ret[v].add(k)
     return dict(ret)
+
+
+T = TypeVar('T')
+
+
+def group_by_key(data: list[T], key: str) -> dict[str, list[T]]:
+    ret = defaultdict(list)
+    for item in data:
+        if isinstance(item, dict):
+            k = item[key]
+        else:
+            k = getattr(item, key)
+        ret[k].append(item)
+
+    return dict(ret)
```

### Comparing `zhtools-0.3.1/zhtools/data_structs/dataclass.py` & `zhtools-1.0.0/zhtools/data_structs/dataclass.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,18 +30,7 @@
                     new_obj = field_type(**value)
                     kwargs[name] = new_obj
             original_init(self, *args, **kwargs)
 
         cls.__init__ = __init__
         return cls
     return wrapper(args[0]) if args else wrapper
-
-
-if __name__ == '__main__':
-    @dataclass
-    class A:
-        m: int
-    @dataclass
-    class B:
-        a: A
-
-    print(B(a={'m': 1}))
```

### Comparing `zhtools-0.3.1/zhtools/security/aes.py` & `zhtools-1.0.0/zhtools/security/aes.py`

 * *Files identical despite different names*

### Comparing `zhtools-0.3.1/zhtools/third_parties/pydantic.py` & `zhtools-1.0.0/zhtools/data_structs/pydantic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import builtins
-import logging
 import typing
 
+from zhtools.config import config
 from zhtools.exceptions import ModuleRequired
 
-if typing.TYPE_CHECKING:
-    from pydantic import BaseModel
+try:
+    from pydantic import BaseModel, fields
+except ImportError:
+    raise ModuleRequired('pydantic')
 
 
-def make_default_model(model: typing.Type['BaseModel']) -> 'BaseModel':
-    try:
-        from pydantic import fields
-    except ImportError:
-        raise ModuleRequired('')
+T = typing.TypeVar('T', bound=BaseModel)
 
+
+def make_default_model(model: typing.Type[T]) -> T:
     attrs = {}
     for k, v in model.__fields__.items():
         if v.default:
             attrs[k] = v.get_default()
             continue
 
         match v.shape:
@@ -42,10 +42,10 @@
                     case builtins.int | builtins.float:
                         attrs[k] = 0
                     case builtins.str:
                         attrs[k] = ''
                     case builtins.bool:
                         attrs[k] = False
                     case _:
-                        logging.warning('unsupport type: %s-%s', k, v.type_)
+                        config.log_warning(f'unsupport type: {k}-{v.type_}')
 
     return model(**attrs)
```

### Comparing `zhtools-0.3.1/zhtools.egg-info/PKG-INFO` & `zhtools-1.0.0/zhtools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,58 @@
 Metadata-Version: 2.1
 Name: zhtools
-Version: 0.3.1
-Summary: Some simple tool methods like cache, exporter and so on.
-Home-page: https://github.com/zhyipeng/zhtools
-Author: zhyipeng
-Author-email: zhyipeng@outlook.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
+Version: 1.0.0
+Summary: Some simple tool methods like cache, timetools and so on.
+Author-email: zhyipeng <zhyipeng@outlook.com>
+Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Provides-Extra: httpx
+Provides-Extra: pydantic
+Provides-Extra: redis
+Provides-Extra: aioredis
 License-File: LICENSE
 
 # Zhtools
-Some simple tool methods like cache, exporter and so on.
+Some simple tool methods like cache, timetools and so on.
 
 
 ## Modules
 - cache: A simple cache decorator.
-- code_generator: 
-  - json2model: Generate pydantic model from json string.
-  - orms: Generate model code from create table sql.
-- exporters: Export data to a file like .xlsx and etc.
-- io_tools: Some io tool methods.
-  - readers: Simple method to read data from a file like .xlsx and etc.
 - data_structs: Some data structs implements and tools.
-- random: Uuid, random string and so on.
-- redis_helper: Some tools base on redis.
-- timetools: Some date/time/timezone tools.
-- type_hint: Common type hints.
+- security: some simple security methods.
 - api_service: Simple way to define an api client.
-- enum: More practical enum.
-- concurrents: Some tools for concurrent base on multi process/thread/coroutine.
-- ctx: Some context tools.
 - async_tools: about python async/await.
-- security: some simple security methods.
-- log: simple logging config tools.
+- calculation: Math calculation methods.
+- cli: Command-line tools.
+- concurrents: Some tools for concurrent base on multi process/thread/coroutine.
+- config: Global config by this tool.
+- context_manager: Common context manager.
+- decorators: Common decorators.
+- exceptions: Common exceptions by this tool.
+- random: Random methods.
 - signals: simple signal dispatcher.
-- \_\_init\_\_: Unclassified tools.
+- timetools: Some date/time/timezone tools.
+- typing: Common type hints.
 
 
 ## Update logs
+- **1.0.0** 2023-06-17:
+  - Refactored code to used more type hint. Now only support python 3.11+.
+  - Because of the ChatGPT, remove the `code_generator` module.
+  - Remove `data_structs.lazy` module, recommend to use `lazy-object-proxy` instead.
+  - Remove `exporters` module.
+  - Remove `io_tools` module.
+  - Remove `redis_helper` module.
+  - Remove `log` module.
+  - Move `enum` to `data_structs.enum`.
+  - Move `third_parties.pydantic` to `data_structs.pydantic`.
+  - Move `type_hint` to `typing`.
+  - Change `requests` and `aiohttp` requirement to `httpx`.
 - **0.3.0** 2022-07-21:
   - Refactored cache.
   - Add signal dispatcher.
 - **0.2.3** 2022-04-08: 
   - Fix & add cli command.
   - Add log module.
 - **0.2.2** 2022-01-08:
@@ -70,9 +76,7 @@
   - Add orm code generators.
 - **0.0.6** 2021-04-25:
   - Add enum module.
 - **0.0.5** 2021-04-19: 
   - Added api service.
   - Optimized the performance of XlsxReader.
   - Added progress bar to XlsxExporter (supported by [tqdm](https://github.com/tqdm/tqdm)).
-
-
```

