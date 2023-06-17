# Comparing `tmp/git2doc-0.1.8.tar.gz` & `tmp/git2doc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2doc-0.1.8.tar", last modified: Sat Jun 17 19:59:45 2023, max compression
+gzip compressed data, was "git2doc-0.2.0.tar", last modified: Sat Jun 17 20:03:55 2023, max compression
```

## Comparing `git2doc-0.1.8.tar` & `git2doc-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 19:59:45.370399 git2doc-0.1.8/
--rw-rw-rw-   0        0        0     3025 2023-06-17 19:59:45.369349 git2doc-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2356 2023-06-17 19:48:08.000000 git2doc-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-17 19:59:45.357826 git2doc-0.1.8/git2doc/
--rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2doc-0.1.8/git2doc/__init__.py
--rw-rw-rw-   0        0        0     7727 2023-06-17 00:03:27.000000 git2doc-0.1.8/git2doc/loader.py
-drwxrwxrwx   0        0        0        0 2023-06-17 19:59:45.367344 git2doc-0.1.8/git2doc.egg-info/
--rw-rw-rw-   0        0        0     3025 2023-06-17 19:59:45.000000 git2doc-0.1.8/git2doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-17 19:59:45.000000 git2doc-0.1.8/git2doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 19:59:45.000000 git2doc-0.1.8/git2doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-17 19:59:45.000000 git2doc-0.1.8/git2doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-17 19:59:45.000000 git2doc-0.1.8/git2doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-17 19:59:45.370399 git2doc-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1011 2023-06-17 19:42:01.000000 git2doc-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:03:55.027524 git2doc-0.2.0/
+-rw-rw-rw-   0        0        0     3025 2023-06-17 20:03:55.026485 git2doc-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2356 2023-06-17 19:48:08.000000 git2doc-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 20:03:54.976636 git2doc-0.2.0/git2doc/
+-rw-rw-rw-   0        0        0        0 2023-06-09 14:25:12.000000 git2doc-0.2.0/git2doc/__init__.py
+-rw-rw-rw-   0        0        0     7727 2023-06-17 00:03:27.000000 git2doc-0.2.0/git2doc/loader.py
+drwxrwxrwx   0        0        0        0 2023-06-17 20:03:55.023489 git2doc-0.2.0/git2doc.egg-info/
+-rw-rw-rw-   0        0        0     3025 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-17 20:03:54.000000 git2doc-0.2.0/git2doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 20:03:55.028486 git2doc-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-06-17 20:02:55.000000 git2doc-0.2.0/setup.py
```

### Comparing `git2doc-0.1.8/PKG-INFO` & `git2doc-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.1.8
+Version: 0.2.0
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2doc-0.1.8/README.md` & `git2doc-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `git2doc-0.1.8/git2doc/loader.py` & `git2doc-0.2.0/git2doc/loader.py`

 * *Files identical despite different names*

### Comparing `git2doc-0.1.8/git2doc.egg-info/PKG-INFO` & `git2doc-0.2.0/git2doc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.1.8
+Version: 0.2.0
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `git2doc-0.1.8/setup.py` & `git2doc-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2doc',
-    version='0.1.8',
+    version='0.2.0',
     description='A tool for converting git repositories into documents',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2doc',
     packages=find_packages(),
     install_requires=[
         'langchain',
-        'pinecone-client',
         'tiktoken',
         'gitpython',
         "python-dotenv",
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',  
         'Intended Audience :: Developers',
```

