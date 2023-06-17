# Comparing `tmp/mo_json-6.412.23165-py2.py3-none-any.whl.zip` & `tmp/mo_json-6.413.23168-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 32235 bytes, number of entries: 12
+Zip file size: 32240 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat    14994 b- defN 23-Jun-02 01:41 mo_json/__init__.py
 -rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-14 10:26 mo_json/decoder.py
 -rw-rw-rw-  2.0 fat    15429 b- defN 23-Apr-14 10:26 mo_json/encoder.py
 -rw-rw-rw-  2.0 fat    16185 b- defN 23-Apr-14 10:26 mo_json/stream.py
 -rw-rw-rw-  2.0 fat    17835 b- defN 23-May-04 10:50 mo_json/typed_encoder.py
 -rw-rw-rw-  2.0 fat     3504 b- defN 23-Jun-14 02:53 mo_json/typed_object.py
 -rw-rw-rw-  2.0 fat    10240 b- defN 23-Apr-30 12:14 mo_json/types.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-14 22:55 mo_json-6.412.23165.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11595 b- defN 23-Jun-14 22:55 mo_json-6.412.23165.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-14 22:55 mo_json-6.412.23165.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-14 22:55 mo_json-6.412.23165.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      956 b- defN 23-Jun-14 22:55 mo_json-6.412.23165.dist-info/RECORD
-12 files, 107894 bytes uncompressed, 30653 bytes compressed:  71.6%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11595 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      956 b- defN 23-Jun-17 01:35 mo_json-6.413.23168.dist-info/RECORD
+12 files, 107894 bytes uncompressed, 30658 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: mo_json/typed_object.py
 Comment: 
 
 Filename: mo_json/types.py
 Comment: 
 
-Filename: mo_json-6.412.23165.dist-info/LICENSE
+Filename: mo_json-6.413.23168.dist-info/LICENSE
 Comment: 
 
-Filename: mo_json-6.412.23165.dist-info/METADATA
+Filename: mo_json-6.413.23168.dist-info/METADATA
 Comment: 
 
-Filename: mo_json-6.412.23165.dist-info/WHEEL
+Filename: mo_json-6.413.23168.dist-info/WHEEL
 Comment: 
 
-Filename: mo_json-6.412.23165.dist-info/top_level.txt
+Filename: mo_json-6.413.23168.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_json-6.412.23165.dist-info/RECORD
+Filename: mo_json-6.413.23168.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mo_json-6.412.23165.dist-info/LICENSE` & `mo_json-6.413.23168.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_json-6.412.23165.dist-info/METADATA` & `mo_json-6.413.23168.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json
-Version: 6.412.23165
+Version: 6.413.23168
 Summary: More JSON Tools! 
 Home-page: https://github.com/klahnakoski/mo-json
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hjson
 Requires-Dist: mo-dots (==9.408.23161)
 Requires-Dist: mo-future (==7.401.23144)
 Requires-Dist: mo-logs (==8.412.23165)
-Requires-Dist: mo-times (==5.412.23165)
+Requires-Dist: mo-times (==5.413.23168)
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 
 # More JSON Tools
```

## Comparing `mo_json-6.412.23165.dist-info/RECORD` & `mo_json-6.413.23168.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mo_json/__init__.py,sha256=W4Bc_NQlPQaM6r8rAhx-QFaeOwYutz8Dyyy7P72hqys,14994
 mo_json/decoder.py,sha256=iCE9aa_bwOCD6iDk461ywcHIBMJye-YIicGM6ILMlBk,313
 mo_json/encoder.py,sha256=PH8y_YEz9TSNhm1QJy2eW1PKUSPE2GdZwtHkASb18Js,15429
 mo_json/stream.py,sha256=DRbMb3IwpyW1s2J-Udws1wjCVCbaXGiXAa_7Ao9W4tI,16185
 mo_json/typed_encoder.py,sha256=ZLYbbeqgVbllDmxmQ4v83EM48w9hfdYnjK9q1R8mU0k,17835
 mo_json/typed_object.py,sha256=Dg3jo9NtkG2z5ImUMij-OcqnEmU5ocxbmscx56N8LnA,3504
 mo_json/types.py,sha256=VSLHgpQ8KF1iTXuqV0XTZILaLO28AGSrab_wdFLgo48,10240
-mo_json-6.412.23165.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_json-6.412.23165.dist-info/METADATA,sha256=23X6PACr4GtUYzE21tfWOzO0C6p8RAERC638TNXFFOY,11595
-mo_json-6.412.23165.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_json-6.412.23165.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
-mo_json-6.412.23165.dist-info/RECORD,,
+mo_json-6.413.23168.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_json-6.413.23168.dist-info/METADATA,sha256=82ylt6jjnBYVViWiZyN9Eq_cOiIdMntzuez_TcnfsGU,11595
+mo_json-6.413.23168.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_json-6.413.23168.dist-info/top_level.txt,sha256=svvpHEXHZaMl3nAq8QPmHxHJjsBFiFLZ2RSfAVPck1g,8
+mo_json-6.413.23168.dist-info/RECORD,,
```

