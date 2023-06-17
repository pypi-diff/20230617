# Comparing `tmp/mo_json_config-4.407.23153-py2.py3-none-any.whl.zip` & `tmp/mo_json_config-4.413.23168-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15641 bytes, number of entries: 8
+Zip file size: 15655 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat    11053 b- defN 23-Jun-02 01:06 mo_json_config/__init__.py
 -rw-rw-rw-  2.0 fat     2411 b- defN 23-Apr-29 14:14 mo_json_config/configuration.py
 -rw-rw-rw-  2.0 fat      697 b- defN 23-Jun-02 01:48 mo_json_config/convert.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-02 01:48 mo_json_config-4.407.23153.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat    11524 b- defN 23-Jun-02 01:48 mo_json_config-4.407.23153.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-02 01:48 mo_json_config-4.407.23153.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jun-02 01:48 mo_json_config-4.407.23153.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      711 b- defN 23-Jun-02 01:48 mo_json_config-4.407.23153.dist-info/RECORD
-8 files, 43246 bytes uncompressed, 14391 bytes compressed:  66.7%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-17 01:44 mo_json_config-4.413.23168.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat    11524 b- defN 23-Jun-17 01:44 mo_json_config-4.413.23168.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-17 01:44 mo_json_config-4.413.23168.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jun-17 01:44 mo_json_config-4.413.23168.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      711 b- defN 23-Jun-17 01:44 mo_json_config-4.413.23168.dist-info/RECORD
+8 files, 43246 bytes uncompressed, 14405 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: mo_json_config/configuration.py
 Comment: 
 
 Filename: mo_json_config/convert.py
 Comment: 
 
-Filename: mo_json_config-4.407.23153.dist-info/LICENSE.txt
+Filename: mo_json_config-4.413.23168.dist-info/LICENSE.txt
 Comment: 
 
-Filename: mo_json_config-4.407.23153.dist-info/METADATA
+Filename: mo_json_config-4.413.23168.dist-info/METADATA
 Comment: 
 
-Filename: mo_json_config-4.407.23153.dist-info/WHEEL
+Filename: mo_json_config-4.413.23168.dist-info/WHEEL
 Comment: 
 
-Filename: mo_json_config-4.407.23153.dist-info/top_level.txt
+Filename: mo_json_config-4.413.23168.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_json_config-4.407.23153.dist-info/RECORD
+Filename: mo_json_config-4.413.23168.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mo_json_config-4.407.23153.dist-info/LICENSE.txt` & `mo_json_config-4.413.23168.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `mo_json_config-4.407.23153.dist-info/METADATA` & `mo_json_config-4.413.23168.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json-config
-Version: 4.407.23153
+Version: 4.413.23168
 Summary: More JSON Configuration! JSON configuration files with `$ref` and template overlays
 Home-page: https://github.com/klahnakoski/mo-json-config
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -12,19 +12,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: hjson
-Requires-Dist: mo-dots (==9.401.23144)
-Requires-Dist: mo-files (==6.407.23153)
+Requires-Dist: mo-dots (==9.408.23161)
+Requires-Dist: mo-files (==6.413.23168)
 Requires-Dist: mo-future (==7.401.23144)
-Requires-Dist: mo-json (==6.407.23153)
-Requires-Dist: mo-logs (==8.407.23153)
+Requires-Dist: mo-json (==6.413.23168)
+Requires-Dist: mo-logs (==8.412.23165)
 Requires-Dist: requests
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: keyring ; extra == 'tests'
 Requires-Dist: boto3 ; extra == 'tests'
 Requires-Dist: moto ; extra == 'tests'
 Requires-Dist: pyyaml ; extra == 'tests'
```

