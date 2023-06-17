# Comparing `tmp/lispi-0.0.5.tar.gz` & `tmp/lispi-0.0.6.tar.gz`

## Comparing `lispi-0.0.5.tar` & `lispi-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.5/.DS_Store
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.5/MANIFEST.in
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.5/requirements.txt
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 lispi-0.0.5/setup.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.5/example/.DS_Store
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 lispi-0.0.5/example/original_example.ipynb
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.5/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/.DS_Store
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/__init__.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/__main__.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/lispi.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/revealjs_template.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/slideEdit.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/text2audio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.5/tests/test_audioText.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.5/tests/test_nbconvert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.5/tests/test_pyscript.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.5/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.5/LICENSE
--rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 lispi-0.0.5/README.md
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 lispi-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 lispi-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.6/.DS_Store
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.6/MANIFEST.in
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.6/requirements.txt
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 lispi-0.0.6/setup.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.6/example/.DS_Store
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 lispi-0.0.6/example/original_example.ipynb
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.6/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.6/src/lispi/.DS_Store
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lispi-0.0.6/src/lispi/__init__.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 lispi-0.0.6/src/lispi/__main__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 lispi-0.0.6/src/lispi/lispi.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.6/src/lispi/revealjs_template.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 lispi-0.0.6/src/lispi/slideEdit.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.6/src/lispi/text2audio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.6/tests/test_audioText.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.6/tests/test_nbconvert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.6/tests/test_pyscript.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 lispi-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3185 2020-02-02 00:00:00.000000 lispi-0.0.6/README.md
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 lispi-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 lispi-0.0.6/PKG-INFO
```

### Comparing `lispi-0.0.5/.DS_Store` & `lispi-0.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/requirements.txt` & `lispi-0.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/example/.DS_Store` & `lispi-0.0.6/example/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/example/original_example.ipynb` & `lispi-0.0.6/example/original_example.ipynb`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/src/.DS_Store` & `lispi-0.0.6/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/src/lispi/.DS_Store` & `lispi-0.0.6/src/lispi/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/src/lispi/__main__.py` & `lispi-0.0.6/src/lispi/__main__.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/src/lispi/lispi.py` & `lispi-0.0.6/src/lispi/lispi.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/src/lispi/slideEdit.py` & `lispi-0.0.6/src/lispi/slideEdit.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/src/lispi/text2audio.py` & `lispi-0.0.6/src/lispi/text2audio.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/LICENSE` & `lispi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lispi-0.0.5/README.md` & `lispi-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Lispi Documentation
 
 ## Introduction
 
-Lispi (Educational Slide Studio) is a Python package that provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements directly from the slides.
+`lispi` (Learning Interactive Slides and PIthon) is a Python package that provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements directly from the slides.
 
 ## Installation
 
 To install `lispi` package, you can use pip, the Python package installer. Open your terminal and run the following command:
 
 ```
 pip install lispi
```

### Comparing `lispi-0.0.5/PKG-INFO` & `lispi-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lispi
-Version: 0.0.5
-Summary: A simple python package for generating live notebooks where you can write code and run it in real time.
+Version: 0.0.6
+Summary: `lispi` (Learning Interactive Slides and PIthon) is a python package for generating live notebooks where you can learn the content by listening to and reading from the slides at the same time you can write and execute yourown code from the slides in real time.
 Project-URL: Homepage, https://github.com/B7M/lispi
 Author-email: B7M <ibsnetwork001@gmail.com>
 License: Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -38,15 +38,15 @@
 Requires-Dist: tomli; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 # Lispi Documentation
 
 ## Introduction
 
-Lispi (Educational Slide Studio) is a Python package that provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements directly from the slides.
+`lispi` (Learning Interactive Slides and PIthon) is a Python package that provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements directly from the slides.
 
 ## Installation
 
 To install `lispi` package, you can use pip, the Python package installer. Open your terminal and run the following command:
 
 ```
 pip install lispi
```

