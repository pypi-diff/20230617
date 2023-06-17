# Comparing `tmp/ohlcv-plus-2.0.0.tar.gz` & `tmp/ohlcv-plus-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohlcv-plus-2.0.0.tar", last modified: Sat Jun 17 17:22:09 2023, max compression
+gzip compressed data, was "ohlcv-plus-2.0.1.tar", last modified: Sat Jun 17 17:26:01 2023, max compression
```

## Comparing `ohlcv-plus-2.0.0.tar` & `ohlcv-plus-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-17 17:22:09.184724 ohlcv-plus-2.0.0/
--rwxrwxrwx   0 root         (0) root         (0)     1062 2023-06-17 04:52:02.000000 ohlcv-plus-2.0.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      267 2023-06-17 17:22:09.184779 ohlcv-plus-2.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1324 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-17 17:22:09.183579 ohlcv-plus-2.0.0/ohlcv/
--rwxrwxrwx   0 root         (0) root         (0)       34 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.0/ohlcv/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    14681 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.0/ohlcv/ohlcv.py
--rwxrwxrwx   0 root         (0) root         (0)     1649 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.0/ohlcv/utils.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-17 17:22:09.184559 ohlcv-plus-2.0.0/ohlcv_plus.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      267 2023-06-17 17:22:09.000000 ohlcv-plus-2.0.0/ohlcv_plus.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      253 2023-06-17 17:22:09.000000 ohlcv-plus-2.0.0/ohlcv_plus.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-17 17:22:09.000000 ohlcv-plus-2.0.0/ohlcv_plus.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       32 2023-06-17 17:22:09.000000 ohlcv-plus-2.0.0/ohlcv_plus.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-17 17:22:09.000000 ohlcv-plus-2.0.0/ohlcv_plus.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-06-17 17:22:09.185048 ohlcv-plus-2.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      393 2023-06-17 17:20:57.000000 ohlcv-plus-2.0.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-17 17:26:01.121529 ohlcv-plus-2.0.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1062 2023-06-17 04:52:02.000000 ohlcv-plus-2.0.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     1633 2023-06-17 17:26:01.121594 ohlcv-plus-2.0.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1324 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-17 17:26:01.120355 ohlcv-plus-2.0.1/ohlcv/
+-rwxrwxrwx   0 root         (0) root         (0)       34 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.1/ohlcv/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    14681 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.1/ohlcv/ohlcv.py
+-rwxrwxrwx   0 root         (0) root         (0)     1649 2023-06-17 17:17:29.000000 ohlcv-plus-2.0.1/ohlcv/utils.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-17 17:26:01.121363 ohlcv-plus-2.0.1/ohlcv_plus.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1633 2023-06-17 17:26:01.000000 ohlcv-plus-2.0.1/ohlcv_plus.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      253 2023-06-17 17:26:01.000000 ohlcv-plus-2.0.1/ohlcv_plus.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-06-17 17:26:01.000000 ohlcv-plus-2.0.1/ohlcv_plus.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       32 2023-06-17 17:26:01.000000 ohlcv-plus-2.0.1/ohlcv_plus.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        6 2023-06-17 17:26:01.000000 ohlcv-plus-2.0.1/ohlcv_plus.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-06-17 17:26:01.121863 ohlcv-plus-2.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      614 2023-06-17 17:25:59.000000 ohlcv-plus-2.0.1/setup.py
```

### Comparing `ohlcv-plus-2.0.0/LICENSE` & `ohlcv-plus-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ohlcv-plus-2.0.0/README.md` & `ohlcv-plus-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ohlcv-plus-2.0.0/ohlcv/ohlcv.py` & `ohlcv-plus-2.0.1/ohlcv/ohlcv.py`

 * *Files identical despite different names*

### Comparing `ohlcv-plus-2.0.0/ohlcv/utils.py` & `ohlcv-plus-2.0.1/ohlcv/utils.py`

 * *Files identical despite different names*

