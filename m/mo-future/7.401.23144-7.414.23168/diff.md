# Comparing `tmp/mo_future-7.401.23144-py2.py3-none-any.whl.zip` & `tmp/mo_future-7.414.23168-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10737 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat     4098 b- defN 23-May-24 02:37 mo_future/__init__.py
+Zip file size: 10724 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat     4081 b- defN 23-Jun-17 09:11 mo_future/__init__.py
 -rw-rw-rw-  2.0 fat     4242 b- defN 23-May-24 02:37 mo_future/cache.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1965 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      581 b- defN 23-May-24 02:37 mo_future-7.401.23144.dist-info/RECORD
-7 files, 27731 bytes uncompressed, 9707 bytes compressed:  65.0%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-17 09:11 mo_future-7.414.23168.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1965 b- defN 23-Jun-17 09:11 mo_future-7.414.23168.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-17 09:11 mo_future-7.414.23168.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Jun-17 09:11 mo_future-7.414.23168.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      581 b- defN 23-Jun-17 09:11 mo_future-7.414.23168.dist-info/RECORD
+7 files, 27714 bytes uncompressed, 9694 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: mo_future/__init__.py
 Comment: 
 
 Filename: mo_future/cache.py
 Comment: 
 
-Filename: mo_future-7.401.23144.dist-info/LICENSE
+Filename: mo_future-7.414.23168.dist-info/LICENSE
 Comment: 
 
-Filename: mo_future-7.401.23144.dist-info/METADATA
+Filename: mo_future-7.414.23168.dist-info/METADATA
 Comment: 
 
-Filename: mo_future-7.401.23144.dist-info/WHEEL
+Filename: mo_future-7.414.23168.dist-info/WHEEL
 Comment: 
 
-Filename: mo_future-7.401.23144.dist-info/top_level.txt
+Filename: mo_future-7.414.23168.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_future-7.401.23144.dist-info/RECORD
+Filename: mo_future-7.414.23168.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_future/__init__.py

```diff
@@ -2,17 +2,14 @@
 #
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
-
-
-
 import json
 import sys
 
 from collections import OrderedDict, UserDict
 from collections.abc import Callable, Iterable, Mapping, Set, MutableMapping
 from functools import cmp_to_key, reduce, update_wrapper
 from configparser import ConfigParser
@@ -22,16 +19,14 @@
 from html.parser import HTMLParser
 from urllib.parse import urlparse
 from io import StringIO
 from io import BytesIO
 from _thread import allocate_lock, get_ident, start_new_thread, interrupt_main
 
 
-__all__ = []
-
 PYPY = False
 PY2 = False
 PY3 = True
 try:
     import __pypy__ as _
 
     PYPY = True
```

## Comparing `mo_future-7.401.23144.dist-info/LICENSE` & `mo_future-7.414.23168.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_future-7.401.23144.dist-info/METADATA` & `mo_future-7.414.23168.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-future
-Version: 7.401.23144
+Version: 7.414.23168
 Summary: More future! Make Python 2/3 compatibility a bit easier
 Home-page: https://github.com/klahnakoski/mo-future
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
```

