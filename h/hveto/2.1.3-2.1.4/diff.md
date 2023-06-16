# Comparing `tmp/hveto-2.1.3.tar.gz` & `tmp/hveto-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hveto-2.1.3.tar", last modified: Fri Jun 16 02:32:12 2023, max compression
+gzip compressed data, was "hveto-2.1.4.tar", last modified: Fri Jun 16 22:51:06 2023, max compression
```

## Comparing `hveto-2.1.3.tar` & `hveto-2.1.4.tar`

### file list

```diff
@@ -1,43 +1,62 @@
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 02:32:12.388761 hveto-2.1.3/
--rw-r--r--   0 areeda     (501) staff       (20)    35147 2022-09-06 21:22:40.000000 hveto-2.1.3/LICENSE
--rw-r--r--   0 areeda     (501) staff       (20)       64 2022-09-06 21:22:40.000000 hveto-2.1.3/MANIFEST.in
--rw-r--r--   0 areeda     (501) staff       (20)     3623 2023-06-16 02:32:12.388886 hveto-2.1.3/PKG-INFO
--rw-r--r--   0 areeda     (501) staff       (20)     2361 2022-09-06 21:22:40.000000 hveto-2.1.3/README.rst
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 02:32:12.389819 hveto-2.1.3/hveto/
--rw-r--r--   0 areeda     (501) staff       (20)      971 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)    36428 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/__main__.py
--rw-r--r--   0 areeda     (501) staff       (20)      471 2023-06-16 02:32:12.389873 hveto-2.1.3/hveto/_version.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 02:32:12.385071 hveto-2.1.3/hveto/cli/
--rw-r--r--   0 areeda     (501) staff       (20)      896 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/cli/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)    14369 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/cli/cache_events.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 02:32:12.385857 hveto-2.1.3/hveto/cli/tests/
--rw-r--r--   0 areeda     (501) staff       (20)      811 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/cli/tests/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)     3063 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/cli/tests/test_trace.py
--rw-r--r--   0 areeda     (501) staff       (20)     3976 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/cli/trace.py
--rw-r--r--   0 areeda     (501) staff       (20)    11142 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/config.py
--rw-r--r--   0 areeda     (501) staff       (20)     1698 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/const.py
--rw-r--r--   0 areeda     (501) staff       (20)    10769 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/core.py
--rw-r--r--   0 areeda     (501) staff       (20)    14806 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/html.py
--rw-r--r--   0 areeda     (501) staff       (20)    18816 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/plot.py
--rw-r--r--   0 areeda     (501) staff       (20)     2681 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/segments.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 02:32:12.388564 hveto-2.1.3/hveto/tests/
--rw-r--r--   0 areeda     (501) staff       (20)      749 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/tests/__init__.py
--rw-r--r--   0 areeda     (501) staff       (20)     1266 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/tests/test_core.py
--rw-r--r--   0 areeda     (501) staff       (20)     3905 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/tests/test_html.py
--rw-r--r--   0 areeda     (501) staff       (20)     1731 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/tests/test_plot.py
--rw-r--r--   0 areeda     (501) staff       (20)     2817 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/tests/test_segments.py
--rw-r--r--   0 areeda     (501) staff       (20)     1860 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/tests/test_triggers.py
--rw-r--r--   0 areeda     (501) staff       (20)     2149 2022-09-06 21:22:40.000000 hveto-2.1.3/hveto/tests/test_utils.py
--rw-r--r--   0 areeda     (501) staff       (20)    11219 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/triggers.py
--rw-r--r--   0 areeda     (501) staff       (20)     4882 2023-06-16 02:24:22.000000 hveto-2.1.3/hveto/utils.py
-drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 02:32:12.384242 hveto-2.1.3/hveto.egg-info/
--rw-r--r--   0 areeda     (501) staff       (20)     3623 2023-06-16 02:32:12.000000 hveto-2.1.3/hveto.egg-info/PKG-INFO
--rw-r--r--   0 areeda     (501) staff       (20)      753 2023-06-16 02:32:12.000000 hveto-2.1.3/hveto.egg-info/SOURCES.txt
--rw-r--r--   0 areeda     (501) staff       (20)        1 2023-06-16 02:32:12.000000 hveto-2.1.3/hveto.egg-info/dependency_links.txt
--rw-r--r--   0 areeda     (501) staff       (20)      130 2023-06-16 02:32:12.000000 hveto-2.1.3/hveto.egg-info/entry_points.txt
--rw-r--r--   0 areeda     (501) staff       (20)        1 2022-09-06 21:34:21.000000 hveto-2.1.3/hveto.egg-info/not-zip-safe
--rw-r--r--   0 areeda     (501) staff       (20)      210 2023-06-16 02:32:12.000000 hveto-2.1.3/hveto.egg-info/requires.txt
--rw-r--r--   0 areeda     (501) staff       (20)        6 2023-06-16 02:32:12.000000 hveto-2.1.3/hveto.egg-info/top_level.txt
--rw-r--r--   0 areeda     (501) staff       (20)     2257 2023-06-16 02:32:12.389594 hveto-2.1.3/setup.cfg
--rw-r--r--   0 areeda     (501) staff       (20)     1184 2022-09-06 21:22:40.000000 hveto-2.1.3/setup.py
--rw-r--r--   0 areeda     (501) staff       (20)    65747 2022-09-06 21:22:40.000000 hveto-2.1.3/versioneer.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.073819 hveto-2.1.4/
+-rw-r--r--   0 areeda     (501) staff       (20)      184 2022-09-06 21:22:40.000000 hveto-2.1.4/.codecov.yml
+-rw-r--r--   0 areeda     (501) staff       (20)      314 2023-06-16 22:35:30.000000 hveto-2.1.4/.flake8
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.032247 hveto-2.1.4/.github/
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.041470 hveto-2.1.4/.github/workflows/
+-rw-r--r--   0 areeda     (501) staff       (20)     2881 2023-06-16 22:35:30.000000 hveto-2.1.4/.github/workflows/build.yml
+-rw-r--r--   0 areeda     (501) staff       (20)      263 2023-06-16 22:35:30.000000 hveto-2.1.4/.gitignore
+-rw-r--r--   0 areeda     (501) staff       (20)      342 2023-06-16 22:35:30.000000 hveto-2.1.4/.readthedocs.yml
+-rw-r--r--   0 areeda     (501) staff       (20)    35147 2022-09-06 21:22:40.000000 hveto-2.1.4/LICENSE
+-rw-r--r--   0 areeda     (501) staff       (20)       42 2023-06-16 22:35:30.000000 hveto-2.1.4/MANIFEST.in
+-rw-r--r--   0 areeda     (501) staff       (20)     3783 2023-06-16 22:51:06.073498 hveto-2.1.4/PKG-INFO
+-rw-r--r--   0 areeda     (501) staff       (20)     2361 2022-09-06 21:22:40.000000 hveto-2.1.4/README.rst
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.043582 hveto-2.1.4/docs/
+-rw-r--r--   0 areeda     (501) staff       (20)     7992 2022-09-06 21:22:40.000000 hveto-2.1.4/docs/Makefile
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.032715 hveto-2.1.4/docs/_static/
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.044090 hveto-2.1.4/docs/_static/css/
+-rw-r--r--   0 areeda     (501) staff       (20)     4997 2022-09-06 21:22:40.000000 hveto-2.1.4/docs/_static/css/custom.css
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.044782 hveto-2.1.4/docs/_templates/
+-rw-r--r--   0 areeda     (501) staff       (20)       91 2022-09-06 21:22:40.000000 hveto-2.1.4/docs/_templates/layout.html
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.045284 hveto-2.1.4/docs/api/
+-rw-r--r--   0 areeda     (501) staff       (20)       54 2022-09-06 21:22:40.000000 hveto-2.1.4/docs/api/index.rst
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.045835 hveto-2.1.4/docs/command-line/
+-rw-r--r--   0 areeda     (501) staff       (20)     3049 2022-09-06 21:22:40.000000 hveto-2.1.4/docs/command-line/index.rst
+-rw-r--r--   0 areeda     (501) staff       (20)    10465 2022-09-06 21:22:40.000000 hveto-2.1.4/docs/conf.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2967 2022-09-06 21:22:40.000000 hveto-2.1.4/docs/index.rst
+-rw-r--r--   0 areeda     (501) staff       (20)       60 2022-09-06 21:22:40.000000 hveto-2.1.4/docs/requirements.txt
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.055605 hveto-2.1.4/hveto/
+-rw-r--r--   0 areeda     (501) staff       (20)     1001 2023-06-16 22:35:30.000000 hveto-2.1.4/hveto/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)    36428 2023-06-16 02:24:22.000000 hveto-2.1.4/hveto/__main__.py
+-rw-r--r--   0 areeda     (501) staff       (20)      160 2023-06-16 22:51:05.000000 hveto-2.1.4/hveto/_version.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.061083 hveto-2.1.4/hveto/cli/
+-rw-r--r--   0 areeda     (501) staff       (20)      896 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/cli/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)    14369 2023-06-16 02:24:22.000000 hveto-2.1.4/hveto/cli/cache_events.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.062357 hveto-2.1.4/hveto/cli/tests/
+-rw-r--r--   0 areeda     (501) staff       (20)      811 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/cli/tests/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)     3063 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/cli/tests/test_trace.py
+-rw-r--r--   0 areeda     (501) staff       (20)     3976 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/cli/trace.py
+-rw-r--r--   0 areeda     (501) staff       (20)    11142 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/config.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1698 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/const.py
+-rw-r--r--   0 areeda     (501) staff       (20)    10769 2023-06-16 02:24:22.000000 hveto-2.1.4/hveto/core.py
+-rw-r--r--   0 areeda     (501) staff       (20)    14863 2023-06-16 22:35:30.000000 hveto-2.1.4/hveto/html.py
+-rw-r--r--   0 areeda     (501) staff       (20)    18816 2023-06-16 02:24:22.000000 hveto-2.1.4/hveto/plot.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2681 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/segments.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.072840 hveto-2.1.4/hveto/tests/
+-rw-r--r--   0 areeda     (501) staff       (20)      749 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/tests/__init__.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1266 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/tests/test_core.py
+-rw-r--r--   0 areeda     (501) staff       (20)     3916 2023-06-16 22:35:30.000000 hveto-2.1.4/hveto/tests/test_html.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1731 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/tests/test_plot.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2817 2023-06-16 02:24:22.000000 hveto-2.1.4/hveto/tests/test_segments.py
+-rw-r--r--   0 areeda     (501) staff       (20)     1860 2023-06-16 02:24:22.000000 hveto-2.1.4/hveto/tests/test_triggers.py
+-rw-r--r--   0 areeda     (501) staff       (20)     2149 2022-09-06 21:22:40.000000 hveto-2.1.4/hveto/tests/test_utils.py
+-rw-r--r--   0 areeda     (501) staff       (20)    11219 2023-06-16 02:24:22.000000 hveto-2.1.4/hveto/triggers.py
+-rw-r--r--   0 areeda     (501) staff       (20)     4882 2023-06-16 02:24:22.000000 hveto-2.1.4/hveto/utils.py
+drwxr-xr-x   0 areeda     (501) staff       (20)        0 2023-06-16 22:51:06.059263 hveto-2.1.4/hveto.egg-info/
+-rw-r--r--   0 areeda     (501) staff       (20)     3783 2023-06-16 22:51:05.000000 hveto-2.1.4/hveto.egg-info/PKG-INFO
+-rw-r--r--   0 areeda     (501) staff       (20)      951 2023-06-16 22:51:06.000000 hveto-2.1.4/hveto.egg-info/SOURCES.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        1 2023-06-16 22:51:05.000000 hveto-2.1.4/hveto.egg-info/dependency_links.txt
+-rw-r--r--   0 areeda     (501) staff       (20)      130 2023-06-16 22:51:05.000000 hveto-2.1.4/hveto.egg-info/entry_points.txt
+-rw-r--r--   0 areeda     (501) staff       (20)      251 2023-06-16 22:51:05.000000 hveto-2.1.4/hveto.egg-info/requires.txt
+-rw-r--r--   0 areeda     (501) staff       (20)        6 2023-06-16 22:51:05.000000 hveto-2.1.4/hveto.egg-info/top_level.txt
+-rw-r--r--   0 areeda     (501) staff       (20)     2523 2023-06-16 22:35:30.000000 hveto-2.1.4/pyproject.toml
+-rw-r--r--   0 areeda     (501) staff       (20)       38 2023-06-16 22:51:06.073886 hveto-2.1.4/setup.cfg
```

### Comparing `hveto-2.1.3/LICENSE` & `hveto-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/PKG-INFO` & `hveto-2.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: hveto
-Version: 2.1.3
-Summary: A python implementation of the HierarchicalVeto (hveto) algorithm.
-Home-page: https://github.com/gwdetchar/hveto/
-Author: Joshua Smith
-Author-email: joshua.smith@ligo.org
-License: GPL-3.0-or-later
-Keywords: physics,astronomy,gravitational-waves,ligo
+Version: 2.1.4
+Summary: A python implementation of the HierarchicalVeto (hveto) algorithm
+Author-email: Joshua Smith <joshua.smith@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
+Maintainer-email: Joe Areeda <joseph.areeda@ligo.org>
+Project-URL: Bug Tracker, https://github.com/gwdetchar/hveto/issues
+Project-URL: Documentation, https://hveto.readthedocs.io
+Project-URL: Source Code, https://github.com/gwdetchar/hveto
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
-Provides-Extra: doc
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 =================
 Hierarchical Veto
 =================
 
 Hveto is a python implementation of the HierarchicalVeto algorithm. It is
```

### Comparing `hveto-2.1.3/README.rst` & `hveto-2.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/__init__.py` & `hveto-2.1.4/hveto/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with hveto.  If not, see <http://www.gnu.org/licenses/>.
 
 """The HierarchichalVeto algorithm
 """
 
-from ._version import get_versions
-
-__version__ = get_versions()['version']
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 __credits__ = 'Joshua Smith <joshua.smith@ligo.org>'
 
-del get_versions
+try:
+    from ._version import version as __version__
+except ModuleNotFoundError:  # development mode
+    __version__ = ''
```

### Comparing `hveto-2.1.3/hveto/__main__.py` & `hveto-2.1.4/hveto/__main__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/cli/__init__.py` & `hveto-2.1.4/hveto/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/cli/cache_events.py` & `hveto-2.1.4/hveto/cli/cache_events.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/cli/tests/__init__.py` & `hveto-2.1.4/hveto/cli/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/cli/tests/test_trace.py` & `hveto-2.1.4/hveto/cli/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/cli/trace.py` & `hveto-2.1.4/hveto/cli/trace.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/config.py` & `hveto-2.1.4/hveto/config.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/const.py` & `hveto-2.1.4/hveto/const.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/core.py` & `hveto-2.1.4/hveto/core.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/html.py` & `hveto-2.1.4/hveto/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from functools import wraps
 
 from MarkupPy import markup
 
 from gwdetchar.io import html as gwhtml
 from gwpy.time import tconvert
 
-from ._version import get_versions
+from . import __version__
 
 __author__ = 'Duncan Macleod <duncan.macleod@ligo.org>'
 __credits__ = 'Josh Smith, Joe Areeda, Alex Urban'
 
 
 # -- HTML construction --------------------------------------------------------
 
@@ -137,16 +137,19 @@
         nav = navbar(ifo, start, winners)
         page = gwhtml.new_bootstrap_page(navbar=nav, **initargs)
         page.add(banner(ifo, start, end))
         # write content
         page.add(str(func(*args, **kwargs)))
         # close page with custom footer
         index = os.path.join(outdir, 'index.html')
-        version = get_versions()['version']
-        commit = get_versions()['full-revisionid']
+        version = __version__
+        if "dev" in __version__:
+            commit = __version__.rsplit("g", 1)[1]
+        else:
+            commit = __version__
         url = 'https://github.com/gwdetchar/hveto/tree/{}'.format(commit)
         gwhtml.close_page(page, index, about=about,
                           link=('hveto-%s' % version, url, 'GitHub'),
                           issues='https://github.com/gwdetchar/hveto/issues')
         return index
     return decorated_func
```

### Comparing `hveto-2.1.3/hveto/plot.py` & `hveto-2.1.4/hveto/plot.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/segments.py` & `hveto-2.1.4/hveto/segments.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/tests/__init__.py` & `hveto-2.1.4/hveto/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/tests/test_core.py` & `hveto-2.1.4/hveto/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/tests/test_html.py` & `hveto-2.1.4/hveto/tests/test_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 import pytest
 
 from gwdetchar.utils import parse_html
 
 from .. import html
 
-BANNER = '''<div class="page-header" role="banner">
+BANNER = """<div class="page-header" role="banner">
 <h1 class="pb-2 mt-3 mb-2 border-bottom">L1 HierarchicalVeto</h1>
-<h3 class="mt-3">0 - 100 1980-01-06 00:00:00 - 1980-01-06 00:01:40</h3>
-</div>'''
+<h3 class="mt-3">0 - 100 1980-01-06 00:00:00 - 1980-01-06 00:01:40 -- 0:01:40</h3>
+</div>"""
 
 NAVBAR = """<nav class="navbar fixed-top navbar-expand-md navbar-h1 shadow-sm">
 <div class="container-fluid">
 <div class="navbar-brand border border-white rounded">H1 Hveto</div>
 <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target=".navbar-collapse">
 <span class="navbar-toggler-icon"></span>
 </button>
```

### Comparing `hveto-2.1.3/hveto/tests/test_plot.py` & `hveto-2.1.4/hveto/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/tests/test_segments.py` & `hveto-2.1.4/hveto/tests/test_segments.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/tests/test_triggers.py` & `hveto-2.1.4/hveto/tests/test_triggers.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/tests/test_utils.py` & `hveto-2.1.4/hveto/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/triggers.py` & `hveto-2.1.4/hveto/triggers.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto/utils.py` & `hveto-2.1.4/hveto/utils.py`

 * *Files identical despite different names*

### Comparing `hveto-2.1.3/hveto.egg-info/PKG-INFO` & `hveto-2.1.4/hveto.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: hveto
-Version: 2.1.3
-Summary: A python implementation of the HierarchicalVeto (hveto) algorithm.
-Home-page: https://github.com/gwdetchar/hveto/
-Author: Joshua Smith
-Author-email: joshua.smith@ligo.org
-License: GPL-3.0-or-later
-Keywords: physics,astronomy,gravitational-waves,ligo
+Version: 2.1.4
+Summary: A python implementation of the HierarchicalVeto (hveto) algorithm
+Author-email: Joshua Smith <joshua.smith@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
+Maintainer-email: Joe Areeda <joseph.areeda@ligo.org>
+Project-URL: Bug Tracker, https://github.com/gwdetchar/hveto/issues
+Project-URL: Documentation, https://hveto.readthedocs.io
+Project-URL: Source Code, https://github.com/gwdetchar/hveto
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6
-Provides-Extra: doc
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 =================
 Hierarchical Veto
 =================
 
 Hveto is a python implementation of the HierarchicalVeto algorithm. It is
```

