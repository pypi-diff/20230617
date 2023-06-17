# Comparing `tmp/holy-diver-0.1.0a1.tar.gz` & `tmp/holy-diver-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holy-diver-0.1.0a1.tar", last modified: Sat Jun 17 03:51:43 2023, max compression
+gzip compressed data, was "holy-diver-0.1.0a2.tar", last modified: Sat Jun 17 04:27:44 2023, max compression
```

## Comparing `holy-diver-0.1.0a1.tar` & `holy-diver-0.1.0a2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 03:51:43.421922 holy-diver-0.1.0a1/
--rw-rw-rw-   0        0        0      174 2023-06-17 01:41:06.000000 holy-diver-0.1.0a1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3681 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      114 2023-06-17 03:50:16.000000 holy-diver-0.1.0a1/HISTORY.rst
--rw-rw-rw-   0        0        0     1093 2023-06-17 01:41:06.000000 holy-diver-0.1.0a1/LICENSE
--rw-rw-rw-   0        0        0      273 2023-06-17 01:41:06.000000 holy-diver-0.1.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0    11785 2023-06-17 03:51:43.421922 holy-diver-0.1.0a1/PKG-INFO
--rw-rw-rw-   0        0        0    10635 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-17 03:51:43.390509 holy-diver-0.1.0a1/docs/
--rw-rw-rw-   0        0        0      631 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/docs/Makefile
--rw-rw-rw-   0        0        0       29 2023-06-17 01:41:06.000000 holy-diver-0.1.0a1/docs/authors.rst
--rw-rw-rw-   0        0        0     5038 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-06-17 01:41:06.000000 holy-diver-0.1.0a1/docs/contributing.rst
--rw-rw-rw-   0        0        0       29 2023-06-17 01:41:06.000000 holy-diver-0.1.0a1/docs/history.rst
--rw-rw-rw-   0        0        0      315 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/docs/index.rst
--rw-rw-rw-   0        0        0     1201 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/docs/installation.rst
--rwxrwxrwx   0        0        0      808 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/docs/make.bat
--rw-rw-rw-   0        0        0       28 2023-06-17 01:41:06.000000 holy-diver-0.1.0a1/docs/readme.rst
--rw-rw-rw-   0        0        0       82 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/docs/usage.rst
-drwxrwxrwx   0        0        0        0 2023-06-17 03:51:43.404416 holy-diver-0.1.0a1/holy_diver/
--rw-rw-rw-   0        0        0      234 2023-06-17 03:41:41.000000 holy-diver-0.1.0a1/holy_diver/__init__.py
--rw-rw-rw-   0        0        0    18814 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/holy_diver/config.py
--rw-rw-rw-   0        0        0     9112 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/holy_diver/config_list.py
--rw-rw-rw-   0        0        0      210 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/holy_diver/constants.py
-drwxrwxrwx   0        0        0        0 2023-06-17 03:51:43.410931 holy-diver-0.1.0a1/holy_diver.egg-info/
--rw-rw-rw-   0        0        0    11785 2023-06-17 03:51:43.000000 holy-diver-0.1.0a1/holy_diver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-06-17 03:51:43.000000 holy-diver-0.1.0a1/holy_diver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 03:51:43.000000 holy-diver-0.1.0a1/holy_diver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-17 03:51:43.000000 holy-diver-0.1.0a1/holy_diver.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-06-17 03:51:43.000000 holy-diver-0.1.0a1/holy_diver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      449 2023-06-17 03:51:43.422922 holy-diver-0.1.0a1/setup.cfg
--rw-rw-rw-   0        0        0     2026 2023-06-17 03:50:36.000000 holy-diver-0.1.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 03:51:43.421922 holy-diver-0.1.0a1/tests/
--rw-rw-rw-   0        0        0       41 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/tests/__init__.py
--rw-rw-rw-   0        0        0    18151 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/tests/test_config.py
--rw-rw-rw-   0        0        0     7795 2023-06-17 03:21:18.000000 holy-diver-0.1.0a1/tests/test_config_list.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:27:44.698923 holy-diver-0.1.0a2/
+-rw-rw-rw-   0        0        0      174 2023-06-17 01:41:06.000000 holy-diver-0.1.0a2/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3681 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      114 2023-06-17 04:26:55.000000 holy-diver-0.1.0a2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1093 2023-06-17 01:41:06.000000 holy-diver-0.1.0a2/LICENSE
+-rw-rw-rw-   0        0        0      273 2023-06-17 01:41:06.000000 holy-diver-0.1.0a2/MANIFEST.in
+-rw-rw-rw-   0        0        0    11660 2023-06-17 04:27:44.698923 holy-diver-0.1.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0    10508 2023-06-17 04:18:28.000000 holy-diver-0.1.0a2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-17 04:27:44.685897 holy-diver-0.1.0a2/docs/
+-rw-rw-rw-   0        0        0      631 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/docs/Makefile
+-rw-rw-rw-   0        0        0       29 2023-06-17 01:41:06.000000 holy-diver-0.1.0a2/docs/authors.rst
+-rw-rw-rw-   0        0        0     5038 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2023-06-17 01:41:06.000000 holy-diver-0.1.0a2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2023-06-17 01:41:06.000000 holy-diver-0.1.0a2/docs/history.rst
+-rw-rw-rw-   0        0        0      315 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/docs/index.rst
+-rw-rw-rw-   0        0        0     1201 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/docs/installation.rst
+-rwxrwxrwx   0        0        0      808 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2023-06-17 01:41:06.000000 holy-diver-0.1.0a2/docs/readme.rst
+-rw-rw-rw-   0        0        0       82 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/docs/usage.rst
+drwxrwxrwx   0        0        0        0 2023-06-17 04:27:44.687897 holy-diver-0.1.0a2/holy_diver/
+-rw-rw-rw-   0        0        0      234 2023-06-17 04:26:55.000000 holy-diver-0.1.0a2/holy_diver/__init__.py
+-rw-rw-rw-   0        0        0    18814 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/holy_diver/config.py
+-rw-rw-rw-   0        0        0     9112 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/holy_diver/config_list.py
+-rw-rw-rw-   0        0        0      210 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/holy_diver/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:27:44.696923 holy-diver-0.1.0a2/holy_diver.egg-info/
+-rw-rw-rw-   0        0        0    11660 2023-06-17 04:27:44.000000 holy-diver-0.1.0a2/holy_diver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-06-17 04:27:44.000000 holy-diver-0.1.0a2/holy_diver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 04:27:44.000000 holy-diver-0.1.0a2/holy_diver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-17 04:27:44.000000 holy-diver-0.1.0a2/holy_diver.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2023-06-17 04:27:44.000000 holy-diver-0.1.0a2/holy_diver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      449 2023-06-17 04:27:44.702046 holy-diver-0.1.0a2/setup.cfg
+-rw-rw-rw-   0        0        0     2026 2023-06-17 04:27:30.000000 holy-diver-0.1.0a2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 04:27:44.698923 holy-diver-0.1.0a2/tests/
+-rw-rw-rw-   0        0        0       41 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/tests/__init__.py
+-rw-rw-rw-   0        0        0    18151 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/tests/test_config.py
+-rw-rw-rw-   0        0        0     7795 2023-06-17 03:21:18.000000 holy-diver-0.1.0a2/tests/test_config_list.py
```

### Comparing `holy-diver-0.1.0a1/CONTRIBUTING.rst` & `holy-diver-0.1.0a2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/LICENSE` & `holy-diver-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/PKG-INFO` & `holy-diver-0.1.0a2/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: holy-diver
-Version: 0.1.0a1
-Summary: A dot-accessible configuration manager for deeply nested configuration files.
-Home-page: https://github.com/ndgigliotti/holy-diver
-Download-URL: https://github.com/ndgigliotti/holy-diver/archive/refs/tags/v0.1.0-alpha.1.tar.gz
-Author: Nick Gigliotti
-Author-email: ndgigliotti@gmail.com
-License: MIT license
-Keywords: holy_diver,holy-diver,dot config,config,configuration,config file,configuration file,configuration manager,config manager,configuration management,yaml,json,dot accessible,dot-accessible,attribute,attribute accessible,attribute-accessible,recursive,nested,nested configuration,nested config,deeply nested
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 ==========
 holy-diver
 ==========
 
 
 .. image:: https://img.shields.io/pypi/v/holy-diver.svg
         :target: https://pypi.python.org/pypi/holy-diver
@@ -52,15 +30,15 @@
 Installation
 ============
 
 To install holy-diver, simply run:
 
 .. code-block:: bash
 
-    pip install https://github.com/ndgigliotti/holy-diver.git
+    pip install holy-diver
 
 Usage
 =====
 
 Config
 -------------
 
@@ -328,12 +306,9 @@
 ``holy-diver`` is released under the MIT License. See the LICENSE file for more details.
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
-Icon created by Smartline_.
-
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _Smartline: https://www.flaticon.com/authors/smartline
+.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

### Comparing `holy-diver-0.1.0a1/README.rst` & `holy-diver-0.1.0a2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: holy-diver
+Version: 0.1.0a2
+Summary: A dot-accessible configuration manager for deeply nested configuration files.
+Home-page: https://github.com/ndgigliotti/holy-diver
+Download-URL: https://github.com/ndgigliotti/holy-diver/archive/refs/tags/v0.1.0-alpha.2.tar.gz
+Author: Nick Gigliotti
+Author-email: ndgigliotti@gmail.com
+License: MIT license
+Keywords: holy_diver,holy-diver,dot config,config,configuration,config file,configuration file,configuration manager,config manager,configuration management,yaml,json,dot accessible,dot-accessible,attribute,attribute accessible,attribute-accessible,recursive,nested,nested configuration,nested config,deeply nested
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+
 ==========
 holy-diver
 ==========
 
 
 .. image:: https://img.shields.io/pypi/v/holy-diver.svg
         :target: https://pypi.python.org/pypi/holy-diver
@@ -30,15 +52,15 @@
 Installation
 ============
 
 To install holy-diver, simply run:
 
 .. code-block:: bash
 
-    pip install https://github.com/ndgigliotti/holy-diver.git
+    pip install holy-diver
 
 Usage
 =====
 
 Config
 -------------
 
@@ -306,12 +328,9 @@
 ``holy-diver`` is released under the MIT License. See the LICENSE file for more details.
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
-Icon created by Smartline_.
-
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _Smartline: https://www.flaticon.com/authors/smartline
```

### Comparing `holy-diver-0.1.0a1/docs/Makefile` & `holy-diver-0.1.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/docs/conf.py` & `holy-diver-0.1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/docs/installation.rst` & `holy-diver-0.1.0a2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/docs/make.bat` & `holy-diver-0.1.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/holy_diver/config.py` & `holy-diver-0.1.0a2/holy_diver/config.py`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/holy_diver/config_list.py` & `holy-diver-0.1.0a2/holy_diver/config_list.py`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/holy_diver.egg-info/PKG-INFO` & `holy-diver-0.1.0a2/holy_diver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: holy-diver
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A dot-accessible configuration manager for deeply nested configuration files.
 Home-page: https://github.com/ndgigliotti/holy-diver
-Download-URL: https://github.com/ndgigliotti/holy-diver/archive/refs/tags/v0.1.0-alpha.1.tar.gz
+Download-URL: https://github.com/ndgigliotti/holy-diver/archive/refs/tags/v0.1.0-alpha.2.tar.gz
 Author: Nick Gigliotti
 Author-email: ndgigliotti@gmail.com
 License: MIT license
 Keywords: holy_diver,holy-diver,dot config,config,configuration,config file,configuration file,configuration manager,config manager,configuration management,yaml,json,dot accessible,dot-accessible,attribute,attribute accessible,attribute-accessible,recursive,nested,nested configuration,nested config,deeply nested
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -52,15 +52,15 @@
 Installation
 ============
 
 To install holy-diver, simply run:
 
 .. code-block:: bash
 
-    pip install https://github.com/ndgigliotti/holy-diver.git
+    pip install holy-diver
 
 Usage
 =====
 
 Config
 -------------
 
@@ -328,12 +328,9 @@
 ``holy-diver`` is released under the MIT License. See the LICENSE file for more details.
 
 Credits
 -------
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
-Icon created by Smartline_.
-
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
-.. _Smartline: https://www.flaticon.com/authors/smartline
```

### Comparing `holy-diver-0.1.0a1/holy_diver.egg-info/SOURCES.txt` & `holy-diver-0.1.0a2/holy_diver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/setup.py` & `holy-diver-0.1.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,11 +60,11 @@
         "deeply nested",
     ],
     name="holy-diver",
     packages=find_packages(include=["holy_diver", "holy_diver.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/ndgigliotti/holy-diver",
-    download_url="https://github.com/ndgigliotti/holy-diver/archive/refs/tags/v0.1.0-alpha.1.tar.gz",
-    version="v0.1.0-alpha.1",
+    download_url="https://github.com/ndgigliotti/holy-diver/archive/refs/tags/v0.1.0-alpha.2.tar.gz",
+    version="v0.1.0-alpha.2",
     zip_safe=False,
 )
```

### Comparing `holy-diver-0.1.0a1/tests/test_config.py` & `holy-diver-0.1.0a2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `holy-diver-0.1.0a1/tests/test_config_list.py` & `holy-diver-0.1.0a2/tests/test_config_list.py`

 * *Files identical despite different names*

