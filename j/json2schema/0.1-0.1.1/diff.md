# Comparing `tmp/json2schema-0.1.tar.gz` & `tmp/json2schema-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json2schema-0.1.tar", last modified: Thu Nov  5 02:13:31 2020, max compression
+gzip compressed data, was "json2schema-0.1.1.tar", last modified: Sat Jun 17 13:41:19 2023, max compression
```

## Comparing `json2schema-0.1.tar` & `json2schema-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2020-11-05 02:13:31.000000 json2schema-0.1/
--rw-r--r--   0 superhin   (502) staff       (20)     1068 2020-06-12 08:53:02.000000 json2schema-0.1/LICENSE
--rw-r--r--   0 superhin   (502) staff       (20)      137 2020-06-12 08:53:02.000000 json2schema-0.1/MANIFEST.in
--rw-r--r--   0 superhin   (502) staff       (20)      826 2020-11-05 02:13:31.000000 json2schema-0.1/PKG-INFO
--rw-r--r--   0 superhin   (502) staff       (20)      169 2020-11-05 02:11:57.000000 json2schema-0.1/README.md
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2020-11-05 02:13:31.000000 json2schema-0.1/json2schema/
--rw-r--r--   0 superhin   (502) staff       (20)     2936 2020-11-05 02:06:59.000000 json2schema-0.1/json2schema/__init__.py
-drwxr-xr-x   0 superhin   (502) staff       (20)        0 2020-11-05 02:13:31.000000 json2schema-0.1/json2schema.egg-info/
--rw-r--r--   0 superhin   (502) staff       (20)      826 2020-11-05 02:13:31.000000 json2schema-0.1/json2schema.egg-info/PKG-INFO
--rw-r--r--   0 superhin   (502) staff       (20)      232 2020-11-05 02:13:31.000000 json2schema-0.1/json2schema.egg-info/SOURCES.txt
--rw-r--r--   0 superhin   (502) staff       (20)        1 2020-11-05 02:13:31.000000 json2schema-0.1/json2schema.egg-info/dependency_links.txt
--rw-r--r--   0 superhin   (502) staff       (20)       12 2020-11-05 02:13:31.000000 json2schema-0.1/json2schema.egg-info/top_level.txt
--rw-r--r--   0 superhin   (502) staff       (20)        1 2020-11-05 02:13:31.000000 json2schema-0.1/json2schema.egg-info/zip-safe
--rw-r--r--   0 superhin   (502) staff       (20)       38 2020-11-05 02:13:31.000000 json2schema-0.1/setup.cfg
--rw-r--r--   0 superhin   (502) staff       (20)     1135 2020-11-05 02:13:09.000000 json2schema-0.1/setup.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-17 13:41:19.052372 json2schema-0.1.1/
+-rw-r--r--   0 superhin   (502) staff       (20)     1068 2023-06-15 10:18:31.000000 json2schema-0.1.1/LICENSE
+-rw-r--r--   0 superhin   (502) staff       (20)      137 2023-06-15 10:18:31.000000 json2schema-0.1.1/MANIFEST.in
+-rw-r--r--   0 superhin   (502) staff       (20)     4788 2023-06-17 13:41:19.052071 json2schema-0.1.1/PKG-INFO
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-17 13:41:19.048712 json2schema-0.1.1/json2schema/
+-rw-r--r--   0 superhin   (502) staff       (20)      240 2023-06-17 13:20:39.000000 json2schema-0.1.1/json2schema/__init__.py
+-rw-r--r--   0 superhin   (502) staff       (20)     3431 2023-06-17 13:32:13.000000 json2schema-0.1.1/json2schema/json2schema.py
+-rw-r--r--   0 superhin   (502) staff       (20)     1270 2023-06-17 13:18:28.000000 json2schema-0.1.1/json2schema/schema2list.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-17 13:41:19.050925 json2schema-0.1.1/json2schema.egg-info/
+-rw-r--r--   0 superhin   (502) staff       (20)     4788 2023-06-17 13:41:18.000000 json2schema-0.1.1/json2schema.egg-info/PKG-INFO
+-rw-r--r--   0 superhin   (502) staff       (20)      319 2023-06-17 13:41:19.000000 json2schema-0.1.1/json2schema.egg-info/SOURCES.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-17 13:41:18.000000 json2schema-0.1.1/json2schema.egg-info/dependency_links.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       12 2023-06-17 13:41:18.000000 json2schema-0.1.1/json2schema.egg-info/top_level.txt
+-rw-r--r--   0 superhin   (502) staff       (20)        1 2023-06-15 10:19:33.000000 json2schema-0.1.1/json2schema.egg-info/zip-safe
+-rw-r--r--   0 superhin   (502) staff       (20)       17 2023-06-15 10:23:41.000000 json2schema-0.1.1/requriements.txt
+-rw-r--r--   0 superhin   (502) staff       (20)       38 2023-06-17 13:41:19.052493 json2schema-0.1.1/setup.cfg
+-rw-r--r--   0 superhin   (502) staff       (20)     1344 2023-06-17 13:41:04.000000 json2schema-0.1.1/setup.py
+drwxr-xr-x   0 superhin   (502) staff       (20)        0 2023-06-17 13:41:19.051406 json2schema-0.1.1/tests/
+-rw-r--r--   0 superhin   (502) staff       (20)     2717 2023-06-17 13:34:36.000000 json2schema-0.1.1/tests/test_json2schema.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `json2schema-0.1/LICENSE` & `json2schema-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `json2schema-0.1/setup.py` & `json2schema-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """The setup script."""
 import os
+
 from setuptools import setup, find_packages
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
+
+version = '0.1.1'
 setup_requirements = []
+install_requires = []
+tests_require = ['jsonschema', 'pytest']
+extra_require = {'dev': tests_require + ['twine']}
 
 
 def read_file(filename):
     with open(os.path.join(this_directory, filename), encoding='utf-8') as f:
         long_description = f.read()
     return long_description
 
 
 setup(
+    name='json2schema',
+    version=version,
     author="Han Zhichao",
     author_email='superhin@126.com',
     description='JSON to JSONSchema',
-    long_description=read_file('README.md'),
+    license="MIT license",
+    long_description=read_file('tests/README.md'),
     long_description_content_type="text/markdown",  # 新参数
+    url='https://github.com/hanzhichao/json2schema',
+    keywords=['json2schema', 'jsonschema', 'json to jsonschema'],
+
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.7',
     ],
-    license="MIT license",
     include_package_data=True,
-    keywords=[
-        'json2schema', 'jsonschema', 'json to jsonschema',
-    ],
-    name='json2schema',
+    zip_safe=True,
     packages=find_packages(include=['json2schema']),
+
     setup_requires=setup_requirements,
-    url='https://github.com/hanzhichao/json2schema',
-    version='0.01',
-    zip_safe=True,
-    install_requires=[]
+    install_requires=install_requires,
+    tests_require=tests_require,
+    extra_require=extra_require,
 )
```

