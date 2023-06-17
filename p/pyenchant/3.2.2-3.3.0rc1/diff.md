# Comparing `tmp/pyenchant-3.2.2.tar.gz` & `tmp/pyenchant-3.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenchant-3.2.2.tar", last modified: Tue Oct  5 17:25:10 2021, max compression
+gzip compressed data, was "pyenchant-3.3.0rc1.tar", last modified: Sat Jun 17 14:40:51 2023, max compression
```

## Comparing `pyenchant-3.2.2.tar` & `pyenchant-3.3.0rc1.tar`

### file list

```diff
@@ -1,27 +1,39 @@
-drwxr-xr-x   0 dmerej    (1000) users      (100)        0 2021-10-05 17:25:10.584174 pyenchant-3.2.2/
--rw-r--r--   0 dmerej    (1000) users      (100)     9454 2021-10-05 17:19:11.000000 pyenchant-3.2.2/Changelog
--rw-r--r--   0 dmerej    (1000) users      (100)    26430 2019-11-11 11:17:11.000000 pyenchant-3.2.2/LICENSE.txt
--rw-r--r--   0 dmerej    (1000) users      (100)       77 2020-06-13 11:58:01.000000 pyenchant-3.2.2/MANIFEST.in
--rw-r--r--   0 dmerej    (1000) users      (100)     4447 2021-10-05 17:25:10.584174 pyenchant-3.2.2/PKG-INFO
--rw-r--r--   0 dmerej    (1000) users      (100)     2582 2021-09-09 17:37:32.000000 pyenchant-3.2.2/README.rst
-drwxr-xr-x   0 dmerej    (1000) users      (100)        0 2021-10-05 17:25:10.580840 pyenchant-3.2.2/enchant/
--rw-r--r--   0 dmerej    (1000) users      (100)    33742 2021-10-05 17:24:12.000000 pyenchant-3.2.2/enchant/__init__.py
--rw-r--r--   0 dmerej    (1000) users      (100)    12275 2021-10-05 17:18:53.000000 pyenchant-3.2.2/enchant/_enchant.py
-drwxr-xr-x   0 dmerej    (1000) users      (100)        0 2021-10-05 17:25:10.584174 pyenchant-3.2.2/enchant/checker/
--rw-r--r--   0 dmerej    (1000) users      (100)    12790 2021-10-05 17:18:53.000000 pyenchant-3.2.2/enchant/checker/CmdLineChecker.py
--rw-r--r--   0 dmerej    (1000) users      (100)    10099 2021-10-05 17:18:53.000000 pyenchant-3.2.2/enchant/checker/GtkSpellCheckerDialog.py
--rw-r--r--   0 dmerej    (1000) users      (100)    14617 2021-10-05 17:18:53.000000 pyenchant-3.2.2/enchant/checker/__init__.py
--rw-r--r--   0 dmerej    (1000) users      (100)    11106 2021-10-05 17:18:53.000000 pyenchant-3.2.2/enchant/checker/wxSpellCheckerDialog.py
--rw-r--r--   0 dmerej    (1000) users      (100)     2091 2020-06-13 11:58:01.000000 pyenchant-3.2.2/enchant/errors.py
--rw-r--r--   0 dmerej    (1000) users      (100)     9212 2021-10-05 17:18:53.000000 pyenchant-3.2.2/enchant/pypwl.py
-drwxr-xr-x   0 dmerej    (1000) users      (100)        0 2021-10-05 17:25:10.584174 pyenchant-3.2.2/enchant/tokenize/
--rw-r--r--   0 dmerej    (1000) users      (100)    20300 2021-10-05 17:18:53.000000 pyenchant-3.2.2/enchant/tokenize/__init__.py
--rw-r--r--   0 dmerej    (1000) users      (100)     7054 2021-10-05 17:18:53.000000 pyenchant-3.2.2/enchant/tokenize/en.py
--rw-r--r--   0 dmerej    (1000) users      (100)     4271 2021-10-05 17:18:53.000000 pyenchant-3.2.2/enchant/utils.py
-drwxr-xr-x   0 dmerej    (1000) users      (100)        0 2021-10-05 17:25:10.584174 pyenchant-3.2.2/pyenchant.egg-info/
--rw-r--r--   0 dmerej    (1000) users      (100)     4447 2021-10-05 17:25:10.000000 pyenchant-3.2.2/pyenchant.egg-info/PKG-INFO
--rw-r--r--   0 dmerej    (1000) users      (100)      482 2021-10-05 17:25:10.000000 pyenchant-3.2.2/pyenchant.egg-info/SOURCES.txt
--rw-r--r--   0 dmerej    (1000) users      (100)        1 2021-10-05 17:25:10.000000 pyenchant-3.2.2/pyenchant.egg-info/dependency_links.txt
--rw-r--r--   0 dmerej    (1000) users      (100)        8 2021-10-05 17:25:10.000000 pyenchant-3.2.2/pyenchant.egg-info/top_level.txt
--rw-r--r--   0 dmerej    (1000) users      (100)     1379 2021-10-05 17:25:10.584174 pyenchant-3.2.2/setup.cfg
--rw-r--r--   0 dmerej    (1000) users      (100)       38 2020-06-13 11:58:01.000000 pyenchant-3.2.2/setup.py
+drwxr-xr-x   0 dmerej    (1000) dmerej    (1000)        0 2023-06-17 14:40:51.880389 pyenchant-3.3.0rc1/
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    10050 2023-06-17 14:22:57.000000 pyenchant-3.3.0rc1/Changelog
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    26436 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/LICENSE.txt
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)       77 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/MANIFEST.in
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     4052 2023-06-17 14:40:51.880389 pyenchant-3.3.0rc1/PKG-INFO
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     2582 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/README.rst
+drwxr-xr-x   0 dmerej    (1000) dmerej    (1000)        0 2023-06-17 14:40:51.877055 pyenchant-3.3.0rc1/enchant/
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    35729 2023-06-17 14:27:17.000000 pyenchant-3.3.0rc1/enchant/__init__.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    13490 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/_enchant.py
+drwxr-xr-x   0 dmerej    (1000) dmerej    (1000)        0 2023-06-17 14:40:51.877055 pyenchant-3.3.0rc1/enchant/checker/
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    12302 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/checker/CmdLineChecker.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    10175 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/checker/GtkSpellCheckerDialog.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    15307 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/checker/__init__.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    10642 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/checker/wxSpellCheckerDialog.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     2091 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/errors.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     9689 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/pypwl.py
+drwxr-xr-x   0 dmerej    (1000) dmerej    (1000)        0 2023-06-17 14:40:51.877055 pyenchant-3.3.0rc1/enchant/tokenize/
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    21342 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/tokenize/__init__.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     1886 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/tokenize/de.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     7447 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/tokenize/en.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     4640 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/enchant/utils.py
+drwxr-xr-x   0 dmerej    (1000) dmerej    (1000)        0 2023-06-17 14:40:51.877055 pyenchant-3.3.0rc1/pyenchant.egg-info/
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     4052 2023-06-17 14:40:51.000000 pyenchant-3.3.0rc1/pyenchant.egg-info/PKG-INFO
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)      717 2023-06-17 14:40:51.000000 pyenchant-3.3.0rc1/pyenchant.egg-info/SOURCES.txt
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)        1 2023-06-17 14:40:51.000000 pyenchant-3.3.0rc1/pyenchant.egg-info/dependency_links.txt
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)        8 2023-06-17 14:40:51.000000 pyenchant-3.3.0rc1/pyenchant.egg-info/top_level.txt
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)       31 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/pyproject.toml
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     1784 2023-06-17 14:40:51.880389 pyenchant-3.3.0rc1/setup.cfg
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)       38 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/setup.py
+drwxr-xr-x   0 dmerej    (1000) dmerej    (1000)        0 2023-06-17 14:40:51.880389 pyenchant-3.3.0rc1/tests/
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     3257 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/tests/test_broker.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     9413 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/tests/test_checker.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     3958 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/tests/test_dict.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     3475 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/tests/test_docstrings.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)      331 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/tests/test_misc.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)      522 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/tests/test_multiprocessing.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)     3487 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/tests/test_pwl.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)    13085 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/tests/test_tokenize.py
+-rw-r--r--   0 dmerej    (1000) dmerej    (1000)      509 2023-05-21 15:23:08.000000 pyenchant-3.3.0rc1/tests/test_utils.py
```

### Comparing `pyenchant-3.2.2/Changelog` & `pyenchant-3.3.0rc1/Changelog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 Changelog
 =========
 
+3.3.0 (unreleased)
+------------------
+
+* Add tokenizer for the German language
+* Improve support for macOS M1 architecture
+* Add support for Python 3.11
+* Remove support for Python 3.6
+* Numerous documentation updates
+* Start adding type annotations (still a work in progress)
+* For the `enchant.checker` package: always setup SpellChecker.
+* Display project urls on ``pypi.org``
+* Sort all imports with ``isort``
+* Numerous tests cleanups
+* Update FSF address in LICENSE.txt
+* Windows wheels:
+   * Use ``enchant`` archive generated from GitHub Actions
+   * Bmup ``enchant`` from 2.2.7 to 3.4.4
+
 3.2.2 (2021-10-05)
 ------------------
 
 * Add support for Python 3.10
 
 3.2.1 (2021-06-24)
 --------------------
```

### Comparing `pyenchant-3.2.2/LICENSE.txt` & `pyenchant-3.3.0rc1/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 		  GNU LESSER GENERAL PUBLIC LICENSE
 		       Version 2.1, February 1999
 
  Copyright (C) 1991, 1999 Free Software Foundation, Inc.
-     59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
+ 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
 [This is the first released version of the Lesser GPL.  It also counts
  as the successor of the GNU Library Public License, version 2, hence
  the version number 2.1.]
 
@@ -481,15 +481,15 @@
     This library is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
     Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public
     License along with this library; if not, write to the Free Software
-    Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA  02111-1307  USA
+    Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 Also add information on how to contact you by electronic and paper mail.
 
 You should also get your employer (if you work as a programmer) or your
 school, if any, to sign a "copyright disclaimer" for the library, if
 necessary.  Here is a sample; alter the names:
```

### Comparing `pyenchant-3.2.2/PKG-INFO` & `pyenchant-3.3.0rc1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,104 +1,107 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pyenchant
-Version: 3.2.2
+Version: 3.3.0rc1
 Summary: Python bindings for the Enchant spellchecking system
 Home-page: https://pyenchant.github.io/pyenchant/
 Author: Dimitri Merejkowsky
 Author-email: d.merej@gmail.com
 License: LGPL
-Description: pyenchant:  Python bindings for the Enchant spellchecker
-        ========================================================
-        
-        .. image:: https://img.shields.io/pypi/v/pyenchant.svg
-            :target: https://pypi.org/project/pyenchant
-        
-        .. image:: https://img.shields.io/pypi/pyversions/pyenchant.svg
-            :target: https://pypi.org/project/pyenchant
-        
-        .. image:: https://github.com/pyenchant/pyenchant/workflows/tests/badge.svg
-            :target: https://github.com/pyenchant/pyenchant/actions
-        
-        .. image:: https://builds.sr.ht/~dmerej/pyenchant.svg
-            :target: https://builds.sr.ht/~dmerej/pyenchant
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/psf/black
-        
-        This package provides a set of Python language bindings for the Enchant
-        spellchecking library.  For more information, visit the project website:
-        
-            http://pyenchant.github.io/pyenchant/
-        
-        What is Enchant?
-        ----------------
-        
-        Enchant is used to check the spelling of words and suggest corrections
-        for words that are miss-spelled.  It can use many popular spellchecking
-        packages to perform this task, including ispell, aspell and MySpell.  It
-        is quite flexible at handling multiple dictionaries and multiple
-        languages.
-        
-        More information is available on the Enchant website:
-        
-            https://abiword.github.io/enchant/
-        
-        
-        How do I use it?
-        ----------------
-        
-        For Windows users, install the pre-built binary packages using
-        pip::
-        
-            pip install pyenchant
-        
-        
-        These packages bundle a pre-built copy of the underlying enchant library.
-        Users on other platforms will need to install "enchant" using their system
-        package manager (brew on macOS).
-        
-        Once the software is installed, python's on-line help facilities can
-        get you started.  Launch python and issue the following commands:
-        
-            >>> import enchant
-            >>> help(enchant)
-        
-        
-        
-        Who is responsible for all this?
-        --------------------------------
-        
-        The credit for Enchant itself goes to Dom Lachowicz.  Find out more details
-        on the Enchant website listed above.  Full marks to Dom for producing such
-        a high-quality library.
-        
-        The glue to pull Enchant into Python via ctypes was written by Ryan Kelly.
-        He needed a decent spellchecker for another project he was working on, and
-        all the solutions turned up by Google were either extremely non-portable
-        (e.g. opening a pipe to ispell) or had completely disappeared from the web
-        (what happened to SnakeSpell?)  It was also a great excuse to teach himself
-        about SWIG, ctypes, and even a little bit of the Python/C API.
-        
-        Finally, after Ryan stepped down from the project, Dimitri Merejkowsky
-        became the new maintainer.
-        
-        
+Project-URL: Changelog, https://pyenchant.github.io/pyenchant/changelog.html
+Project-URL: Source, https://github.com/pyenchant/pyenchant
+Project-URL: Tracker, https://github.com/pyenchant/pyenchant/issues
 Keywords: spelling spellcheck enchant
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.5
+Requires-Python: >=3.7
+License-File: LICENSE.txt
+
+pyenchant:  Python bindings for the Enchant spellchecker
+========================================================
+
+.. image:: https://img.shields.io/pypi/v/pyenchant.svg
+    :target: https://pypi.org/project/pyenchant
+
+.. image:: https://img.shields.io/pypi/pyversions/pyenchant.svg
+    :target: https://pypi.org/project/pyenchant
+
+.. image:: https://github.com/pyenchant/pyenchant/workflows/tests/badge.svg
+    :target: https://github.com/pyenchant/pyenchant/actions
+
+.. image:: https://builds.sr.ht/~dmerej/pyenchant.svg
+    :target: https://builds.sr.ht/~dmerej/pyenchant
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+This package provides a set of Python language bindings for the Enchant
+spellchecking library.  For more information, visit the project website:
+
+    http://pyenchant.github.io/pyenchant/
+
+What is Enchant?
+----------------
+
+Enchant is used to check the spelling of words and suggest corrections
+for words that are miss-spelled.  It can use many popular spellchecking
+packages to perform this task, including ispell, aspell and MySpell.  It
+is quite flexible at handling multiple dictionaries and multiple
+languages.
+
+More information is available on the Enchant website:
+
+    https://abiword.github.io/enchant/
+
+
+How do I use it?
+----------------
+
+For Windows users, install the pre-built binary packages using
+pip::
+
+    pip install pyenchant
+
+
+These packages bundle a pre-built copy of the underlying enchant library.
+Users on other platforms will need to install "enchant" using their system
+package manager (brew on macOS).
+
+Once the software is installed, python's on-line help facilities can
+get you started.  Launch python and issue the following commands:
+
+    >>> import enchant
+    >>> help(enchant)
+
+
+
+Who is responsible for all this?
+--------------------------------
+
+The credit for Enchant itself goes to Dom Lachowicz.  Find out more details
+on the Enchant website listed above.  Full marks to Dom for producing such
+a high-quality library.
+
+The glue to pull Enchant into Python via ctypes was written by Ryan Kelly.
+He needed a decent spellchecker for another project he was working on, and
+all the solutions turned up by Google were either extremely non-portable
+(e.g. opening a pipe to ispell) or had completely disappeared from the web
+(what happened to SnakeSpell?)  It was also a great excuse to teach himself
+about SWIG, ctypes, and even a little bit of the Python/C API.
+
+Finally, after Ryan stepped down from the project, Dimitri Merejkowsky
+became the new maintainer.
+
```

### Comparing `pyenchant-3.2.2/README.rst` & `pyenchant-3.3.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `pyenchant-3.2.2/enchant/__init__.py` & `pyenchant-3.3.0rc1/enchant/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 This module provides several classes for performing spell checking
 via the Enchant spellchecking library.  For more details on Enchant,
 visit the project website:
 
     https://abiword.github.io/enchant/
 
-Spellchecking is performed using 'Dict' objects, which represent
+Spellchecking is performed using :py:class:`Dict` objects, which represent
 a language dictionary.  Their use is best demonstrated by a quick
 example::
 
     >>> import enchant
     >>> d = enchant.Dict("en_US")   # create dictionary for US English
     >>> d.check("enchant")
     True
@@ -52,125 +52,132 @@
 
 Languages are identified by standard string tags such as "en" (English)
 and "fr" (French).  Specific language dialects can be specified by
 including an additional code - for example, "en_AU" refers to Australian
 English.  The later form is preferred as it is more widely supported.
 
 To check whether a dictionary exists for a given language, the function
-'dict_exists' is available.  Dictionaries may also be created using the
-function 'request_dict'.
+:py:func:`dict_exists` is available.  Dictionaries may also be created using the
+function :py:func:`request_dict`.
 
 A finer degree of control over the dictionaries and how they are created
-can be obtained using one or more 'Broker' objects.  These objects are
+can be obtained using one or more :py:class:`Broker` objects.  These objects are
 responsible for locating dictionaries for a specific language.
 
 Note that unicode strings are expected throughout the entire API.
 Bytestrings should not be passed into any function.
 
 Errors that occur in this module are reported by raising subclasses
-of 'Error'.
+of :py:exc:`~.errors.Error`.
 
 """
 _DOC_ERRORS = ["enchnt", "enchnt", "incant", "fr"]
 
-__version__ = "3.2.2"
+__version__ = "3.3.0rc1"
 
 import os
 import warnings
 
 try:
     from enchant import _enchant as _e
 except ImportError:
     if not os.environ.get("PYENCHANT_IGNORE_MISSING_LIB", False):
         raise
-    _e = None
+    _e = None  # type: ignore
 
-from enchant.errors import Error, DictNotFoundError
-from enchant.utils import get_default_language
+from typing import Any, List, NoReturn, Optional, Tuple, Type, Union  # noqa F401
+
+from enchant.errors import *  # noqa F401,F403
+from enchant.errors import DictNotFoundError, Error
 from enchant.pypwl import PyPWL
+from enchant.utils import get_default_language
 
 
 class ProviderDesc:
     """Simple class describing an Enchant provider.
 
     Each provider has the following information associated with it:
 
-        * name:        Internal provider name (e.g. "aspell")
-        * desc:        Human-readable description (e.g. "Aspell Provider")
-        * file:        Location of the library containing the provider
+        * :py:attr:`name`:        Internal provider name (e.g. "aspell")
+        * :py:attr:`desc`:        Human-readable description (e.g. "Aspell Provider")
+        * :py:attr:`file`:        Location of the library containing the provider
 
     """
 
     _DOC_ERRORS = ["desc"]
 
-    def __init__(self, name, desc, file):
+    def __init__(self, name: str, desc: str, file: str) -> None:
         self.name = name
         self.desc = desc
         self.file = file
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "<Enchant: %s>" % self.desc
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return str(self)
 
     def __eq__(self, pd):
         """Equality operator on ProviderDesc objects."""
+        if not isinstance(pd, ProviderDesc):
+            return False
         return self.name == pd.name and self.desc == pd.desc and self.file == pd.file
 
     def __hash__(self):
         """Hash operator on ProviderDesc objects."""
         return hash(self.name + self.desc + self.file)
 
 
 class _EnchantObject:
     """Base class for enchant objects.
 
     This class implements some general functionality for interfacing with
     the '_enchant' C-library in a consistent way.  All public objects
     from the 'enchant' module are subclasses of this class.
 
-    All enchant objects have an attribute '_this' which contains the
-    pointer to the underlying C-library object.  The method '_check_this'
+    All enchant objects have an attribute :py:attr:`_this` which contains the
+    pointer to the underlying C-library object.  The method :py:meth:`_check_this`
     can be called to ensure that this point is not None, raising an
     exception if it is.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """_EnchantObject constructor."""
         self._this = None
         #  To be importable when enchant C lib is missing, we need
         #  to create a dummy default broker.
         if _e is not None:
             self._init_this()
 
-    def _check_this(self, msg=None):
-        """Check that self._this is set to a pointer, rather than None."""
+    def _check_this(self, msg: str = None) -> None:
+        """Check that :py:attr:`_this` is set to a pointer, rather than `None`."""
         if self._this is None:
             if msg is None:
                 msg = "%s unusable: the underlying C-library object has been freed."
                 msg = msg % (self.__class__.__name__,)
             raise Error(msg)
 
-    def _init_this(self):
+    def _init_this(self) -> None:
         """Initialise the underlying C-library object pointer."""
         raise NotImplementedError
 
-    def _raise_error(self, default="Unspecified Error", eclass=Error):
+    def _raise_error(
+        self, default: str = "Unspecified Error", eclass: Type[Error] = Error
+    ) -> NoReturn:
         """Raise an exception based on available error messages.
 
-        This method causes an Error to be raised.  Subclasses should
+        This method causes an :py:exc:`~.errors.Error` to be raised.  Subclasses should
         override it to retrieve an error indication from the underlying
         API if possible.  If such a message cannot be retrieved, the
-        argument value <default> is used.  The class of the exception
-        can be specified using the argument <eclass>
+        argument value `default` is used.  The class of the exception
+        can be specified using the argument `eclass`
         """
         raise eclass(default)
 
-    _raise_error._DOC_ERRORS = ["eclass"]
+    _raise_error._DOC_ERRORS = ["eclass"]  # type: ignore
 
     def __getstate__(self):
         """Customize pickling of PyEnchant objects.
 
         Since it's not safe for multiple objects to share the same C-library
         object, we make sure it's unset when pickling.
         """
@@ -182,102 +189,104 @@
         self.__dict__.update(state)
         self._init_this()
 
 
 class Broker(_EnchantObject):
     """Broker object for the Enchant spellchecker.
 
-    Broker objects are responsible for locating and managing dictionaries.
-    Unless custom functionality is required, there is no need to use Broker
-    objects directly. The 'enchant' module provides a default broker object
-    so that 'Dict' objects can be created directly.
+    `Broker` objects are responsible for locating and managing dictionaries.
+    Unless custom functionality is required, there is no need to use `Broker`
+    objects directly. The py:mod:`enchant` module provides a default broker object
+    so that :py:class:`Dict` objects can be created directly.
 
     The most important methods of this class include:
 
         * :py:meth:`dict_exists`:   check existence of a specific language dictionary
         * :py:meth:`request_dict`:  obtain a dictionary for specific language
         * :py:meth:`set_ordering`:  specify which dictionaries to try for a given language.
 
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Broker object constructor.
 
-        This method is the constructor for the 'Broker' object.  No
+        This method is the constructor for the `Broker` object.  No
         arguments are required.
         """
         super().__init__()
 
-    def _init_this(self):
+    def _init_this(self) -> None:
         self._this = _e.broker_init()
         if not self._this:
             raise Error("Could not initialise an enchant broker.")
         self._live_dicts = {}
 
-    def __del__(self):
+    def __del__(self) -> None:
         """Broker object destructor."""
         # Calling free() might fail if python is shutting down
         try:
             self._free()
         except (AttributeError, TypeError):
             pass
 
     def __getstate__(self):
         state = super().__getstate__()
         state.pop("_live_dicts")
         return state
 
-    def _raise_error(self, default="Unspecified Error", eclass=Error):
+    def _raise_error(
+        self, default: str = "Unspecified Error", eclass: Type[Error] = Error
+    ) -> NoReturn:
         """Overrides _EnchantObject._raise_error to check broker errors."""
         err = _e.broker_get_error(self._this)
         if err == "" or err is None:
             raise eclass(default)
         raise eclass(err.decode())
 
-    def _free(self):
+    def _free(self) -> None:
         """Free system resource associated with a Broker object.
 
         This method can be called to free the underlying system resources
-        associated with a Broker object.  It is called automatically when
+        associated with a `Broker` object.  It is called automatically when
         the object is garbage collected.  If called explicitly, the
-        Broker and any associated Dict objects must no longer be used.
+        `Broker` and any associated `Dict` objects must no longer be used.
         """
         if self._this is not None:
             # During shutdown, this finalizer may be called before
             # some Dict finalizers.  Ensure all pointers are freed.
             for (dict, count) in list(self._live_dicts.items()):
                 while count:
                     self._free_dict_data(dict)
                     count -= 1
             _e.broker_free(self._this)
             self._this = None
 
-    def request_dict(self, tag=None):
-        """Request a Dict object for the language specified by <tag>.
+    def request_dict(self, tag: str = None) -> "Dict":
+        """Request a :py:class:`Dict` object for the language specified by `tag`.
 
-        This method constructs and returns a Dict object for the
-        requested language.  'tag' should be a string of the appropriate
+        This method constructs and returns a :py:class:`Dict` object for the
+        requested language.  `tag` should be a string of the appropriate
         form for specifying a language, such as "fr" (French) or "en_AU"
         (Australian English).  The existence of a specific language can
-        be tested using the 'dict_exists' method.
+        be tested using the method :py:meth:`dict_exists`.
 
-        If <tag> is not given or is None, an attempt is made to determine
-        the current language in use.  If this cannot be determined, Error
+        If `tag` is not given or is `None`, an attempt is made to determine
+        the current language in use.  If this cannot be determined, :py:exc:`~.errors.Error`
         is raised.
 
         .. note::
-            this method is functionally equivalent to calling the Dict()
-            constructor and passing in the <broker> argument.
+            this method is functionally equivalent to calling the :py:class:`Dict()`
+            constructor and passing in the `broker` argument.
 
         """
         return Dict(tag, self)
 
-    request_dict._DOC_ERRORS = ["fr"]
+    request_dict._DOC_ERRORS = ["fr"]  # type: ignore
 
-    def _request_dict_data(self, tag):
+    def _request_dict_data(self, tag: str) -> _e.t_dict:
         """Request raw C pointer data for a dictionary.
 
         This method call passes on the call to the C library, and does
         some internal bookkeeping.
         """
         self._check_this()
         new_dict = _e.broker_request_dict(self._this, tag.encode())
@@ -287,18 +296,18 @@
             self._raise_error(e_str % (tag,), DictNotFoundError)
         if new_dict not in self._live_dicts:
             self._live_dicts[new_dict] = 1
         else:
             self._live_dicts[new_dict] += 1
         return new_dict
 
-    def request_pwl_dict(self, pwl):
+    def request_pwl_dict(self, pwl: str) -> "Dict":
         """Request a Dict object for a personal word list.
 
-        This method behaves as 'request_dict' but rather than returning
+        This method behaves as :py:meth:`request_dict` but rather than returning
         a dictionary for a specific language, it returns a dictionary
         referencing a personal word list.  A personal word list is a file
         of custom dictionary entries, one word per line.
         """
         self._check_this()
         new_dict = _e.broker_request_pwl_dict(self._this, pwl.encode())
         if new_dict is None:
@@ -308,128 +317,128 @@
             self._live_dicts[new_dict] = 1
         else:
             self._live_dicts[new_dict] += 1
         d = Dict(False)
         d._switch_this(new_dict, self)
         return d
 
-    def _free_dict(self, dict):
+    def _free_dict(self, dict: "Dict") -> None:
         """Free memory associated with a dictionary.
 
-        This method frees system resources associated with a Dict object.
-        It is equivalent to calling the object's 'free' method.  Once this
+        This method frees system resources associated with a `Dict` object.
+        It is equivalent to calling the object`s `free' method.  Once this
         method has been called on a dictionary, it must not be used again.
         """
         self._free_dict_data(dict._this)
         dict._this = None
         dict._broker = None
 
-    def _free_dict_data(self, dict):
+    def _free_dict_data(self, dict: _e.t_dict) -> None:
         """Free the underlying pointer for a dict."""
         self._check_this()
         _e.broker_free_dict(self._this, dict)
         self._live_dicts[dict] -= 1
         if self._live_dicts[dict] == 0:
             del self._live_dicts[dict]
 
-    def dict_exists(self, tag):
+    def dict_exists(self, tag: str) -> bool:
         """Check availability of a dictionary.
 
         This method checks whether there is a dictionary available for
-        the language specified by 'tag'.  It returns True if a dictionary
-        is available, and False otherwise.
+        the language specified by `tag`.  It returns `True` if a dictionary
+        is available, and `False` otherwise.
         """
         self._check_this()
         val = _e.broker_dict_exists(self._this, tag.encode())
         return bool(val)
 
-    def set_ordering(self, tag, ordering):
+    def set_ordering(self, tag: str, ordering: str) -> None:
         """Set dictionary preferences for a language.
 
         The Enchant library supports the use of multiple dictionary programs
         and multiple languages.  This method specifies which dictionaries
-        the broker should prefer when dealing with a given language.  'tag'
-        must be an appropriate language specification and 'ordering' is a
+        the broker should prefer when dealing with a given language.  `tag`
+        must be an appropriate language specification and `ordering` is a
         string listing the dictionaries in order of preference.  For example
         a valid ordering might be "aspell,myspell,ispell".
-        The value of 'tag' can also be set to "*" to set a default ordering
+        The value of `tag` can also be set to "*" to set a default ordering
         for all languages for which one has not been set explicitly.
         """
         self._check_this()
         _e.broker_set_ordering(self._this, tag.encode(), ordering.encode())
 
-    def describe(self):
+    def describe(self) -> List[ProviderDesc]:
         """Return list of provider descriptions.
 
         This method returns a list of descriptions of each of the
         dictionary providers available.  Each entry in the list is a
-        ProviderDesc object.
+        :py:class:`ProviderDesc` object.
         """
         self._check_this()
         self.__describe_result = []
         _e.broker_describe(self._this, self.__describe_callback)
         return [ProviderDesc(*r) for r in self.__describe_result]
 
-    def __describe_callback(self, name, desc, file):
+    def __describe_callback(self, name: bytes, desc: bytes, file: bytes) -> None:
         """Collector callback for dictionary description.
 
         This method is used as a callback into the _enchant function
-        'enchant_broker_describe'.  It collects the given arguments in
-        a tuple and appends them to the list '__describe_result'.
+        `enchant_broker_describe`.  It collects the given arguments in
+        a tuple and appends them to the list :py:attr:`__describe_result`.
         """
         name = name.decode()
         desc = desc.decode()
         file = file.decode()
         self.__describe_result.append((name, desc, file))
 
-    def list_dicts(self):
+    def list_dicts(self) -> List[Tuple[str, ProviderDesc]]:
         """Return list of available dictionaries.
 
         This method returns a list of dictionaries available to the
         broker.  Each entry in the list is a two-tuple of the form:
 
             (tag,provider)
 
-        where <tag> is the language lag for the dictionary and
-        <provider> is a ProviderDesc object describing the provider
+        where `tag` is the language lag for the dictionary and
+        `provider` is a :py:class:`ProviderDesc` object describing the provider
         through which that dictionary can be obtained.
         """
         self._check_this()
         self.__list_dicts_result = []
         _e.broker_list_dicts(self._this, self.__list_dicts_callback)
         return [(r[0], ProviderDesc(*r[1])) for r in self.__list_dicts_result]
 
     def __list_dicts_callback(self, tag, name, desc, file):
         """Collector callback for listing dictionaries.
 
         This method is used as a callback into the _enchant function
-        'enchant_broker_list_dicts'.  It collects the given arguments into
-        an appropriate tuple and appends them to '__list_dicts_result'.
+        `enchant_broker_list_dicts`.  It collects the given arguments into
+        an appropriate tuple and appends them to :py:attr:`__list_dicts_result`.
         """
         tag = tag.decode()
         name = name.decode()
         desc = desc.decode()
         file = file.decode()
         self.__list_dicts_result.append((tag, (name, desc, file)))
 
-    def list_languages(self):
+    def list_languages(self) -> List[str]:
         """List languages for which dictionaries are available.
 
         This function returns a list of language tags for which a
         dictionary is available.
         """
         langs = []
         for (tag, prov) in self.list_dicts():
             if tag not in langs:
                 langs.append(tag)
         return langs
 
     def __describe_dict(self, dict_data):
         """Get the description tuple for a dict data object.
-        <dict_data> must be a C-library pointer to an enchant dictionary.
+        `dict_data` must be a C-library pointer to an enchant dictionary.
         The return value is a tuple of the form:
                 (<tag>,<name>,<desc>,<file>)
         """
         # Define local callback function
         cb_result = []
 
         def cb_func(tag, name, desc, file):
@@ -439,17 +448,17 @@
             file = file.decode()
             cb_result.append((tag, name, desc, file))
 
         # Actually call the describer function
         _e.dict_describe(dict_data, cb_func)
         return cb_result[0]
 
-    __describe_dict._DOC_ERRORS = ["desc"]
+    __describe_dict._DOC_ERRORS = ["desc"]  # type: ignore
 
-    def get_param(self, name):
+    def get_param(self, name: str) -> Any:
         """Get the value of a named parameter on this broker.
 
         Parameters are used to provide runtime information to individual
         provider backends.  See the method :py:meth:`set_param` for more details.
 
         .. warning::
 
@@ -457,17 +466,17 @@
             library version 2.0 and above
         """
         param = _e.broker_get_param(self._this, name.encode())
         if param is not None:
             param = param.decode()
         return param
 
-    get_param._DOC_ERRORS = ["param"]
+    get_param._DOC_ERRORS = ["param"]  # type: ignore
 
-    def set_param(self, name, value):
+    def set_param(self, name: str, value: Any) -> None:
         """Set the value of a named parameter on this broker.
 
         Parameters are used to provide runtime information to individual
         provider backends.
 
         .. warning::
 
@@ -481,257 +490,261 @@
 
 
 class Dict(_EnchantObject):
     """Dictionary object for the Enchant spellchecker.
 
     Dictionary objects are responsible for checking the spelling of words
     and suggesting possible corrections.  Each dictionary is owned by a
-    Broker object, but unless a new Broker has explicitly been created
-    then this will be the 'enchant' module default Broker and is of little
+    :py:class:`Broker` object, but unless a new :py:class:`Broker` has explicitly been created
+    then this will be the :py:mod:`enchant` module default :py:class:`Broker` and is of little
     interest.
 
     The important methods of this class include:
 
-        * check():              check whether a word id spelled correctly
-        * suggest():            suggest correct spellings for a word
-        * add():                add a word to the user's personal dictionary
-        * remove():             add a word to the user's personal exclude list
-        * add_to_session():     add a word to the current spellcheck session
-        * store_replacement():  indicate a replacement for a given word
+        * :py:meth:`check()`:              check whether a word is spelled correctly
+        * :py:meth:`suggest()`:            suggest correct spellings for a word
+        * :py:meth:`add()`:                add a word to the user's personal dictionary
+        * :py:meth:`remove()`:             add a word to the user's personal exclude list
+        * :py:meth:`add_to_session()`:     add a word to the current spellcheck session
+        * :py:meth:`store_replacement()`:  indicate a replacement for a given word
 
     Information about the dictionary is available using the following
     attributes:
 
-        * tag:        the language tag of the dictionary
-        * provider:   a ProviderDesc object for the dictionary provider
+        * :py:attr:`tag`:        the language tag of the dictionary
+        * :py:attr:`provider`:   a :py:class:`ProviderDesc` object for the dictionary provider
 
     """
 
-    def __init__(self, tag=None, broker=None):
+    def __init__(
+        self, tag: Optional[str] = None, broker: Optional[Broker] = None
+    ) -> None:
         """Dict object constructor.
 
         A dictionary belongs to a specific language, identified by the
-        string <tag>.  If the tag is not given or is None, an attempt to
-        determine the language currently in use is made using the 'locale'
-        module.  If the current language cannot be determined, Error is raised.
+        string `tag`.  If the tag is not given or is `None`, an attempt to
+        determine the language currently in use is made using the :py:mod:`locale`
+        module.  If the current language cannot be determined, :py:exc:`~.errors.Error` is raised.
 
-        If <tag> is instead given the value of False, a 'dead' Dict object
+        If `tag` is instead given the value of `False`, a 'dead' Dict object
         is created without any reference to a language.  This is typically
         only useful within PyEnchant itself.  Any other non-string value
-        for <tag> raises Error.
+        for `tag` raises :py:exc:`~.errors.Error`.
 
-        Each dictionary must also have an associated Broker object which
+        Each dictionary must also have an associated `Broker` object which
         obtains the dictionary information from the underlying system. This
-        may be specified using <broker>.  If not given, the default broker
+        may be specified using `broker`.  If not given, the default broker
         is used.
         """
         # Initialise misc object attributes to None
         self.provider = None
         # If no tag was given, use the default language
         if tag is None:
             tag = get_default_language()
             if tag is None:
-                err = "No tag specified and default language could not "
-                err = err + "be determined."
-                raise Error(err)
+                raise Error(
+                    "No tag specified and default language could not be determined."
+                )
         self.tag = tag
         # If no broker was given, use the default broker
         if broker is None:
             broker = _broker
         self._broker = broker
         # Now let the superclass initialise the C-library object
         super().__init__()
 
-    def _init_this(self):
+    def _init_this(self) -> None:
         # Create dead object if False was given as the tag.
         # Otherwise, use the broker to get C-library pointer data.
         self._this = None
         if self.tag:
             this = self._broker._request_dict_data(self.tag)
             self._switch_this(this, self._broker)
 
-    def __del__(self):
+    def __del__(self) -> None:
         """Dict object destructor."""
         # Calling free() might fail if python is shutting down
         try:
             self._free()
         except (AttributeError, TypeError):
             pass
 
-    def _switch_this(self, this, broker):
+    def _switch_this(self, this, broker: Broker) -> None:
         """Switch the underlying C-library pointer for this object.
 
-        As all useful state for a Dict is stored by the underlying C-library
+        As all useful state for a `Dict` is stored by the underlying C-library
         pointer, it is very convenient to allow this to be switched at
         run-time.  Pass a new dict data object into this method to affect
-        the necessary changes.  The creating Broker object (at the Python
+        the necessary changes.  The creating `Broker` object (at the Python
         level) must also be provided.
 
         This should *never* *ever* be used by application code.  It's
-        a convenience for developers only, replacing the clunkier <data>
-        parameter to __init__ from earlier versions.
+        a convenience for developers only, replacing the clunkier `data`
+        parameter to `__init__` from earlier versions.
         """
         # Free old dict data
         Dict._free(self)
         # Hook in the new stuff
         self._this = this
         self._broker = broker
         # Update object properties
         desc = self.__describe(check_this=False)
         self.tag = desc[0]
         self.provider = ProviderDesc(*desc[1:])
 
-    _switch_this._DOC_ERRORS = ["init"]
+    _switch_this._DOC_ERRORS = ["init"]  # type: ignore
 
-    def _check_this(self, msg=None):
-        """Extend _EnchantObject._check_this() to check Broker validity.
+    def _check_this(self, msg: Optional[str] = None) -> None:
+        """Extend `_EnchantObject._check_this()` to check Broker validity.
 
         It is possible for the managing Broker object to be freed without
-        freeing the Dict.  Thus validity checking must take into account
-        self._broker._this as well as self._this.
+        freeing the `Dict`.  Thus validity checking must take into account
+        `self._broker._this` as well as `self._this`.
         """
         if self._broker is None or self._broker._this is None:
             self._this = None
         super()._check_this(msg)
 
-    def _raise_error(self, default="Unspecified Error", eclass=Error):
-        """Overrides _EnchantObject._raise_error to check dict errors."""
+    def _raise_error(
+        self, default: str = "Unspecified Error", eclass: Type[Error] = Error
+    ) -> NoReturn:
+        """Overrides `_EnchantObject._raise_error` to check dict errors."""
         err = _e.dict_get_error(self._this)
         if err == "" or err is None:
             raise eclass(default)
         raise eclass(err.decode())
 
-    def _free(self):
-        """Free the system resources associated with a Dict object.
+    def _free(self) -> None:
+        """Free the system resources associated with a `Dict` object.
 
-        This method frees underlying system resources for a Dict object.
-        Once it has been called, the Dict object must no longer be used.
+        This method frees underlying system resources for a `Dict` object.
+        Once it has been called, the `Dict` object must no longer be used.
         It is called automatically when the object is garbage collected.
         """
         if self._this is not None:
             # The broker may have been freed before the dict.
             # It will have freed the underlying pointers already.
             if self._broker is not None and self._broker._this is not None:
                 self._broker._free_dict(self)
 
-    def check(self, word):
+    def check(self, word: str) -> bool:
         """Check spelling of a word.
 
         This method takes a word in the dictionary language and returns
-        True if it is correctly spelled, and false otherwise.
+        `True` if it is correctly spelled, and `False` otherwise.
         """
         self._check_this()
         # Enchant asserts that the word is non-empty.
         # Check it up-front to avoid nasty warnings on stderr.
         if len(word) == 0:
             raise ValueError("can't check spelling of empty string")
         val = _e.dict_check(self._this, word.encode())
         if val == 0:
             return True
         if val > 0:
             return False
         self._raise_error()
 
-    def suggest(self, word):
+    def suggest(self, word: str) -> List[str]:
         """Suggest possible spellings for a word.
 
         This method tries to guess the correct spelling for a given
         word, returning the possibilities in a list.
         """
         self._check_this()
         # Enchant asserts that the word is non-empty.
         # Check it up-front to avoid nasty warnings on stderr.
         if len(word) == 0:
             raise ValueError("can't suggest spellings for empty string")
         suggs = _e.dict_suggest(self._this, word.encode())
         return [w.decode() for w in suggs]
 
-    def add(self, word):
+    def add(self, word: str) -> None:
         """Add a word to the user's personal word list."""
         self._check_this()
         _e.dict_add(self._this, word.encode())
 
-    def remove(self, word):
+    def remove(self, word: str) -> None:
         """Add a word to the user's personal exclude list."""
         self._check_this()
         _e.dict_remove(self._this, word.encode())
 
-    def add_to_pwl(self, word):
+    def add_to_pwl(self, word: str) -> None:
         """Add a word to the user's personal word list."""
         warnings.warn(
             "Dict.add_to_pwl is deprecated, please use Dict.add",
             category=DeprecationWarning,
             stacklevel=2,
         )
         self._check_this()
         _e.dict_add_to_pwl(self._this, word.encode())
 
-    def add_to_session(self, word):
+    def add_to_session(self, word: str) -> None:
         """Add a word to the session personal list."""
         self._check_this()
         _e.dict_add_to_session(self._this, word.encode())
 
-    def remove_from_session(self, word):
+    def remove_from_session(self, word: str) -> None:
         """Add a word to the session exclude list."""
         self._check_this()
         _e.dict_remove_from_session(self._this, word.encode())
 
-    def is_added(self, word):
+    def is_added(self, word: str) -> bool:
         """Check whether a word is in the personal word list."""
         self._check_this()
         return _e.dict_is_added(self._this, word.encode())
 
-    def is_removed(self, word):
+    def is_removed(self, word: str) -> bool:
         """Check whether a word is in the personal exclude list."""
         self._check_this()
         return _e.dict_is_removed(self._this, word.encode())
 
-    def store_replacement(self, mis, cor):
+    def store_replacement(self, mis: str, cor: str) -> None:
         """Store a replacement spelling for a miss-spelled word.
 
         This method makes a suggestion to the spellchecking engine that the
-        miss-spelled word <mis> is in fact correctly spelled as <cor>.  Such
-        a suggestion will typically mean that <cor> appears early in the
-        list of suggested spellings offered for later instances of <mis>.
+        miss-spelled word `mis` is in fact correctly spelled as `cor`.  Such
+        a suggestion will typically mean that `cor` appears early in the
+        list of suggested spellings offered for later instances of `mis`.
         """
         if not mis:
             raise ValueError("can't store replacement for an empty string")
         if not cor:
             raise ValueError("can't store empty string as a replacement")
         self._check_this()
         _e.dict_store_replacement(self._this, mis.encode(), cor.encode())
 
-    store_replacement._DOC_ERRORS = ["mis", "mis"]
+    store_replacement._DOC_ERRORS = ["mis", "mis"]  # type: ignore
 
-    def __describe(self, check_this=True):
+    def __describe(self, check_this: bool = True) -> Tuple[str, str, str, str]:
         """Return a tuple describing the dictionary.
 
         This method returns a four-element tuple describing the underlying
         spellchecker system providing the dictionary.  It will contain the
         following strings:
 
             * language tag
             * name of dictionary provider
             * description of dictionary provider
             * dictionary file
 
         Direct use of this method is not recommended - instead, access this
-        information through the 'tag' and 'provider' attributes.
+        information through the attributes :py:attr:`tag` and :py:attr:`provider`.
         """
         if check_this:
             self._check_this()
         _e.dict_describe(self._this, self.__describe_callback)
         return self.__describe_result
 
     def __describe_callback(self, tag, name, desc, file):
         """Collector callback for dictionary description.
 
-        This method is used as a callback into the _enchant function
-        'enchant_dict_describe'.  It collects the given arguments in
-        a tuple and stores them in the attribute '__describe_result'.
+        This method is used as a callback into the `_enchant` function
+        `enchant_dict_describe`.  It collects the given arguments in
+        a tuple and stores them in the attribute :py:attr:`__describe_result`.
         """
         tag = tag.decode()
         name = name.decode()
         desc = desc.decode()
         file = file.decode()
         self.__describe_result = (tag, name, desc, file)
 
@@ -741,44 +754,46 @@
 
     .. note::
         As of version 1.4.0, enchant manages a per-user pwl and
         exclude list.  This class is now only needed if you want
         to explicitly maintain a separate word list in addition to
         the default one.
 
-    This class behaves as the standard Dict class, but also manages a
+    This class behaves as the standard class :py:class:`Dict`, but also manages a
     personal word list stored in a separate file.  The file must be
-    specified at creation time by the 'pwl' argument to the constructor.
+    specified at creation time by the `pwl` argument to the constructor.
     Words added to the dictionary are automatically appended to the pwl file.
 
     A personal exclude list can also be managed, by passing another filename
-    to the constructor in the optional 'pel' argument.  If this is not given,
+    to the constructor in the optional `pel` argument.  If this is not given,
     requests to exclude words are ignored.
 
-    If either 'pwl' or 'pel' are None, an in-memory word list is used.
-    This will prevent calls to add() and remove() from affecting the user's
+    If either `pwl` or `pel` are `None`, an in-memory word list is used.
+    This will prevent calls to :py:meth:`add()` and :py:meth:`remove()` from affecting the user's
     default word lists.
 
-    The Dict object managing the PWL is available as the 'pwl' attribute.
-    The Dict object managing the PEL is available as the 'pel' attribute.
+    The `Dict` object managing the PWL is available as the :py:attr:`pwl` attribute.
+    The `Dict` object managing the PEL is available as the :py:attr:`pel` attribute.
 
-    To create a DictWithPWL from the user's default language, use None
-    as the 'tag' argument.
+    To create a `DictWithPWL` from the user's default language, use `None`
+    as the `tag` argument.
     """
 
     _DOC_ERRORS = ["pel", "pel", "PEL", "pel"]
 
-    def __init__(self, tag, pwl=None, pel=None, broker=None):
+    def __init__(
+        self, tag: str, pwl: str = None, pel: str = None, broker: Broker = None
+    ) -> None:
         """DictWithPWL constructor.
 
-        The argument 'pwl', if not None, names a file containing the
+        The argument `pwl`, if not `None,` names a file containing the
         personal word list.  If this file does not exist, it is created
         with default permissions.
 
-        The argument 'pel', if not None, names a file containing the personal
+        The argument `pel`, if not `None,` names a file containing the personal
         exclude list.  If this file does not exist, it is created with
         default permissions.
         """
         super().__init__(tag, broker)
         if pwl is not None:
             if not os.path.exists(pwl):
                 f = open(pwl, "wt")
@@ -788,98 +803,100 @@
         else:
             self.pwl = PyPWL()
         if pel is not None:
             if not os.path.exists(pel):
                 f = open(pel, "wt")
                 f.close()
                 del f
-            self.pel = self._broker.request_pwl_dict(pel)
+            self.pel = self._broker.request_pwl_dict(
+                pel
+            )  # type: Union[None, _e.t_dict, PyPWL]
         else:
             self.pel = PyPWL()
 
-    def _check_this(self, msg=None):
-        """Extend Dict._check_this() to check PWL validity."""
+    def _check_this(self, msg: Optional[str] = None) -> None:
+        """Extend :py:meth:`Dict._check_this()` to check PWL validity."""
         if self.pwl is None:
             self._free()
         if self.pel is None:
             self._free()
         super()._check_this(msg)
         self.pwl._check_this(msg)
         self.pel._check_this(msg)
 
-    def _free(self):
-        """Extend Dict._free() to free the PWL as well."""
+    def _free(self) -> None:
+        """Extend :py:meth:`Dict._free()` to free the PWL as well."""
         if self.pwl is not None:
             self.pwl._free()
             self.pwl = None
         if self.pel is not None:
             self.pel._free()
             self.pel = None
         super()._free()
 
-    def check(self, word):
+    def check(self, word: str) -> bool:
         """Check spelling of a word.
 
         This method takes a word in the dictionary language and returns
-        True if it is correctly spelled, and false otherwise.  It checks
+        `True` if it is correctly spelled, and `False` otherwise.  It checks
         both the dictionary and the personal word list.
         """
         if self.pel.check(word):
             return False
         if self.pwl.check(word):
             return True
         if super().check(word):
             return True
         return False
 
-    def suggest(self, word):
+    def suggest(self, word: str) -> List[str]:
         """Suggest possible spellings for a word.
 
         This method tries to guess the correct spelling for a given
         word, returning the possibilities in a list.
         """
         suggs = super().suggest(word)
         suggs.extend([w for w in self.pwl.suggest(word) if w not in suggs])
         for i in range(len(suggs) - 1, -1, -1):
             if self.pel.check(suggs[i]):
                 del suggs[i]
         return suggs
 
-    def add(self, word):
+    def add(self, word: str) -> None:
         """Add a word to the associated personal word list.
 
         This method adds the given word to the personal word list, and
         automatically saves the list to disk.
         """
         self._check_this()
         self.pwl.add(word)
         self.pel.remove(word)
 
-    def remove(self, word):
+    def remove(self, word: str) -> None:
         """Add a word to the associated exclude list."""
         self._check_this()
         self.pwl.remove(word)
         self.pel.add(word)
 
-    def add_to_pwl(self, word):
+    def add_to_pwl(self, word: str) -> None:
         """Add a word to the associated personal word list.
 
         This method adds the given word to the personal word list, and
         automatically saves the list to disk.
         """
         self._check_this()
         self.pwl.add_to_pwl(word)
         self.pel.remove(word)
 
-    def is_added(self, word):
+    def is_added(self, word: str) -> bool:
         """Check whether a word is in the personal word list."""
         self._check_this()
         return self.pwl.is_added(word)
 
-    def is_removed(self, word):
+    def is_removed(self, word: str) -> bool:
         """Check whether a word is in the personal exclude list."""
         self._check_this()
         return self.pel.is_added(word)
 
 
 ##  Create a module-level default broker object, and make its important
 ##  methods available at the module level.
@@ -889,29 +906,29 @@
 dict_exists = _broker.dict_exists
 list_dicts = _broker.list_dicts
 list_languages = _broker.list_languages
 get_param = _broker.get_param
 set_param = _broker.set_param
 
 #  Expose the "get_version" function.
-def get_enchant_version():
+def get_enchant_version() -> str:
     """Get the version string for the underlying enchant library."""
     return _e.get_version().decode()
 
 
 #  Expose the "set_prefix_dir" function.
-def set_prefix_dir(path):
+def set_prefix_dir(path: str) -> None:
     """Set the prefix used by the Enchant library to find its plugins
 
     Called automatically when the Python library is imported when
     required.
     """
     return _e.set_prefix_dir(path)
 
     set_prefix_dir._DOC_ERRORS = ["plugins"]
 
 
-def get_user_config_dir():
+def get_user_config_dir() -> str:
     """Return the path that will be used by some
     Enchant providers to look for custom dictionaries.
     """
     return _e.get_user_config_dir().decode()
```

### Comparing `pyenchant-3.2.2/enchant/_enchant.py` & `pyenchant-3.3.0rc1/enchant/_enchant.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,89 +45,99 @@
         * callback functions do not take a user_data argument, since
           python has proper closures that can manage this internally
         * string lengths are not passed into functions such as dict_check,
           since python strings know how long they are
 
 """
 
-import sys
-import os
-import os.path
 import ctypes
-from ctypes import c_char_p, c_int, c_size_t, c_void_p, pointer, CFUNCTYPE, POINTER
 import ctypes.util
+import os
+import os.path
 import platform
+import sys
 import textwrap
+from ctypes import CFUNCTYPE, POINTER, c_char_p, c_int, c_size_t, c_void_p, pointer
+from typing import Callable, List, Optional, TypeVar  # noqa F401
 
 
-def from_prefix(prefix):
+def from_prefix(prefix: str) -> str:
     find_message("finding from prefix ", prefix)
     assert os.path.exists(prefix), prefix + "  does not exist"
     bin_path = os.path.join(prefix, "bin")
     enchant_dll_path = os.path.join(bin_path, "libenchant-2.dll")
     assert os.path.exists(enchant_dll_path), enchant_dll_path + " does not exist"
     # Make sure all the dlls found next to libenchant-2.dll
     # (libglib-2.0-0.dll, libgmodule-2.0-0.dll, ...) can be
     # used without having to modify %PATH%
     new_path = bin_path + os.pathsep + os.environ["PATH"]
     find_message("Prepending ", bin_path, " to %PATH%")
     os.environ["PATH"] = new_path
     return enchant_dll_path
 
 
-def from_env_var(library_path):
+def from_env_var(library_path: str) -> str:
     find_message("using PYENCHANT_LIBRARY_PATH env var")
     assert os.path.exists(library_path), library_path + " does not exist"
     return library_path
 
 
-def from_package_resources():
+def from_package_resources() -> Optional[str]:
     if sys.platform != "win32":
         return None
     bits, _ = platform.architecture()
     if bits == "64bit":
         subdir = "mingw64"  # hopefully this is compatible
     else:
         subdir = "mingw32"  # ditto
     this_path = os.path.dirname(os.path.abspath(__file__))
     data_path = os.path.join(this_path, "data", subdir)
     find_message("looking in ", data_path)
     if os.path.exists(data_path):
         return from_prefix(data_path)
+    return None
 
 
-def from_system():
+def from_system() -> Optional[str]:
     # Note: keep enchant-2 first
     find_message("looking in system")
     candidates = [
         "enchant-2",
         "libenchant-2",
         "enchant",
         "libenchant",
         "enchant-1",
         "libenchant-1",
     ]
 
+    # On M1 macs, Homebrew is in /opt, which isn't on the default
+    # DYLD_LIBRARY_PATH. Look for the homebrew path explicitly.
+    if sys.platform == "darwin" and platform.machine() == "arm64":
+        candidates.extend(
+            [f"/opt/homebrew/lib/{candidate}" for candidate in candidates]
+        )
+
     for name in candidates:
         find_message("with name ", name)
         res = ctypes.util.find_library(name)
         if res:
             return res
+    return None
 
 
 VERBOSE_FIND = False
 
 
-def find_message(*args):
+def find_message(*args: str) -> None:
     if not VERBOSE_FIND:
         return
     print("pyenchant:: ", *args, sep="")
 
 
-def find_c_enchant_lib():
+def find_c_enchant_lib() -> Optional[str]:
     verbose = os.environ.get("PYENCHANT_VERBOSE_FIND")
     if verbose:
         global VERBOSE_FIND
         VERBOSE_FIND = True
     prefix = os.environ.get("PYENCHANT_ENCHANT_PREFIX")
     if prefix:
         return from_prefix(prefix)
@@ -181,14 +191,16 @@
 t_dict_desc_func = callback(None, c_char_p, c_char_p, c_char_p, c_char_p, c_void_p)
 
 
 # Simple typedefs for readability
 
 t_broker = c_void_p
 t_dict = c_void_p
+_B = TypeVar("_B", bound=t_broker)
+_D = TypeVar("_D", bound=t_dict)
 
 
 # Now we can define the types of each function we are going to use
 
 broker_init = e.enchant_broker_init
 broker_init.argtypes = []
 broker_init.restype = t_broker
@@ -222,108 +234,105 @@
 broker_get_error.restype = c_char_p
 
 broker_describe1 = e.enchant_broker_describe
 broker_describe1.argtypes = [t_broker, t_broker_desc_func, c_void_p]
 broker_describe1.restype = None
 
 
-def broker_describe(broker, cbfunc):
+def broker_describe(broker: _B, cbfunc) -> None:
     def cbfunc1(*args):
         cbfunc(*args[:-1])
 
     broker_describe1(broker, t_broker_desc_func(cbfunc1), None)
 
 
 broker_list_dicts1 = e.enchant_broker_list_dicts
 broker_list_dicts1.argtypes = [t_broker, t_dict_desc_func, c_void_p]
 broker_list_dicts1.restype = None
 
 
-def broker_list_dicts(broker, cbfunc):
+def broker_list_dicts(broker: _B, cbfunc) -> None:
     def cbfunc1(*args):
         cbfunc(*args[:-1])
 
     broker_list_dicts1(broker, t_dict_desc_func(cbfunc1), None)
 
 
 try:
-    broker_get_param = e.enchant_broker_get_param
+    broker_get_param = e.enchant_broker_get_param  # type: Callable[[_B, bytes], bytes]
 except AttributeError:
     #  Make the lookup error occur at runtime
-    def broker_get_param(broker, name):
+    def broker_get_param(broker: _B, name: bytes) -> bytes:
         return e.enchant_broker_get_param(broker, name)
 
-
 else:
-    broker_get_param.argtypes = [t_broker, c_char_p]
-    broker_get_param.restype = c_char_p
+    broker_get_param.argtypes = [t_broker, c_char_p]  # type: ignore
+    broker_get_param.restype = c_char_p  # type: ignore
 
 try:
-    broker_set_param = e.enchant_broker_set_param
+    broker_set_param = (
+        e.enchant_broker_set_param
+    )  # type: Callable[[_B, bytes, bytes], None]
 except AttributeError:
     #  Make the lookup error occur at runtime
-    def broker_set_param(broker, name, value):
+    def broker_set_param(broker: _B, name: bytes, value: bytes) -> None:
         return e.enchant_broker_set_param(broker, name, value)
 
-
 else:
-    broker_set_param.argtypes = [t_broker, c_char_p, c_char_p]
-    broker_set_param.restype = None
+    broker_set_param.argtypes = [t_broker, c_char_p, c_char_p]  # type: ignore
+    broker_set_param.restype = None  # type: ignore
 
 try:
-    get_version = e.enchant_get_version
+    get_version = e.enchant_get_version  # type: Callable[[], bytes]
 except AttributeError:
     #  Make the lookup error occur at runtime
-    def get_version():
+    def get_version() -> bytes:
         return e.enchant_get_version()
 
-
 else:
-    get_version.argtypes = []
-    get_version.restype = c_char_p
+    get_version.argtypes = []  # type: ignore
+    get_version.restype = c_char_p  # type: ignore
 
 try:
-    set_prefix_dir = e.enchant_set_prefix_dir
+    set_prefix_dir = e.enchant_set_prefix_dir  # type: Callable[[bytes], None]
 except AttributeError:
     #  Make the lookup error occur at runtime
-    def set_prefix_dir(path):
+    def set_prefix_dir(path: bytes):
         return e.enchant_set_prefix_dir(path)
 
-
 else:
-    set_prefix_dir.argtypes = [c_char_p]
-    set_prefix_dir.restype = None
+    set_prefix_dir.argtypes = [c_char_p]  # type: ignore
+    set_prefix_dir.restype = None  # type: ignore
 
 try:
-    get_user_config_dir = e.enchant_get_user_config_dir
+    get_user_config_dir = e.enchant_get_user_config_dir  # type: Callable[[], bytes]
 except AttributeError:
     #  Make the lookup error occur at runtime
-    def get_user_config_dir():
+    def get_user_config_dir() -> bytes:
         return e.enchant_get_user_config_dir()
 
-
 else:
-    get_user_config_dir.argtypes = []
-    get_user_config_dir.restype = c_char_p
+    get_user_config_dir.argtypes = []  # type: ignore
+    get_user_config_dir.restype = c_char_p  # type: ignore
 
 dict_check1 = e.enchant_dict_check
 dict_check1.argtypes = [t_dict, c_char_p, c_size_t]
 dict_check1.restype = c_int
 
 
-def dict_check(dict, word):
+def dict_check(dict: _D, word: bytes) -> int:
     return dict_check1(dict, word, len(word))
 
 
 dict_suggest1 = e.enchant_dict_suggest
 dict_suggest1.argtypes = [t_dict, c_char_p, c_size_t, POINTER(c_size_t)]
 dict_suggest1.restype = POINTER(c_char_p)
 
 
-def dict_suggest(dict, word):
+def dict_suggest(dict: _D, word: bytes) -> List[bytes]:
     num_suggs_p = pointer(c_size_t(0))
     suggs_c = dict_suggest1(dict, word, len(word), num_suggs_p)
     suggs = []
     n = 0
     while n < num_suggs_p.contents.value:
         suggs.append(suggs_c[n])
         n = n + 1
@@ -333,78 +342,78 @@
 
 
 dict_add1 = e.enchant_dict_add
 dict_add1.argtypes = [t_dict, c_char_p, c_size_t]
 dict_add1.restype = None
 
 
-def dict_add(dict, word):
+def dict_add(dict: _D, word: bytes) -> None:
     return dict_add1(dict, word, len(word))
 
 
 dict_add_to_pwl1 = e.enchant_dict_add
 dict_add_to_pwl1.argtypes = [t_dict, c_char_p, c_size_t]
 dict_add_to_pwl1.restype = None
 
 
-def dict_add_to_pwl(dict, word):
+def dict_add_to_pwl(dict: _D, word: bytes) -> None:
     return dict_add_to_pwl1(dict, word, len(word))
 
 
 dict_add_to_session1 = e.enchant_dict_add_to_session
 dict_add_to_session1.argtypes = [t_dict, c_char_p, c_size_t]
 dict_add_to_session1.restype = None
 
 
-def dict_add_to_session(dict, word):
+def dict_add_to_session(dict: _D, word: bytes) -> None:
     return dict_add_to_session1(dict, word, len(word))
 
 
 dict_remove1 = e.enchant_dict_remove
 dict_remove1.argtypes = [t_dict, c_char_p, c_size_t]
 dict_remove1.restype = None
 
 
-def dict_remove(dict, word):
+def dict_remove(dict: _D, word: bytes) -> None:
     return dict_remove1(dict, word, len(word))
 
 
 dict_remove_from_session1 = e.enchant_dict_remove_from_session
 dict_remove_from_session1.argtypes = [t_dict, c_char_p, c_size_t]
 dict_remove_from_session1.restype = c_int
 
 
-def dict_remove_from_session(dict, word):
+def dict_remove_from_session(dict: _D, word: bytes) -> int:
     return dict_remove_from_session1(dict, word, len(word))
 
 
 dict_is_added1 = e.enchant_dict_is_added
 dict_is_added1.argtypes = [t_dict, c_char_p, c_size_t]
 dict_is_added1.restype = c_int
 
 
-def dict_is_added(dict, word):
+def dict_is_added(dict: _D, word: bytes) -> int:
     return dict_is_added1(dict, word, len(word))
 
 
 dict_is_removed1 = e.enchant_dict_is_removed
 dict_is_removed1.argtypes = [t_dict, c_char_p, c_size_t]
 dict_is_removed1.restype = c_int
 
 
-def dict_is_removed(dict, word):
+def dict_is_removed(dict: _D, word: bytes) -> int:
     return dict_is_removed1(dict, word, len(word))
 
 
 dict_store_replacement1 = e.enchant_dict_store_replacement
 dict_store_replacement1.argtypes = [t_dict, c_char_p, c_size_t, c_char_p, c_size_t]
 dict_store_replacement1.restype = None
 
 
-def dict_store_replacement(dict, mis, cor):
+def dict_store_replacement(dict: _D, mis: bytes, cor: bytes) -> None:
     return dict_store_replacement1(dict, mis, len(mis), cor, len(cor))
 
 
 dict_free_string_list = e.enchant_dict_free_string_list
 dict_free_string_list.argtypes = [t_dict, POINTER(c_char_p)]
 dict_free_string_list.restype = None
 
@@ -413,12 +422,12 @@
 dict_get_error.restype = c_char_p
 
 dict_describe1 = e.enchant_dict_describe
 dict_describe1.argtypes = [t_dict, t_dict_desc_func, c_void_p]
 dict_describe1.restype = None
 
 
-def dict_describe(dict, cbfunc):
+def dict_describe(dict: _D, cbfunc) -> None:
     def cbfunc1(tag, name, desc, file, data):
         cbfunc(tag, name, desc, file)
 
     dict_describe1(dict, t_dict_desc_func(cbfunc1), None)
```

### Comparing `pyenchant-3.2.2/enchant/checker/CmdLineChecker.py` & `pyenchant-3.3.0rc1/enchant/checker/CmdLineChecker.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,23 @@
 # file, but you are not obligated to do so.  If you do not wish to
 # do so, delete this exception statement from your version.
 #
 """
 
     enchant.checker.CmdLineChecker:  Command-Line spell checker
 
-    This module provides the class CmdLineChecker, which interactively
+    This module provides the class :py:class:`CmdLineChecker`, which interactively
     spellchecks a piece of text by interacting with the user on the
     command line.  It can also be run as a script to spellcheck a file.
 
 """
 
 import sys
+from argparse import ArgumentParser
+from typing import Optional
 
 from enchant.checker import SpellChecker
 
 # Helpers
 
 colors = {
     "normal": "\x1b[0m",
@@ -54,15 +56,15 @@
     "cyan": "\x1b[36m",
     "grey": "\x1b[90m",
     "gray": "\x1b[90m",
     "bold": "\x1b[1m",
 }
 
 
-def color(string, color="normal", prefix=""):
+def color(string: str, color: str = "normal", prefix: str = "") -> str:
     """
     Change text color for the Linux terminal.
 
     Args:
         string (str): String to colorify
         color (str): Color to colorify the string in the following list:
             black, red, green, yellow, blue, purple, cyan, gr[ae]y
@@ -70,95 +72,92 @@
     """
     if sys.stdout.isatty():
         return colors[color] + prefix + string + colors["normal"]
     else:
         return prefix + string
 
 
-def success(string):
+def success(string: str) -> str:
     return "[" + color("+", color="green") + "] " + string
 
 
-def error(string):
+def error(string: str) -> str:
     return "[" + color("!", color="red") + "] " + string
 
 
-def warning(string):
+def warning(string: str) -> str:
     return "[" + color("*", color="yellow") + "] " + string
 
 
-def info(string):
+def info(string: str) -> str:
     return "[" + color(".", color="blue") + "] " + string
 
 
 class CmdLineChecker:
     """A simple command-line spell checker.
 
     This class implements a simple command-line spell checker.  It must
     be given a SpellChecker instance to operate on, and interacts with
     the user by printing instructions on stdout and reading commands from
     stdin.
     """
 
     _DOC_ERRORS = ["stdout", "stdin"]
 
-    def __init__(self):
+    def __init__(self, checker: SpellChecker) -> None:
         self._stop = False
-        self._checker = None
+        self._checker = checker
 
-    def set_checker(self, chkr):
-        self._checker = chkr
-
-    def get_checker(self, chkr):
+    def get_checker(self, chkr: SpellChecker) -> SpellChecker:
         return self._checker
 
-    def run(self):
+    def run(self) -> None:
         """Run the spellchecking loop."""
         self._stop = False
         for err in self._checker:
             self.error = err
             self.print_error()
             self.print_suggestions()
             status = self.read_command()
             while not status and not self._stop:
                 status = self.read_command()
             if self._stop:
                 break
 
-    def print_error(self):
+    def print_error(self) -> None:
         """print the spelling error to the console.
 
         Prints the misspelled word along with 100 characters of
         context on either side.  This number was arbitrarily chosen
         and could be modified to be tunable or changed entirely.
         It seems to be enough context to be helpful though
         """
         error_string = self._build_context(
             self.error.get_text(), self.error.word, self.error.wordpos
         )
-        print([error("ERROR: %s" % color(self.error.word, color="red"))])
-        print([info("")])
-        print([info(error_string)])
-        print([info("")])
+        print(error("ERROR: %s" % color(self.error.word, color="red")))
+        print(info(""))
+        print(info(error_string))
+        print(info(""))
 
     @staticmethod
-    def _build_context(text, error_word, error_start):
+    def _build_context(text: str, error_word: str, error_start: int) -> str:
         """creates the context line.
 
         This function will search forward and backward
         from the error word to find the nearest newlines.
         it will return this line with the error word
         colored red."""
         start_newline = text.rfind("\n", 0, error_start)
         end_newline = text.find("\n", error_start)
         return text[start_newline + 1 : end_newline].replace(
             error_word, color(error_word, color="red")
         )
 
-    def print_suggestions(self):
+    def print_suggestions(self) -> None:
         """Prints out the suggestions for a given error.
 
         This function will add vertical pipes to separate choices
         as well as the index of the replacement as expected by the replace function.
         I don't believe zero indexing is a problem as long as the user can see the numbers :)
         """
         result = ""
@@ -175,138 +174,120 @@
                 result = (
                     result
                     + " | "
                     + color(str(index), color="yellow")
                     + ": "
                     + color(sugg, color="bold")
                 )
-        print([info("HOW ABOUT:"), result])
+        print(info("HOW ABOUT:"), result)
 
-    def print_help(self):
+    def print_help(self) -> None:
         print(
-            [
-                info(
-                    color("0", color="yellow")
-                    + ".."
-                    + color("N", color="yellow")
-                    + ":\t"
-                    + color("replace", color="bold")
-                    + " with the numbered suggestion"
-                )
-            ]
+            info(
+                color("0", color="yellow")
+                + ".."
+                + color("N", color="yellow")
+                + ":\t"
+                + color("replace", color="bold")
+                + " with the numbered suggestion"
+            )
         )
         print(
-            [
-                info(
-                    color("R", color="cyan")
-                    + color("0", color="yellow")
-                    + ".."
-                    + color("R", color="cyan")
-                    + color("N", color="yellow")
-                    + ":\t"
-                    + color("always replace", color="bold")
-                    + " with the numbered suggestion"
-                )
-            ]
+            info(
+                color("R", color="cyan")
+                + color("0", color="yellow")
+                + ".."
+                + color("R", color="cyan")
+                + color("N", color="yellow")
+                + ":\t"
+                + color("always replace", color="bold")
+                + " with the numbered suggestion"
+            )
         )
         print(
-            [
-                info(
-                    color("i", color="cyan")
-                    + ":\t\t"
-                    + color("ignore", color="bold")
-                    + " this word"
-                )
-            ]
+            info(
+                color("i", color="cyan")
+                + ":\t\t"
+                + color("ignore", color="bold")
+                + " this word"
+            )
         )
         print(
-            [
-                info(
-                    color("I", color="cyan")
-                    + ":\t\t"
-                    + color("always ignore", color="bold")
-                    + " this word"
-                )
-            ]
+            info(
+                color("I", color="cyan")
+                + ":\t\t"
+                + color("always ignore", color="bold")
+                + " this word"
+            )
         )
         print(
-            [
-                info(
-                    color("a", color="cyan")
-                    + ":\t\t"
-                    + color("add", color="bold")
-                    + " word to personal dictionary"
-                )
-            ]
+            info(
+                color("a", color="cyan")
+                + ":\t\t"
+                + color("add", color="bold")
+                + " word to personal dictionary"
+            )
         )
         print(
-            [
-                info(
-                    color("e", color="cyan")
-                    + ":\t\t"
-                    + color("edit", color="bold")
-                    + " the word"
-                )
-            ]
+            info(
+                color("e", color="cyan")
+                + ":\t\t"
+                + color("edit", color="bold")
+                + " the word"
+            )
         )
         print(
-            [
-                info(
-                    color("q", color="cyan")
-                    + ":\t\t"
-                    + color("quit", color="bold")
-                    + " checking"
-                )
-            ]
+            info(
+                color("q", color="cyan")
+                + ":\t\t"
+                + color("quit", color="bold")
+                + " checking"
+            )
         )
         print(
-            [
-                info(
-                    color("h", color="cyan")
-                    + ":\t\tprint this "
-                    + color("help", color="bold")
-                    + " message"
-                )
-            ]
+            info(
+                color("h", color="cyan")
+                + ":\t\tprint this "
+                + color("help", color="bold")
+                + " message"
+            )
         )
-        print([info("----------------------------------------------------")])
+        print(info("----------------------------------------------------"))
         self.print_suggestions()
 
-    def read_command(self):
+    def read_command(self) -> bool:
         cmd = input(">> ")
         cmd = cmd.strip()
 
         if cmd.isdigit():
             repl = int(cmd)
             suggs = self.error.suggest()
             if repl >= len(suggs):
-                print([warning("No suggestion number"), repl])
+                print(warning("No suggestion number"), repl)
                 return False
             print(
-                [
-                    success(
-                        "Replacing '%s' with '%s'"
-                        % (
-                            color(self.error.word, color="red"),
-                            color(suggs[repl], color="green"),
-                        )
+                success(
+                    "Replacing '%s' with '%s'"
+                    % (
+                        color(self.error.word, color="red"),
+                        color(suggs[repl], color="green"),
                     )
-                ]
+                )
             )
             self.error.replace(suggs[repl])
             return True
 
         if cmd[0] == "R":
             if not cmd[1:].isdigit():
-                print([warning("Badly formatted command (try 'help')")])
+                print(warning("Badly formatted command (try 'help')"))
                 return False
             repl = int(cmd[1:])
             suggs = self.error.suggest()
             if repl >= len(suggs):
-                print([warning("No suggestion number"), repl])
+                print(warning("No suggestion number"), repl)
                 return False
             self.error.replace_always(suggs[repl])
             return True
 
         if cmd == "i":
             return True
 
@@ -315,98 +296,88 @@
             return True
 
         if cmd == "a":
             self.error.add()
             return True
 
         if cmd == "e":
-            repl = input(info("New Word: "))
-            self.error.replace(repl.strip())
+            replacement = get_input(info("New Word: "))
+            self.error.replace(replacement.strip())
             return True
 
         if cmd == "q":
             self._stop = True
             return True
 
         if "help".startswith(cmd.lower()):
             self.print_help()
             return False
 
-        print([warning("Badly formatted command (try 'help')")])
+        print(warning("Badly formatted command (try 'help')"))
         return False
 
-    def run_on_file(self, infile, outfile=None, enc=None):
+    def run_on_file(
+        self, infile: str, outfile: Optional[str] = None, enc: Optional[str] = None
+    ) -> None:
         """Run spellchecking on the named file.
         This method can be used to run the spellchecker over the named file.
-        If <outfile> is not given, the corrected contents replace the contents
-        of <infile>.  If <outfile> is given, the corrected contents will be
+        If `outfile` is not given, the corrected contents replace the contents
+        of `infile`.  If `outfile` is given, the corrected contents will be
         written to that file.  Use "-" to have the contents written to stdout.
-        If <enc> is given, it specifies the encoding used to read the
+        If `enc` is given, it specifies the encoding used to read the
         file's contents into a unicode string.  The output will be written
         in the same encoding.
         """
-        inStr = "".join(open(infile).readlines())
-        if enc is not None:
-            inStr = inStr.decode(enc)
+        inStr = open(infile, "r", encoding=enc).read()
         self._checker.set_text(inStr)
         begin_msg = "Beginning spell check of %s" % infile
-        print([info(begin_msg)])
-        print([info("-" * len(begin_msg))])
+        print(info(begin_msg))
+        print(info("-" * len(begin_msg)))
         self.run()
-        print([success("Completed spell check of %s" % infile)])
+        print(success("Completed spell check of %s" % infile))
         outStr = self._checker.get_text()
-        if enc is not None:
-            outStr = outStr.encode(enc)
         if outfile is None:
-            outF = open(infile, "w")
+            outF = open(infile, "w", encoding=enc)
         elif outfile == "-":
             outF = sys.stdout
         else:
-            outF = open(outfile, "w")
+            outF = open(outfile, "w", encoding=enc)
         outF.write(outStr)
         outF.close()
 
-    run_on_file._DOC_ERRORS = ["outfile", "infile", "outfile", "stdout"]
+    run_on_file._DOC_ERRORS = ["outfile", "infile", "outfile", "stdout"]  # type: ignore
 
 
-def _run_as_script():
+def _run_as_script() -> None:
     """Run the command-line spellchecker as a script.
     This function allows the spellchecker to be invoked from the command-line
     to check spelling in a file.
     """
-    # Check necessary command-line options
-    from optparse import OptionParser
-
-    op = OptionParser()
-    op.add_option(
+    parser = ArgumentParser()
+    parser.add_argument(
         "-o", "--output", dest="outfile", metavar="FILE", help="write changes into FILE"
     )
-    op.add_option(
+    parser.add_argument(
         "-l",
         "--lang",
         dest="lang",
         metavar="TAG",
         default="en_US",
         help="use language idenfified by TAG",
     )
-    op.add_option(
+    parser.add_argument(
         "-e",
         "--encoding",
         dest="enc",
         metavar="ENC",
         help="file is unicode with encoding ENC",
     )
-    (opts, args) = op.parse_args()
-    # Sanity check
-    if len(args) < 1:
-        raise ValueError("Must name a file to check")
-    if len(args) > 1:
-        raise ValueError("Can only check a single file")
+    parser.add_argument("infile", metavar="FILE", help="Input file name to check")
+    args = parser.parse_args()
     # Create and run the checker
-    chkr = SpellChecker(opts.lang)
-    cmdln = CmdLineChecker()
-    cmdln.set_checker(chkr)
-    cmdln.run_on_file(args[0], opts.outfile, opts.enc)
+    chkr = SpellChecker(args.lang)
+    cmdln = CmdLineChecker(chkr)
+    cmdln.run_on_file(args.infile, args.outfile, args.enc)
 
 
 if __name__ == "__main__":
     _run_as_script()
```

### Comparing `pyenchant-3.2.2/enchant/checker/GtkSpellCheckerDialog.py` & `pyenchant-3.3.0rc1/enchant/checker/GtkSpellCheckerDialog.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,24 +24,25 @@
 # the two.  You must obey the GNU Lesser General Public License in all
 # respects for all of the code used other than said providers.  If you modify
 # this file, you may extend this exception to your version of the
 # file, but you are not obligated to do so.  If you do not wish to
 # do so, delete this exception statement from your version.
 #
 
+from typing import Any, Iterable, List, Optional
+
 import gtk
 
+from enchant.checker import SpellChecker
 
 #   columns
 COLUMN_SUGGESTION = 0
 
 
-def create_list_view(
-    col_label,
-):
+def create_list_view(col_label: str) -> gtk.TreeView:
     # create list widget
     list_ = gtk.ListStore(str)
     list_view = gtk.TreeView(model=list_)
 
     list_view.set_rules_hint(True)
     list_view.get_selection().set_mode(gtk.SELECTION_SINGLE)
     # Add Colums
@@ -49,30 +50,30 @@
     renderer.set_data("column", COLUMN_SUGGESTION)
     column = gtk.TreeViewColumn(col_label, renderer, text=COLUMN_SUGGESTION)
     list_view.append_column(column)
     return list_view
 
 
 class GtkSpellCheckerDialog(gtk.Window):
-    def __init__(self, *args, **kwargs):
+    def __init__(self, checker: SpellChecker, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.set_title("Spell check")
         self.set_default_size(350, 200)
 
-        self._checker = None
+        self._checker = checker
         self._numContext = 40
 
         self.errors = None
 
         # create accel group
         accel_group = gtk.AccelGroup()
         self.add_accel_group(accel_group)
 
         # list of widgets to disable if there's no spell error left
-        self._conditional_widgets = []
+        self._conditional_widgets = []  # type: List[gtk.Widget]
         conditional = self._conditional_widgets.append
 
         # layout
         mainbox = gtk.VBox(spacing=5)
         hbox = gtk.HBox(spacing=5)
         self.add(mainbox)
         mainbox.pack_start(hbox, padding=5)
@@ -161,98 +162,86 @@
         button.connect("clicked", self._onClose)
         button.add_accelerator(
             "activate", accel_group, gtk.keysyms.Escape, 0, gtk.ACCEL_VISIBLE
         )
         button_box.pack_end(button)
 
         # dictionary label
-        self._dict_lable = gtk.Label("")
+        self._dict_lable = gtk.Label("Dictionary:%s" % (checker.dict.tag,))
         mainbox.pack_start(self._dict_lable, False, False, padding=5)
 
         mainbox.show_all()
 
-    def _onIgnore(self, w, *args):
+    def _onIgnore(self, w: gtk.Widget, *args: Any) -> None:
         print(["ignore"])
         self._advance()
 
-    def _onIgnoreAll(self, w, *args):
+    def _onIgnoreAll(self, w: gtk.Widget, *args: Any) -> None:
         print(["ignore all"])
         self._checker.ignore_always()
         self._advance()
 
-    def _onReplace(self, *args):
+    def _onReplace(self, *args: Any) -> None:
         print(["Replace"])
         repl = self._getRepl()
         self._checker.replace(repl)
         self._advance()
 
-    def _onReplaceAll(self, *args):
+    def _onReplaceAll(self, *args: Any) -> None:
         print(["Replace all"])
         repl = self._getRepl()
         self._checker.replace_always(repl)
         self._advance()
 
-    def _onAdd(self, *args):
+    def _onAdd(self, *args: Any) -> None:
         """Callback for the "add" button."""
         self._checker.add()
         self._advance()
 
-    def _onClose(self, w, *args):
+    def _onClose(self, w: gtk.Widget, *args: Any) -> bool:
         self.emit("delete_event", gtk.gdk.Event(gtk.gdk.BUTTON_PRESS))
         return True
 
-    def _onButtonPress(self, widget, event):
+    def _onButtonPress(self, widget: gtk.Widget, event) -> None:
         if event.type == gtk.gdk._2BUTTON_PRESS:
             print(["Double click!"])
             self._onReplace()
 
-    def _onSuggestionChanged(self, widget, *args):
+    def _onSuggestionChanged(self, widget: gtk.Widget, *args: Any) -> None:
         selection = self.suggestion_list_view.get_selection()
         model, iter = selection.get_selected()
         if iter:
             suggestion = model.get_value(iter, COLUMN_SUGGESTION)
             self.replace_text.set_text(suggestion)
 
-    def _getRepl(self):
+    def _getRepl(self) -> str:
         """Get the chosen replacement string."""
         repl = self.replace_text.get_text()
         repl = self._checker.coerce_string(repl)
         return repl
 
-    def _fillSuggestionList(self, suggestions):
+    def _fillSuggestionList(self, suggestions: Iterable[str]) -> None:
         model = self.suggestion_list_view.get_model()
         model.clear()
         for suggestion in suggestions:
             value = "%s" % (suggestion,)
-            model.append(
-                [
-                    value,
-                ]
-            )
-
-    def setSpellChecker(self, checker):
-        assert checker, "checker can't be None"
-        self._checker = checker
-        self._dict_lable.set_text("Dictionary:%s" % (checker.dict.tag,))
-
-    def getSpellChecker(self, checker):
-        return self._checker
+            model.append([value])
 
-    def updateUI(self):
+    def updateUI(self) -> None:
         self._advance()
 
-    def _disableButtons(self):
+    def _disableButtons(self) -> None:
         for w in self._conditional_widgets:
             w.set_sensitive(False)
 
-    def _enableButtons(self):
+    def _enableButtons(self) -> None:
         for w in self._conditional_widgets:
             w.set_sensitive(True)
 
-    def _advance(self):
+    def _advance(self) -> None:
         """Advance to the next error.
         This method advances the SpellChecker to the next error, if
         any.  It then displays the error and some surrounding context,
         and well as listing the suggested replacements.
         """
         # Disable interaction if no checker
         if self._checker is None:
@@ -287,25 +276,24 @@
         self._fillSuggestionList(suggs)
         if suggs:
             self.replace_text.set_text(suggs[0])
         else:
             self.replace_text.set_text("")
 
 
-def _test():
+def _test() -> None:
     from enchant.checker import SpellChecker
 
     text = "This is sme text with a fw speling errors in it. Here are a fw more to tst it ut."
     print(["BEFORE:", text])
-    chk_dlg = GtkSpellCheckerDialog()
+    chkr = SpellChecker("en_US", text)
+
+    chk_dlg = GtkSpellCheckerDialog(chkr)
     chk_dlg.show()
     chk_dlg.connect("delete_event", gtk.main_quit)
 
-    chkr = SpellChecker("en_US", text)
-
-    chk_dlg.setSpellChecker(chkr)
     chk_dlg.updateUI()
     gtk.main()
 
 
 if __name__ == "__main__":
     _test()
```

### Comparing `pyenchant-3.2.2/enchant/checker/__init__.py` & `pyenchant-3.3.0rc1/enchant/checker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,106 +32,114 @@
 enchant.checker:  High-level spellchecking functionality
 ========================================================
 
 This package is designed to host higher-level spellchecking functionality
 than is available in the base enchant package.  It should make writing
 applications that follow common usage idioms significantly easier.
 
-The most useful class is SpellChecker, which implements a spellchecking
+The most useful class is :py:class:`SpellChecker`, which implements a spellchecking
 loop over a block of text.  It is capable of modifying the text in-place
 if given an array of characters to work with.
 
 This package also contains several interfaces to the SpellChecker class,
 such as a wxPython GUI dialog and a command-line interface.
 
 """
 
 import array
 import warnings
+from typing import List, Optional, Type, Union
 
 import enchant
+from enchant import Dict
+from enchant.errors import *  # noqa F401,F403
 from enchant.errors import (
     DefaultLanguageNotFoundError,
     DictNotFoundError,
     TokenizerNotFoundError,
 )
-from enchant.tokenize import get_tokenizer
+from enchant.tokenize import Chunker, Filter, get_tokenizer, tokenize
 from enchant.utils import get_default_language
 
 
 class SpellChecker:
     """Class implementing stateful spellchecking behaviour.
 
     This class is designed to implement a spell-checking loop over
     a block of text, correcting/ignoring/replacing words as required.
     This loop is implemented using an iterator paradigm so it can be
     embedded inside other loops of control.
 
-    The SpellChecker object is stateful, and the appropriate methods
+    The `SpellChecker` object is stateful, and the appropriate methods
     must be called to alter its state and affect the progress of
     the spell checking session.  At any point during the checking
-    session, the attribute 'word' will hold the current erroneously
+    session, the attribute :py:attr:`word` will hold the current erroneously
     spelled word under consideration.  The action to take on this word
-    is determined by calling methods such as 'replace', 'replace_always'
-    and 'ignore_always'.  Once this is done, calling 'next' advances
+    is determined by calling methods such as :py:meth:`replace`, :py:meth:`replace_always`
+    and :py:meth:`ignore_always`.  Once this is done, calling :py:meth:`next` advances
     to the next misspelled word.
 
     As a quick (and rather silly) example, the following code replaces
     each misspelled word with the string "SPAM":
 
         >>> text = "This is sme text with a fw speling errors in it."
         >>> chkr = SpellChecker("en_US",text)
         >>> for err in chkr:
         ...   err.replace("SPAM")
         ...
         >>> chkr.get_text()
         'This is SPAM text with a SPAM SPAM errors in it.'
         >>>
 
-    Internally, the SpellChecker always works with arrays of (possibly
+    Internally, the `SpellChecker` always works with arrays of (possibly
     unicode) character elements.  This allows the in-place modification
     of the string as it is checked, and is the closest thing Python has
     to a mutable string.  The text can be set as any of a normal string,
     unicode string, character array or unicode character array. The
-    'get_text' method will return the modified array object if an
+    :py:meth:`get_text` method will return the modified array object if an
     array is used, or a new string object if a string it used.
 
-    Words input to the SpellChecker may be either plain strings or
+    Words input to the `SpellChecker` may be either plain strings or
     unicode objects.  They will be converted to the same type as the
     text being checked, using python's default encoding/decoding
     settings.
 
     If using an array of characters with this object and the
     array is modified outside of the spellchecking loop, use the
-    'set_offset' method to reposition the internal loop pointer
+    method :py:meth:`set_offset` to reposition the internal loop pointer
     to make sure it doesn't skip any words.
 
     """
 
     _DOC_ERRORS = ["sme", "fw", "speling", "chkr", "chkr", "chkr"]
 
     def __init__(
-        self, lang=None, text=None, tokenize=None, chunkers=None, filters=None
-    ):
-        """Constructor for the SpellChecker class.
+        self,
+        lang: Union[Dict, str] = None,
+        text: Optional[str] = None,
+        tokenize: Union[Type[tokenize], Filter] = None,
+        chunkers: List[Chunker] = None,
+        filters: List[Filter] = None,
+    ) -> None:
+        """Constructor for the `SpellChecker` class.
 
-        SpellChecker objects can be created in two ways, depending on
+        `SpellChecker` objects can be created in two ways, depending on
         the nature of the first argument.  If it is a string, it
         specifies a language tag from which a dictionary is created.
-        Otherwise, it must be an enchant Dict object to be used.
+        Otherwise, it must be an :py:class:`enchant.Dict` object to be used.
 
         Optional keyword arguments are:
 
-            * text:  to set the text to be checked at creation time
-            * tokenize:  a custom tokenization function to use
-            * chunkers:  a list of chunkers to apply during tokenization
-            * filters:  a list of filters to apply during tokenization
+        :param text: to set the text to be checked at creation time
+        :param tokenize: a custom tokenization function to use
+        :param chunkers: a list of chunkers to apply during tokenization
+        :param filters: a list of filters to apply during tokenization
 
-        If <tokenize> is not given and the first argument is a Dict,
-        its 'tag' attribute must be a language tag so that a tokenization
+        If `tokenize` is not given and the first argument is a :py:class:`Dict`,
+        its `tag` attribute must be a language tag so that a tokenization
         function can be created automatically.  If this attribute is missing
         the user's default language will be used.
         """
         if lang is None:
             lang = get_default_language()
         if isinstance(lang, (str, bytes)):
             try:
@@ -168,56 +176,54 @@
         if text is not None:
             self.set_text(text)
 
     def __iter__(self):
         """Each SpellChecker object is its own iterator"""
         return self
 
-    def set_text(self, text):
+    def set_text(self, text: str) -> None:
         """Set the text to be spell-checked.
 
-        This method must be called, or the 'text' argument supplied
-        to the constructor, before calling the 'next()' method.
+        This method must be called, or the `text` argument supplied
+        to the constructor, before calling the method :py:meth:`next()`.
         """
         # Convert to an array object if necessary
         if isinstance(text, (str, bytes)):
             if type(text) is str:
                 self._text = array.array("u", text)
             else:
                 self._text = array.array("c", text)
             self._use_tostring = True
         else:
             self._text = text
             self._use_tostring = False
         self._tokens = self._tokenize(self._text)
 
-    def get_text(self):
+    def get_text(self) -> str:
         """Return the spell-checked text."""
         if self._use_tostring:
             return self._array_to_string(self._text)
         return self._text
 
     def _array_to_string(self, text):
         """Format an internal array as a standard string."""
         if text.typecode == "u":
             return text.tounicode()
         return text.tostring()
 
-    def wants_unicode(self):
+    def wants_unicode(self) -> bool:
         """Check whether the checker wants unicode strings.
 
-        This method will return True if the checker wants unicode strings
-        as input, False if it wants normal strings.  It's important to
+        This method will return `True` if the checker wants unicode strings
+        as input, `False` if it wants normal strings.  It's important to
         provide the correct type of string to the checker.
         """
-        if self._text.typecode == "u":
-            return True
-        return False
+        return self._text.typecode == "u"
 
-    def coerce_string(self, text, enc=None):
+    def coerce_string(self, text: str, enc: Optional[str] = None) -> str:
         """Coerce string into the required type.
 
         This method can be used to automatically ensure that strings
         are of the correct type required by this checker - either unicode
         or standard.  If there is a mismatch, conversion is done using
         python's default encoding unless another encoding is specified.
         """
@@ -234,24 +240,24 @@
             else:
                 return text.encode(enc)
         return text
 
     def __next__(self):
         return self.next()
 
-    def next(self):
+    def next(self) -> "SpellChecker":
         """Process text up to the next spelling error.
 
         This method is designed to support the iterator protocol.
-        Each time it is called, it will advance the 'word' attribute
+        Each time it is called, it will advance the :py:attr:`word` attribute
         to the next spelling error in the text.  When no more errors
-        are found, it will raise StopIteration.
+        are found, it will raise :py:exc:`StopIteration`.
 
-        The method will always return self, so that it can be used
-        sensibly in common idioms such as:
+        The method will always return `self`, so that it can be used
+        sensibly in common idioms such as::
 
             for err in checker:
                 err.do_something()
 
         """
         # Find the next spelling error.
         # The uncaught StopIteration from next(self._tokens)
@@ -268,25 +274,25 @@
             self.wordpos = pos
             if word in self._replace_words:
                 self.replace(self._replace_words[word])
                 continue
             break
         return self
 
-    def replace(self, repl):
+    def replace(self, repl: str) -> None:
         """Replace the current erroneous word with the given string."""
         repl = self.coerce_string(repl)
         a_repl = array.array(self._text.typecode, repl)
         if repl:
             self.dict.store_replacement(self.word, repl)
         self._text[self.wordpos : self.wordpos + len(self.word)] = a_repl
         incr = len(repl) - len(self.word)
         self._tokens.set_offset(self._tokens.offset + incr, replaced=True)
 
-    def replace_always(self, word, repl=None):
+    def replace_always(self, word: str, repl: Optional[str] = None) -> None:
         """Always replace given word with given replacement.
 
         If a single argument is given, this is used to replace the
         current erroneous word.  If two arguments are given, that
         combination is added to the list for future use.
         """
         if repl is None:
@@ -294,99 +300,99 @@
             word = self.word
         repl = self.coerce_string(repl)
         word = self.coerce_string(word)
         self._replace_words[word] = repl
         if self.word == word:
             self.replace(repl)
 
-    def ignore_always(self, word=None):
+    def ignore_always(self, word: Optional[str] = None) -> None:
         """Add given word to list of words to ignore.
 
         If no word is given, the current erroneous word is added.
         """
         if word is None:
             word = self.word
         word = self.coerce_string(word)
         if word not in self._ignore_words:
             self._ignore_words[word] = True
 
-    def add_to_personal(self, word=None):
+    def add_to_personal(self, word: Optional[str] = None) -> None:
         """Add given word to the personal word list.
 
         If no word is given, the current erroneous word is added.
         """
         warnings.warn(
             "SpellChecker.add_to_personal is deprecated, "
             "please use SpellChecker.add",
             category=DeprecationWarning,
             stacklevel=2,
         )
         self.add(word)
 
-    def add(self, word=None):
+    def add(self, word: Optional[str] = None) -> None:
         """Add given word to the personal word list.
 
         If no word is given, the current erroneous word is added.
         """
         if word is None:
             word = self.word
         self.dict.add(word)
 
-    def suggest(self, word=None):
+    def suggest(self, word: Optional[str] = None) -> List[str]:
         """Return suggested spellings for the given word.
 
         If no word is given, the current erroneous word is used.
         """
         if word is None:
             word = self.word
         suggs = self.dict.suggest(word)
         return suggs
 
-    def check(self, word):
+    def check(self, word: str) -> bool:
         """Check correctness of the given word."""
         return self.dict.check(word)
 
-    def set_offset(self, off, whence=0):
+    def set_offset(self, off: int, whence: int = 0) -> None:
         """Set the offset of the tokenization routine.
 
         For more details on the purpose of the tokenization offset,
-        see the documentation of the 'enchant.tokenize' module.
-        The optional argument whence indicates the method by
+        see the documentation of the module :py:mod:`enchant.tokenize`.
+        The optional argument `whence` indicates the method by
         which to change the offset:
 
-            * 0 (the default) treats <off> as an increment
-            * 1 treats <off> as a distance from the start
-            * 2 treats <off> as a distance from the end
+            * 0 (the default) treats `off` as an increment
+            * 1 treats `off` as a distance from the start
+            * 2 treats `off` as a distance from the end
         """
         if whence == 0:
             self._tokens.set_offset(self._tokens.offset + off)
         elif whence == 1:
             assert off > 0
             self._tokens.set_offset(off)
         elif whence == 2:
             assert off > 0
             self._tokens.set_offset(len(self._text) - 1 - off)
         else:
             raise ValueError("Invalid value for whence: %s" % (whence,))
 
-    def leading_context(self, chars):
-        """Get <chars> characters of leading context.
+    def leading_context(self, chars: int) -> str:
+        """Get `chars` characters of leading context.
 
-        This method returns up to <chars> characters of leading
+        This method returns up to `chars` characters of leading
         context - the text that occurs in the string immediately
         before the current erroneous word.
         """
         start = max(self.wordpos - chars, 0)
         context = self._text[start : self.wordpos]
         return self._array_to_string(context)
 
-    def trailing_context(self, chars):
-        """Get <chars> characters of trailing context.
+    def trailing_context(self, chars: int) -> str:
+        """Get `chars` characters of trailing context.
 
-        This method returns up to <chars> characters of trailing
+        This method returns up to `chars` characters of trailing
         context - the text that occurs in the string immediately
         after the current erroneous word.
         """
         start = self.wordpos + len(self.word)
         end = min(start + chars, len(self._text))
         context = self._text[start:end]
         return self._array_to_string(context)
```

### Comparing `pyenchant-3.2.2/enchant/checker/wxSpellCheckerDialog.py` & `pyenchant-3.3.0rc1/enchant/checker/wxSpellCheckerDialog.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,105 +29,105 @@
 #
 # Major code cleanup and re-write thanks to Phil Mayes, 2007
 #
 """
 
     enchant.checker.wxSpellCheckerDialog: wxPython spellchecker interface
 
-    This module provides the class wxSpellCheckerDialog, which provides
+    This module provides the class :py:class:`wxSpellCheckerDialog`, which provides
     a wxPython dialog that can be used as an interface to a spell checking
     session.  Currently it is intended as a proof-of-concept and demonstration
     class, but it should be suitable for general-purpose use in a program.
 
-    The class must be given an enchant.checker.SpellChecker object with
+    The class must be given an :py:class:`enchant.checker.SpellChecker` object with
     which to operate.  It can (in theory...) be used in modal and non-modal
-    modes.  Use Show() when operating on an array of characters as it will
+    modes.  Use `Show()` when operating on an array of characters as it will
     modify the array in place, meaning other work can be done at the same
-    time.  Use ShowModal() when operating on a static string.
+    time.  Use `ShowModal()` when operating on a static string.
 
 """
 _DOC_ERRORS = ["ShowModal"]
 
+from typing import Any, Optional
+
 import wx
 
+from enchant.checker import SpellChecker
+
 
 class wxSpellCheckerDialog(wx.Dialog):
     """Simple spellcheck dialog for wxPython
 
     This class implements a simple spellcheck interface for wxPython,
     in the form of a dialog.  It's intended mainly of an example of
     how to do this, although it should be useful for applications that
     just need a simple graphical spellchecker.
 
-    To use, a SpellChecker instance must be created and passed to the
+    To use, a :py:class:`SpellChecker` instance must be created and passed to the
     dialog before it is shown:
 
-        >>> dlg = wxSpellCheckerDialog(None,-1,"")
         >>> chkr = SpellChecker("en_AU",text)
-        >>> dlg.SetSpellChecker(chkr)
+        >>> dlg = wxSpellCheckerDialog(chkr,None,-1,"")
         >>> dlg.Show()
 
     This is most useful when the text to be checked is in the form of
     a character array, as it will be modified in place as the user
     interacts with the dialog.  For checking strings, the final result
-    will need to be obtained from the SpellChecker object:
+    will need to be obtained from the `SpellChecker` object:
 
-        >>> dlg = wxSpellCheckerDialog(None,-1,"")
         >>> chkr = SpellChecker("en_AU",text)
-        >>> dlg.SetSpellChecker(chkr)
+        >>> dlg = wxSpellCheckerDialog(chkr,None,-1,"")
         >>> dlg.ShowModal()
-        >>> text = dlg.GetSpellChecker().get_text()
+        >>> text = chkr.get_text()
 
     Currently the checker must deal with strings of the same type as
     returned by wxPython - unicode or normal string depending on the
     underlying system.  This needs to be fixed, somehow...
     """
 
     _DOC_ERRORS = [
         "dlg",
         "chkr",
         "dlg",
-        "SetSpellChecker",
         "chkr",
         "dlg",
         "dlg",
         "chkr",
         "dlg",
-        "SetSpellChecker",
         "chkr",
         "dlg",
         "ShowModal",
         "dlg",
-        "GetSpellChecker",
     ]
 
     # Remember dialog size across invocations by storing it on the class
     sz = (300, 70)
 
-    def __init__(self, parent=None, id=-1, title="Checking Spelling..."):
-        super().__init__(
-            parent,
-            id,
-            title,
-            size=wxSpellCheckerDialog.sz,
-            style=wx.DEFAULT_DIALOG_STYLE | wx.RESIZE_BORDER,
-        )
+    def __init__(
+        self,
+        checker: SpellChecker,
+        parent: Optional[Any] = None,
+        id: int = -1,
+        title: str = "Checking Spelling...",
+        size=wxSpellCheckerDialog.sz,
+        style=wx.DEFAULT_DIALOG_STYLE | wx.RESIZE_BORDER,
+    ) -> None:
         self._numContext = 40
-        self._checker = None
+        self._checker = checker
         self._buttonsEnabled = True
         self.error_text = wx.TextCtrl(
             self, -1, "", style=wx.TE_MULTILINE | wx.TE_READONLY | wx.TE_RICH
         )
         self.replace_text = wx.TextCtrl(self, -1, "", style=wx.TE_PROCESS_ENTER)
         self.replace_list = wx.ListBox(self, -1, style=wx.LB_SINGLE)
         self.InitLayout()
         wx.EVT_LISTBOX(self, self.replace_list.GetId(), self.OnReplSelect)
         wx.EVT_LISTBOX_DCLICK(self, self.replace_list.GetId(), self.OnReplace)
 
-    def InitLayout(self):
+    def InitLayout(self) -> None:
         """Lay out controls and add buttons."""
         sizer = wx.BoxSizer(wx.HORIZONTAL)
         txtSizer = wx.BoxSizer(wx.VERTICAL)
         btnSizer = wx.BoxSizer(wx.VERTICAL)
         replaceSizer = wx.BoxSizer(wx.HORIZONTAL)
         txtSizer.Add(
             wx.StaticText(self, -1, "Unrecognised Word:"), 0, wx.LEFT | wx.TOP, 5
@@ -162,25 +162,21 @@
             btn.Bind(wx.EVT_BUTTON, action)
             self.buttons.append(btn)
         sizer.Add(btnSizer, 0, wx.ALL | wx.EXPAND, 5)
         self.SetAutoLayout(True)
         self.SetSizer(sizer)
         sizer.Fit(self)
 
-    def Advance(self):
+    def Advance(self) -> bool:
         """Advance to the next error.
 
         This method advances the SpellChecker to the next error, if
         any.  It then displays the error and some surrounding context,
         and well as listing the suggested replacements.
         """
-        # Disable interaction if no checker
-        if self._checker is None:
-            self.EnableButtons(False)
-            return False
         # Advance to next error, disable if not available
         try:
             self._checker.next()
         except StopIteration:
             self.EnableButtons(False)
             self.error_text.SetValue("")
             self.replace_list.Clear()
@@ -204,101 +200,89 @@
         self.error_text.AppendText(tContext)
         # Display suggestions in the replacements list
         suggs = self._checker.suggest()
         self.replace_list.Set(suggs)
         self.replace_text.SetValue(suggs and suggs[0] or "")
         return True
 
-    def EnableButtons(self, state=True):
+    def EnableButtons(self, state: bool = True) -> None:
         """Enable the checking-related buttons"""
         if state != self._buttonsEnabled:
             for btn in self.buttons[:-1]:
                 btn.Enable(state)
             self._buttonsEnabled = state
 
-    def GetRepl(self):
+    def GetRepl(self) -> str:
         """Get the chosen replacement string."""
         repl = self.replace_text.GetValue()
         return repl
 
-    def OnAdd(self, evt):
+    def OnAdd(self, evt: Any) -> None:
         """Callback for the "add" button."""
         self._checker.add()
         self.Advance()
 
-    def OnDone(self, evt):
+    def OnDone(self, evt: Any) -> None:
         """Callback for the "close" button."""
         wxSpellCheckerDialog.sz = self.error_text.GetSizeTuple()
         if self.IsModal():
             self.EndModal(wx.ID_OK)
         else:
             self.Close()
 
-    def OnIgnore(self, evt):
+    def OnIgnore(self, evt: Any) -> None:
         """Callback for the "ignore" button.
         This simply advances to the next error.
         """
         self.Advance()
 
-    def OnIgnoreAll(self, evt):
+    def OnIgnoreAll(self, evt: Any) -> None:
         """Callback for the "ignore all" button."""
         self._checker.ignore_always()
         self.Advance()
 
-    def OnReplace(self, evt):
+    def OnReplace(self, evt: Any) -> None:
         """Callback for the "replace" button."""
         repl = self.GetRepl()
         if repl:
             self._checker.replace(repl)
         self.Advance()
 
-    def OnReplaceAll(self, evt):
+    def OnReplaceAll(self, evt: Any) -> None:
         """Callback for the "replace all" button."""
         repl = self.GetRepl()
         self._checker.replace_always(repl)
         self.Advance()
 
-    def OnReplSelect(self, evt):
+    def OnReplSelect(self, evt: Any) -> None:
         """Callback when a new replacement option is selected."""
         sel = self.replace_list.GetSelection()
         if sel == -1:
             return
         opt = self.replace_list.GetString(sel)
         self.replace_text.SetValue(opt)
 
-    def GetSpellChecker(self):
-        """Get the spell checker object."""
-        return self._checker
-
-    def SetSpellChecker(self, chkr):
-        """Set the spell checker, advancing to the first error.
-        Return True if error(s) to correct, else False."""
-        self._checker = chkr
-        return self.Advance()
-
 
 def _test():
     class TestDialog(wxSpellCheckerDialog):
         def __init__(self, *args):
             super().__init__(*args)
             wx.EVT_CLOSE(self, self.OnClose)
 
         def OnClose(self, evnt):
-            chkr = dlg.GetSpellChecker()
-            if chkr is not None:
-                print(["AFTER:", chkr.get_text()])
+            print(["AFTER:", dlg._checker.get_text()])
             self.Destroy()
 
     from enchant.checker import SpellChecker
 
     text = "This is sme text with a fw speling errors in it. Here are a fw more to tst it ut."
     print(["BEFORE:", text])
-    app = wx.App(False)
-    dlg = TestDialog()
     chkr = SpellChecker("en_US", text)
-    dlg.SetSpellChecker(chkr)
+
+    app = wx.App(False)
+    dlg = TestDialog(chkr)
     dlg.Show()
     app.MainLoop()
 
 
 if __name__ == "__main__":
     _test()
```

### Comparing `pyenchant-3.2.2/enchant/errors.py` & `pyenchant-3.3.0rc1/enchant/errors.py`

 * *Files identical despite different names*

### Comparing `pyenchant-3.2.2/enchant/pypwl.py` & `pyenchant-3.3.0rc1/enchant/pypwl.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,61 +42,62 @@
 prototype for the C version found in Enchant).
 
 """
 
 
 import os
 import warnings
+from typing import Dict, Iterable, Iterator, List, Optional  # noqa F401
 
 
 class Trie:
     """Class implementing a trie-based dictionary of words.
 
     A Trie is a recursive data structure storing words by their prefix.
     "Fuzzy matching" can be done by allowing a certain number of missteps
     when traversing the Trie.
     """
 
-    def __init__(self, words=()):
+    def __init__(self, words: Iterable[str] = ()) -> None:
         self._eos = False  # whether I am the end of a word
-        self._keys = {}  # letters at this level of the trie
+        self._keys = {}  # type: Dict[str, Trie] # letters at this level of the trie
         for w in words:
             self.insert(w)
 
-    def insert(self, word):
+    def insert(self, word: str) -> None:
         if word == "":
             self._eos = True
         else:
             key = word[0]
             try:
                 subtrie = self[key]
             except KeyError:
                 subtrie = Trie()
                 self[key] = subtrie
             subtrie.insert(word[1:])
 
-    def remove(self, word):
+    def remove(self, word: str) -> None:
         if word == "":
             self._eos = False
         else:
             key = word[0]
             try:
                 subtrie = self[key]
             except KeyError:
                 pass
             else:
                 subtrie.remove(word[1:])
 
-    def search(self, word, nerrs=0):
+    def search(self, word: str, nerrs: int = 0) -> List[str]:
         """Search for the given word, possibly making errors.
 
-        This method searches the trie for the given <word>, making
-        precisely <nerrs> errors.  It returns a list of words found.
+        This method searches the trie for the given `word`, making
+        precisely `nerrs` errors.  It returns a list of words found.
         """
-        res = []
+        res = []  # type: List[str]
         # Terminate if we've run out of errors
         if nerrs < 0:
             return res
         # Precise match at the end of the word
         if nerrs == 0 and word == "":
             if self._eos:
                 res.append("")
@@ -137,70 +138,70 @@
                     if w2 not in res:
                         res.append(w2)
         except (IndexError, KeyError):
             pass
         # All done!
         return res
 
-    search._DOC_ERRORS = ["nerrs"]
+    search._DOC_ERRORS = ["nerrs"]  # type: ignore
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> "Trie":
         return self._keys[key]
 
-    def __setitem__(self, key, val):
+    def __setitem__(self, key: str, val: "Trie") -> None:
         self._keys[key] = val
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         if self._eos:
             yield ""
         for k in self._keys:
             for w2 in self._keys[k]:
                 yield k + w2
 
 
 class PyPWL:
     """Pure-python implementation of Personal Word List dictionary.
     This class emulates the PWL objects provided by PyEnchant, but
     implemented purely in python.
     """
 
-    def __init__(self, pwl=None):
+    def __init__(self, pwl: Optional[str] = None) -> None:
         """PyPWL constructor.
         This method takes as its only argument the name of a file
         containing the personal word list, one word per line.  Entries
         will be read from this file, and new entries will be written to
         it automatically.
 
-        If <pwl> is not specified or None, the list is maintained in
+        If `pwl` is not specified or None, the list is maintained in
         memory only.
         """
         self.provider = None
         self._words = Trie()
         if pwl is not None:
-            self.pwl = os.path.abspath(pwl)
+            self.pwl = os.path.abspath(pwl)  # type: Optional[str]
             self.tag = self.pwl
             pwl_f = open(pwl)
             for ln in pwl_f:
                 word = ln.strip()
                 self.add_to_session(word)
             pwl_f.close()
         else:
             self.pwl = None
             self.tag = "PyPWL"
 
-    def check(self, word):
+    def check(self, word: str) -> bool:
         """Check spelling of a word.
 
         This method takes a word in the dictionary language and returns
-        True if it is correctly spelled, and false otherwise.
+        `True` if it is correctly spelled, and `False` otherwise.
         """
         res = self._words.search(word)
         return bool(res)
 
-    def suggest(self, word):
+    def suggest(self, word: str) -> List[str]:
         """Suggest possible spellings for a word.
 
         This method tries to guess the correct spelling for a given
         word, returning the possibilities in a list.
         """
         limit = 10
         maxdepth = 5
@@ -211,71 +212,71 @@
             depth += 1
             for w in self._words.search(word, depth):
                 if w not in res:
                     res.append(w)
         # Limit number of suggs
         return res[:limit]
 
-    def add(self, word):
+    def add(self, word: str) -> None:
         """Add a word to the user's personal dictionary.
         For a PWL, this means appending it to the file.
         """
         if self.pwl is not None:
             pwl_f = open(self.pwl, "a")
             pwl_f.write("%s\n" % (word.strip(),))
             pwl_f.close()
         self.add_to_session(word)
 
-    def add_to_pwl(self, word):
+    def add_to_pwl(self, word: str) -> None:
         """Add a word to the user's personal dictionary.
         For a PWL, this means appending it to the file.
         """
         warnings.warn(
             "PyPWL.add_to_pwl is deprecated, please use PyPWL.add",
             category=DeprecationWarning,
             stacklevel=2,
         )
         self.add(word)
 
-    def remove(self, word):
+    def remove(self, word: str) -> None:
         """Add a word to the user's personal exclude list."""
         # There's no exclude list for a stand-alone PWL.
         # Just remove it from the list.
         self._words.remove(word)
         if self.pwl is not None:
             pwl_f = open(self.pwl, "wt")
             for w in self._words:
                 pwl_f.write("%s\n" % (w.strip(),))
             pwl_f.close()
 
-    def add_to_session(self, word):
+    def add_to_session(self, word: str) -> None:
         """Add a word to the session list."""
         self._words.insert(word)
 
-    def store_replacement(self, mis, cor):
+    def store_replacement(self, mis: str, cor: str) -> None:
         """Store a replacement spelling for a miss-spelled word.
 
         This method makes a suggestion to the spellchecking engine that the
-        miss-spelled word <mis> is in fact correctly spelled as <cor>.  Such
-        a suggestion will typically mean that <cor> appears early in the
-        list of suggested spellings offered for later instances of <mis>.
+        miss-spelled word `mis` is in fact correctly spelled as `cor`.  Such
+        a suggestion will typically mean that `cor` appears early in the
+        list of suggested spellings offered for later instances of `mis`.
         """
         # Too much work for this simple spellchecker
         pass
 
-    store_replacement._DOC_ERRORS = ["mis", "mis"]
+    store_replacement._DOC_ERRORS = ["mis", "mis"]  # type: ignore
 
-    def is_added(self, word):
+    def is_added(self, word: str) -> bool:
         """Check whether a word is in the personal word list."""
         return self.check(word)
 
-    def is_removed(self, word):
+    def is_removed(self, word: str) -> bool:
         """Check whether a word is in the personal exclude list."""
         return False
 
     #  No-op methods to support internal use as a Dict() replacement
 
-    def _check_this(self, msg):
+    def _check_this(self, msg: str) -> None:
         pass
 
-    def _free(self):
+    def _free(self) -> None:
         pass
```

### Comparing `pyenchant-3.2.2/enchant/tokenize/__init__.py` & `pyenchant-3.3.0rc1/enchant/tokenize/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,55 +39,55 @@
 
 Each tokenization function accepts a string as its only positional
 argument, and returns an iterator that yields tuples of the following
 form, one for each word found::
 
     (<word>,<pos>)
 
-The meanings of these fields should be clear: <word> is the word
-that was found and <pos> is the position within the text at which
+The meanings of these fields should be clear: `word` is the word
+that was found and `pos` is the position within the text at which
 the word began (zero indexed, of course).  The function will work
 on any string-like object that supports array-slicing; in particular
-character-array objects from the 'array' module may be used.
+character-array objects from the :py:mod:`array` module may be used.
 
-The iterator also provides the attribute 'offset' which gives the current
+The iterator also provides the attribute :py:attr:`~.tokenize.offset` which gives the current
 position of the tokenizer inside the string being split, and the method
-'set_offset' for manually adjusting this position.  This can be used for
+:py:meth:`~tokenize.set_offset` for manually adjusting this position.  This can be used for
 example if the string's contents have changed during the tokenization
 process.
 
 To obtain an appropriate tokenization function for the language
-identified by <tag>, use the function 'get_tokenizer(tag)'::
+identified by `tag`, use the function :py:func:`get_tokenizer`::
 
     tknzr = get_tokenizer("en_US")
     for (word,pos) in tknzr("text to be tokenized goes here")
         do_something(word)
 
 This library is designed to be easily extendible by third-party
 authors.  To register a tokenization function for the language
-<tag>, implement it as the function 'tokenize' within the
-module enchant.tokenize.<tag>.  The 'get_tokenizer' function
+`tag`, implement it as the function `tokenize` within the
+module `enchant.tokenize.<tag>`.  The function :py:func:`get_tokenizer`
 will automatically detect it.  Note that the underscore must be
 used as the tag component separator in this case, in order to
 form a valid python module name. (e.g. "en_US" rather than "en-US")
 
 Currently, a tokenizer has only been implemented for the English
 language.  Based on the author's limited experience, this should
 be at least partially suitable for other languages.
 
-This module also provides various implementations of "Chunkers" and
-"Filters".  These classes are designed to make it easy to work with
+This module also provides various implementations of Chunkers and
+Filters.  These classes are designed to make it easy to work with
 text in a variety of common formats, by detecting and excluding parts
 of the text that don't need to be checked.
 
-A Chunker is a class designed to break a body of text into large chunks
-of checkable content; for example the HTMLChunker class extracts the
+A :py:class:`Chunker` is a class designed to break a body of text into large chunks
+of checkable content; for example the :py:class:`HTMLChunker` class extracts the
 text content from all HTML tags but excludes the tags themselves.
-A Filter is a class designed to skip individual words during the checking
-process; for example the URLFilter class skips over any words that
+A :py:class:`Filter` is a class designed to skip individual words during the checking
+process; for example the :py:class:`URLFilter` class skips over any words that
 have the format of a URL.
 
 For example, to spellcheck an HTML document it is necessary to split the
 text into chunks based on HTML tags, and to filter out common word forms
 such as URLs and WikiWords.  This would look something like the following::
 
     tknzr = get_tokenizer("en_US",(HTMLChunker,),(URLFilter,WikiWordFilter)))
@@ -105,85 +105,92 @@
     "WikiWordFilter",
     "tkns",
     "tknzr",
     "pos",
     "tkns",
 ]
 
+import array
 import re
 import warnings
-import array
+from typing import Callable, Iterable, List, Optional, Tuple, Type, Union, cast
 
 from enchant.errors import TokenizerNotFoundError
 
+Token = Tuple[str, int]
+
 #  For backwards-compatibility.  This will eventually be removed, but how
 #  does one mark a module-level constant as deprecated?
 Error = TokenizerNotFoundError
 
 
 class tokenize:  # noqa: N801
     """Base class for all tokenizer objects.
 
-    Each tokenizer must be an iterator and provide the 'offset'
+    Each tokenizer must be an iterator and provide the :py:attr:`offset`
     attribute as described in the documentation for this module.
 
     While tokenizers are in fact classes, they should be treated
     like functions, and so are named using lower_case rather than
     the CamelCase more traditional of class names.
     """
 
     _DOC_ERRORS = ["CamelCase"]
 
-    def __init__(self, text):
+    def __init__(self, text: str) -> None:
         self._text = text
         self._offset = 0
 
-    def __next__(self):
+    def __next__(self) -> Token:
         return self.next()
 
-    def next(self):
+    def next(self) -> Token:
         raise NotImplementedError()
 
     def __iter__(self):
         return self
 
-    def set_offset(self, offset, replaced=False):
+    def set_offset(self, offset: int, replaced: bool = False) -> None:
         self._offset = offset
 
-    def _get_offset(self):
+    def _get_offset(self) -> int:
         return self._offset
 
-    def _set_offset(self, offset):
+    def _set_offset(self, offset: int) -> None:
         msg = (
-            "changing a tokenizers 'offset' attribute is deprecated;"
-            " use the 'set_offset' method"
+            "changing a tokenizers :py:attr:`offset` attribute is deprecated;"
+            " use the :py:meth:`set_offset` method"
         )
         warnings.warn(msg, category=DeprecationWarning, stacklevel=2)
         self.set_offset(offset)
 
     offset = property(_get_offset, _set_offset)
 
 
-def get_tokenizer(tag=None, chunkers=None, filters=None):
+def get_tokenizer(
+    tag: str = None,
+    chunkers: Iterable[Union[Type["Chunker"], Type["Filter"]]] = None,
+    filters: Iterable[Type["Filter"]] = None,
+) -> tokenize:
     """Locate an appropriate tokenizer by language tag.
 
-    This requires importing the function 'tokenize' from an appropriate
+    This requires importing the function `tokenize` from an appropriate
     module.  Modules tried are named after the language tag, tried in the
     following order:
 
         * the entire tag (e.g. "en_AU.py")
         * the base country code of the tag (e.g. "en.py")
 
-    If the language tag is None, a default tokenizer (actually the English
+    If the language tag is `None`, a default tokenizer (actually the English
     one) is returned.  It's unicode aware and should work OK for most
     latin-derived languages.
 
-    If a suitable function cannot be found, raises TokenizerNotFoundError.
+    If a suitable function cannot be found, raises :py:exc:`~.errors.TokenizerNotFoundError`.
 
-    If given and not None, 'chunkers' and 'filters' must be lists of chunker
+    If given and not `None`, `chunkers` and `filters` must be lists of chunker
     classes and filter classes respectively.  These will be applied to the
     tokenizer during creation.
     """
     if tag is None:
         tag = "en"
     # "filters" used to be the second argument.  Try to catch cases
     # where it is given positionally and issue a DeprecationWarning.
@@ -197,15 +204,15 @@
             else:
                 if chunkers_are_filters:
                     msg = (
                         "passing 'filters' as a non-keyword argument "
                         "to get_tokenizer() is deprecated"
                     )
                     warnings.warn(msg, category=DeprecationWarning, stacklevel=2)
-                    filters = chunkers
+                    filters = cast(List[Type[Filter]], chunkers)
                     chunkers = None
     # Ensure only '_' used as separator
     tag = tag.replace("-", "_")
     # First try the whole tag
     tk_func = _try_tokenizer(tag)
     if tk_func is None:
         # Try just the base
@@ -228,35 +235,35 @@
     if filters is not None:
         for f in filters:
             tokenizer = f(tokenizer)
     tokenizer = wrap_tokenizer(tokenizer, tk_func)
     return tokenizer
 
 
-get_tokenizer._DOC_ERRORS = ["py", "py"]
+get_tokenizer._DOC_ERRORS = ["py", "py"]  # type: ignore
 
 
 class empty_tokenize(tokenize):  # noqa: N801
     """Tokenizer class that yields no elements."""
 
-    _DOC_ERRORS = []
+    _DOC_ERRORS = []  # type: ignore
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__("")
 
     def next(self):
         raise StopIteration()
 
 
 class unit_tokenize(tokenize):  # noqa: N801
     """Tokenizer class that yields the text as a single token."""
 
-    _DOC_ERRORS = []
+    _DOC_ERRORS = []  # type: ignore
 
-    def __init__(self, text):
+    def __init__(self, text: str) -> None:
         super().__init__(text)
         self._done = False
 
     def next(self):
         if self._done:
             raise StopIteration()
         self._done = True
@@ -267,15 +274,15 @@
     """Tokenizer class that performs very basic word-finding.
 
     This tokenizer does the most basic thing that could work - it splits
     text into words based on whitespace boundaries, and removes basic
     punctuation symbols from the start and end of each word.
     """
 
-    _DOC_ERRORS = []
+    _DOC_ERRORS = []  # type: ignore
 
     # Chars to remove from start/end of words
     strip_from_start = '"' + "'`(["
     strip_from_end = '"' + "'`]).!,?;:"
 
     def next(self):
         text = self._text
@@ -299,45 +306,48 @@
                 e_pos -= 1
             # Return if word isn't empty
             if s_pos < e_pos:
                 return (text[s_pos:e_pos], s_pos)
         raise StopIteration()
 
 
-def _try_tokenizer(mod_name):
+def _try_tokenizer(mod_name: str) -> Optional[Callable]:
     """Look for a tokenizer in the named module.
 
     Returns the function if found, None otherwise.
     """
     mod_base = "enchant.tokenize."
     func_name = "tokenize"
     mod_name = mod_base + mod_name
     try:
         mod = __import__(mod_name, globals(), {}, func_name)
         return getattr(mod, func_name)
     except ImportError:
         return None
 
 
-def wrap_tokenizer(tk1, tk2):
+_Filter = Union[Type[tokenize], "Filter"]
+
+
+def wrap_tokenizer(tk1: _Filter, tk2: _Filter) -> "Filter":
     """Wrap one tokenizer inside another.
 
-    This function takes two tokenizer functions 'tk1' and 'tk2',
+    This function takes two tokenizer functions `tk1` and `tk2`,
     and returns a new tokenizer function that passes the output
-    of tk1 through tk2 before yielding it to the calling code.
+    of `tk1` through `tk2` before yielding it to the calling code.
     """
     # This logic is already implemented in the Filter class.
     # We simply use tk2 as the _split() method for a filter
     # around tk1.
     tkw = Filter(tk1)
-    tkw._split = tk2
+    tkw._split = tk2  # type: ignore
     return tkw
 
 
-wrap_tokenizer._DOC_ERRORS = ["tk", "tk", "tk", "tk"]
+wrap_tokenizer._DOC_ERRORS = ["tk", "tk", "tk", "tk"]  # type: ignore
 
 
 class Chunker(tokenize):
     """Base class for text chunking functions.
 
     A chunker is designed to chunk text into large blocks of tokens.  It
     has the same interface as a tokenizer but is for a different purpose.
@@ -345,118 +355,123 @@
 
     pass
 
 
 class Filter:
     """Base class for token filtering functions.
 
-    A filter is designed to wrap a tokenizer (or another filter) and do
+    A filter is designed to wrap a tokenizer (or another :py:class:`Filter`) and do
     two things:
 
       * skip over tokens
       * split tokens into sub-tokens
 
     Subclasses have two basic options for customising their behaviour.  The
-    method _skip(word) may be overridden to return True for words that
-    should be skipped, and false otherwise.  The method _split(word) may
+    method :py:meth:`_skip` may be overridden to return `True` for words that
+    should be skipped, and `False` otherwise.  The method :py:meth:`_split` may
     be overridden as tokenization function that will be applied to further
     tokenize any words that aren't skipped.
     """
 
-    def __init__(self, tokenizer):
+    def __init__(self, tokenizer: _Filter) -> None:
         """Filter class constructor."""
         self._tokenizer = tokenizer
 
     def __call__(self, *args, **kwds):
         tkn = self._tokenizer(*args, **kwds)
         return self._TokenFilter(tkn, self._skip, self._split)
 
-    def _skip(self, word):
+    def _skip(self, word: str) -> bool:
         """Filter method for identifying skippable tokens.
 
-        If this method returns true, the given word will be skipped by
+        If this method returns `True`, the given word will be skipped by
         the filter.  This should be overridden in subclasses to produce the
         desired functionality.  The default behaviour is not to skip any words.
         """
         return False
 
-    def _split(self, word):
+    def _split(self, word: str) -> tokenize:
         """Filter method for sub-tokenization of tokens.
 
         This method must be a tokenization function that will split the
         given word into sub-tokens according to the needs of the filter.
         The default behaviour is not to split any words.
         """
         return unit_tokenize(word)
 
     class _TokenFilter:
         """Private inner class implementing the tokenizer-wrapping logic.
 
         This might seem convoluted, but we're trying to create something
-        akin to a meta-class - when Filter(tknzr) is called it must return
+        akin to a meta-class - when `Filter(tknzr)` is called it must return
         a *callable* that can then be applied to a particular string to
         perform the tokenization.  Since we need to manage a lot of state
         during tokenization, returning a class is the best option.
         """
 
         _DOC_ERRORS = ["tknzr"]
 
-        def __init__(self, tokenizer, skip, split):
+        def __init__(
+            self,
+            tokenizer: _Filter,
+            skip: Callable[[str], bool],
+            split: Callable[[str], tokenize],
+        ) -> None:
             self._skip = skip
             self._split = split
             self._tokenizer = tokenizer
             # for managing state of sub-tokenization
             self._curtok = empty_tokenize()
             self._curword = ""
             self._curpos = 0
 
         def __iter__(self):
             return self
 
         def __next__(self):
             return self.next()
 
-        def next(self):
+        def next(self) -> Token:
             # Try to get the next sub-token from word currently being split.
             # If unavailable, move on to the next word and try again.
             while True:
                 try:
                     (word, pos) = next(self._curtok)
                     return (word, pos + self._curpos)
                 except StopIteration:
                     (word, pos) = next(self._tokenizer)
                     while self._skip(self._to_string(word)):
                         (word, pos) = next(self._tokenizer)
                     self._curword = word
                     self._curpos = pos
                     self._curtok = self._split(word)
 
-        def _to_string(self, word):
+        def _to_string(self, word) -> str:
             if type(word) is array.array:
                 if word.typecode == "u":
                     return word.tounicode()
                 elif word.typecode == "c":
                     return word.tostring()
             return word
 
         # Pass on access to 'offset' to the underlying tokenizer.
-        def _get_offset(self):
+        def _get_offset(self) -> int:
             return self._tokenizer.offset
 
-        def _set_offset(self, offset):
+        def _set_offset(self, offset: int) -> None:
             msg = (
                 "changing a tokenizers 'offset' attribute is deprecated;"
                 " use the 'set_offset' method"
             )
             warnings.warn(msg, category=DeprecationWarning, stacklevel=2)
             self.set_offset(offset)
 
         offset = property(_get_offset, _set_offset)
 
-        def set_offset(self, val, replaced=False):
+        def set_offset(self, val, replaced: bool = False) -> None:
             old_offset = self._tokenizer.offset
             self._tokenizer.set_offset(val, replaced=replaced)
             # If we move forward within the current word, also set on _curtok.
             # Otherwise, throw away _curtok and set to empty iterator.
             keep_curtok = True
             curtok_offset = val - self._curpos
             if old_offset > val:
@@ -483,15 +498,15 @@
            ^[a-zA-Z]+:\/\/[^\s].*
 
     That is, any words that are URLs.
     """
     _DOC_ERRORS = ["zA"]
     _pattern = re.compile(r"^[a-zA-Z]+:\/\/[^\s].*")
 
-    def _skip(self, word):
+    def _skip(self, word: str) -> bool:
         if self._pattern.match(word):
             return True
         return False
 
 
 class WikiWordFilter(Filter):
     r"""Filter skipping over WikiWords.
@@ -499,15 +514,15 @@
 
            ^([A-Z]\w+[A-Z]+\w+)
 
     That is, any words that are WikiWords.
     """
     _pattern = re.compile(r"^([A-Z]\w+[A-Z]+\w+)")
 
-    def _skip(self, word):
+    def _skip(self, word: str) -> bool:
         if self._pattern.match(word):
             return True
         return False
 
 
 class EmailFilter(Filter):
     r"""Filter skipping over email addresses.
@@ -515,15 +530,15 @@
 
            ^.+@[^\.].*\.[a-z]{2,}$
 
     That is, any words that resemble email addresses.
     """
     _pattern = re.compile(r"^.+@[^\.].*\.[a-z]{2,}$")
 
-    def _skip(self, word):
+    def _skip(self, word: str) -> bool:
         if self._pattern.match(word):
             return True
         return False
 
 
 class MentionFilter(Filter):
     r"""Filter skipping over @mention.
@@ -532,15 +547,15 @@
            (\A|\s)@(\w+)
 
     That is, any words that are @mention.
     """
     _DOC_ERRORS = ["zA"]
     _pattern = re.compile(r"(\A|\s)@(\w+)")
 
-    def _skip(self, word):
+    def _skip(self, word: str) -> bool:
         if self._pattern.match(word):
             return True
         return False
 
 
 class HashtagFilter(Filter):
     r"""Filter skipping over #hashtag.
@@ -549,29 +564,29 @@
            (\A|\s)#(\w+)
 
     That is, any words that are #hashtag.
     """
     _DOC_ERRORS = ["zA"]
     _pattern = re.compile(r"(\A|\s)#(\w+)")
 
-    def _skip(self, word):
+    def _skip(self, word: str) -> bool:
         if self._pattern.match(word):
             return True
         return False
 
 
 class HTMLChunker(Chunker):
     """Chunker for breaking up HTML documents into chunks of checkable text.
 
     The operation of this chunker is very simple - anything between a "<"
     and a ">" will be ignored.  Later versions may improve the algorithm
     slightly.
     """
 
-    def next(self):
+    def next(self) -> Token:
         text = self._text
         offset = self.offset
         while True:
             if offset >= len(text):
                 break
             #  Skip to the end of the current tag, if any.
             if text[offset] == "<":
@@ -592,15 +607,15 @@
                 offset += 1
             self._offset = offset
             # Return if chunk isn't empty
             if s_pos < offset:
                 return (text[s_pos:offset], s_pos)
         raise StopIteration()
 
-    def _is_tag(self, text, offset):
+    def _is_tag(self, text: str, offset: int) -> bool:
         if offset + 1 < len(text):
             if text[offset + 1].isalpha():
                 return True
             if text[offset + 1] == "/":
                 return True
         return False
```

### Comparing `pyenchant-3.2.2/enchant/tokenize/en.py` & `pyenchant-3.3.0rc1/enchant/tokenize/en.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,41 +33,45 @@
 
     This module implements a PyEnchant text tokenizer for the English
     language, based on very simple rules.
 
 """
 
 import unicodedata
+from typing import Any, Callable, Container, Union  # noqa F401
 
 import enchant.tokenize
 
+_TextLike = Union[bytes, str, bytearray]
+_BinaryLike = Union[bytes, bytearray]
+
 
 class tokenize(enchant.tokenize.tokenize):  # noqa: N801
     """Iterator splitting text into words, reporting position.
 
     This iterator takes a text string as input, and yields tuples
     representing each distinct word found in the text.  The tuples
     take the form:
 
         (<word>,<pos>)
 
-    Where <word> is the word string found and <pos> is the position
+    Where `word` is the word string found and `pos` is the position
     of the start of the word within the text.
 
-    The optional argument <valid_chars> may be used to specify a
+    The optional argument `valid_chars` may be used to specify a
     list of additional characters that can form part of a word.
     By default, this list contains only the apostrophe ('). Note that
     these characters cannot appear at the start or end of a word.
     """
 
     _DOC_ERRORS = ["pos", "pos"]
 
-    def __init__(self, text, valid_chars=None):
-        self._valid_chars = valid_chars
-        self._text = text
+    def __init__(self, text: _TextLike, valid_chars: Container[str] = None) -> None:
+        self._valid_chars = valid_chars  # type: Container[str] # type: ignore
+        self._text = text  # type: ignore
         self._offset = 0
         # Select proper implementation of self._consume_alpha.
         # 'text' isn't necessarily a string (it could be e.g. a mutable array)
         # so we can't use isinstance(text, str) to detect unicode.
         # Instead we typetest the first character of the text.
         # If there's no characters then it doesn't matter what implementation
         # we use since it won't be called anyway.
@@ -77,70 +81,70 @@
             self._initialize_for_binary()
         else:
             if isinstance(char1, str):
                 self._initialize_for_unicode()
             else:
                 self._initialize_for_binary()
 
-    def _initialize_for_binary(self):
-        self._consume_alpha = self._consume_alpha_b
+    def _initialize_for_binary(self) -> None:
+        self._consume_alpha = self._consume_alpha_b  # type: Callable[[Any, int], int]
         if self._valid_chars is None:
             self._valid_chars = ("'",)
 
-    def _initialize_for_unicode(self):
+    def _initialize_for_unicode(self) -> None:
         self._consume_alpha = self._consume_alpha_u
         if self._valid_chars is None:
             # XXX TODO: this doesn't seem to work correctly with the
             # MySpell provider, disabling for now.
             # Allow unicode typographic apostrophe
             # self._valid_chars = (u"'",u"\u2019")
             self._valid_chars = ("'",)
 
-    def _consume_alpha_b(self, text, offset):
+    def _consume_alpha_b(self, text: _BinaryLike, offset: int) -> int:
         """Consume an alphabetic character from the given bytestring.
 
         Given a bytestring and the current offset, this method returns
         the number of characters occupied by the next alphabetic character
         in the string.  Non-ASCII bytes are interpreted as utf-8 and can
         result in multiple characters being consumed.
         """
         assert offset < len(text)
-        if text[offset].isalpha():
-            return 1
-        elif text[offset] >= "\x80":
+        if text[offset] >= 0x80:
             return self._consume_alpha_utf8(text, offset)
+        if chr(text[offset]).isalpha():
+            return 1
         return 0
 
-    def _consume_alpha_utf8(self, text, offset):
+    def _consume_alpha_utf8(self, text: _BinaryLike, offset: int) -> int:
         """Consume a sequence of utf8 bytes forming an alphabetic character."""
         incr = 2
         u = ""
         while not u and incr <= 4:
             try:
                 try:
                     #  In the common case this will be a string
                     u = text[offset : offset + incr].decode("utf8")
                 except AttributeError:
                     #  Looks like it was e.g. a mutable char array.
                     try:
-                        s = text[offset : offset + incr].tostring()
+                        s = text[offset : offset + incr].tostring()  # type: ignore
                     except AttributeError:
-                        s = "".join([c for c in text[offset : offset + incr]])
+                        s = bytes(c for c in text[offset : offset + incr])
                     u = s.decode("utf8")
             except UnicodeDecodeError:
                 incr += 1
         if not u:
             return 0
         if u.isalpha():
             return incr
         if unicodedata.category(u)[0] == "M":
             return incr
         return 0
 
-    def _consume_alpha_u(self, text, offset):
+    def _consume_alpha_u(self, text: str, offset: int) -> int:
         """Consume an alphabetic character from the given unicode string.
 
         Given a unicode string and the current offset, this method returns
         the number of characters occupied by the next alphabetic character
         in the string.  Trailing combining characters are consumed as a
         single letter.
         """
@@ -150,15 +154,15 @@
             incr = 1
             while offset + incr < len(text):
                 if unicodedata.category(text[offset + incr])[0] != "M":
                     break
                 incr += 1
         return incr
 
-    def next(self):
+    def next(self) -> enchant.tokenize.Token:
         text = self._text
         offset = self._offset
         while offset < len(text):
             # Find start of next word (must be alpha)
             while offset < len(text):
                 incr = self._consume_alpha(text, offset)
                 if incr:
```

### Comparing `pyenchant-3.2.2/enchant/utils.py` & `pyenchant-3.3.0rc1/enchant/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,72 +38,80 @@
 
     * functions for dealing with locale/language settings
     * ability to list supporting data files (win32 only)
     * functions for bundling supporting data files from a build
 
 """
 
-from enchant.errors import Error
 import locale
+from typing import Callable, Iterable, List, Optional, Sequence  # noqa F401
+
+from enchant.errors import *  # noqa F401,F403
+from enchant.errors import Error
 
 
-def levenshtein(s1, s2):
+def levenshtein(s1: str, s2: str) -> int:
     """Calculate the Levenshtein distance between two strings.
 
-    This is straight from Wikipedia.
+    This is straight from `Wikipedia <https://en.wikipedia.org/wiki/Levenshtein_distance>`_.
     """
     if len(s1) < len(s2):
         return levenshtein(s2, s1)
     if not s1:
         return len(s2)
 
-    previous_row = range(len(s2) + 1)
+    previous_row = range(len(s2) + 1)  # type: Sequence[int]
     for i, c1 in enumerate(s1):
         current_row = [i + 1]
         for j, c2 in enumerate(s2):
             insertions = previous_row[j + 1] + 1
             deletions = current_row[j] + 1
             substitutions = previous_row[j] + (c1 != c2)
             current_row.append(min(insertions, deletions, substitutions))
         previous_row = current_row
 
     return previous_row[-1]
 
 
-def trim_suggestions(word, suggs, maxlen, calcdist=None):
+def trim_suggestions(
+    word: str,
+    suggs: Iterable[str],
+    maxlen: int,
+    calcdist: Callable[[str, str], int] = None,
+) -> List[str]:
     """Trim a list of suggestions to a maximum length.
 
     If the list of suggested words is too long, you can use this function
     to trim it down to a maximum length.  It tries to keep the "best"
     suggestions based on similarity to the original word.
 
-    If the optional "calcdist" argument is provided, it must be a callable
+    If the optional `calcdist` argument is provided, it must be a callable
     taking two words and returning the distance between them.  It will be
     used to determine which words to retain in the list.  The default is
     a simple Levenshtein distance.
     """
     if calcdist is None:
         calcdist = levenshtein
     decorated = [(calcdist(word, s), s) for s in suggs]
     decorated.sort()
     return [s for (l, s) in decorated[:maxlen]]
 
 
-def get_default_language(default=None):
+def get_default_language(default: Optional[str] = None) -> Optional[str]:
     """Determine the user's default language, if possible.
 
-    This function uses the 'locale' module to try to determine
+    This function uses the :py:mod:`locale` module to try to determine
     the user's preferred language.  The return value is as
     follows:
 
-        * if a locale is available for the LC_MESSAGES category,
+        * if a locale is available for the `LC_MESSAGES` category,
           that language is used
         * if a default locale is available, that language is used
-        * if the keyword argument <default> is given, it is used
-        * if nothing else works, None is returned
+        * if the keyword argument `default` is given, it is used
+        * if nothing else works, `None` is returned
 
     Note that determining the user's language is in general only
     possible if they have set the necessary environment variables
     on their system.
     """
     try:
         tag = locale.getlocale()[0]
@@ -113,8 +121,8 @@
                 raise Error("No default language available")
         return tag
     except Exception:
         pass
     return default
 
 
-get_default_language._DOC_ERRORS = ["LC"]
+get_default_language._DOC_ERRORS = ["LC"]  # type: ignore
```

### Comparing `pyenchant-3.2.2/pyenchant.egg-info/PKG-INFO` & `pyenchant-3.3.0rc1/pyenchant.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,104 +1,107 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pyenchant
-Version: 3.2.2
+Version: 3.3.0rc1
 Summary: Python bindings for the Enchant spellchecking system
 Home-page: https://pyenchant.github.io/pyenchant/
 Author: Dimitri Merejkowsky
 Author-email: d.merej@gmail.com
 License: LGPL
-Description: pyenchant:  Python bindings for the Enchant spellchecker
-        ========================================================
-        
-        .. image:: https://img.shields.io/pypi/v/pyenchant.svg
-            :target: https://pypi.org/project/pyenchant
-        
-        .. image:: https://img.shields.io/pypi/pyversions/pyenchant.svg
-            :target: https://pypi.org/project/pyenchant
-        
-        .. image:: https://github.com/pyenchant/pyenchant/workflows/tests/badge.svg
-            :target: https://github.com/pyenchant/pyenchant/actions
-        
-        .. image:: https://builds.sr.ht/~dmerej/pyenchant.svg
-            :target: https://builds.sr.ht/~dmerej/pyenchant
-        
-        .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/psf/black
-        
-        This package provides a set of Python language bindings for the Enchant
-        spellchecking library.  For more information, visit the project website:
-        
-            http://pyenchant.github.io/pyenchant/
-        
-        What is Enchant?
-        ----------------
-        
-        Enchant is used to check the spelling of words and suggest corrections
-        for words that are miss-spelled.  It can use many popular spellchecking
-        packages to perform this task, including ispell, aspell and MySpell.  It
-        is quite flexible at handling multiple dictionaries and multiple
-        languages.
-        
-        More information is available on the Enchant website:
-        
-            https://abiword.github.io/enchant/
-        
-        
-        How do I use it?
-        ----------------
-        
-        For Windows users, install the pre-built binary packages using
-        pip::
-        
-            pip install pyenchant
-        
-        
-        These packages bundle a pre-built copy of the underlying enchant library.
-        Users on other platforms will need to install "enchant" using their system
-        package manager (brew on macOS).
-        
-        Once the software is installed, python's on-line help facilities can
-        get you started.  Launch python and issue the following commands:
-        
-            >>> import enchant
-            >>> help(enchant)
-        
-        
-        
-        Who is responsible for all this?
-        --------------------------------
-        
-        The credit for Enchant itself goes to Dom Lachowicz.  Find out more details
-        on the Enchant website listed above.  Full marks to Dom for producing such
-        a high-quality library.
-        
-        The glue to pull Enchant into Python via ctypes was written by Ryan Kelly.
-        He needed a decent spellchecker for another project he was working on, and
-        all the solutions turned up by Google were either extremely non-portable
-        (e.g. opening a pipe to ispell) or had completely disappeared from the web
-        (what happened to SnakeSpell?)  It was also a great excuse to teach himself
-        about SWIG, ctypes, and even a little bit of the Python/C API.
-        
-        Finally, after Ryan stepped down from the project, Dimitri Merejkowsky
-        became the new maintainer.
-        
-        
+Project-URL: Changelog, https://pyenchant.github.io/pyenchant/changelog.html
+Project-URL: Source, https://github.com/pyenchant/pyenchant
+Project-URL: Tracker, https://github.com/pyenchant/pyenchant/issues
 Keywords: spelling spellcheck enchant
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3.5
+Requires-Python: >=3.7
+License-File: LICENSE.txt
+
+pyenchant:  Python bindings for the Enchant spellchecker
+========================================================
+
+.. image:: https://img.shields.io/pypi/v/pyenchant.svg
+    :target: https://pypi.org/project/pyenchant
+
+.. image:: https://img.shields.io/pypi/pyversions/pyenchant.svg
+    :target: https://pypi.org/project/pyenchant
+
+.. image:: https://github.com/pyenchant/pyenchant/workflows/tests/badge.svg
+    :target: https://github.com/pyenchant/pyenchant/actions
+
+.. image:: https://builds.sr.ht/~dmerej/pyenchant.svg
+    :target: https://builds.sr.ht/~dmerej/pyenchant
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+This package provides a set of Python language bindings for the Enchant
+spellchecking library.  For more information, visit the project website:
+
+    http://pyenchant.github.io/pyenchant/
+
+What is Enchant?
+----------------
+
+Enchant is used to check the spelling of words and suggest corrections
+for words that are miss-spelled.  It can use many popular spellchecking
+packages to perform this task, including ispell, aspell and MySpell.  It
+is quite flexible at handling multiple dictionaries and multiple
+languages.
+
+More information is available on the Enchant website:
+
+    https://abiword.github.io/enchant/
+
+
+How do I use it?
+----------------
+
+For Windows users, install the pre-built binary packages using
+pip::
+
+    pip install pyenchant
+
+
+These packages bundle a pre-built copy of the underlying enchant library.
+Users on other platforms will need to install "enchant" using their system
+package manager (brew on macOS).
+
+Once the software is installed, python's on-line help facilities can
+get you started.  Launch python and issue the following commands:
+
+    >>> import enchant
+    >>> help(enchant)
+
+
+
+Who is responsible for all this?
+--------------------------------
+
+The credit for Enchant itself goes to Dom Lachowicz.  Find out more details
+on the Enchant website listed above.  Full marks to Dom for producing such
+a high-quality library.
+
+The glue to pull Enchant into Python via ctypes was written by Ryan Kelly.
+He needed a decent spellchecker for another project he was working on, and
+all the solutions turned up by Google were either extremely non-portable
+(e.g. opening a pipe to ispell) or had completely disappeared from the web
+(what happened to SnakeSpell?)  It was also a great excuse to teach himself
+about SWIG, ctypes, and even a little bit of the Python/C API.
+
+Finally, after Ryan stepped down from the project, Dimitri Merejkowsky
+became the new maintainer.
+
```

