# Comparing `tmp/Artec-0.1.1.tar.gz` & `tmp/Artec-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Artec-0.1.1.tar", last modified: Thu Jun 15 14:43:07 2023, max compression
+gzip compressed data, was "Artec-0.1.2.tar", last modified: Sat Jun 17 13:12:20 2023, max compression
```

## Comparing `Artec-0.1.1.tar` & `Artec-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:43:07.213577 Artec-0.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-15 14:43:07.205670 Artec-0.1.1/Artec.egg-info/
--rw-rw-rw-   0        0        0     2366 2023-06-15 14:43:07.000000 Artec-0.1.1/Artec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-06-15 14:43:07.000000 Artec-0.1.1/Artec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:43:07.000000 Artec-0.1.1/Artec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-15 14:43:07.000000 Artec-0.1.1/Artec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 14:43:07.000000 Artec-0.1.1/Artec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-06-09 04:27:29.000000 Artec-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2366 2023-06-15 14:43:07.213577 Artec-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1707 2023-06-15 14:41:45.000000 Artec-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 14:43:07.210929 Artec-0.1.1/artec/
--rw-rw-rw-   0        0        0      359 2023-06-15 14:42:15.000000 Artec-0.1.1/artec/__init__.py
--rw-rw-rw-   0        0        0      231 2023-06-15 01:44:05.000000 Artec-0.1.1/artec/__main__.py
--rw-rw-rw-   0        0        0     1285 2023-06-15 01:41:05.000000 Artec-0.1.1/artec/argparser.py
--rw-rw-rw-   0        0        0     1433 2023-06-15 01:35:54.000000 Artec-0.1.1/artec/boiler.py
--rw-rw-rw-   0        0        0        0 2023-06-15 01:44:26.000000 Artec-0.1.1/artec/tui.py
--rw-rw-rw-   0        0        0      829 2023-06-15 14:42:25.000000 Artec-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-15 14:43:07.213577 Artec-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-06-13 22:05:57.000000 Artec-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 13:12:20.345672 Artec-0.1.2/
+drwxrwxrwx   0        0        0        0 2023-06-17 13:12:20.328313 Artec-0.1.2/Artec.egg-info/
+-rw-rw-rw-   0        0        0     2366 2023-06-17 13:12:20.000000 Artec-0.1.2/Artec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-06-17 13:12:20.000000 Artec-0.1.2/Artec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 13:12:20.000000 Artec-0.1.2/Artec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-17 13:12:20.000000 Artec-0.1.2/Artec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2023-06-17 13:12:20.000000 Artec-0.1.2/Artec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-06-09 04:27:29.000000 Artec-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2366 2023-06-17 13:12:20.345672 Artec-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1707 2023-06-17 13:06:18.000000 Artec-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-17 13:12:20.342070 Artec-0.1.2/artec/
+-rw-rw-rw-   0        0        0      388 2023-06-17 13:06:18.000000 Artec-0.1.2/artec/__init__.py
+-rw-rw-rw-   0        0        0      257 2023-06-17 12:39:07.000000 Artec-0.1.2/artec/__main__.py
+-rw-rw-rw-   0        0        0     1748 2023-06-17 12:44:40.000000 Artec-0.1.2/artec/argparser.py
+-rw-rw-rw-   0        0        0     2345 2023-06-17 13:05:18.000000 Artec-0.1.2/artec/boiler.py
+-rw-rw-rw-   0        0        0        0 2023-06-15 01:44:26.000000 Artec-0.1.2/artec/tui.py
+-rw-rw-rw-   0        0        0      829 2023-06-17 13:06:18.000000 Artec-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-17 13:12:20.349543 Artec-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-06-13 22:05:57.000000 Artec-0.1.2/setup.py
```

### Comparing `Artec-0.1.1/Artec.egg-info/PKG-INFO` & `Artec-0.1.2/Artec.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Artec
-Version: 0.1.1
+Version: 0.1.2
 Summary: Creates a configurable python project template in a given directory.
 Author-email: HushmKun <HushmKun@outlook.com>, Link- <bsm.dgdy@gmail.com>
 Project-URL: Homepage, https://github.com/HushmKun/Artec
 Project-URL: Bug Tracker, https://github.com/HushmKun/Artec/issues
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -65,15 +65,15 @@
 
     Examples :
             artec -o dest
             artec -o dest -s res/simple.json
 ```
 ## Version
 
-    0.1.1
+    0.1.2
 
 ## Contributing
 
 Big Thanks to [Link-](https://github.com/Link-) for jump starting the project.
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `Artec-0.1.1/LICENSE` & `Artec-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Artec-0.1.1/PKG-INFO` & `Artec-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Artec
-Version: 0.1.1
+Version: 0.1.2
 Summary: Creates a configurable python project template in a given directory.
 Author-email: HushmKun <HushmKun@outlook.com>, Link- <bsm.dgdy@gmail.com>
 Project-URL: Homepage, https://github.com/HushmKun/Artec
 Project-URL: Bug Tracker, https://github.com/HushmKun/Artec/issues
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -65,15 +65,15 @@
 
     Examples :
             artec -o dest
             artec -o dest -s res/simple.json
 ```
 ## Version
 
-    0.1.1
+    0.1.2
 
 ## Contributing
 
 Big Thanks to [Link-](https://github.com/Link-) for jump starting the project.
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `Artec-0.1.1/README.md` & `Artec-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     Examples :
             artec -o dest
             artec -o dest -s res/simple.json
 ```
 ## Version
 
-    0.1.1
+    0.1.2
 
 ## Contributing
 
 Big Thanks to [Link-](https://github.com/Link-) for jump starting the project.
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `Artec-0.1.1/pyproject.toml` & `Artec-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 733e 3d36 312e 3022 5d0d  uptools>=61.0"].
 00000030: 0a62 7569 6c64 2d62 6163 6b65 6e64 203d  .build-backend =
 00000040: 2022 7365 7475 7074 6f6f 6c73 2e62 7569   "setuptools.bui
 00000050: 6c64 5f6d 6574 6122 0d0a 0d0a 5b70 726f  ld_meta"....[pro
 00000060: 6a65 6374 5d0d 0a6e 616d 6520 3d20 2241  ject]..name = "A
 00000070: 7274 6563 220d 0a76 6572 7369 6f6e 203d  rtec"..version =
-00000080: 2022 302e 312e 3122 0d0a 6175 7468 6f72   "0.1.1"..author
+00000080: 2022 302e 312e 3222 0d0a 6175 7468 6f72   "0.1.2"..author
 00000090: 7320 3d20 5b0d 0a20 207b 206e 616d 653d  s = [..  { name=
 000000a0: 2248 7573 686d 4b75 6e22 2c20 656d 6169  "HushmKun", emai
 000000b0: 6c3d 2248 7573 686d 4b75 6e40 6f75 746c  l="HushmKun@outl
 000000c0: 6f6f 6b2e 636f 6d22 207d 2c0d 0a20 207b  ook.com" },..  {
 000000d0: 206e 616d 653d 224c 696e 6b2d 222c 2065   name="Link-", e
 000000e0: 6d61 696c 3d22 6273 6d2e 6467 6479 4067  mail="bsm.dgdy@g
 000000f0: 6d61 696c 2e63 6f6d 2220 7d2c 0d0a 5d0d  mail.com" },..].
```

