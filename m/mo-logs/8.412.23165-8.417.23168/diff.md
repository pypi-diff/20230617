# Comparing `tmp/mo_logs-8.412.23165-py2.py3-none-any.whl.zip` & `tmp/mo_logs-8.417.23168-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 43117 bytes, number of entries: 21
+Zip file size: 43103 bytes, number of entries: 21
 -rw-rw-rw-  2.0 fat    15892 b- defN 23-Jun-14 22:50 mo_logs/__init__.py
 -rw-rw-rw-  2.0 fat     2329 b- defN 23-Apr-30 18:00 mo_logs/constants.py
 -rw-rw-rw-  2.0 fat     2407 b- defN 23-May-30 00:22 mo_logs/convert.py
 -rw-rw-rw-  2.0 fat     8762 b- defN 23-Jun-14 02:49 mo_logs/exceptions.py
 -rw-rw-rw-  2.0 fat     3524 b- defN 23-Apr-30 18:00 mo_logs/log_usingEmail.py
 -rw-rw-rw-  2.0 fat     1099 b- defN 23-Apr-30 18:00 mo_logs/log_usingFile.py
 -rw-rw-rw-  2.0 fat     3301 b- defN 23-May-09 22:44 mo_logs/log_usingHandler.py
@@ -11,13 +11,13 @@
 -rw-rw-rw-  2.0 fat     1454 b- defN 23-Apr-30 18:00 mo_logs/log_usingMulti.py
 -rw-rw-rw-  2.0 fat      450 b- defN 23-Apr-30 18:00 mo_logs/log_usingNothing.py
 -rw-rw-rw-  2.0 fat     4069 b- defN 23-Apr-30 18:00 mo_logs/log_usingSES.py
 -rw-rw-rw-  2.0 fat     1525 b- defN 23-May-30 00:22 mo_logs/log_usingStream.py
 -rw-rw-rw-  2.0 fat     2325 b- defN 23-Apr-30 18:00 mo_logs/log_usingThread.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-May-30 00:22 mo_logs/startup.py
 -rw-rw-rw-  2.0 fat    25364 b- defN 23-Jun-14 02:49 mo_logs/strings.py
--rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    17648 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1700 b- defN 23-Jun-14 22:50 mo_logs-8.412.23165.dist-info/RECORD
-21 files, 119604 bytes uncompressed, 40383 bytes compressed:  66.2%
+-rw-rw-rw-  2.0 fat    16725 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    17648 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1700 b- defN 23-Jun-17 10:48 mo_logs-8.417.23168.dist-info/RECORD
+21 files, 119604 bytes uncompressed, 40369 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: mo_logs/startup.py
 Comment: 
 
 Filename: mo_logs/strings.py
 Comment: 
 
-Filename: mo_logs-8.412.23165.dist-info/LICENSE
+Filename: mo_logs-8.417.23168.dist-info/LICENSE
 Comment: 
 
-Filename: mo_logs-8.412.23165.dist-info/METADATA
+Filename: mo_logs-8.417.23168.dist-info/METADATA
 Comment: 
 
-Filename: mo_logs-8.412.23165.dist-info/WHEEL
+Filename: mo_logs-8.417.23168.dist-info/WHEEL
 Comment: 
 
-Filename: mo_logs-8.412.23165.dist-info/top_level.txt
+Filename: mo_logs-8.417.23168.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_logs-8.412.23165.dist-info/RECORD
+Filename: mo_logs-8.417.23168.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `mo_logs-8.412.23165.dist-info/LICENSE` & `mo_logs-8.417.23168.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_logs-8.412.23165.dist-info/METADATA` & `mo_logs-8.417.23168.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-logs
-Version: 8.412.23165
+Version: 8.417.23168
 Summary: More Logs! Structured Logging and Exception Handling
 Home-page: https://github.com/klahnakoski/mo-logs
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -12,18 +12,18 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots (==9.408.23161)
-Requires-Dist: mo-future (==7.401.23144)
-Requires-Dist: mo-imports (==7.408.23161)
-Requires-Dist: mo-kwargs (==7.409.23162)
+Requires-Dist: mo-dots (==9.417.23168)
+Requires-Dist: mo-future (==7.416.23168)
+Requires-Dist: mo-imports (==7.416.23168)
+Requires-Dist: mo-kwargs (==7.417.23168)
 Provides-Extra: tests
 Requires-Dist: mo-json ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-kwargs ; extra == 'tests'
 Requires-Dist: jx-python ; extra == 'tests'
 Requires-Dist: boto ; extra == 'tests'
```

## Comparing `mo_logs-8.412.23165.dist-info/RECORD` & `mo_logs-8.417.23168.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -10,12 +10,12 @@
 mo_logs/log_usingMulti.py,sha256=2uUM3zHgpviKL5xJUIhi-5ReFEC51Zqv9-imi0xjBi0,1454
 mo_logs/log_usingNothing.py,sha256=RAJGGPwg4bw-eX4kDFT0kdEHH4hFsLicnJeq9Pf4Y3Q,450
 mo_logs/log_usingSES.py,sha256=hzfmQSiMnBudy4ptn73nGLUOXB-uhBXbOdUpv42HYjs,4069
 mo_logs/log_usingStream.py,sha256=t9q7Ju7F9wMKjReWXkUIcpkKRkiat2FHa---s8gdJ4s,1525
 mo_logs/log_usingThread.py,sha256=LbWlEBNGbjPBEFFIegmXhuT1_AA7H18Lv8YGDRVUpMc,2325
 mo_logs/startup.py,sha256=sMOxbRnsb-GPoMidGoTYAS9ooasv4BfwJRvyklY7fKM,6310
 mo_logs/strings.py,sha256=d63f-90qN-YlyqSDU8YqSS3HzcN18OT8zY-UMk6HF5I,25364
-mo_logs-8.412.23165.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
-mo_logs-8.412.23165.dist-info/METADATA,sha256=T37CdE3LWxVhLNOZPrbLBgM3Rb4UuGF_DT0UkjZsqFQ,17648
-mo_logs-8.412.23165.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_logs-8.412.23165.dist-info/top_level.txt,sha256=yqpeBBL3Yw2CDh1_FthlIK34KbT5cyZcAEjxlQ3MpDA,8
-mo_logs-8.412.23165.dist-info/RECORD,,
+mo_logs-8.417.23168.dist-info/LICENSE,sha256=HyVuytGSiAUQ6ErWBHTqt1iSGHhLmlC8fO7jTCuR8dU,16725
+mo_logs-8.417.23168.dist-info/METADATA,sha256=F9f8apmNTbglHO2OhNQB9zzuRMYeAsEwcydYH249-bU,17648
+mo_logs-8.417.23168.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_logs-8.417.23168.dist-info/top_level.txt,sha256=yqpeBBL3Yw2CDh1_FthlIK34KbT5cyZcAEjxlQ3MpDA,8
+mo_logs-8.417.23168.dist-info/RECORD,,
```

