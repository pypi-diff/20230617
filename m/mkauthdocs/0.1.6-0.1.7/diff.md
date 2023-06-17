# Comparing `tmp/mkauthdocs-0.1.6.tar.gz` & `tmp/mkauthdocs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mkauthdocs-0.1.6.tar", last modified: Sat Oct 12 19:11:35 2019, max compression
+gzip compressed data, was "mkauthdocs-0.1.7.tar", last modified: Sat Jun 17 03:28:13 2023, max compression
```

## Comparing `mkauthdocs-0.1.6.tar` & `mkauthdocs-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/
--rw-rw-r--   0 root         (0) root         (0)       31 2019-10-11 22:51:10.000000 mkauthdocs-0.1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1077 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     5034 2019-10-11 22:51:10.000000 mkauthdocs-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/mkauthdocs/
--rw-rw-r--   0 root         (0) root         (0)     1135 2019-10-11 22:51:10.000000 mkauthdocs-0.1.6/mkauthdocs/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3947 2019-10-11 22:51:47.000000 mkauthdocs-0.1.6/mkauthdocs/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/mkauthdocs/templates/
--rw-rw-r--   0 root         (0) root         (0)     1653 2019-10-11 22:51:10.000000 mkauthdocs-0.1.6/mkauthdocs/templates/login_template.php
--rw-rw-r--   0 root         (0) root         (0)      314 2019-10-11 22:51:10.000000 mkauthdocs-0.1.6/mkauthdocs/templates/session_guard_template.php
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/mkauthdocs.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     1077 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/mkauthdocs.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      337 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/mkauthdocs.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/mkauthdocs.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       57 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/mkauthdocs.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       11 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/mkauthdocs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2019-10-12 19:11:35.000000 mkauthdocs-0.1.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2602 2019-10-12 19:08:32.000000 mkauthdocs-0.1.6/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-17 03:28:13.259179 mkauthdocs-0.1.7/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1083 2023-06-17 03:09:45.000000 mkauthdocs-0.1.7/LICENSE.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       31 2023-06-17 03:09:45.000000 mkauthdocs-0.1.7/MANIFEST.in
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1092 2023-06-17 03:28:13.259179 mkauthdocs-0.1.7/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5504 2023-06-17 03:23:47.000000 mkauthdocs-0.1.7/README.md
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-17 03:28:13.259179 mkauthdocs-0.1.7/mkauthdocs/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1135 2023-06-17 03:09:45.000000 mkauthdocs-0.1.7/mkauthdocs/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3947 2023-06-17 03:09:45.000000 mkauthdocs-0.1.7/mkauthdocs/__main__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-17 03:28:13.259179 mkauthdocs-0.1.7/mkauthdocs/templates/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1695 2023-06-17 03:09:45.000000 mkauthdocs-0.1.7/mkauthdocs/templates/login_template.php
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      279 2023-06-17 03:09:45.000000 mkauthdocs-0.1.7/mkauthdocs/templates/session_guard_template.php
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-06-17 03:28:13.259179 mkauthdocs-0.1.7/mkauthdocs.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1092 2023-06-17 03:28:13.000000 mkauthdocs-0.1.7/mkauthdocs.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      349 2023-06-17 03:28:13.000000 mkauthdocs-0.1.7/mkauthdocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-06-17 03:28:13.000000 mkauthdocs-0.1.7/mkauthdocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       57 2023-06-17 03:28:13.000000 mkauthdocs-0.1.7/mkauthdocs.egg-info/entry_points.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       11 2023-06-17 03:28:13.000000 mkauthdocs-0.1.7/mkauthdocs.egg-info/top_level.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-06-17 03:28:13.259179 mkauthdocs-0.1.7/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2595 2023-06-17 03:26:40.000000 mkauthdocs-0.1.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mkauthdocs-0.1.6/PKG-INFO` & `mkauthdocs-0.1.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mkauthdocs
-Version: 0.1.6
+Version: 0.1.7
 Summary: An authentication tool for mkdocs builds
 Home-page: https://github.com/ctxz/mkauthdocs
 Author: Patrick Pedersen
 Author-email: ctx.xda@gmail.com
 License: UNKNOWN
 Project-URL: Mkdocs, http://www.mkdocs.org/
 Project-URL: Bug Reports, https://github.com/ctxz/mkauthdocs/issues
 Project-URL: Source, https://github.com/ctxz/mkauthdocs/
-Description: Mkauthdocs is a tool specifically made to implement simple authentication around [mkdocs](www.mkdocs.com) builds.
 Keywords: mkdocs authentication documentation
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE.txt
+
+Mkauthdocs is a tool specifically made to implement simple authentication around [mkdocs](www.mkdocs.com) builds.
+
```

### Comparing `mkauthdocs-0.1.6/README.md` & `mkauthdocs-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Mkauthdocs
+# Mkauthdocs <!-- omit in toc -->
 Mkauthdocs is a tool specifically made to implement simple authentication around [mkdocs](www.mkdocs.org) builds.
 
 ![Screenshot](img/Screenshot.png)
 
-## Table of contents
+## Table of contents <!-- omit in toc -->
 - [Installation](#installation)
 - [Usage](#usage)
 - [Functional overview](#functional-overview)
 - [License](#license)
 
 ## Installation
 
@@ -26,14 +26,15 @@
   build_dir          Path to build output directory
 
 optional arguments:
   -h, --help         show this help message and exit
   --heading HEADING  Heading on login page (default: 'Login')
 ```
 
+> **Warning: The password is stored as plain text in the generated php code! Altough this code is only accessible to the server, it is still a risk you should be aware of!**
 > Note: This tool **only** applies on **mkdocs builds**, not previews served by `mkdocs serve`
 
 This section attempts to guide the reader trough a typical use case in oder to provide understanding in a context-based environment.
 
 We begin by building our documentation using mkdocs:
 ```
 mkdocs build
@@ -66,32 +67,30 @@
 Mkauthdocs implements authentication by injecting a minimally customizable login form into the mkdocs build directory (typically `site/`) and appending PHP session guards at the top of every page.
 
 The login page as well as the session guards are generated from templates which can be found in the [mkauthdocs/templates/](mkauthdocs/templates) directory. If necessary, with a bit of php and html skills those can be customized as desired.
 
 **Example of a generated PHP guard for the index page:**
 ```php
 <?php
-	session_start();
-	if (!$_SESSION['login']) {
-		$dirname = $_SERVER['REQUEST_URI'];
-
-		if (substr($dirname, -1) != '/') {
-			$dirname=dirname($dirname).'/';
-		} else {
-			$dirname = preg_replace('~/+~', '/', $dirname);
-		}
+  session_start();
+  if (! isset($_SESSION['login']) || ! $_SESSION['login']) {
+    $dirname = $_SERVER['REQUEST_URI'] ?? '';
+    $dirname = preg_replace('/index.php$/', '', $dirname);
 
-		header("Location: ".$dirname."login.php?redirect=footer.php");
-	}
+    header("Location: ".$dirname."{calibration}login.php?redirect={redirect}");
+  }
 ?>
+
 ```
 
-Access to the site is only granted if the `login` session variable (`$_SESSION['login']`) set to true, otherwise the user is redirected to the login page where he or she is required authenticate himself or herself in order to set `$_SESSION['login']` to true and gain access to the docs.
+Access to the site is restricted based on the state of the `login` session variable (`$_SESSION['login']`). The user is only granted access if the variable is set to `true`. If the `login` variable is not set or is `false`, the user is redirected to the login page.
+
+To gain access, the user must authenticate themselves on the login page. Upon successful authentication, the `$_SESSION['login']` variable is set to `true`, allowing the user to proceed to the documentation.
 
-If the provided credentials match to those set in the generated login page, then the user is redirected to the page he or she attempted to access. The page to which the user is redirected after a successful login, is defined by the `redirect` URL parameter set by the session guards.
+If the provided credentials match those set in the generated login page, the user is redirected to the page they originally attempted to access. The destination page after successful login is determined by the `redirect` URL parameter, which is set by the session guards. This mechanism ensures a smooth transition to the desired page following successful authentication.
 
 ## License
 All files provided by this project fall under the OSS [MIT License](https://en.wikipedia.org/wiki/MIT_License)
 ```
 The MIT License (MIT)
 
 Copyright (c) 2018 Patrick Pedersen
```

### Comparing `mkauthdocs-0.1.6/mkauthdocs/__init__.py` & `mkauthdocs-0.1.7/mkauthdocs/__init__.py`

 * *Files identical despite different names*

### Comparing `mkauthdocs-0.1.6/mkauthdocs/__main__.py` & `mkauthdocs-0.1.7/mkauthdocs/__main__.py`

 * *Files identical despite different names*

### Comparing `mkauthdocs-0.1.6/mkauthdocs/templates/login_template.php` & `mkauthdocs-0.1.7/mkauthdocs/templates/login_template.php`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 <?php
 session_start();
+$uname = $_POST["uname"] ?? '';
+$pwd = $_POST["pwd"] ?? '';
 
-if ($_POST["uname"] == "{username}" && $_POST["pwd"] == "{password}") {
+if ($uname == "{username}" && $pwd == "{password}") {
   $_SESSION['login'] = true;
   header("Location: ".$_GET["redirect"]);
 }
 
 if (isset($_POST['submit'])) {
   print('<div class="alert alert-danger" role="alert"><center>The username or password is invalid</center></div>');
 }
```

### Comparing `mkauthdocs-0.1.6/mkauthdocs.egg-info/PKG-INFO` & `mkauthdocs-0.1.7/mkauthdocs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: mkauthdocs
-Version: 0.1.6
+Version: 0.1.7
 Summary: An authentication tool for mkdocs builds
 Home-page: https://github.com/ctxz/mkauthdocs
 Author: Patrick Pedersen
 Author-email: ctx.xda@gmail.com
 License: UNKNOWN
 Project-URL: Mkdocs, http://www.mkdocs.org/
 Project-URL: Bug Reports, https://github.com/ctxz/mkauthdocs/issues
 Project-URL: Source, https://github.com/ctxz/mkauthdocs/
-Description: Mkauthdocs is a tool specifically made to implement simple authentication around [mkdocs](www.mkdocs.com) builds.
 Keywords: mkdocs authentication documentation
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+License-File: LICENSE.txt
+
+Mkauthdocs is a tool specifically made to implement simple authentication around [mkdocs](www.mkdocs.com) builds.
+
```

### Comparing `mkauthdocs-0.1.6/setup.py` & `mkauthdocs-0.1.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,47 +23,40 @@
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
 long_description = "Mkauthdocs is a tool specifically made to implement simple authentication around [mkdocs](www.mkdocs.com) builds."
 
 setup(
-    name='mkauthdocs',
-    version='0.1.6',
-    description='An authentication tool for mkdocs builds',
+    name="mkauthdocs",
+    version="0.1.7",
+    description="An authentication tool for mkdocs builds",
     long_description=long_description,
-    url='https://github.com/ctxz/mkauthdocs',
-    author='Patrick Pedersen',
-    author_email='ctx.xda@gmail.com',
+    url="https://github.com/ctxz/mkauthdocs",
+    author="Patrick Pedersen",
+    author_email="ctx.xda@gmail.com",
     classifiers=[
-        'Development Status :: 4 - Beta',
-
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Documentation',
-
-        'License :: OSI Approved :: MIT License',
-
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Documentation",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
     ],
-
-    keywords='mkdocs authentication documentation',
-
+    keywords="mkdocs authentication documentation",
     packages=find_packages(),
     include_package_data=True,
-
     entry_points={
-        'console_scripts': [
-            'mkauthdocs=mkauthdocs.__main__:main',
+        "console_scripts": [
+            "mkauthdocs=mkauthdocs.__main__:main",
         ],
     },
-
     project_urls={  # Optional
-        'Mkdocs': 'http://www.mkdocs.org/',
-        'Bug Reports': 'https://github.com/ctxz/mkauthdocs/issues',
-        'Source': 'https://github.com/ctxz/mkauthdocs/',
+        "Mkdocs": "http://www.mkdocs.org/",
+        "Bug Reports": "https://github.com/ctxz/mkauthdocs/issues",
+        "Source": "https://github.com/ctxz/mkauthdocs/",
     },
 )
```

