# Comparing `tmp/pyrepresent-0.0.9.tar.gz` & `tmp/pyrepresent-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.0.9.tar", last modified: Mon May 15 13:44:21 2023, max compression
+gzip compressed data, was "pyrepresent-0.1.0.tar", last modified: Sat Jun 17 15:04:53 2023, max compression
```

## Comparing `pyrepresent-0.0.9.tar` & `pyrepresent-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 13:44:21.429749 pyrepresent-0.0.9/
--rw-rw-rw-   0        0        0      115 2023-05-15 13:44:21.000000 pyrepresent-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     5268 2023-05-15 13:44:21.429749 pyrepresent-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.0.9/README.md
--rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.0.9/build.py
--rw-rw-rw-   0        0        0      715 2023-05-15 13:44:21.000000 pyrepresent-0.0.9/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-15 13:44:21.409592 pyrepresent-0.0.9/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     5268 2023-05-15 13:44:21.000000 pyrepresent-0.0.9/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-05-15 13:44:21.000000 pyrepresent-0.0.9/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 13:44:21.000000 pyrepresent-0.0.9/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-15 13:44:21.000000 pyrepresent-0.0.9/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-15 13:44:21.000000 pyrepresent-0.0.9/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-15 13:44:21.428244 pyrepresent-0.0.9/represent/
--rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.0.9/represent/__init__.py
--rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.0.9/represent/base.py
--rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.0.9/represent/document.py
--rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.0.9/represent/indentation.py
--rw-rw-rw-   0        0        0    11473 2023-05-15 13:43:14.000000 pyrepresent-0.0.9/represent/object.py
--rw-rw-rw-   0        0        0    19724 2023-04-25 10:08:07.000000 pyrepresent-0.0.9/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.0.9/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.0.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 13:44:21.429749 pyrepresent-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-05-15 13:44:09.000000 pyrepresent-0.0.9/setup.py
--rw-rw-rw-   0        0        0      669 2023-03-28 10:53:06.000000 pyrepresent-0.0.9/test.py
+drwxrwxrwx   0        0        0        0 2023-06-17 15:04:53.178463 pyrepresent-0.1.0/
+-rw-rw-rw-   0        0        0      115 2023-06-17 15:04:52.000000 pyrepresent-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5268 2023-06-17 15:04:53.177463 pyrepresent-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.1.0/README.md
+-rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.1.0/build.py
+-rw-rw-rw-   0        0        0      715 2023-06-17 15:04:52.000000 pyrepresent-0.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-17 15:04:53.171461 pyrepresent-0.1.0/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     5268 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-17 15:04:53.000000 pyrepresent-0.1.0/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 15:04:53.176462 pyrepresent-0.1.0/represent/
+-rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.1.0/represent/__init__.py
+-rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.1.0/represent/base.py
+-rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.1.0/represent/document.py
+-rw-rw-rw-   0        0        0     2133 2023-05-15 13:38:04.000000 pyrepresent-0.1.0/represent/indentation.py
+-rw-rw-rw-   0        0        0    17977 2023-06-17 15:03:59.000000 pyrepresent-0.1.0/represent/object.py
+-rw-rw-rw-   0        0        0    20797 2023-06-17 15:02:03.000000 pyrepresent-0.1.0/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-17 15:04:53.178463 pyrepresent-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-17 15:04:48.000000 pyrepresent-0.1.0/setup.py
+-rw-rw-rw-   0        0        0      971 2023-06-13 13:18:42.000000 pyrepresent-0.1.0/test.py
```

### Comparing `pyrepresent-0.0.9/PKG-INFO` & `pyrepresent-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.0.9
+Version: 0.1.0
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.0.9/README.md` & `pyrepresent-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.9/build.py` & `pyrepresent-0.1.0/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.9/pyproject.toml` & `pyrepresent-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.0.9'
+version = '0.1.0'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.0.9/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.1.0/pyrepresent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.0.9
+Version: 0.1.0
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.0.9/represent/base.py` & `pyrepresent-0.1.0/represent/base.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.9/represent/indentation.py` & `pyrepresent-0.1.0/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.9/represent/structures.py` & `pyrepresent-0.1.0/represent/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # structures.py
 
 import datetime as dt
+import types
 from typing import Union, Any, Optional, Callable
 from functools import wraps
 
 from colorama import Fore, Style
 
 import pandas as pd
 import numpy as np
@@ -23,15 +24,16 @@
     "CircularReferenceStructure",
     "TupleStructure",
     "structures",
     "structure_types",
     "colorize",
     "decolorize",
     "TypeStructure",
-    "ObjectStructure"
+    "ObjectStructure",
+    "FunctionStructure"
 ]
 
 Args = Kwargs = Any
 
 class Colors:
     """A class to represent colors."""
 
@@ -93,19 +95,19 @@
         if not color:
             return content
         # end if
 
         name = content
 
         return (
-            name[:name.rfind(".") + 1] +
-            Colors.CYAN +
-            name[name.rfind(".") + 1:len(name) + name.find("(") + 1] +
-            Colors.END +
-            name[len(name) + name.find("(") + 1:]
+                name[:name.rfind(".") + 1] +
+                Colors.CYAN +
+                name[name.rfind(".") + 1:len(name) + name.find("(") + 1] +
+                Colors.END +
+                name[len(name) + name.find("(") + 1:]
         )
     # end color_repr_class
 
     @staticmethod
     def color_repr_class(content: str, color: Optional[bool] = True) -> str:
         """
         Colors the string of the object's repr.
@@ -119,19 +121,19 @@
         if not color:
             return content
         # end if
 
         name = content
 
         return (
-            name[:name.rfind(".") + 1] +
-            Colors.CYAN +
-            name[name.rfind(".") + 1:name.find(" object at")] +
-            Colors.END +
-            name[name.find(" object at"):]
+                name[:name.rfind(".") + 1] +
+                Colors.CYAN +
+                name[name.rfind(".") + 1:name.find(" object at")] +
+                Colors.END +
+                name[name.find(" object at"):]
         )
     # end color_repr_class
 
     @staticmethod
     def color_repr(content: str, value: Any, color: Optional[bool] = True) -> str:
         """
         Colors the string of the object's repr.
@@ -204,14 +206,16 @@
 
         try:
             color = {
                 str: Colors.YELLOW,
                 int: Colors.MAGENTA,
                 float: Colors.MAGENTA,
                 dt.timedelta: Colors.MAGENTA,
+                dt.datetime: Colors.MAGENTA,
+                dt.date: Colors.MAGENTA,
                 bool: Colors.CYAN,
                 type(None): Colors.CYAN
             }[type(value)]
 
             if type(value) == str:
                 chars = ["/", "\\", r"\t", r"\n"]
                 content = "".join(
@@ -231,15 +235,15 @@
                     content = content.replace(
                         char, f"{Colors.MAGENTA}{char}{Colors.END}"
                     )
                 # end for
 
                 return content
 
-            elif type(value) == dt.timedelta:
+            elif type(value) in (dt.datetime, dt.timedelta, dt.date):
                 content = "".join(
                     f"{color}{char}{Colors.END}"
                     if char != ":"
                     else char for char in content
                 )
                 content = content.replace(
                     ":", f"{Colors.RED}:{Colors.END}"
@@ -330,15 +334,21 @@
         :param args: Any positional arguments.
         :param kwargs: Any keyword arguments
 
         :returns: The model object.
         """
 
         try:
-            return constructor(*args, **kwargs).replace("END$$(", Colors.END)
+            return (
+                constructor(*args, **kwargs).
+                replace("END$$(", Colors.END + "(").
+                replace("END$$,", Colors.END + ",").
+                replace("END$$[", Colors.END + "[").
+                replace("END$${", Colors.END + "{")
+            )
 
         except RecursionError:
             return repr(CircularReferenceStructure(*args, **kwargs))
         # end try
     # end __str__
 
     return __str__
@@ -563,33 +573,14 @@
 
         if self.__type__ is None:
             return "{" + content + "}"
         # end if
 
         return f"{self.name}({content})"
     # end __str__
-
-    def __hash__(self) -> int:
-        """
-        Creates the hash for the object.
-
-        :return: The hash for the data.
-        """
-
-        if self._hash is None:
-            hash_ = 0
-
-            for pair in self.items():
-                hash_ ^= hash(pair)
-            # end for
-
-            self._hash = hash_
-        # end if
-
-        return self._hash
 # end DictStructure
 
 class ListStructure(DataStructure, list):
     """A class to represent a structure."""
 
     def __str__(self) -> str:
         """
@@ -682,14 +673,48 @@
         :return: A string representation for the commands of the object.
         """
 
         return self.value
     # end __str__
 # end StringWrapper
 
+class FunctionStructure(DataStructure):
+    """A class to represent a structure."""
+
+    def __init__(self, value: Any) -> None:
+        """
+        Defines the class attributes.
+
+        :param value: The value to hold.
+        """
+
+        self.__value__ = value
+
+        self.__type__ = type(self.__value__)
+    # end __init__
+
+    def __str__(self) -> str:
+        """
+        Returns a string to represent the object.
+
+        :return: A string representation for the commands of the object.
+        """
+
+        return Colors.color_repr_address(
+            (
+                    f"<{Colors.CYAN}function{Colors.END}" +
+                    self.name[self.name.find(' '):self.name.find(self.__value__.__name__)] +
+                    f"{Colors.GREEN}{self.__value__.__name__}{Colors.END}" +
+                    self.name[self.name.find(" at "):]
+            ),
+            color=self.color
+        )
+    # end __str__
+# end FunctionStructure
+
 class CircularReferenceStructure(DataStructure):
     """A class to represent a structure."""
 
     def __init__(self, value: Any) -> None:
         """
         Defines the class attributes.
 
@@ -749,13 +774,14 @@
 
 Structure = Union[
     SetStructure, DictStructure, ListStructure, TupleStructure
 ]
 structures = {
     set: SetStructure, list: ListStructure,
     tuple: TupleStructure, dict: DictStructure,
-    type: TypeStructure
+    type: TypeStructure, types.FunctionType: FunctionStructure
 }
 
 structure_types = (
-    SetStructure, DictStructure, ListStructure, TupleStructure
+    SetStructure, DictStructure, ListStructure,
+    TupleStructure, FunctionStructure
 )
```

### Comparing `pyrepresent-0.0.9/setup.py` & `pyrepresent-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.0.9',
+        version='0.1.0',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

