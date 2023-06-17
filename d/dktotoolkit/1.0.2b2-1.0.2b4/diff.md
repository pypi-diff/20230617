# Comparing `tmp/dktotoolkit-1.0.2b2.tar.gz` & `tmp/dktotoolkit-1.0.2b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dktotoolkit-1.0.2b2.tar", last modified: Sun Jun 11 10:18:53 2023, max compression
+gzip compressed data, was "dktotoolkit-1.0.2b4.tar", last modified: Sat Jun 17 01:34:55 2023, max compression
```

## Comparing `dktotoolkit-1.0.2b2.tar` & `dktotoolkit-1.0.2b4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 10:18:53.117102 dktotoolkit-1.0.2b2/
--rw-rw-rw-   0 root         (0) root         (0)    34483 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4657 2023-06-11 10:18:53.117102 dktotoolkit-1.0.2b2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3813 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 10:18:53.113102 dktotoolkit-1.0.2b2/dktotoolkit/
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     7002 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/datestr.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/dict.py
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/envvar.py
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2430 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/function_recursive.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     2821 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 10:18:53.117102 dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/
--rw-rw-rw-   0 root         (0) root         (0)     3360 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_html_to_markdown.py
--rw-rw-rw-   0 root         (0) root         (0)     1334 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_html_to_utf8.py
--rw-rw-rw-   0 root         (0) root         (0)      998 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_remove_duplicates.py
--rw-rw-rw-   0 root         (0) root         (0)     4828 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_simplify_html.py
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_utf8_to_html.py
--rw-rw-rw-   0 root         (0) root         (0)     1264 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/dktotoolkit/str.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 10:18:53.113102 dktotoolkit-1.0.2b2/dktotoolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4657 2023-06-11 10:18:53.000000 dktotoolkit-1.0.2b2/dktotoolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      733 2023-06-11 10:18:53.000000 dktotoolkit-1.0.2b2/dktotoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 10:18:53.000000 dktotoolkit-1.0.2b2/dktotoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-11 10:18:53.000000 dktotoolkit-1.0.2b2/dktotoolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-11 10:18:53.000000 dktotoolkit-1.0.2b2/dktotoolkit.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-11 10:18:53.117102 dktotoolkit-1.0.2b2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-06-11 10:18:18.000000 dktotoolkit-1.0.2b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 01:34:55.329532 dktotoolkit-1.0.2b4/
+-rw-rw-rw-   0 root         (0) root         (0)    34483 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4738 2023-06-17 01:34:55.329532 dktotoolkit-1.0.2b4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3894 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 01:34:55.329532 dktotoolkit-1.0.2b4/dktotoolkit/
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8598 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/datestr.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/envvar.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/function_recursive.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 01:34:55.329532 dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/
+-rw-rw-rw-   0 root         (0) root         (0)     3470 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_html_to_markdown.py
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_html_to_utf8.py
+-rw-rw-rw-   0 root         (0) root         (0)      998 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_remove_duplicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4828 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_simplify_html.py
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_utf8_to_html.py
+-rw-rw-rw-   0 root         (0) root         (0)      863 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/sqlite3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1264 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/dktotoolkit/str.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 01:34:55.329532 dktotoolkit-1.0.2b4/dktotoolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4738 2023-06-17 01:34:55.000000 dktotoolkit-1.0.2b4/dktotoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      756 2023-06-17 01:34:55.000000 dktotoolkit-1.0.2b4/dktotoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 01:34:55.000000 dktotoolkit-1.0.2b4/dktotoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-17 01:34:55.000000 dktotoolkit-1.0.2b4/dktotoolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-17 01:34:55.000000 dktotoolkit-1.0.2b4/dktotoolkit.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-17 01:34:55.329532 dktotoolkit-1.0.2b4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-06-17 01:34:21.000000 dktotoolkit-1.0.2b4/setup.py
```

### Comparing `dktotoolkit-1.0.2b2/LICENSE` & `dktotoolkit-1.0.2b4/LICENSE`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/PKG-INFO` & `dktotoolkit-1.0.2b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dktotoolkit
-Version: 1.0.2b2
+Version: 1.0.2b4
 Summary: A little toolkit with fancy functions
 Home-page: https://discord-catho.frama.io/module_toolkit
 Author: Pierre
 Author-email: pierre@exemple.com
 License: AGPL 3
 Keywords: dotenv,.env,toolkit,parse dates
 Classifier: Development Status :: 3 - Alpha
@@ -128,11 +128,11 @@
 
 ```
 
 # TODO
 * [ ] submodule git pour CI et setup
 * [ ] Add substitution inside .. literalinclude:: ../../dktotoolkit/__version__.py (setup.rst)
 * [ ] Improve tests for parserhtml
-
+* [ ] load dotenv : if path : check if exists, add argument : raise if not exists
 
 # Licence
 GNU AGPL 3 (cf LICENCE.md)
```

### Comparing `dktotoolkit-1.0.2b2/README.md` & `dktotoolkit-1.0.2b4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -103,11 +103,11 @@
 
 ```
 
 # TODO
 * [ ] submodule git pour CI et setup
 * [ ] Add substitution inside .. literalinclude:: ../../dktotoolkit/__version__.py (setup.rst)
 * [ ] Improve tests for parserhtml
-
+* [ ] load dotenv : if path : check if exists, add argument : raise if not exists
 
 # Licence
 GNU AGPL 3 (cf LICENCE.md)
```

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/__init__.py` & `dktotoolkit-1.0.2b4/dktotoolkit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,22 +23,24 @@
 from .str import str2digit
 from .datestr import parser_date, date2str
 from .envvar import load_dotenv, getEnvironVar, getTimesReminder
 from .exceptions import ParseError
 from .functions import compatMode
 from .function_recursive import recurs_function
 from .parserhtml import ParserHTML
+from .sqlite3 import recursive_sql
 
 # Declaration explicite de tous les modules (pep8)
 __all__ = [
     'ParseError',
     '__author__', '__author_email__',
     '__copyright__', '__description__', '__license__',
     '__title__', '__version__', '__pkg_name__',
     'dict2obj',
     'replace_with_mask', "castList",
     'str2digit',
     'parser_date', 'date2str',
     'load_dotenv', 'getEnvironVar', 'getTimesReminder',
     'compatMode', 'recurs_function',
-    'ParserHTML'
+    'ParserHTML',
+    "recursive_sql"
 ]
```

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/datestr.py` & `dktotoolkit-1.0.2b4/dktotoolkit/datestr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,66 @@
 import sys
 import re
-from datetime import date, timedelta
+from datetime import date, timedelta, datetime
 import traceback
 
 from .exceptions import ParseError
 
+def is_valid_date(date_str:str, date_format:str="yyyy-mm-dd", check_sep:bool=True):
+    """Verifier qu'une date est au bon format
+:param str date_str: Date a verifier
+:param str date_format: Format de la date (default: yyyy-mm-dd)
+:param bool check_sep: Reconnaissance du separateur egalement, ou non
+
+:return: Vrai si la date est dans le bon format, Faux sinon
+:rtypes: bool
+"""
+
+    # Vérification de la longueur de la date et du format
+    if len(date_str) != len(date_format):
+        return False
+
+    # Vérification des séparateurs si nécessaire
+    if check_sep:
+        for i, char in enumerate(date_format):
+            if char not in ("y", "m", "d") and date_str[i] != char:
+                return False
+
+    # Définition des correspondances entre les symboles du format et les parties de la date
+    symbols = {"y": "year", "m": "month", "d": "day"}
+    date_format = date_format.lower()
+
+    if "yyyy" in date_format:
+        year_digits = 4
+    elif "yy" in date_format:
+        year_digits = 2
+    else:
+        raise ValueError(f'date_format : {date_format} must have yy or yyyy')
+    #
+
+    # Extraction des parties de la date en fonction du format
+    parts = {"year":"", "month":"", "day":""}
+
+    for i, char in enumerate(date_format):
+        if char in symbols:
+            part = symbols[char]
+            parts[part] += date_str[i]
+        #
+    #
+    parts = {k:int(v) for k, v in parts.items()}
+
+    # Vérification des chiffres dans les parties de la date
+    try:
+        datetime(**parts)
+    except ValueError:
+        return False
+
+    return True
+
+#
 
 def _parse_month(month_in):
     """Convert month to the month number
 
 :param str month_in: The month to parse
 :return: The month number
 :rtypes: str "01"-"12" for months between january-december
```

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/dict.py` & `dktotoolkit-1.0.2b4/dktotoolkit/dict.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/envvar.py` & `dktotoolkit-1.0.2b4/dktotoolkit/envvar.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/function_recursive.py` & `dktotoolkit-1.0.2b4/dktotoolkit/function_recursive.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/functions.py` & `dktotoolkit-1.0.2b4/dktotoolkit/functions.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/list.py` & `dktotoolkit-1.0.2b4/dktotoolkit/list.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/__init__.py` & `dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,21 @@
     #endDef
 
     from ._html_to_utf8 import html_to_utf8
     from ._utf8_to_html import utf8_to_html
     from ._html_to_markdown import html_to_markdown
     from ._simplify_html import simplify_html
 
+    def get_data(self):
+        """
+        Retourner les donnees
+        """
+        return self.data
+    #
+
     # Static methods
     @staticmethod
     def removeDuplicates(content, tag="br"):
         """
         Supprime les balises en double dans le contenu HTML.
 
         :param content: Le contenu HTML à traiter.
```

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_html_to_markdown.py` & `dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_html_to_markdown.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_html_to_utf8.py` & `dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_html_to_utf8.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_remove_duplicates.py` & `dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_simplify_html.py` & `dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_simplify_html.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/parserhtml/_utf8_to_html.py` & `dktotoolkit-1.0.2b4/dktotoolkit/parserhtml/_utf8_to_html.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit/str.py` & `dktotoolkit-1.0.2b4/dktotoolkit/str.py`

 * *Files identical despite different names*

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit.egg-info/PKG-INFO` & `dktotoolkit-1.0.2b4/dktotoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dktotoolkit
-Version: 1.0.2b2
+Version: 1.0.2b4
 Summary: A little toolkit with fancy functions
 Home-page: https://discord-catho.frama.io/module_toolkit
 Author: Pierre
 Author-email: pierre@exemple.com
 License: AGPL 3
 Keywords: dotenv,.env,toolkit,parse dates
 Classifier: Development Status :: 3 - Alpha
@@ -128,11 +128,11 @@
 
 ```
 
 # TODO
 * [ ] submodule git pour CI et setup
 * [ ] Add substitution inside .. literalinclude:: ../../dktotoolkit/__version__.py (setup.rst)
 * [ ] Improve tests for parserhtml
-
+* [ ] load dotenv : if path : check if exists, add argument : raise if not exists
 
 # Licence
 GNU AGPL 3 (cf LICENCE.md)
```

### Comparing `dktotoolkit-1.0.2b2/dktotoolkit.egg-info/SOURCES.txt` & `dktotoolkit-1.0.2b4/dktotoolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 dktotoolkit/datestr.py
 dktotoolkit/dict.py
 dktotoolkit/envvar.py
 dktotoolkit/exceptions.py
 dktotoolkit/function_recursive.py
 dktotoolkit/functions.py
 dktotoolkit/list.py
+dktotoolkit/sqlite3.py
 dktotoolkit/str.py
 dktotoolkit.egg-info/PKG-INFO
 dktotoolkit.egg-info/SOURCES.txt
 dktotoolkit.egg-info/dependency_links.txt
 dktotoolkit.egg-info/requires.txt
 dktotoolkit.egg-info/top_level.txt
 dktotoolkit/parserhtml/__init__.py
```

### Comparing `dktotoolkit-1.0.2b2/setup.py` & `dktotoolkit-1.0.2b4/setup.py`

 * *Files identical despite different names*

