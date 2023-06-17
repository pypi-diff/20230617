# Comparing `tmp/shamela2epub-1.3.0.tar.gz` & `tmp/shamela2epub-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shamela2epub-1.3.0.tar", max compression
+gzip compressed data, was "shamela2epub-1.3.1.tar", max compression
```

## Comparing `shamela2epub-1.3.0.tar` & `shamela2epub-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0    35149 2022-07-09 23:30:01.570497 shamela2epub-1.3.0/LICENSE
--rw-r--r--   0        0        0     4177 2022-08-10 16:37:20.585434 shamela2epub-1.3.0/README.md
--rw-r--r--   0        0        0     2210 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1421 2023-05-29 12:26:02.759708 shamela2epub-1.3.0/shamela2epub/__init__.py
--rw-r--r--   0        0        0      360 2023-06-17 11:18:18.736301 shamela2epub-1.3.0/shamela2epub/__main__.py
--rw-r--r--   0        0        0   132340 2022-07-12 09:01:57.456000 shamela2epub-1.3.0/shamela2epub/assets/NotoNaskhArabic-Regular.ttf
--rw-r--r--   0        0        0     2642 2022-07-11 21:45:18.273814 shamela2epub-1.3.0/shamela2epub/assets/books-duotone-128.png
--rw-r--r--   0        0        0    12405 2022-07-11 21:44:58.343656 shamela2epub-1.3.0/shamela2epub/assets/books-duotone-512.png
--rw-r--r--   0        0        0     9212 2022-07-16 12:17:14.319639 shamela2epub-1.3.0/shamela2epub/assets/books-duotone.ico
--rw-r--r--   0        0        0     1622 2022-07-11 21:40:01.487963 shamela2epub-1.3.0/shamela2epub/assets/books-duotone.svg
--rw-r--r--   0        0        0      715 2022-07-11 21:45:26.597214 shamela2epub-1.3.0/shamela2epub/assets/download-duotone-64.png
--rw-r--r--   0        0        0      752 2022-07-11 21:40:31.408201 shamela2epub-1.3.0/shamela2epub/assets/download-duotone.svg
--rw-r--r--   0        0        0      296 2022-08-09 16:51:53.801245 shamela2epub-1.3.0/shamela2epub/assets/styles.css
--rw-r--r--   0        0        0        0 2022-07-12 10:44:40.993865 shamela2epub-1.3.0/shamela2epub/cli/__init__.py
--rw-r--r--   0        0        0     1138 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/cli/app.py
--rw-r--r--   0        0        0        0 2023-05-29 12:01:12.937795 shamela2epub-1.3.0/shamela2epub/gui/__init__.py
--rw-r--r--   0        0        0     6724 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/gui/app.py
--rw-r--r--   0        0        0     3366 2022-07-15 20:49:22.620403 shamela2epub-1.3.0/shamela2epub/gui/ui.ui
--rw-r--r--   0        0        0     2948 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/main.py
--rw-r--r--   0        0        0        0 2022-07-09 23:30:06.020458 shamela2epub-1.3.0/shamela2epub/misc/__init__.py
--rw-r--r--   0        0        0       53 2022-07-15 20:49:22.700404 shamela2epub-1.3.0/shamela2epub/misc/constants.py
--rw-r--r--   0        0        0     1146 2023-05-29 12:01:12.951128 shamela2epub-1.3.0/shamela2epub/misc/patterns.py
--rw-r--r--   0        0        0     1374 2023-05-29 12:01:12.954462 shamela2epub-1.3.0/shamela2epub/misc/utils.py
--rw-r--r--   0        0        0        0 2022-07-09 23:30:06.020458 shamela2epub-1.3.0/shamela2epub/models/__init__.py
--rw-r--r--   0        0        0      450 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/models/book_base_html_page.py
--rw-r--r--   0        0        0    10952 2023-06-17 11:40:51.296651 shamela2epub-1.3.0/shamela2epub/models/book_html_page.py
--rw-r--r--   0        0        0     1019 2023-05-29 12:01:12.957795 shamela2epub-1.3.0/shamela2epub/models/book_info_html_page.py
--rw-r--r--   0        0        0     6924 2023-06-17 11:40:51.299984 shamela2epub-1.3.0/shamela2epub/models/epub_book.py
--rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 shamela2epub-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-09 23:30:01.570497 shamela2epub-1.3.1/LICENSE
+-rw-r--r--   0        0        0     4177 2022-08-10 16:37:20.585434 shamela2epub-1.3.1/README.md
+-rw-r--r--   0        0        0     2210 2023-06-17 13:25:52.843283 shamela2epub-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1421 2023-05-29 12:26:02.759708 shamela2epub-1.3.1/shamela2epub/__init__.py
+-rw-r--r--   0        0        0      360 2023-06-17 11:18:18.736301 shamela2epub-1.3.1/shamela2epub/__main__.py
+-rw-r--r--   0        0        0   132340 2022-07-12 09:01:57.456000 shamela2epub-1.3.1/shamela2epub/assets/NotoNaskhArabic-Regular.ttf
+-rw-r--r--   0        0        0     2642 2022-07-11 21:45:18.273814 shamela2epub-1.3.1/shamela2epub/assets/books-duotone-128.png
+-rw-r--r--   0        0        0    12405 2022-07-11 21:44:58.343656 shamela2epub-1.3.1/shamela2epub/assets/books-duotone-512.png
+-rw-r--r--   0        0        0     9212 2022-07-16 12:17:14.319639 shamela2epub-1.3.1/shamela2epub/assets/books-duotone.ico
+-rw-r--r--   0        0        0     1622 2022-07-11 21:40:01.487963 shamela2epub-1.3.1/shamela2epub/assets/books-duotone.svg
+-rw-r--r--   0        0        0      715 2022-07-11 21:45:26.597214 shamela2epub-1.3.1/shamela2epub/assets/download-duotone-64.png
+-rw-r--r--   0        0        0      752 2022-07-11 21:40:31.408201 shamela2epub-1.3.1/shamela2epub/assets/download-duotone.svg
+-rw-r--r--   0        0        0      296 2022-08-09 16:51:53.801245 shamela2epub-1.3.1/shamela2epub/assets/styles.css
+-rw-r--r--   0        0        0        0 2022-07-12 10:44:40.993865 shamela2epub-1.3.1/shamela2epub/cli/__init__.py
+-rw-r--r--   0        0        0     1138 2023-06-17 11:40:51.296651 shamela2epub-1.3.1/shamela2epub/cli/app.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:01:12.937795 shamela2epub-1.3.1/shamela2epub/gui/__init__.py
+-rw-r--r--   0        0        0     6724 2023-06-17 11:40:51.296651 shamela2epub-1.3.1/shamela2epub/gui/app.py
+-rw-r--r--   0        0        0     3366 2022-07-15 20:49:22.620403 shamela2epub-1.3.1/shamela2epub/gui/ui.ui
+-rw-r--r--   0        0        0     2948 2023-06-17 11:40:51.296651 shamela2epub-1.3.1/shamela2epub/main.py
+-rw-r--r--   0        0        0        0 2022-07-09 23:30:06.020458 shamela2epub-1.3.1/shamela2epub/misc/__init__.py
+-rw-r--r--   0        0        0       53 2022-07-15 20:49:22.700404 shamela2epub-1.3.1/shamela2epub/misc/constants.py
+-rw-r--r--   0        0        0      564 2023-06-17 13:25:29.313033 shamela2epub-1.3.1/shamela2epub/misc/http.py
+-rw-r--r--   0        0        0     1146 2023-05-29 12:01:12.951128 shamela2epub-1.3.1/shamela2epub/misc/patterns.py
+-rw-r--r--   0        0        0     1374 2023-05-29 12:01:12.954462 shamela2epub-1.3.1/shamela2epub/misc/utils.py
+-rw-r--r--   0        0        0        0 2022-07-09 23:30:06.020458 shamela2epub-1.3.1/shamela2epub/models/__init__.py
+-rw-r--r--   0        0        0      411 2023-06-17 13:24:49.572607 shamela2epub-1.3.1/shamela2epub/models/book_base_html_page.py
+-rw-r--r--   0        0        0    10952 2023-06-17 11:40:51.296651 shamela2epub-1.3.1/shamela2epub/models/book_html_page.py
+-rw-r--r--   0        0        0     1019 2023-05-29 12:01:12.957795 shamela2epub-1.3.1/shamela2epub/models/book_info_html_page.py
+-rw-r--r--   0        0        0     6924 2023-06-17 11:40:51.299984 shamela2epub-1.3.1/shamela2epub/models/epub_book.py
+-rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 shamela2epub-1.3.1/PKG-INFO
```

### Comparing `shamela2epub-1.3.0/LICENSE` & `shamela2epub-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/README.md` & `shamela2epub-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/pyproject.toml` & `shamela2epub-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shamela2epub"
-version = "1.3.0"
+version = "1.3.1"
 description = "A CLI and GUI tool to download a book on https://shamela.ws to an EPUB book."
 authors = ["yshalsager <ysh-alsager@hotmail.com>"]
 license = "GPL-3.0-only"
 repository = "https://github.com/yshalsager/shamela2epub/"
 keywords = ["epub3", "shamela", "book", "epub", "islamic"]
 packages = [
     { include = "shamela2epub" }
```

### Comparing `shamela2epub-1.3.0/shamela2epub/__init__.py` & `shamela2epub-1.3.1/shamela2epub/__init__.py`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/assets/NotoNaskhArabic-Regular.ttf` & `shamela2epub-1.3.1/shamela2epub/assets/NotoNaskhArabic-Regular.ttf`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/assets/books-duotone-128.png` & `shamela2epub-1.3.1/shamela2epub/assets/books-duotone-128.png`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/assets/books-duotone-512.png` & `shamela2epub-1.3.1/shamela2epub/assets/books-duotone-512.png`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/assets/books-duotone.ico` & `shamela2epub-1.3.1/shamela2epub/assets/books-duotone.ico`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/assets/books-duotone.svg` & `shamela2epub-1.3.1/shamela2epub/assets/books-duotone.svg`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/assets/download-duotone-64.png` & `shamela2epub-1.3.1/shamela2epub/assets/download-duotone-64.png`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/assets/download-duotone.svg` & `shamela2epub-1.3.1/shamela2epub/assets/download-duotone.svg`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/cli/app.py` & `shamela2epub-1.3.1/shamela2epub/cli/app.py`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/gui/app.py` & `shamela2epub-1.3.1/shamela2epub/gui/app.py`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/gui/ui.ui` & `shamela2epub-1.3.1/shamela2epub/gui/ui.ui`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/main.py` & `shamela2epub-1.3.1/shamela2epub/main.py`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/misc/patterns.py` & `shamela2epub-1.3.1/shamela2epub/misc/patterns.py`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/misc/utils.py` & `shamela2epub-1.3.1/shamela2epub/misc/utils.py`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/models/book_html_page.py` & `shamela2epub-1.3.1/shamela2epub/models/book_html_page.py`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/models/book_info_html_page.py` & `shamela2epub-1.3.1/shamela2epub/models/book_info_html_page.py`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/shamela2epub/models/epub_book.py` & `shamela2epub-1.3.1/shamela2epub/models/epub_book.py`

 * *Files identical despite different names*

### Comparing `shamela2epub-1.3.0/PKG-INFO` & `shamela2epub-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shamela2epub
-Version: 1.3.0
+Version: 1.3.1
 Summary: A CLI and GUI tool to download a book on https://shamela.ws to an EPUB book.
 Home-page: https://github.com/yshalsager/shamela2epub/
 License: GPL-3.0-only
 Keywords: epub3,shamela,book,epub,islamic
 Author: yshalsager
 Author-email: ysh-alsager@hotmail.com
 Requires-Python: >=3.11,<3.12
```

