# Comparing `tmp/pydatawork-0.0.4.tar.gz` & `tmp/pydatawork-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydatawork-0.0.4.tar", last modified: Sat Jun 17 09:33:41 2023, max compression
+gzip compressed data, was "dist/pydatawork-0.0.5.tar", last modified: Sat Jun 17 10:14:10 2023, max compression
```

## Comparing `pydatawork-0.0.4.tar` & `pydatawork-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 09:33:41.000000 pydatawork-0.0.4/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      744 2023-06-17 09:33:41.000000 pydatawork-0.0.4/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      196 2023-06-17 09:33:33.000000 pydatawork-0.0.4/README.md
-drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      744 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/PKG-INFO
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/SOURCES.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/dependency_links.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-17 09:33:41.000000 pydatawork-0.0.4/pydatawork.egg-info/top_level.txt
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1052 2023-06-15 10:29:59.000000 pydatawork-0.0.4/pydatawork.py
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-17 09:33:41.000000 pydatawork-0.0.4/setup.cfg
--rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-17 09:32:30.000000 pydatawork-0.0.4/setup.py
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 10:14:10.000000 pydatawork-0.0.5/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      744 2023-06-17 10:14:10.000000 pydatawork-0.0.5/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      196 2023-06-17 09:33:33.000000 pydatawork-0.0.5/README.md
+drwxrwxr-x   0 jkzhou    (1000) jkzhou    (1000)        0 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      744 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/PKG-INFO
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      168 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/SOURCES.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)        1 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/dependency_links.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       11 2023-06-17 10:14:10.000000 pydatawork-0.0.5/pydatawork.egg-info/top_level.txt
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)     1056 2023-06-17 10:13:17.000000 pydatawork-0.0.5/pydatawork.py
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)       38 2023-06-17 10:14:10.000000 pydatawork-0.0.5/setup.cfg
+-rw-rw-r--   0 jkzhou    (1000) jkzhou    (1000)      793 2023-06-17 10:13:32.000000 pydatawork-0.0.5/setup.py
```

### Comparing `pydatawork-0.0.4/PKG-INFO` & `pydatawork-0.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.4
+Version: 0.0.5
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description:
```

### Comparing `pydatawork-0.0.4/pydatawork.egg-info/PKG-INFO` & `pydatawork-0.0.5/pydatawork.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatawork
-Version: 0.0.4
+Version: 0.0.5
 Summary: jk.zhou's datawork
 Home-page: https://github.com/jkjoker/datawork
 Author: jk.zhou
 Author-email: zhouqiling.bjfu@foxmail.com
 License: MIT
 Description:
```

### Comparing `pydatawork-0.0.4/pydatawork.py` & `pydatawork-0.0.5/pydatawork.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 
 
 
+
+
 def break_words(stuff):
     """This function will break up words for us."""
     words = stuff.split(' ')
     return words
 
 def sort_words(words):
     """Sorts the words.""" # 文档字符串，是注释的一种
@@ -33,7 +35,9 @@
 
 def print_first_and_last_sorted(sentence):
     """Sorts the words then prints the first and last one."""
     words = sort_sentence(sentence)
     print_first_word(words)
     print_last_word(words)
     
+
+
```

### Comparing `pydatawork-0.0.4/setup.py` & `pydatawork-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pydatawork',
-    version='0.0.4',
+    version='0.0.5',
     py_modules=['pydatawork'],
     author='jk.zhou',
     author_email='zhouqiling.bjfu@foxmail.com',
     description="jk.zhou's datawork",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

