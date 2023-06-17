# Comparing `tmp/mlbi_at_dku_lib-0.1.7.tar.gz` & `tmp/mlbi_at_dku_lib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlbi_at_dku_lib-0.1.7.tar", last modified: Thu Jun 15 08:57:00 2023, max compression
+gzip compressed data, was "mlbi_at_dku_lib-0.1.8.tar", last modified: Sat Jun 17 08:47:21 2023, max compression
```

## Comparing `mlbi_at_dku_lib-0.1.7.tar` & `mlbi_at_dku_lib-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.7/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.7/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.7/README.md
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     9385 2023-06-12 09:03:17.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/cpdb.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/misc.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/not-zip-safe
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-15 08:57:00.000000 mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/top_level.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-15 08:56:42.000000 mlbi_at_dku_lib-0.1.7/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-15 08:57:00.805514 mlbi_at_dku_lib-0.1.7/tests/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.7/tests/__init__.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-17 08:47:21.485413 mlbi_at_dku_lib-0.1.8/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.8/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       60 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.8/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-17 08:47:21.485413 mlbi_at_dku_lib-0.1.8/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-05-23 01:43:50.000000 mlbi_at_dku_lib-0.1.8/README.md
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-17 08:47:21.453413 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    17825 2023-06-17 08:33:06.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/cpdb.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6012 2023-06-15 08:56:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30883 2023-05-23 01:44:36.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    37323 2023-06-15 04:24:26.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/misc.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-17 08:47:21.473413 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      832 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      447 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-06-08 06:54:08.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/not-zip-safe
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       27 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       22 2023-06-17 08:47:21.000000 mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/top_level.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       79 2023-06-17 08:47:21.485413 mlbi_at_dku_lib-0.1.8/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     2823 2023-06-17 08:47:14.000000 mlbi_at_dku_lib-0.1.8/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-06-17 08:47:21.473413 mlbi_at_dku_lib-0.1.8/tests/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      124 2023-05-22 09:19:00.000000 mlbi_at_dku_lib-0.1.8/tests/__init__.py
```

### Comparing `mlbi_at_dku_lib-0.1.7/LICENSE` & `mlbi_at_dku_lib-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.7/PKG-INFO` & `mlbi_at_dku_lib-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi_at_dku_lib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/deiso.py` & `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/deiso.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/gsea.py` & `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/gsea.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/icnv.py` & `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/icnv.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib/misc.py` & `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib/misc.py`

 * *Files identical despite different names*

### Comparing `mlbi_at_dku_lib-0.1.7/mlbi_at_dku_lib.egg-info/PKG-INFO` & `mlbi_at_dku_lib-0.1.8/mlbi_at_dku_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlbi-at-dku-lib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Home-page: https://github.com/combio-dku
 Download-URL: https://github.com/combio-dku
 Author: Seokhyun Yoon
 Author-email: syoon@dku.edu
 Keywords: pypi mlbi_at_dku_lib
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mlbi_at_dku_lib-0.1.7/setup.py` & `mlbi_at_dku_lib-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     # 배포할 패키지의 이름을 적어줍니다. setup.py파일을 가지는 폴더 이름과 동일하게 합니다.
     name                = 'mlbi_at_dku_lib',
     # 배포할 패키지의 버전을 적어줍니다. 첫 등록이므로 0.1 또는 0.0.1을 사용합니다.
-    version             = '0.1.7',
+    version             = '0.1.8',
     # 배포할 패키지에 대한 설명을 작성합니다.
     description         = 'Toolkits for single-cell RNA-Seq data analysis. (Wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)',
     # 배포하는 사람의 이름을 작성합니다.
     author              = 'Seokhyun Yoon',
     # 배포하는 사람의 메일주소를 작성합니다.
     author_email        = 'syoon@dku.edu',
     # 배포하는 패키지의 url을 적어줍니다. 보통 github 링크를 적습니다.
```

