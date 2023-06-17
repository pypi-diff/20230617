# Comparing `tmp/mathtranslate-2.4.2.tar.gz` & `tmp/mathtranslate-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.4.2.tar", last modified: Wed Jun 14 20:30:52 2023, max compression
+gzip compressed data, was "mathtranslate-2.4.3.tar", last modified: Sat Jun 17 03:55:32 2023, max compression
```

## Comparing `mathtranslate-2.4.2.tar` & `mathtranslate-2.4.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.730088 mathtranslate-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17250 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 20:30:52.726087 mathtranslate-2.4.2/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-14 20:30:52.000000 mathtranslate-2.4.2/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 20:30:52.730088 mathtranslate-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-14 20:30:34.000000 mathtranslate-2.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17256 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5047 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 03:55:32.000000 mathtranslate-2.4.3/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 03:55:32.443421 mathtranslate-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-17 03:55:18.000000 mathtranslate-2.4.3/setup.py
```

### Comparing `mathtranslate-2.4.2/LICENSE` & `mathtranslate-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/PKG-INFO` & `mathtranslate-2.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.4.2
+Version: 2.4.3
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.2 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.3 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.4.2/README.md` & `mathtranslate-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/cache.py` & `mathtranslate-2.4.3/mathtranslate/cache.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/config.py` & `mathtranslate-2.4.3/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/encoding.py` & `mathtranslate-2.4.3/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/process_file.py` & `mathtranslate-2.4.3/mathtranslate/process_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     '''
     path_tex = f'{tex}.tex'
     path_bbl = f'{tex}.bbl'
     encoding = get_file_encoding(path_tex)
     content = open(path_tex, encoding=encoding).read()
     encoding = get_file_encoding(path_bbl)
     bbl = open(path_bbl, encoding=encoding).read()
-    pattern_input = re.compile(r'\\bibliography\{(.*?)\}', re.DOTALL)
-    while True:
-        result = pattern_input.search(content)
-        if result is None:
-            break
-        begin, end = result.span()
-        content = content[:begin] + bbl + content[end:]
-    print(content, file=open(path_tex, "w", encoding='utf-8'))
+    patterns = [r'\\bibliography\{(.*?)\}', r'\\thebibliography\{(.*?)\}']
+    for pattern in patterns:
+        pattern_input = re.compile(pattern, re.DOTALL)
+        while True:
+            result = pattern_input.search(content)
+            if result is None:
+                break
+            begin, end = result.span()
+            content = content[:begin] + bbl + content[end:]
+        print(content, file=open(path_tex, "w", encoding='utf-8'))
```

### Comparing `mathtranslate-2.4.2/mathtranslate/process_latex.py` & `mathtranslate-2.4.3/mathtranslate/process_latex.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 math_code = config.math_code
 test_environment = config.test_environment
 
 match_code = r"(" + math_code + r"_\d+(?:_\d+)*)"
 match_code_replace = math_code + r"_(\d+(?:_\d+)*)*"
 
 #options = r"\[[a-zA-Z\s,\\\*\.\+\-=_{}\(\)\!]*?\]"  # ,\*.+-=_{}!
-options = r"\[.*?\]"
+options = r"\[[^\[\]]*?\]"
 spaces = r"[ \t]*"
 
 get_pattern_brace = lambda index: rf"\{{((?:[^{{}}]++|(?{index}))*+)\}}"
 get_pattern_env = lambda name: rf"\\begin{spaces}\{{({name})\}}{spaces}({options})?(.*?)\\end{spaces}\{{\1\}}"
 
 
 def get_pattern_command_full(name, n=None):
```

### Comparing `mathtranslate-2.4.2/mathtranslate/process_text.py` & `mathtranslate-2.4.3/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencent.py` & `mathtranslate-2.4.3/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-2.4.3/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/translate.py` & `mathtranslate-2.4.3/mathtranslate/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,26 +186,27 @@
                 print('Cache is found')
             cache.create_cache(hash_key)
 
         self.nbad = 0
         self.ntotal = 0
 
         latex_original = process_latex.remove_tex_comments(latex_original)
+        latex_original = latex_original.replace(r'\mathbf', r'\boldsymbol')
         latex_original = process_latex.process_newcommands(latex_original)
 
         latex_original = process_latex.replace_accent(latex_original)
         latex_original = process_latex.replace_special(latex_original)
 
         self.complete = process_latex.is_complete(latex_original)
         self.theorems = process_latex.get_theorems(latex_original)
         if self.complete:
             print('It is a full latex document')
             latex_original, tex_begin, tex_end = process_latex.split_latex_document(latex_original, r'\begin{document}', r'\end{document}')
             tex_begin = process_latex.remove_blank_lines(tex_begin)
-            tex_begin = process_latex.insert_macro(tex_begin, r'\usepackage{xeCJK}')
+            tex_begin = process_latex.insert_macro(tex_begin, '\\usepackage{xeCJK}\n\\usepackage{amsmath}')
         else:
             print('It is not a full latex document')
             latex_original = process_text.connect_paragraphs(latex_original)
             if make_complete:
                 tex_begin = default_begin
                 tex_end = default_end
             else:
```

### Comparing `mathtranslate-2.4.2/mathtranslate/translate_arxiv.py` & `mathtranslate-2.4.3/mathtranslate/translate_arxiv.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/translate_tex.py` & `mathtranslate-2.4.3/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/upload_overleaf.py` & `mathtranslate-2.4.3/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate/utils.py` & `mathtranslate-2.4.3/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.4.3/mathtranslate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.4.2
+Version: 2.4.3
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.2 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.4.3 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.4.2/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-2.4.3/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.4.2/setup.py` & `mathtranslate-2.4.3/setup.py`

 * *Files identical despite different names*

