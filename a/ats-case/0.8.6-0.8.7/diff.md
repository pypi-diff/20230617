# Comparing `tmp/ats_case-0.8.6.tar.gz` & `tmp/ats_case-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.8.6.tar", last modified: Sat Jun 17 05:25:54 2023, max compression
+gzip compressed data, was "ats_case-0.8.7.tar", last modified: Sat Jun 17 06:14:57 2023, max compression
```

## Comparing `ats_case-0.8.6.tar` & `ats_case-0.8.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 05:25:54.280900 ats_case-0.8.6/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.6/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-06-17 05:25:54.278930 ats_case-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 05:25:53.851727 ats_case-0.8.6/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.6/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:25:54.084826 ats_case-0.8.6/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.6/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18831 2023-06-14 05:51:39.000000 ats_case-0.8.6/ats_case/case/command.py
--rw-rw-rw-   0        0        0    11904 2023-06-17 05:24:59.000000 ats_case-0.8.6/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7505 2023-06-15 02:18:37.000000 ats_case-0.8.6/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.6/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:25:54.160627 ats_case-0.8.6/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.6/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.6/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.6/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:25:54.230061 ats_case-0.8.6/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.6/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.6/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.8.6/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-06-17 05:25:54.268933 ats_case-0.8.6/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.6/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.6/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-06-17 05:25:53.955145 ats_case-0.8.6/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-06-17 05:25:53.000000 ats_case-0.8.6/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-06-17 05:25:53.000000 ats_case-0.8.6/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 05:25:53.000000 ats_case-0.8.6/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-17 05:25:53.000000 ats_case-0.8.6/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-17 05:25:53.000000 ats_case-0.8.6/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 05:25:54.280900 ats_case-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-06-17 05:25:46.000000 ats_case-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.637641 ats_case-0.8.7/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.7/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-06-17 06:14:57.631662 ats_case-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.146163 ats_case-0.8.7/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.7/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.353406 ats_case-0.8.7/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.7/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18831 2023-06-14 05:51:39.000000 ats_case-0.8.7/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    12042 2023-06-17 06:14:22.000000 ats_case-0.8.7/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7505 2023-06-15 02:18:37.000000 ats_case-0.8.7/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.7/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.453134 ats_case-0.8.7/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.7/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.7/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.7/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.526937 ats_case-0.8.7/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.7/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.7/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     4039 2023-06-16 06:59:03.000000 ats_case-0.8.7/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.585785 ats_case-0.8.7/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.7/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.7/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-06-17 06:14:57.238956 ats_case-0.8.7/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-17 06:14:56.000000 ats_case-0.8.7/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 06:14:57.638646 ats_case-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-06-17 06:14:44.000000 ats_case-0.8.7/setup.py
```

### Comparing `ats_case-0.8.6/PKG-INFO` & `ats_case-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.8.6
+Version: 0.8.7
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.6/README.md` & `ats_case-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.6/ats_case/case/command.py` & `ats_case-0.8.7/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.6/ats_case/case/context.py` & `ats_case-0.8.7/ats_case/case/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,16 +133,18 @@
             self._steps = data.get('steps', {})
 
             if self._code is not None:
                 self._name = '{}_{}'.format(self._name, self._code)
             if self._version is not None:
                 self._name = '{}_{}'.format(self._name, self._version)
             if isinstance(self._control, str):
+                self._control = self._control.replace('null', 'None')
                 self._control = eval(self._control)
             if isinstance(self._steps, str):
+                self._steps = self._steps.replace('null', 'None')
                 self._steps = eval(self._steps)
 
         #         self._script = 'script.{}'.format(data.get('script'))
         #         self._bench_step_orders = data.get('bench_step_orders', [])
         #         # 用户发起的参数
         #         self._req_params = self.ReqParams(data.get('req_params'))
         #
```

### Comparing `ats_case-0.8.6/ats_case/case/executor.py` & `ats_case-0.8.7/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.6/ats_case/case/translator.py` & `ats_case-0.8.7/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.6/ats_case/common/error.py` & `ats_case-0.8.7/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.6/ats_case/manage/core.py` & `ats_case-0.8.7/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.6/ats_case/manage/start.py` & `ats_case-0.8.7/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.6/ats_case/template/testcase_v1.tmp` & `ats_case-0.8.7/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.6/ats_case.egg-info/PKG-INFO` & `ats_case-0.8.7/ats_case.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.8.6
+Version: 0.8.7
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.6/ats_case.egg-info/SOURCES.txt` & `ats_case-0.8.7/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.6/setup.py` & `ats_case-0.8.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.8.6",
+    version="0.8.7",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

