# Comparing `tmp/micropython-lis3dh-0.1.0.tar.gz` & `tmp/micropython-lis3dh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-lis3dh-0.1.0.tar", last modified: Thu Apr  6 18:50:02 2023, max compression
+gzip compressed data, was "micropython-lis3dh-0.1.1.tar", last modified: Sat Jun 17 15:03:06 2023, max compression
```

## Comparing `micropython-lis3dh-0.1.0.tar` & `micropython-lis3dh-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:50:02.756128 micropython-lis3dh-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:50:02.752128 micropython-lis3dh-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:50:02.752128 micropython-lis3dh-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:50:02.756128 micropython-lis3dh-0.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-06 18:50:02.756128 micropython-lis3dh-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:50:02.756128 micropython-lis3dh-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:50:02.756128 micropython-lis3dh-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:50:02.756128 micropython-lis3dh-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-06 18:49:55.000000 micropython-lis3dh-0.1.0/examples/lis3dh_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-06 18:49:55.000000 micropython-lis3dh-0.1.0/lis3dh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 18:50:02.756128 micropython-lis3dh-0.1.0/micropython_lis3dh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-06 18:50:02.000000 micropython-lis3dh-0.1.0/micropython_lis3dh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-06 18:50:02.000000 micropython-lis3dh-0.1.0/micropython_lis3dh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 18:50:02.000000 micropython-lis3dh-0.1.0/micropython_lis3dh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-06 18:50:02.000000 micropython-lis3dh-0.1.0/micropython_lis3dh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-06 18:50:02.000000 micropython-lis3dh-0.1.0/micropython_lis3dh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-06 18:49:55.000000 micropython-lis3dh-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-06 18:49:45.000000 micropython-lis3dh-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 18:50:02.756128 micropython-lis3dh-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.389334 micropython-lis3dh-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.381333 micropython-lis3dh-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-17 15:03:06.389334 micropython-lis3dh-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/examples/lis3dg_data_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/examples/lis3dh_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/examples/lis3dh_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.385334 micropython-lis3dh-0.1.1/micropython_lis3dh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/micropython_lis3dh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/micropython_lis3dh/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/micropython_lis3dh/lis3dh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:03:06.389334 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 15:03:06.000000 micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-17 15:02:58.000000 micropython-lis3dh-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 15:02:51.000000 micropython-lis3dh-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:03:06.389334 micropython-lis3dh-0.1.1/setup.cfg
```

### Comparing `micropython-lis3dh-0.1.0/.gitignore` & `micropython-lis3dh-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.0/.pre-commit-config.yaml` & `micropython-lis3dh-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.0/.pylintrc` & `micropython-lis3dh-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.0/LICENSE` & `micropython-lis3dh-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-lis3dh-0.1.0/PKG-INFO` & `micropython-lis3dh-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,89 @@
 Metadata-Version: 2.1
 Name: micropython-lis3dh
-Version: 0.1.0
+Version: 0.1.1
 Summary: LIS3DH MicroPython Driver
 Author-email: "Jose D. Montoya" <lis3dh@mailmeto.mozmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/jposada202020/LIS3DH
+Project-URL: Homepage, https://github.com/jposada202020/MicroPython_LIS3DH
 Keywords: micropython,lis3dh,sernsor,acceleration,tap,movement,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 
-.. image:: https://readthedocs.org/projects/circuitpython-lis3dh/badge/?version=latest
-    :target: https://micropython-lis3dh.readthedocs.io/
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
+.. image:: https://readthedocs.org/projects/lis3dh/badge/?version=latest
+    :target: https://lis3dh.readthedocs.io/
     :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/v/micropython-lis3dh.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/micropython-lis3dh
+
+.. image:: https://static.pepy.tech/personalized-badge/micropython-lis3dh?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-lis3dh
+
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-LIS3DH MicroPython Driver
+LIS3DH MicroPython Driver. Work is based in:
+    * https://github.com/adafruit/Adafruit_CircuitPython_LIS3DH/
+    * https://github.com/adafruit/Adafruit_CircuitPython_Register
+
+
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_LIS3DH
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_LIS3DH
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_LIS3DH/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_LIS3DH/examples.json
+
+
+
+Installation
+=============
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-lis3dh/>`_.
 To install for current user:
 
 .. code-block:: shell
```

### Comparing `micropython-lis3dh-0.1.0/docs/conf.py` & `micropython-lis3dh-0.1.1/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,41 +8,36 @@
 import sys
 import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
-# Add any Sphinx extension module names here, as strings. They can be
-# extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
-# ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
+    "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
+    "sphinx_immaterial",
 ]
 
 # autodoc_mock_imports = [""]
 
 autodoc_preserve_defaults = True
 
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "MicroPython": ("https://docs.micropython.org/en/latest/", None),
 }
 
-# Show the docstring from both the class and its __init__() method.
 autoclass_content = "both"
-
-# Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
-
 source_suffix = ".rst"
-
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "MicroPython LIS3DH Library"
 creation_year = "2023"
 current_year = str(datetime.datetime.now().year)
@@ -58,77 +53,158 @@
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = "1.0"
 # The full version, including alpha/beta/rc tags.
 release = "1.0"
-
-# The language for content autogenerated by Sphinx. Refer to documentation
-# for a list of supported languages.
-#
-# This is also used if you do content translation via gettext catalogs.
-# Usually you set "language" from the command line for these cases.
+html_baseurl = "https://micropython-lisd3h.readthedocs.io/"
 language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = [
-    "_build",
-    "Thumbs.db",
-    ".DS_Store",
-    ".env",
-]
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", ".env", "requirements.txt"]
 
 # The reST default role (used for this markup: `text`) to use for all
 # documents.
 #
 default_role = "any"
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 #
 add_function_parentheses = True
 
-# The name of the Pygments (syntax highlighting) style to use.
-pygments_style = "sphinx"
+rst_prolog = """
+.. role:: python(code)
+   :language: python
+   :class: highlight
+.. default-literal-role:: python
+"""
+
 todo_include_todos = False
-todo_emit_warnings = True
+todo_emit_warnings = False
 napoleon_numpy_docstring = False
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-#
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+html_theme = "sphinx_immaterial"
 
-if not on_rtd:  # only import and set the theme if we're building docs locally
-    try:
-        import sphinx_rtd_theme
-
-        html_theme = "sphinx_rtd_theme"
-        html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
-    except:
-        html_theme = "default"
-        html_theme_path = ["."]
-else:
-    html_theme_path = ["."]
+html_theme_options = {
+    "features": [
+        "search.share",
+    ],
+    # Set the color and the accent color
+    "palette": [
+        {
+            "media": "(prefers-color-scheme: light)",
+            "scheme": "default",
+            "primary": "purple",
+            "accent": "light-blue",
+            "toggle": {
+                "icon": "material/lightbulb-outline",
+                "name": "Switch to dark mode",
+            },
+        },
+        {
+            "media": "(prefers-color-scheme: dark)",
+            "scheme": "slate",
+            "primary": "purple",
+            "accent": "light-blue",
+            "toggle": {
+                "icon": "material/lightbulb",
+                "name": "Switch to light mode",
+            },
+        },
+    ],
+    # Set the repo location to get a badge with stats
+    "repo_url": "https://github.com/jposada202020/MicroPython_LIS3DH/",
+    "repo_name": "MicroPython LIS3DH",
+    "social": [
+        {
+            "icon": "fontawesome/brands/github",
+            "link": "https://github.com/jposada202020/MicroPython_LIS3DH",
+        },
+        {
+            "icon": "fontawesome/brands/python",
+            "link": "https://pypi.org/project/micropython-lis3dh/",
+        },
+        {
+            "name": "MicroPython Downloads",
+            "icon": "octicons/download-24",
+            "link": "https://micropython.org",
+        },
+    ],
+}
+
+sphinx_immaterial_custom_admonitions = [
+    {
+        "name": "warning",
+        "color": (255, 66, 66),
+        "icon": "octicons/alert-24",
+        "override": True,
+    },
+    {
+        "name": "note",
+        "icon": "octicons/pencil-24",
+        "override": True,
+    },
+    {
+        "name": "seealso",
+        "color": (255, 66, 252),
+        "icon": "octicons/eye-24",
+        "title": "See Also",
+        "override": True,
+    },
+    {
+        "name": "hint",
+        "icon": "material/school",
+        "override": True,
+    },
+    {
+        "name": "tip",
+        "icon": "material/school",
+        "override": True,
+    },
+    {
+        "name": "important",
+        "icon": "material/school",
+        "override": True,
+    },
+]
+
+python_type_aliases = {
+    "DigitalInOut": "digitalio.DigitalInOut",
+}
+
+object_description_options = [
+    ("py:.*", dict(generate_synopses="first_sentence")),
+]
+
+# Set link name generated in the top bar.
+html_title = "MicroPython LIS3DH"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
+# These paths are either relative to html_static_path
+# or fully qualified paths (eg. https://...)
+html_css_files = ["extra_css.css"]
+
 # The name of an image file (relative to this directory) to use as a favicon of
 # the docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 #
 html_favicon = "_static/favicon.ico"
 
+html_logo = "_static/Logo.png"
 # Output file base name for HTML help builder.
 htmlhelp_basename = "MicroPython_Lis3dh_Librarydoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
```

### Comparing `micropython-lis3dh-0.1.0/lis3dh.py` & `micropython-lis3dh-0.1.1/micropython_lis3dh/lis3dh.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,22 @@
 LIS3DH MicroPython Driver
 
 
 * Author(s): Jose D. Montoya
 
 
 """
-# pylint: disable=unused-argument
+# pylint: disable=unused-argument, no-name-in-module
 
 import time
 from micropython import const
+from micropython_lis3dh.i2c_helpers import RegisterStruct, CBits
 
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
-
-
-__version__ = "0.1.0"
-__repo__ = "https://github.com/jposada202020/LIS3DH.git"
+__version__ = "0.1.1"
+__repo__ = "https://github.com/jposada202020/MicroPython_LIS3DH.git"
 
 
 _REG_WHOAMI = const(0x0F)
 _REG_TEMPCFG = const(0x1F)
 _REG_CTRL1 = const(0x20)  # Defaults to 0b00000000
 _REG_CTRL3 = const(0x22)
 _REG_CTRL4 = const(0x23)
@@ -50,94 +45,55 @@
 
 # Data Range
 DATARANGE_2 = const(0b00)  # +/- 2g (default value)
 DATARANGE_4 = const(0b01)  # +/- 4g
 DATARANGE_8 = const(0b10)  # +/- 8g
 DATARANGE_16 = const(0b11)  # +/- 16g
 
+# Axes Enabling
 AXES_X = const(0b001)
 AXES_Y = const(0b010)
 AXES_X_Y = const(0b011)
 AXES_Z = const(0b100)
 AXES_Z_X = const(0b101)
 AXES_Z_Y = const(0b110)
 AXES_Z_Y_X = const(0b111)
 
 
-class CBits:
-    """
-    Changes bits from a byte register
-    """
-
-    def __init__(self, num_bits: int, register_address: int, start_bit: int) -> None:
-        self.bit_mask = ((1 << num_bits) - 1) << start_bit
-        self.register = register_address
-        self.star_bit = start_bit
-
-    def __get__(
-        self,
-        obj,
-        objtype=None,
-    ) -> int:
-
-        reg = obj._i2c.readfrom_mem(obj._address, self.register, True)[0]
-        reg = (reg & self.bit_mask) >> self.star_bit
-
-        return reg
-
-    def __set__(self, obj, value: int) -> None:
+class LIS3DH:
+    """Main class for the Sensor
 
-        memory_value = obj._i2c.readfrom_mem(obj._address, self.register, True)[0]
-        memory_value &= ~self.bit_mask
+    :param ~machine.I2C i2c: The I2C bus the LIS3DH is connected to.
+    :param int address: The I2C device address. Defaults to :const:`0x18`
 
-        value <<= self.star_bit
-        memory_value |= value
+    :raises RuntimeError: if the sensor is not found
 
-        obj._i2c.writeto_mem(obj._address, self.register, bytes([memory_value]))
 
+    **Quickstart: Importing and using the device**
 
-class RegisterStruct:
-    """
-    Register Struct
-    """
+    Here is an example of using the :class:`lis3dh.LIS3DH` class.
+    First you will need to import the libraries to use the sensor
 
-    def __init__(self, register_address: int, form: str, lenght=1) -> None:
-        self.format = form
-        self.register = register_address
-        self.lenght = struct.calcsize(form)
-
-    def __get__(
-        self,
-        obj,
-        objtype=None,
-    ):
-        if self.lenght == 1:
-            value = obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)[0]
-        else:
-            value = struct.unpack(
-                self.format,
-                memoryview(
-                    obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
-                ),
-            )
+    .. code-block:: python
 
-        return value
+        from machine import Pin, I2C
+        from micropython_lis3dh import lis3dh
 
-    def __set__(self, obj, value):
+    Once this is done you can define your `machine.I2C` object and define your sensor object
 
-        obj._i2c.writeto_mem(obj._address, self.register, bytes([value]))
+    .. code-block:: python
 
+        i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
+        lis = lis3dh.LIS3DH(i2c)
 
-class LIS3DH:
-    """Main class for the Sensor
+    Now you have access to the :attr:`acceleration` attribute
 
-    :param ~machine.I2C i2c: The I2C bus the LIS3DH is connected to.
-    :param int address: The I2C device address. Defaults to :const:`0x18`
+    .. code-block:: python
 
-    :raises RuntimeError: if the sensor is not found
+        acc_x, acc_y, acc_z = lis3dh.acceleration
 
     """
 
     _device_id = RegisterStruct(_REG_WHOAMI, "B")
     _device_control = RegisterStruct(_REG_CTRL1, "B")
     _reboot_register = RegisterStruct(_REG_CTRL5, "B")
     _ctrl4_register = RegisterStruct(_REG_CTRL4, "B")
@@ -176,15 +132,17 @@
         self._data_rate = DATARATE_400
         self._high_resolution = 1
         self._block_data = 1
         self._adc_pd = 1
 
     @property
     def axes_enabled(self):
-        """The data rate of the accelerometer
+        """The data rate of the accelerometer. you could selected different axes to
+        be on. Take a look at the table to select the Aces that you are interested
+        in.
 
         +--------------------------------------------+-------------------------+
         | Mode                                       | Value                   |
         +============================================+=========================+
         | :py:const:`lis3dh.AXES_X`                  | :py:const:`0b001`       |
         +--------------------------------------------+-------------------------+
         | :py:const:`lis3dh.AXES_Y`                  | :py:const:`0b010`       |
@@ -209,14 +167,16 @@
     def axes_enabled(self, value):
 
         self._axes_enabled = value
 
     @property
     def data_rate(self):
         """The data rate of the accelerometer
+        ODR <3:0> is used to set power mode and ODR selection. In the following
+        table are reported all frequency resulting in combination of ODR<3:0>
 
         +--------------------------------------------+-------------------------+
         | Mode                                       | Value                   |
         +============================================+=========================+
         | :py:const:`lis3dh.DATARATE_1`              | :py:const:`0b0001`      |
         +--------------------------------------------+-------------------------+
         | :py:const:`lis3dh.DATARATE_10`             | :py:const:`0b0010`      |
@@ -246,16 +206,18 @@
 
     @data_rate.setter
     def data_rate(self, value):
 
         self._data_rate = value
 
     @property
-    def range(self):
-        """The range of the accelerometer.
+    def data_range(self):
+        """The range of the accelerometer. The LIS3DH has dynamically user
+        selectable full scales of ±2g/±4g/±8g/±16g and it is capable of
+        measuring accelerations with output data rates from 1 Hz to 5 kHz.
 
         +--------------------------------------------+-------------------------+
         | Mode                                       | Value                   |
         +============================================+=========================+
         | :py:const:`lis3dh.DATARANGE_2`             | :py:const:`0b00`        |
         +--------------------------------------------+-------------------------+
         | :py:const:`lis3dh.DATARANGE_4`             | :py:const:`0b01`        |
@@ -266,23 +228,23 @@
         +--------------------------------------------+-------------------------+
 
 
         """
 
         return self._range
 
-    @range.setter
-    def range(self, value):
+    @data_range.setter
+    def data_range(self, value):
         self._range = value
 
     @property
     def acceleration(self):
         """
         The x, y, z acceleration values returned in a 3-tuple and are in :math:`m/s^2`
 
         """
 
         x, y, z = self._reg_xl
 
-        factor = self.acceleration_scale[self.range]
+        factor = self.acceleration_scale[self.data_range]
 
         return (x / factor) * 9.806, (y / factor) * 9.806, (z / factor) * 9.806
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `micropython-lis3dh-0.1.0/micropython_lis3dh.egg-info/PKG-INFO` & `micropython-lis3dh-0.1.1/micropython_lis3dh.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,89 @@
 Metadata-Version: 2.1
 Name: micropython-lis3dh
-Version: 0.1.0
+Version: 0.1.1
 Summary: LIS3DH MicroPython Driver
 Author-email: "Jose D. Montoya" <lis3dh@mailmeto.mozmail.com>
 License: MIT
-Project-URL: Homepage, https://github.com/jposada202020/LIS3DH
+Project-URL: Homepage, https://github.com/jposada202020/MicroPython_LIS3DH
 Keywords: micropython,lis3dh,sernsor,acceleration,tap,movement,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: MicroPython
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 
-.. image:: https://readthedocs.org/projects/circuitpython-lis3dh/badge/?version=latest
-    :target: https://micropython-lis3dh.readthedocs.io/
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
+.. image:: https://readthedocs.org/projects/lis3dh/badge/?version=latest
+    :target: https://lis3dh.readthedocs.io/
     :alt: Documentation Status
 
+.. image:: https://img.shields.io/pypi/v/micropython-lis3dh.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/micropython-lis3dh
+
+.. image:: https://static.pepy.tech/personalized-badge/micropython-lis3dh?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-lis3dh
+
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-LIS3DH MicroPython Driver
+LIS3DH MicroPython Driver. Work is based in:
+    * https://github.com/adafruit/Adafruit_CircuitPython_LIS3DH/
+    * https://github.com/adafruit/Adafruit_CircuitPython_Register
+
+
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_LIS3DH
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_LIS3DH
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_LIS3DH/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_LIS3DH/examples.json
+
+
+
+Installation
+=============
 
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-lis3dh/>`_.
 To install for current user:
 
 .. code-block:: shell
```

### Comparing `micropython-lis3dh-0.1.0/pyproject.toml` & `micropython-lis3dh-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,20 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-lis3dh"
 description = "LIS3DH MicroPython Driver"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "lis3dh@mailmeto.mozmail.com"}
 ]
-urls = {Homepage = "https://github.com/jposada202020/LIS3DH"}
+urls = {Homepage = "https://github.com/jposada202020/MicroPython_LIS3DH"}
 keywords = [
     "micropython",
     "lis3dh",
     "sernsor",
     "acceleration",
     "tap",
     "movement",
@@ -30,16 +30,16 @@
 license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: System :: Hardware",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: Implementation :: MicroPython",
 ]
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools]
-py-modules = ["lis3dh"]
+packages = ["micropython_lis3dh"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
```

