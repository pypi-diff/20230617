# Comparing `tmp/web_ext_helper-1.0.0.tar.gz` & `tmp/web_ext_helper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web_ext_helper-1.0.0.tar", max compression
+gzip compressed data, was "web_ext_helper-1.0.1.tar", max compression
```

## Comparing `web_ext_helper-1.0.0.tar` & `web_ext_helper-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.0/LICENSE
--rw-r--r--   0        0        0      567 2023-06-17 19:25:10.347579 web_ext_helper-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1595 2023-06-17 19:18:19.199084 web_ext_helper-1.0.0/README.md
--rw-r--r--   0        0        0     9875 2023-06-17 18:50:16.248365 web_ext_helper-1.0.0/web_ext_helper/web_ext_helper.py
--rw-r--r--   0        0        0     2003 1970-01-01 00:00:00.000000 web_ext_helper-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35822 2023-06-17 19:16:11.163007 web_ext_helper-1.0.1/LICENSE
+-rw-r--r--   0        0        0      567 2023-06-17 20:41:01.933949 web_ext_helper-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1754 2023-06-17 20:34:00.666577 web_ext_helper-1.0.1/README.md
+-rw-r--r--   0        0        0     9875 2023-06-17 18:50:16.248365 web_ext_helper-1.0.1/web_ext_helper/web_ext_helper.py
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 web_ext_helper-1.0.1/PKG-INFO
```

### Comparing `web_ext_helper-1.0.0/LICENSE` & `web_ext_helper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.0/pyproject.toml` & `web_ext_helper-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web-ext-helper"
-version = "1.0.0"
+version = "1.0.1"
 description = "A simple cli tool that helps you building your web extensions."
 authors = ["AppSolves <appsolves@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "web_ext_helper"}]
 
 [tool.poetry.dependencies]
```

### Comparing `web_ext_helper-1.0.0/README.md` & `web_ext_helper-1.0.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Web Extension Helper
 
-Web Extension Helper is a command-line tool that simplifies the process of building web extensions. It provides a convenient interface to streamline the development and packaging of your web extensions.
+[Web Extension Helper](https://www.appsolves.dev/python-packages/web-extension-helper) is a command-line tool that simplifies the process of building web extensions. It provides a convenient interface to streamline the development and packaging of your web extensions.
 
 ## Features
 
 - Easily scaffold a new web extension project.
 - Automate common tasks like bundling and minification.
 - Simplify the process of publishing your web extension.
 
@@ -36,18 +36,18 @@
 
 * View the help menu
 web-ext-helper --help
 ```
 
 ## Documentation
 
-For more information, please visit the [documentation](https://www.appsolves.dev/docs/web-ext-helper/).
+For more information, please visit the [documentation](https://www.appsolves.dev/python-packages/web-extension-helper/documentation).
 
 ## License
-This project is licensed under the terms of the [GNU GPL v3.0 license](LICENSE).
+This project is licensed under the terms of the [GNU GPL v3.0 license](https://www.appsolves.dev/python-packages/web-extension-helper/license).
 
 # Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please create an issue or submit a pull request.
 
 # Credits
```

### Comparing `web_ext_helper-1.0.0/web_ext_helper/web_ext_helper.py` & `web_ext_helper-1.0.1/web_ext_helper/web_ext_helper.py`

 * *Files identical despite different names*

### Comparing `web_ext_helper-1.0.0/PKG-INFO` & `web_ext_helper-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: web-ext-helper
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple cli tool that helps you building your web extensions.
 License: GPL-3.0-or-later
 Author: AppSolves
 Author-email: appsolves@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Web Extension Helper
 
-Web Extension Helper is a command-line tool that simplifies the process of building web extensions. It provides a convenient interface to streamline the development and packaging of your web extensions.
+[Web Extension Helper](https://www.appsolves.dev/python-packages/web-extension-helper) is a command-line tool that simplifies the process of building web extensions. It provides a convenient interface to streamline the development and packaging of your web extensions.
 
 ## Features
 
 - Easily scaffold a new web extension project.
 - Automate common tasks like bundling and minification.
 - Simplify the process of publishing your web extension.
 
@@ -49,18 +49,18 @@
 
 * View the help menu
 web-ext-helper --help
 ```
 
 ## Documentation
 
-For more information, please visit the [documentation](https://www.appsolves.dev/docs/web-ext-helper/).
+For more information, please visit the [documentation](https://www.appsolves.dev/python-packages/web-extension-helper/documentation).
 
 ## License
-This project is licensed under the terms of the [GNU GPL v3.0 license](LICENSE).
+This project is licensed under the terms of the [GNU GPL v3.0 license](https://www.appsolves.dev/python-packages/web-extension-helper/license).
 
 # Contributing
 
 Contributions are welcome! If you encounter any issues or have suggestions for improvements, please create an issue or submit a pull request.
 
 # Credits
```

