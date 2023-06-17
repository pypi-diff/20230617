# Comparing `tmp/web_ext_helper-1.0.2.tar.gz` & `tmp/web_ext_helper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.0.2.tar", max compression
+gzip compressed data, was "web_ext_helper-1.0.3.tar", max compression
```

## Comparing `web_ext_helper-1.0.2.tar` & `web_ext_helper-1.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.2/LICENSE
--rw-r--r--   0        0        0      573 2023-06-17 20:47:52.667149 web_ext_helper-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.2/README.md
--rw-r--r--   0        0        0     9875 2023-06-17 18:50:16.248365 web_ext_helper-1.0.2/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 web_ext_helper-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.3/LICENSE
+-rw-r--r--   0        0        0      572 2023-06-17 20:50:14.892163 web_ext_helper-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.3/README.md
+-rw-r--r--   0        0        0     9875 2023-06-17 18:50:16.248365 web_ext_helper-1.0.3/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 web_ext_helper-1.0.3/PKG-INFO
```

### Comparing `web_ext_helper-1.0.2/LICENSE` & `web_ext_helper-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.2/pyproject.toml` & `web_ext_helper-1.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.0.2"
+version = "1.0.3"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 
 [tool.poetry.group.dev.dependencies]
 Pillow = "^9.5.0"
 typer = "^0.9.0"
 
 [tool.poetry.scripts]
-web-ext-helper = "web_ext_helper.web_ext_helper:main"
+web-ext-helper = "web_ext_helper.web_ext_helper:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `web_ext_helper-1.0.2/README.md` & `web_ext_helper-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.2/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.0.3/web_ext_helper/web_ext_helper.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.2/PKG-INFO` & `web_ext_helper-1.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

