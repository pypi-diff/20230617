# Comparing `tmp/mo_json-6.413.23168-py2.py3-none-any.whl.zip` & `tmp/mo_json-6.420.23168-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 32240 bytes, number of entries: 12
+Zip file size: 32297 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat    14994 b- defN 23-Jun-02 01:41 mo_json/__init__.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-14 10:26 mo_json/decoder.py
 -rw-rw-rw-  2.0 fat    15429 b- defN 23-Apr-14 10:26 mo_json/encoder.py
 -rw-rw-rw-  2.0 fat    16185 b- defN 23-Apr-14 10:26 mo_json/stream.py
--rw-rw-rw-  2.0 fat    17835 b- defN 23-May-04 10:50 mo_json/typed_encoder.py
--rw-rw-rw-  2.0 fat     3504 b- defN 23-Jun-14 02:53 mo_json/typed_object.py
+-rw-rw-rw-  2.0 fat    17677 b- defN 23-Jun-17 11:19 mo_json/typed_encoder.py
+-rw-rw-rw-  2.0 fat     3962 b- defN 23-Jun-17 11:19 mo_json/typed_object.py
 -rw-rw-rw-  2.0 fat    10240 b- defN 23-Apr-30 12:14 mo_json/types.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11595 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      956 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/RECORD
-12 files, 107894 bytes uncompressed, 30658 bytes compressed:  71.6%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-17 11:19 mo_json-6.420.23168.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11595 b- defN 23-Jun-17 11:19 mo_json-6.420.23168.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-17 11:19 mo_json-6.420.23168.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-17 11:19 mo_json-6.420.23168.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      956 b- defN 23-Jun-17 11:19 mo_json-6.420.23168.dist-info/RECORD
+12 files, 108194 bytes uncompressed, 30715 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: mo_json/typed_object.py
 Comment: 
 
 Filename: mo_json/types.py
 Comment: 
 
-Filename: mo_json-6.413.23168.dist-info/LICENSE
+Filename: mo_json-6.420.23168.dist-info/LICENSE
 Comment: 
 
-Filename: mo_json-6.413.23168.dist-info/METADATA
+Filename: mo_json-6.420.23168.dist-info/METADATA
 Comment: 
 
-Filename: mo_json-6.413.23168.dist-info/WHEEL
+Filename: mo_json-6.420.23168.dist-info/WHEEL
 Comment: 
 
-Filename: mo_json-6.413.23168.dist-info/top_level.txt
+Filename: mo_json-6.420.23168.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_json-6.413.23168.dist-info/RECORD
+Filename: mo_json-6.420.23168.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_json/typed_encoder.py

```diff
@@ -112,20 +112,15 @@
 
 
 def detype(value):
     return _detype_value(value)
 
 
 def _detype_list(value):
-    if any(is_data(v) for v in value):
-        # MAY BE MORE TYPED OBJECTS IN THIS LIST
-        return [_detype_value(v) for v in value]
-    else:
-        # LIST OF PRIMITIVE VALUES
-        return value
+    return [_detype_value(v) for v in value]
 
 
 def _detype_dict(value):
     output = {}
 
     for k, v in value.items():
         if IS_TYPE_KEY.match(k):
```

## mo_json/typed_object.py

```diff
@@ -6,14 +6,15 @@
 #
 # Contact: Kyle Lahnakoski (kyle@lahnakoski.com)
 #
 from collections import OrderedDict
 
 from mo_dots import is_many, is_data, exists, is_missing
 from mo_dots.datas import register_data
+from mo_logs import logger
 
 from mo_json import python_type_to_jx_type_key, IS_PRIMITIVE_KEY, ARRAY_KEY, EXISTS_KEY, NUMBER_KEY
 
 
 def entype(value):
     """
     MAKE SURE VALUE IS TYPED
@@ -30,29 +31,41 @@
 
 class TypedObject(OrderedDict):
     """
     LAZY BOX FOR TYPED OBJECTS
     """
     __slots__ = ["_attachments", "_boxed_value"]
 
-    def __init__(self, value):
-        self._attachments = {}
+    def __init__(self, value, **attachments):
+        self._attachments = attachments
+        if isinstance(value, TypedObject):
+            logger.error("expecting plain object")
         self._boxed_value = value
 
+    def __iter__(self):
+        if is_many(self._boxed_value):
+            yield from self._boxed_value
+        else:
+            yield self._boxed_value
+
     def __getitem__(self, item):
         if item in self._attachments:
             return self._attachments[item]
         if item == NUMBER_KEY:
             if isinstance(self._boxed_value, (int, float)):
                 return self._boxed_value
             return None
         if item == ARRAY_KEY:
             if is_many(self._boxed_value):
-                return [TypedObject(v) for v in self._boxed_value]
+                return [entype(v) for v in self._boxed_value]
             return None
+        try:
+            IS_PRIMITIVE_KEY.match(item)
+        except Exception:
+            logger.error("expecting primitive key not {item}", item=item.__class__.__name__)
         if IS_PRIMITIVE_KEY.match(item):
             expected = python_type_to_jx_type_key.get(type(self._boxed_value))
             if item == expected:
                 return self._boxed_value
             return None
         if item == EXISTS_KEY:
             if is_many(self._boxed_value):
@@ -60,19 +73,19 @@
             elif exists(self._boxed_value):
                 return 1
             return 0
         if is_missing(self._boxed_value):
             return None
         else:
             try:
-                return TypedObject(self._boxed_value[item])
+                return entype(self._boxed_value[item])
             except Exception:
                 pass
             try:
-                return TypedObject(getattr(self._boxed_value, item))
+                return entype(getattr(self._boxed_value, item))
             except Exception:
                 pass
             return None
 
     def __setitem__(self, key, value):
         if isinstance(value, TypedObject):
             value = value._boxed_value
```

## Comparing `mo_json-6.413.23168.dist-info/LICENSE` & `mo_json-6.420.23168.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_json-6.413.23168.dist-info/METADATA` & `mo_json-6.420.23168.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json
-Version: 6.413.23168
+Version: 6.420.23168
 Summary: More JSON Tools! 
 Home-page: https://github.com/klahnakoski/mo-json
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
-Requires-Dist: mo-dots (==9.408.23161)
-Requires-Dist: mo-future (==7.401.23144)
-Requires-Dist: mo-logs (==8.412.23165)
-Requires-Dist: mo-times (==5.413.23168)
+Requires-Dist: mo-dots (==9.417.23168)
+Requires-Dist: mo-future (==7.416.23168)
+Requires-Dist: mo-logs (==8.417.23168)
+Requires-Dist: mo-times (==5.417.23168)
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 
 # More JSON Tools
```

## Comparing `mo_json-6.413.23168.dist-info/RECORD` & `mo_json-6.420.23168.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mo_json/__init__.py,sha256=W4Bc_NQlPQaM6r8rAhx-QFaeOwYutz8Dyyy7P72hqys,14994
 mo_json/decoder.py,sha256=iCE9aa_bwOCD6iDk461ywcHIBMJye-YIicGM6ILMlBk,313
 mo_json/encoder.py,sha256=PH8y_YEz9TSNhm1QJy2eW1PKUSPE2GdZwtHkASb18Js,15429
 mo_json/stream.py,sha256=DRbMb3IwpyW1s2J-Udws1wjCVCbaXGiXAa_7Ao9W4tI,16185
-mo_json/typed_encoder.py,sha256=ZLYbbeqgVbllDmxmQ4v83EM48w9hfdYnjK9q1R8mU0k,17835
-mo_json/typed_object.py,sha256=Dg3jo9NtkG2z5ImUMij-OcqnEmU5ocxbmscx56N8LnA,3504
+mo_json/typed_encoder.py,sha256=Gk3nrw9K8x11XO2mgCPXL2QDROOcY-BCwi4KpbX6T3g,17677
+mo_json/typed_object.py,sha256=uz0hhzm7p9C3fZJNg5MZuiqFaOqz9luxx7GFXqA6Sxw,3962
 mo_json/types.py,sha256=VSLHgpQ8KF1iTXuqV0XTZILaLO28AGSrab_wdFLgo48,10240
-mo_json-6.413.23168.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_json-6.413.23168.dist-info/METADATA,sha256=82ylt6jjnBYVViWiZyN9Eq_cOiIdMntzuez_TcnfsGU,11595
-mo_json-6.413.23168.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_json-6.413.23168.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
-mo_json-6.413.23168.dist-info/RECORD,,
+mo_json-6.420.23168.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_json-6.420.23168.dist-info/METADATA,sha256=mgHFmqgNT82XXQcU27QOJYYsj9Dd1NF18Jv6Z2cCgnw,11595
+mo_json-6.420.23168.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_json-6.420.23168.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
+mo_json-6.420.23168.dist-info/RECORD,,
```

