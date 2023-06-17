# Comparing `tmp/soul_knight_data_processing-0.0.3.tar.gz` & `tmp/soul_knight_data_processing-0.0.4.tar.gz`

## Comparing `soul_knight_data_processing-0.0.3.tar` & `soul_knight_data_processing-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.3/example.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.3/SKD/__init__.py
--rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.3/SKD/core.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.3/LICENSE
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.3/README.md
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    41073 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/example.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/get_data.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/SKD/__init__.py
+-rw-r--r--   0        0        0     5296 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/SKD/core.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/SKD/get_official_data.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/LICENSE
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/README.md
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    41405 2020-02-02 00:00:00.000000 soul_knight_data_processing-0.0.4/PKG-INFO
```

### Comparing `soul_knight_data_processing-0.0.3/.github/workflows/python-publish.yml` & `soul_knight_data_processing-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `soul_knight_data_processing-0.0.3/SKD/core.py` & `soul_knight_data_processing-0.0.4/SKD/core.py`

 * *Files identical despite different names*

### Comparing `soul_knight_data_processing-0.0.3/LICENSE` & `soul_knight_data_processing-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `soul_knight_data_processing-0.0.3/PKG-INFO` & `soul_knight_data_processing-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soul_knight_data_processing
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for encode or decode soul_knight data files.
 Project-URL: Homepage, https://github.com/Suto-Commune/soul_knight/
 Author-email: Roren Natsumi <RorenNatsumi@outlook.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -675,19 +675,24 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 License-File: LICENSE
-Requires-Dist: crypto>=1.4.1
+Requires-Dist: pycryptodome
+Requires-Dist: requests
+Requires-Dist: wget
 Description-Content-Type: text/markdown
 
-使用方法看example.py，或者自己翻源码
+[![Pypi](https://img.shields.io/pypi/v/soul-knight-data-processing)](https://pypi.org/project/soul-knight-data-processing/)
+[![Upload Python Package](https://github.com/Suto-Commune/soul_knight/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Suto-Commune/soul_knight/actions/workflows/python-publish.yml)
 
-使用GPLV3协议
 
-PIPY： https://pypi.org/project/soul-knight-data-processing/
+使用方法看`example.py`  或者 `example.py`，或者自己翻源码
+
+使用GPL V3协议
+
 
 ```
 pip install soul-knight-data-processing
 ```
```

