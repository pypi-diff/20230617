# Comparing `tmp/micropython-tmp117-0.2.0.tar.gz` & `tmp/micropython-tmp117-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-tmp117-0.2.0.tar", last modified: Sun Apr  9 15:54:09 2023, max compression
+gzip compressed data, was "micropython-tmp117-0.2.1.tar", last modified: Sat Jun 17 14:40:42 2023, max compression
```

## Comparing `micropython-tmp117-0.2.0.tar` & `micropython-tmp117-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:54:09.935938 micropython-tmp117-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:54:09.931938 micropython-tmp117-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:54:09.931938 micropython-tmp117-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-09 15:54:09.935938 micropython-tmp117-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:54:09.935938 micropython-tmp117-0.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:54:09.935938 micropython-tmp117-0.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:54:09.935938 micropython-tmp117-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-09 15:54:02.000000 micropython-tmp117-0.2.0/examples/tmp117_alert_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-09 15:54:02.000000 micropython-tmp117-0.2.0/examples/tmp117_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-09 15:54:02.000000 micropython-tmp117-0.2.0/examples/tmp177_temperature_offset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 15:54:09.935938 micropython-tmp117-0.2.0/micropython_tmp117.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-09 15:54:09.000000 micropython-tmp117-0.2.0/micropython_tmp117.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-09 15:54:09.000000 micropython-tmp117-0.2.0/micropython_tmp117.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 15:54:09.000000 micropython-tmp117-0.2.0/micropython_tmp117.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-09 15:54:09.000000 micropython-tmp117-0.2.0/micropython_tmp117.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-09 15:54:09.000000 micropython-tmp117-0.2.0/micropython_tmp117.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-09 15:54:02.000000 micropython-tmp117-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-09 15:53:55.000000 micropython-tmp117-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 15:54:09.935938 micropython-tmp117-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-04-09 15:54:02.000000 micropython-tmp117-0.2.0/tmp117.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.670043 micropython-tmp117-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.670043 micropython-tmp117-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/examples/tmp117_alert_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/examples/tmp117_averaging_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/examples/tmp117_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/examples/tmp177_temperature_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/examples.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/micropython_tmp117/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/micropython_tmp117/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/micropython_tmp117/i2c_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/micropython_tmp117/tmp117.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-17 14:40:42.000000 micropython-tmp117-0.2.1/micropython_tmp117.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/packages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-17 14:40:35.000000 micropython-tmp117-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-17 14:40:27.000000 micropython-tmp117-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:40:42.674043 micropython-tmp117-0.2.1/setup.cfg
```

### Comparing `micropython-tmp117-0.2.0/.gitignore` & `micropython-tmp117-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `micropython-tmp117-0.2.0/.pre-commit-config.yaml` & `micropython-tmp117-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropython-tmp117-0.2.0/.pylintrc` & `micropython-tmp117-0.2.1/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
 # disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
-disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding,consider-using-from-import
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
```

### Comparing `micropython-tmp117-0.2.0/LICENSE` & `micropython-tmp117-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-tmp117-0.2.0/PKG-INFO` & `micropython-tmp117-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,91 @@
 Metadata-Version: 2.1
 Name: micropython-tmp117
-Version: 0.2.0
+Version: 0.2.1
 Summary: MicroPython Driver for the TMP117 temperature sensor
 Author-email: "Jose D. Montoya" <tmp117@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/micropython_TMP117
 Keywords: micropython,tmp117,temperature,sensor
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
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/tmp117/badge/?version=latest
     :target: https://tmp117.readthedocs.io/
     :alt: Documentation Status
 
 
+.. image:: https://img.shields.io/pypi/v/micropython-tmp117.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/micropython-tmp117
+
+.. image:: https://static.pepy.tech/personalized-badge/micropython-tmp117?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-tmp117
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the TMP117 temperature sensor
 
 Register reding based on
 https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_TMP117
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_TMP117
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_TMP117/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_TMP117/examples.json
+
+
+
+Installation
+===============
+
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-tmp117/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install micropython-tmp117
```

### Comparing `micropython-tmp117-0.2.0/docs/conf.py` & `micropython-tmp117-0.2.1/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,42 +8,36 @@
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
     "sphinx.ext.todo",
+    "sphinx.ext.viewcode",
+    "sphinx_immaterial",
 ]
 
 # autodoc_mock_imports = ["digitalio", "busio"]
 
 autodoc_preserve_defaults = True
 
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
-    "micropython": ("https://docs.micropython.org/en/latest/", None),
+    "MicroPython": ("https://docs.micropython.org/en/latest/", None),
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
 project = "micropython TMP117 Library"
 creation_year = "2023"
 current_year = str(datetime.datetime.now().year)
@@ -59,79 +53,158 @@
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
+html_baseurl = "https://micropython-tmp117.readthedocs.io/"
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
 
 todo_include_todos = False
-todo_emit_warnings = True
-
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
+    "repo_url": "https://github.com/jposada202020/MicroPython_TMP117/",
+    "repo_name": "MicroPython TMP117",
+    "social": [
+        {
+            "icon": "fontawesome/brands/github",
+            "link": "https://github.com/jposada202020/MicroPython_TMP117",
+        },
+        {
+            "icon": "fontawesome/brands/python",
+            "link": "https://pypi.org/project/micropython-tmp117/",
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
+html_title = "MicroPython TMP117"
 
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
 htmlhelp_basename = "Micropython_Tmp117_Librarydoc"
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
```

### Comparing `micropython-tmp117-0.2.0/examples/tmp117_alert_mode.py` & `micropython-tmp117-0.2.1/examples/tmp117_alert_mode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023 Jose D. Montoya
 
 import time
 from machine import Pin, I2C
-import tmp117
+import micropython_tmp117.tmp117 as tmp117
 
 i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
 tmp = tmp117.TMP117(i2c)
 
 tmp.high_limit = 23
 tmp.low_limit = 20
```

### Comparing `micropython-tmp117-0.2.0/micropython_tmp117.egg-info/PKG-INFO` & `micropython-tmp117-0.2.1/micropython_tmp117.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,91 @@
 Metadata-Version: 2.1
 Name: micropython-tmp117
-Version: 0.2.0
+Version: 0.2.1
 Summary: MicroPython Driver for the TMP117 temperature sensor
 Author-email: "Jose D. Montoya" <tmp117@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/micropython_TMP117
 Keywords: micropython,tmp117,temperature,sensor
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
 
 
+.. image:: https://img.shields.io/badge/micropython-Ok-purple.svg
+    :target: https://micropython.org
+    :alt: micropython
+
 .. image:: https://readthedocs.org/projects/tmp117/badge/?version=latest
     :target: https://tmp117.readthedocs.io/
     :alt: Documentation Status
 
 
+.. image:: https://img.shields.io/pypi/v/micropython-tmp117.svg
+    :alt: latest version on PyPI
+    :target: https://pypi.python.org/pypi/micropython-tmp117
+
+.. image:: https://static.pepy.tech/personalized-badge/micropython-tmp117?period=total&units=international_system&left_color=grey&right_color=blue&left_text=Pypi%20Downloads
+    :alt: Total PyPI downloads
+    :target: https://pepy.tech/project/micropython-tmp117
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
 MicroPython Driver for the TMP117 temperature sensor
 
 Register reding based on
 https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 
+Installing with mip
+====================
+
+To install using mpremote
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_TMP117
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_TMP117
+
+
+Installing Library Examples
+============================
+
+If you want to install library examples:
+
+.. code-block:: shell
+
+    mpremote mip install github:jposada202020/MicroPython_TMP117/examples.json
+
+To install directly using a WIFI capable board
+
+.. code-block:: shell
+
+    mip install github:jposada202020/MicroPython_TMP117/examples.json
+
+
+
+Installation
+===============
+
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/micropython-tmp117/>`_.
 To install for current user:
 
 .. code-block:: shell
 
     pip3 install micropython-tmp117
```

### Comparing `micropython-tmp117-0.2.0/micropython_tmp117.egg-info/SOURCES.txt` & `micropython-tmp117-0.2.1/micropython_tmp117.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 LICENSE
 README.rst
+examples.json
 optional_requirements.txt
+packages.json
 pyproject.toml
 requirements.txt
-tmp117.py
 .github/workflows/release_pypi.yml
 docs/api.rst
 docs/conf.py
 docs/examples.rst
 docs/index.rst
 docs/requirements.txt
+docs/_static/Logo.png
+docs/_static/extra_css.css
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/tmp117_alert_mode.py
+examples/tmp117_averaging_measurements.py
 examples/tmp117_simpletest.py
 examples/tmp177_temperature_offset.py
+micropython_tmp117/__init__.py
+micropython_tmp117/i2c_helpers.py
+micropython_tmp117/tmp117.py
 micropython_tmp117.egg-info/PKG-INFO
 micropython_tmp117.egg-info/SOURCES.txt
 micropython_tmp117.egg-info/dependency_links.txt
 micropython_tmp117.egg-info/requires.txt
 micropython_tmp117.egg-info/top_level.txt
```

### Comparing `micropython-tmp117-0.2.0/pyproject.toml` & `micropython-tmp117-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "micropython-tmp117"
 description = "MicroPython Driver for the TMP117 temperature sensor"
-version = "0.2.0"
+version = "0.2.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "tmp117@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/micropython_TMP117"}
 keywords = [
     "micropython",
@@ -28,15 +28,15 @@
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
 py-modules = ["tmp117"]
 
 [tool.setuptools.dynamic]
```

### Comparing `micropython-tmp117-0.2.0/tmp117.py` & `micropython-tmp117-0.2.1/micropython_tmp117/tmp117.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,141 +15,48 @@
 
 **Software and Dependencies:**
 
 This library depends on Micropython
 
 """
 
-# pylint: disable=unused-argument, too-many-arguments
+# pylint: disable=too-many-arguments, line-too-long
 
 import time
 from collections import namedtuple
 from micropython import const
+from micropython_tmp117.i2c_helpers import CBits, RegisterStruct
 
 
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
-
-
-__version__ = "0.2.0"
-__repo__ = "https://github.com/jposada202020/TMP117.git"
+__version__ = "0.2.1"
+__repo__ = "https://github.com/jposada202020/MicroPython_TMP117.git"
 
 
 _REG_WHOAMI = const(0x0F)
 _TEMP_RESULT = const(0x00)
 _CONFIGURATION = const(0x01)
 _TEMP_HIGH_LIMIT = const(0x02)
 _TEMP_LOW_LIMIT = const(0x03)
 _TEMP_OFFSET = const(0x07)
 
-_CONTINUOUS_CONVERSION_MODE = const(0b00)  # Continuous Conversion Mode
-_ONE_SHOT_MODE = const(0b11)  # One Shot Conversion Mode
-_SHUTDOWN_MODE = const(0b01)  # Shutdown Conversion Mode
+CONTINUOUS_CONVERSION_MODE = const(0b00)  # Continuous Conversion Mode
+ONE_SHOT_MODE = const(0b11)  # One Shot Conversion Mode
+SHUTDOWN_MODE = const(0b01)  # Shutdown Conversion Mode
 
 _TMP117_RESOLUTION = const(0.0078125)
 
 AlertStatus = namedtuple("AlertStatus", ["high_alert", "low_alert"])
 ALERT_WINDOW = const(0)
 ALERT_HYSTERESIS = const(1)
 
-
-class CBits:
-    """
-    Changes bits from a byte register
-    """
-
-    def __init__(
-        self,
-        num_bits: int,
-        register_address: int,
-        start_bit: int,
-        register_width=1,
-        lsb_first=True,
-    ) -> None:
-        self.bit_mask = ((1 << num_bits) - 1) << start_bit
-        self.register = register_address
-        self.star_bit = start_bit
-        self.lenght = register_width
-        self.lsb_first = lsb_first
-
-    def __get__(
-        self,
-        obj,
-        objtype=None,
-    ) -> int:
-
-        mem_value = obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
-
-        reg = 0
-        order = range(len(mem_value) - 1, -1, -1)
-        if not self.lsb_first:
-            order = reversed(order)
-        for i in order:
-            reg = (reg << 8) | mem_value[i]
-
-        reg = (reg & self.bit_mask) >> self.star_bit
-
-        return reg
-
-    def __set__(self, obj, value: int) -> None:
-
-        memory_value = obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
-
-        reg = 0
-        order = range(len(memory_value) - 1, -1, -1)
-        if not self.lsb_first:
-            order = range(0, len(memory_value))
-        for i in order:
-            reg = (reg << 8) | memory_value[i]
-        reg &= ~self.bit_mask
-
-        value <<= self.star_bit
-        reg |= value
-        reg = reg.to_bytes(self.lenght, "big")
-
-        obj._i2c.writeto_mem(obj._address, self.register, reg)
-
-
-class RegisterStruct:
-    """
-    Register Struct
-    """
-
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
-
-        if self.lenght <= 2:
-            value = struct.unpack(
-                self.format,
-                memoryview(
-                    obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
-                ),
-            )[0]
-        else:
-            value = struct.unpack(
-                self.format,
-                memoryview(
-                    obj._i2c.readfrom_mem(obj._address, self.register, self.lenght)
-                ),
-            )
-        return value
-
-    def __set__(self, obj, value):
-        mem_value = value.to_bytes(self.lenght, "big")
-        obj._i2c.writeto_mem(obj._address, self.register, mem_value)
+# Conversion Averaging Mode
+AVERAGE_1X = const(0b00)
+AVERAGE_8X = const(0b01)
+AVERAGE_32X = const(0b10)
+AVERAGE_64X = const(0b11)
 
 
 class TMP117:
     """Main class for the Sensor
 
     :param ~machine.I2C i2c: The I2C bus the TMP117 is connected to.
     :param int address: The I2C device address. Defaults to :const:`0x48`
@@ -161,15 +68,15 @@
 
     Here is an example of using the :class:`TMP117` class.
     First you will need to import the libraries to use the sensor
 
     .. code-block:: python
 
         from machine import Pin, I2C
-        import tmp117
+        import micropython_tmp117.tmp117 as tmp117
 
     Once this is done you can define your `machine.I2C` object and define your sensor object
 
     .. code-block:: python
 
         i2c = I2C(sda=Pin(8), scl=Pin(9))
         tmp117 = tmp117.TMP117(i2c)
@@ -194,14 +101,15 @@
     # ----------------------------------------------------------------------------------------
     # CONV0(1)  | AVG1(1) |AVG0(1)   |T/nA(1)    |POL(1)   |DR/Alert(1)   |Soft_Reset|   —
     _high_alert = CBits(1, _CONFIGURATION, 15, 2, False)
     _low_alert = CBits(1, _CONFIGURATION, 14, 2, False)
     _data_ready = CBits(1, _CONFIGURATION, 13, 2, False)
     _mode = CBits(2, _CONFIGURATION, 10, 2, False)
     _soft_reset = CBits(1, _CONFIGURATION, 1, 2, False)
+
     _conversion_averaging_mode = CBits(2, _CONFIGURATION, 5, 2, False)
     _conversion_cycle_bit = CBits(3, _CONFIGURATION, 7, 2, False)
     _raw_alert_mode = CBits(1, _CONFIGURATION, 4, 2, False)
 
     _avg_3 = {0: 1, 1: 1, 2: 1, 3: 1, 4: 1, 5: 4, 6: 8, 7: 16}
     _avg_2 = {0: 0.5, 1: 0.5, 2: 0.5, 3: 0.5, 4: 1, 5: 4, 6: 8, 7: 16}
     _avg_1 = {0: 0.125, 1: 0.125, 2: 0.25, 3: 0.5, 4: 1, 5: 4, 6: 8, 7: 16}
@@ -220,39 +128,35 @@
         # Following a reset, the temperature register reads –256 °C until the first
         # conversion, including averaging, is complete. So we sleep for that amount of time
         time.sleep(
             self._averaging_modes[self._conversion_averaging_mode][
                 self._conversion_cycle_bit
             ]
         )
-        self._mode = _CONTINUOUS_CONVERSION_MODE
+        self._mode = CONTINUOUS_CONVERSION_MODE
         while not self._data_ready:
             time.sleep(0.001)
-        self._read_temperature()
-
-    def _read_temperature(self):
-        return self._raw_temperature * _TMP117_RESOLUTION
+        _ = self._raw_temperature * _TMP117_RESOLUTION
 
     @property
     def temperature(self):
         """The current measured temperature in Celsius"""
 
-        return self._read_temperature()
+        return self._raw_temperature * _TMP117_RESOLUTION
 
     @property
     def temperature_offset(self):
         """User defined temperature offset to be added to measurements from `temperature`.
         In order the see the new change in the temperature we need for the data to be ready.
         There is a time delay calculated according to current configuration.
 
         .. code-block::python
 
-            import time
             from machine import Pin, I2C
-            import tmp117
+            import micropython_tmp117.tmp117 as tmp117
 
             i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
             tmp = tmp117.TMP117(i2c)
 
             print("Temperature without offset: ", tmp.temperature)
             tmp117.temperature_offset = 10.0
             print("Temperature with offset: ", tmp.temperature)
@@ -303,17 +207,16 @@
     @property
     def alert_status(self):
         """The current triggered status of the high and low temperature alerts as a AlertStatus
         named tuple with attributes for the triggered status of each alert.
 
         .. code-block :: python
 
-            import time
             from machine import Pin, I2C
-            import tmp117
+            import micropython_tmp117.tmp117 as tmp117
 
             i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
             tmp = tmp117.TMP117(i2c)
 
             tmp.low_limit = 20
             tmp.high_limit = 23
 
@@ -344,24 +247,130 @@
         measured temperature goes below `high_limit`. Similarly `low_limit` will be True or False
         depending on if the measured temperature is below (`False`) or above(`True`) `low_limit`.
 
         When set to :py:const:`ALERT_HYSTERESIS`, the `high_limit` property will be set to
         `False` when the measured temperature goes below `low_limit`. In this mode, the `low_limit`
         property of `alert_status` will not be set.
 
-        The default is :py:const:`ALERT_WINDOW`"""
+        The default is :py:const:`ALERT_WINDOW`
 
-        return self._raw_alert_mode
+        +----------------------------------------+-------------------------+
+        | Mode                                   | Value                   |
+        +========================================+=========================+
+        | :py:const:`tmp117.ALERT_WINDOW`        | :py:const:`0b0`         |
+        +----------------------------------------+-------------------------+
+        | :py:const:`tmp117.ALERT_HYSTERESIS`    | :py:const:`0b1`         |
+        +----------------------------------------+-------------------------+
+
+        """
+
+        alert_modes = {
+            0: "ALERT_WINDOW",
+            1: "ALERT_HYSTERESIS",
+        }
+
+        return alert_modes[self._raw_alert_mode]
 
     @alert_mode.setter
     def alert_mode(self, value):
-        """The alert_mode of the sensor
 
-        Could have the following values:
+        if value not in [0, 1]:
+            raise ValueError("alert_mode must be set to 0 or 1")
+        self._raw_alert_mode = value
+
+    @property
+    def averaging_measurements(self):
+        """Users can configure the device to report the average of multiple temperature
+        conversions with the AVG[1:0] bits to reduce noise in the conversion results.
+        When the TMP117 is configured to perform averaging with AVG set to 01, the device executes
+        the configured number of conversions to eight. The device accumulates those conversion
+        results and reports the average of all the collected results at the end of the process.
+
+        +----------------------------------------+-------------------------+
+        | Mode                                   | Value                   |
+        +========================================+=========================+
+        | :py:const:`TMP117.AVERAGE_1X`          | :py:const:`0b00`        |
+        +----------------------------------------+-------------------------+
+        | :py:const:`TMP117.AVERAGE_8X`          | :py:const:`0b01`        |
+        +----------------------------------------+-------------------------+
+        | :py:const:`TMP117.AVERAGE_32X`         | :py:const:`0b10`        |
+        +----------------------------------------+-------------------------+
+        | :py:const:`TMP117.AVERAGE_64X`         | :py:const:`0b11`        |
+        +----------------------------------------+-------------------------+
+
+
+        .. code-block::python3
+
+            from machine import Pin, I2C
+            import micropython_tmp117.tmp117 as tmp117
+
+            i2c = I2C(sda=Pin(8), scl=Pin(9))  # Correct I2C pins for UM FeatherS2
+            tmp = tmp117.TMP117(i2c)
 
-        * ALERT_WINDOW
-        * ALERT_HYSTERESIS
+            tmp.averaging_measurements = tmp117.AVERAGE_32X
+            print("Averaging Measurements: ",tmp.averaging_measurements)
+
+            while True:
+                print("Temperature:", tmp.temperature)
+                time.sleep(1)
 
         """
-        if value not in [0, 1]:
-            raise ValueError("alert_mode must be an 0 or 1")
-        self._raw_alert_mode = value
+        average_measure = {
+            0: "AVERAGE_1X",
+            1: "AVERAGE_8X",
+            2: "AVERAGE_32X",
+            3: "AVERAGE_64X",
+        }
+
+        return average_measure[self._conversion_averaging_mode]
+
+    @averaging_measurements.setter
+    def averaging_measurements(self, value: int):
+        if value not in range(0, 4):
+            raise ValueError("Value must be set to 0, 1, 2 or 3")
+        self._conversion_averaging_mode = value
+
+    @property
+    def measurement_mode(self):
+        """Sets the measurement mode, specifying the behavior of how often measurements are taken.
+                `measurement_mode` must be one of:
+
+        When we use the sensor in One shot mode, the sensor will take the average_measurement value
+        into account. However, this measure is done with the formula (15.5 ms × average_time), so in
+        normal operation average_time will be 8, therefore time for measure is 124 ms.
+        (See datasheet. 7.3.2 Averaging for more information). If we use 64, time will be 15.5 x 65 = 992 ms,
+        the standby time will decrease, but the measure is still under 1 Hz cycle.
+        (See Fig 7.2 on the datasheet)
+
+        +----------------------------------------+------------------------------------------------------+
+        | Mode                                   | Behavior                                             |
+        +========================================+======================================================+
+        | :py:const:`MEASUREMENTMODE_CONTINUOUS` | Measurements are made at the interval determined by  |
+        |                                        | `averaging_measurements`.                            |
+        |                                        | `temperature` returns the most recent measurement    |
+        +----------------------------------------+------------------------------------------------------+
+        | :py:const:`MEASUREMENTMODE_ONE_SHOT`   | Take a single measurement with the current number of |
+        |                                        | `averaging_measurements` and switch to               |
+        |                                        | :py:const:`SHUTDOWN` when finished.                  |
+        |                                        | `temperature` will return the new measurement until  |
+        |                                        | `measurement_mode` is set to :py:const:`CONTINUOUS`  |
+        |                                        | or :py:const:`ONE_SHOT` is                           |
+        |                                        | set again.                                           |
+        +----------------------------------------+------------------------------------------------------+
+        | :py:const:`MEASUREMENTMODE_SHUTDOWN`   | The sensor is put into a low power state and no new  |
+        |                                        | measurements are taken.                              |
+        |                                        | `temperature` will return the last measurement until |
+        |                                        | a new `measurement_mode` is selected.                |
+        +----------------------------------------+------------------------------------------------------+
+
+        """
+
+        sensor_modes = {
+            0: "CONTINUOUS_CONVERSION_MODE",
+            1: "SHUTDOWN_MODE",
+            3: "ONE_SHOT_MODE",
+        }
+        return sensor_modes[self._mode]
+
+    @measurement_mode.setter
+    def measurement_mode(self, value: int) -> None:
+        self._mode = value
```

