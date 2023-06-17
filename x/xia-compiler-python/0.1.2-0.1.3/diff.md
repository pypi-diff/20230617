# Comparing `tmp/xia_compiler_python-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_python-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 167395 bytes, number of entries: 7
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-05 10:01 xia_compiler_python/__init__.py
--rw-r--r--  2.0 unx   426496 b- defN 23-Jun-05 10:04 xia_compiler_python/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-05 10:04 xia_compiler_python-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      674 b- defN 23-Jun-05 10:04 xia_compiler_python-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-05 10:04 xia_compiler_python-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-05 10:04 xia_compiler_python-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      641 b- defN 23-Jun-05 10:04 xia_compiler_python-0.1.2.dist-info/RECORD
-7 files, 428197 bytes uncompressed, 166239 bytes compressed:  61.2%
+Zip file size: 168610 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-17 06:36 xia_compiler_python/__init__.py
+-rw-r--r--  2.0 unx   429568 b- defN 23-Jun-17 06:39 xia_compiler_python/compiler.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-17 06:39 xia_compiler_python-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-17 06:39 xia_compiler_python-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-17 06:39 xia_compiler_python-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-17 06:39 xia_compiler_python-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      641 b- defN 23-Jun-17 06:39 xia_compiler_python-0.1.3.dist-info/RECORD
+7 files, 431269 bytes uncompressed, 167454 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_python/__init__.py
 Comment: 
 
 Filename: xia_compiler_python/compiler.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_compiler_python-0.1.2.dist-info/LICENSE.txt
+Filename: xia_compiler_python-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.2.dist-info/METADATA
+Filename: xia_compiler_python-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_python-0.1.2.dist-info/WHEEL
+Filename: xia_compiler_python-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_python-0.1.2.dist-info/top_level.txt
+Filename: xia_compiler_python-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.2.dist-info/RECORD
+Filename: xia_compiler_python-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_python/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_python.compiler import PythonCompiler
 
 
 __all__ = [
     "PythonCompiler"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_compiler_python-0.1.2.dist-info/METADATA` & `xia_compiler_python-0.1.3.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-compiler-python
-Version: 0.1.2
+Version: 0.1.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-python/0.1.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-python/0.1.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_compiler_python-0.1.2.dist-info/RECORD` & `xia_compiler_python-0.1.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_python/__init__.py,sha256=7qjnZ-uFjM6WnlO7qY8jQX6GNYHQ8IvZTKcNsSfQ_xk,116
-xia_compiler_python/compiler.cp39-win_amd64.pyd,sha256=TQHUmUfW5vj1bWEL1Wwj0yEQyoPq3Dqr6KYBrYnsa3A,426496
-xia_compiler_python-0.1.2.dist-info/LICENSE.txt,sha256=uYnvfTF5TW6hakbLwlmA14uetnfEmRohRS_PHhU5dY4,151
-xia_compiler_python-0.1.2.dist-info/METADATA,sha256=KjSlnl6ZNUFs29osG9PNw9ly2ZjIPH9ORnVQ4uq9i_k,674
-xia_compiler_python-0.1.2.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_compiler_python-0.1.2.dist-info/top_level.txt,sha256=R07z9GUYJwDzaFPJq6hLs3IP0HWGFMzYXFe9Dx7Lh-c,20
-xia_compiler_python-0.1.2.dist-info/RECORD,,
+xia_compiler_python/__init__.py,sha256=yBG52Mjmiz5XFuuC8HPKxJ5PjwzedKZRDqCb7Ziuk90,116
+xia_compiler_python/compiler.cp39-win_amd64.pyd,sha256=uRXV7jC8oH3kjMNjZpAcM31HOkfJajXnj2hUTc4OD-A,429568
+xia_compiler_python-0.1.3.dist-info/LICENSE.txt,sha256=gNAozHm4-2o3q0DsWBseQDOxAxNL0nSoJBA5UU4udf4,151
+xia_compiler_python-0.1.3.dist-info/METADATA,sha256=LJPxjNcRU5JRSkoca7l_43Wo33hJ43WFPWawoYCSnw0,674
+xia_compiler_python-0.1.3.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
+xia_compiler_python-0.1.3.dist-info/top_level.txt,sha256=R07z9GUYJwDzaFPJq6hLs3IP0HWGFMzYXFe9Dx7Lh-c,20
+xia_compiler_python-0.1.3.dist-info/RECORD,,
```

