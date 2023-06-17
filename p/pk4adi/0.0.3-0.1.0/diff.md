# Comparing `tmp/pk4adi-0.0.3.tar.gz` & `tmp/pk4adi-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pk4adi-0.0.3.tar", last modified: Tue Jun 13 13:29:29 2023, max compression
+gzip compressed data, was "pk4adi-0.1.0.tar", last modified: Sat Jun 17 07:24:33 2023, max compression
```

## Comparing `pk4adi-0.0.3.tar` & `pk4adi-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 13:29:29.844149 pk4adi-0.0.3/
--rw-rw-rw-   0        0        0     1088 2023-01-04 20:12:34.000000 pk4adi-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2112 2023-06-13 13:29:29.843648 pk4adi-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1366 2023-06-13 13:27:59.000000 pk4adi-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 13:29:29.822147 pk4adi-0.0.3/pk4adi/
--rw-rw-rw-   0        0        0      463 2023-06-13 13:09:09.000000 pk4adi-0.0.3/pk4adi/__init__.py
--rw-rw-rw-   0        0        0    12910 2023-06-13 13:09:09.000000 pk4adi-0.0.3/pk4adi/pk.py
--rw-rw-rw-   0        0        0     1727 2023-06-13 13:09:09.000000 pk4adi-0.0.3/pk4adi/pk_error_cn.py
--rw-rw-rw-   0        0        0     3506 2023-06-13 13:09:09.000000 pk4adi-0.0.3/pk4adi/pkc.py
-drwxrwxrwx   0        0        0        0 2023-06-13 13:29:29.843157 pk4adi-0.0.3/pk4adi.egg-info/
--rw-rw-rw-   0        0        0     2112 2023-06-13 13:29:29.000000 pk4adi-0.0.3/pk4adi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-13 13:29:29.000000 pk4adi-0.0.3/pk4adi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 13:29:29.000000 pk4adi-0.0.3/pk4adi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-06-13 13:29:29.000000 pk4adi-0.0.3/pk4adi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-13 13:29:29.000000 pk4adi-0.0.3/pk4adi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 13:29:29.844149 pk4adi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1756 2023-01-18 13:14:12.000000 pk4adi-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:24:33.214684 pk4adi-0.1.0/
+-rw-rw-rw-   0        0        0     1088 2023-01-04 20:12:34.000000 pk4adi-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7471 2023-06-17 07:24:33.213150 pk4adi-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6551 2023-06-17 07:17:09.000000 pk4adi-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 07:24:33.179894 pk4adi-0.1.0/pk4adi/
+-rw-rw-rw-   0        0        0      458 2023-06-16 10:10:12.000000 pk4adi-0.1.0/pk4adi/__init__.py
+-rw-rw-rw-   0        0        0     9771 2023-06-17 06:56:44.000000 pk4adi-0.1.0/pk4adi/pk.py
+-rw-rw-rw-   0        0        0     7997 2023-06-17 06:56:08.000000 pk4adi-0.1.0/pk4adi/pkc.py
+-rw-rw-rw-   0        0        0     1143 2023-06-17 06:56:55.000000 pk4adi-0.1.0/pk4adi/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-17 07:24:33.211672 pk4adi-0.1.0/pk4adi.egg-info/
+-rw-rw-rw-   0        0        0     7471 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-17 07:24:33.000000 pk4adi-0.1.0/pk4adi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 07:24:33.214684 pk4adi-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2017 2023-06-17 07:14:57.000000 pk4adi-0.1.0/setup.py
```

### Comparing `pk4adi-0.0.3/LICENSE` & `pk4adi-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pk4adi-0.0.3/setup.py` & `pk4adi-0.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,18 @@
-#   -*- coding:utf-8 -*-
-#   The setup.py in pk
-#   created by Jiang Feng(silencejiang@zju.edu.cn)
-#   created at 20:52 on 2023/1/18
+#!/usr/bin/env python
+# -*- encoding: utf-8 -*-
+"""
+@File    :   setup.py
+@Contact :   Jiang Feng(silencejiang@zju.edu.cn)
+@License :   (C)Copyright 2004-2020, Zhejiang University
+
+@Modify Time        @Author       @Version    @Desciption
+------------        -------       --------    -----------
+2023/6/13 16:20   silencejiang      0.1.0         None
+"""
 
 
 import os
 import re
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
@@ -14,27 +21,28 @@
 __version__ = re.sub(
     r".*\b__version__\s+=\s+'([^']+)'.*",
     r'\1',
     [line.strip() for line in version_file if '__version__' in line].pop(0)
 )
 version_file.close()
 
-short_description = """Using PK to Measure the Performance of Anesthetic Depth
- Indicators."""
+short_description = """Using PK to Measure the Performance of Anesthetic Depth Indicators."""
 
 try:
     long_description = open('README.md', encoding="utf-8").read(),
 except IOError:
     long_description = "See README.md where installed."
 
 
 def get_install_requires():
     reqs = [
         'pandas>=0.18.0',
-        'numpy>=1.9.2'
+        'numpy>=1.21.6',
+        'scipy>=1.9.0',
+        'tabulate'
     ]
     return reqs
 
 
 setup(
     name="pk4adi",
     version=__version__,
@@ -45,17 +53,17 @@
     long_description_content_type="text/markdown",
     long_description=long_description,
     python_requires=">=3.8",
     install_requires=get_install_requires(),
     packages=find_packages(),
     license='MIT License',
     classifiers=[
-         'License :: OSI Approved :: MIT License',
+        'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     package_data={'': ['*.csv', '*.txt', '.toml']},
-    include_package_data=True  # 也选上
+    include_package_data=True
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

