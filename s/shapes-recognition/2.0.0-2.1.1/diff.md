# Comparing `tmp/shapes_recognition-2.0.0.tar.gz` & `tmp/shapes_recognition-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapes_recognition-2.0.0.tar", last modified: Mon Jun  5 11:08:24 2023, max compression
+gzip compressed data, was "shapes_recognition-2.1.1.tar", last modified: Sat Jun 17 13:22:06 2023, max compression
```

## Comparing `shapes_recognition-2.0.0.tar` & `shapes_recognition-2.1.1.tar`

### file list

```diff
@@ -1,14 +1,10 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-05 11:08:24.851884 shapes_recognition-2.0.0/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-05 11:08:24.851557 shapes_recognition-2.0.0/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.0.0/README.md
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-05 11:08:24.851972 shapes_recognition-2.0.0/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-05 11:07:55.000000 shapes_recognition-2.0.0/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-05 11:08:24.848701 shapes_recognition-2.0.0/shapes_recognition/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      266 2023-06-04 14:33:45.000000 shapes_recognition-2.0.0/shapes_recognition/__init__.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-05 11:08:24.850372 shapes_recognition-2.0.0/shapes_recognition/pure_cython/
--rwxr-xr-x   0 boriskravtsov   (501) staff       (20)   656872 2023-06-05 10:09:55.000000 shapes_recognition-2.0.0/shapes_recognition/pure_cython/ai_tables.cpython-310-darwin.so
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-05 11:08:24.850038 shapes_recognition-2.0.0/shapes_recognition.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-05 11:08:24.000000 shapes_recognition-2.0.0/shapes_recognition.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      280 2023-06-05 11:08:24.000000 shapes_recognition-2.0.0/shapes_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-05 11:08:24.000000 shapes_recognition-2.0.0/shapes_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-05 11:08:24.000000 shapes_recognition-2.0.0/shapes_recognition.egg-info/top_level.txt
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-17 13:22:06.430363 shapes_recognition-2.1.1/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-17 13:22:06.430098 shapes_recognition-2.1.1/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.1.1/README.md
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-17 13:22:06.430444 shapes_recognition-2.1.1/setup.cfg
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-17 13:10:39.000000 shapes_recognition-2.1.1/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-17 13:22:06.429753 shapes_recognition-2.1.1/shapes_recognition.egg-info/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-17 13:22:06.000000 shapes_recognition-2.1.1/shapes_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      186 2023-06-17 13:22:06.000000 shapes_recognition-2.1.1/shapes_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-17 13:22:06.000000 shapes_recognition-2.1.1/shapes_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-17 13:22:06.000000 shapes_recognition-2.1.1/shapes_recognition.egg-info/top_level.txt
```

### Comparing `shapes_recognition-2.0.0/PKG-INFO` & `shapes_recognition-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapes_recognition
-Version: 2.0.0
+Version: 2.1.1
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shapes_recognition-2.0.0/README.md` & `shapes_recognition-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shapes_recognition-2.0.0/setup.py` & `shapes_recognition-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="shapes_recognition",
-    version="2.0.0",
+    version="2.1.1",
     description="New Shape Matching Technology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://boriskravtsov.com/",
     author="Boris Kravtsov",
     author_email="boriskravtsov.contacts@gmail.com",
     license="MIT",
```

### Comparing `shapes_recognition-2.0.0/shapes_recognition.egg-info/PKG-INFO` & `shapes_recognition-2.1.1/shapes_recognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapes-recognition
-Version: 2.0.0
+Version: 2.1.1
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

