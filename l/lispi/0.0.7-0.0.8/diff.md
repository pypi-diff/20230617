# Comparing `tmp/lispi-0.0.7.tar.gz` & `tmp/lispi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "lispi-0.0.8.tar", last modified: Sat Jun 17 02:19:34 2023, max compression
```

## Comparing `lispi-0.0.7.tar` & `lispi-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lispi-0.0.7/.DS_Store
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.7/MANIFEST.in
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.7/requirements.txt
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 lispi-0.0.7/setup.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.7/example/.DS_Store
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 lispi-0.0.7/example/original_example.ipynb
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.7/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.7/src/lispi/.DS_Store
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lispi-0.0.7/src/lispi/__init__.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 lispi-0.0.7/src/lispi/__main__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 lispi-0.0.7/src/lispi/lispi.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.7/src/lispi/revealjs_template.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 lispi-0.0.7/src/lispi/slideEdit.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.7/src/lispi/text2audio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.7/tests/test_audioText.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.7/tests/test_nbconvert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.7/tests/test_pyscript.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lispi-0.0.7/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.7/LICENSE
--rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 lispi-0.0.7/README.md
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 lispi-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 lispi-0.0.7/PKG-INFO
+drwxr-xr-x   0 bm         (503) staff       (20)        0 2023-06-17 02:19:34.982879 lispi-0.0.8/
+-rw-r--r--   0 bm         (503) staff       (20)     1073 2023-06-09 14:52:04.000000 lispi-0.0.8/LICENSE
+-rw-r--r--   0 bm         (503) staff       (20)       32 2023-06-15 16:14:25.000000 lispi-0.0.8/MANIFEST.in
+-rw-r--r--   0 bm         (503) staff       (20)     5164 2023-06-17 02:19:34.982761 lispi-0.0.8/PKG-INFO
+-rw-r--r--   0 bm         (503) staff       (20)     3185 2023-06-17 00:10:17.000000 lispi-0.0.8/README.md
+drwxr-xr-x   0 bm         (503) staff       (20)        0 2023-06-17 02:19:34.981331 lispi-0.0.8/example/
+-rw-r--r--   0 bm         (503) staff       (20)     6148 2023-06-15 14:03:25.000000 lispi-0.0.8/example/.DS_Store
+-rw-r--r--   0 bm         (503) staff       (20)     2384 2023-06-17 00:33:09.000000 lispi-0.0.8/example/original_example.ipynb
+drwxr-xr-x   0 bm         (503) staff       (20)        0 2023-06-17 02:19:34.982227 lispi-0.0.8/lispi.egg-info/
+-rw-r--r--   0 bm         (503) staff       (20)     5164 2023-06-17 02:19:34.000000 lispi-0.0.8/lispi.egg-info/PKG-INFO
+-rw-r--r--   0 bm         (503) staff       (20)      349 2023-06-17 02:19:34.000000 lispi-0.0.8/lispi.egg-info/SOURCES.txt
+-rw-r--r--   0 bm         (503) staff       (20)        1 2023-06-17 02:19:34.000000 lispi-0.0.8/lispi.egg-info/dependency_links.txt
+-rw-r--r--   0 bm         (503) staff       (20)       46 2023-06-17 02:19:34.000000 lispi-0.0.8/lispi.egg-info/entry_points.txt
+-rw-r--r--   0 bm         (503) staff       (20)       83 2023-06-17 02:19:34.000000 lispi-0.0.8/lispi.egg-info/requires.txt
+-rw-r--r--   0 bm         (503) staff       (20)        1 2023-06-17 02:19:34.000000 lispi-0.0.8/lispi.egg-info/top_level.txt
+-rw-r--r--   0 bm         (503) staff       (20)     1431 2023-06-17 02:17:03.000000 lispi-0.0.8/pyproject.toml
+-rw-r--r--   0 bm         (503) staff       (20)       38 2023-06-17 02:19:34.982914 lispi-0.0.8/setup.cfg
+-rw-r--r--   0 bm         (503) staff       (20)      630 2023-06-17 02:15:08.000000 lispi-0.0.8/setup.py
+drwxr-xr-x   0 bm         (503) staff       (20)        0 2023-06-17 02:19:34.982605 lispi-0.0.8/tests/
+-rw-r--r--   0 bm         (503) staff       (20)        0 2023-06-13 19:47:12.000000 lispi-0.0.8/tests/test_audioText.py
+-rw-r--r--   0 bm         (503) staff       (20)        0 2023-06-09 15:13:18.000000 lispi-0.0.8/tests/test_nbconvert.py
+-rw-r--r--   0 bm         (503) staff       (20)        0 2023-06-14 19:24:57.000000 lispi-0.0.8/tests/test_pyscript.py
```

### Comparing `lispi-0.0.7/example/.DS_Store` & `lispi-0.0.8/example/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.7/example/original_example.ipynb` & `lispi-0.0.8/example/original_example.ipynb`

 * *Files identical despite different names*

### Comparing `lispi-0.0.7/LICENSE` & `lispi-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lispi-0.0.7/README.md` & `lispi-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lispi-0.0.7/pyproject.toml` & `lispi-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.include]
 include = [".example/**"]
 
 [project]
 name = "lispi"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="B7M", email="ibsnetwork001@gmail.com" },
 ]
 license = { file = "LICENSE" }
 description = "`lispi` (Learning Interactive Slides and PIthon) is a python package for generating live notebooks where you can learn the content by listening to and reading from the slides at the same time you can write and execute yourown code from the slides in real time."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -38,15 +38,15 @@
 Homepage = "https://github.com/B7M/lispi"
 
 [project.scripts]
 lispi = "lispi.__main__:main"
 
 
 [tool.bumpver]
-current_version = "0.0.7"
+current_version = "0.0.8"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lispi-0.0.7/PKG-INFO` & `lispi-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: lispi
-Version: 0.0.7
+Version: 0.0.8
 Summary: `lispi` (Learning Interactive Slides and PIthon) is a python package for generating live notebooks where you can learn the content by listening to and reading from the slides at the same time you can write and execute yourown code from the slides in real time.
-Project-URL: Homepage, https://github.com/B7M/lispi
+Home-page: https://github.com/yourusername/your-repo
+Author: B7M
 Author-email: B7M <ibsnetwork001@gmail.com>
 License: Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -19,28 +20,22 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-License-File: LICENSE
-Keywords: code,live,notebook,py-scripts
+Project-URL: Homepage, https://github.com/B7M/lispi
+Keywords: notebook,live,code,py-scripts
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: click
-Requires-Dist: gtts
-Requires-Dist: jupyter
-Requires-Dist: jupyterlab
-Requires-Dist: nbconvert
-Requires-Dist: nbformat
-Requires-Dist: tomli; python_version < '3.11'
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Lispi Documentation
 
 ## Introduction
 
 `lispi` (Learning Interactive Slides and PIthon) is a Python package that provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements directly from the slides.
```

