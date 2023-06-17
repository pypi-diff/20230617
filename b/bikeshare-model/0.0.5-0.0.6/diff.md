# Comparing `tmp/bikeshare_model-0.0.5-py3-none-any.whl.zip` & `tmp/bikeshare_model-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 577744 bytes, number of entries: 22
+Zip file size: 577732 bytes, number of entries: 22
 -rw-r--r--  2.0 unx     6148 b- defN 23-Jun-16 16:18 .DS_Store
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-16 18:11 bikeshare_model/VERSION
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-17 03:47 bikeshare_model/VERSION
 -rw-r--r--  2.0 unx      253 b- defN 23-Jun-08 23:54 bikeshare_model/__init__.py
 -rw-rw-r--  2.0 unx     2061 b- defN 23-Jun-09 22:47 bikeshare_model/config.yml
 -rw-r--r--  2.0 unx     2134 b- defN 23-Jun-09 21:41 bikeshare_model/pipeline.py
 -rw-r--r--  2.0 unx     1878 b- defN 23-Jun-10 01:55 bikeshare_model/predict.py
 -rw-r--r--  2.0 unx     1679 b- defN 23-Jun-09 22:58 bikeshare_model/train_pipeline.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:16 bikeshare_model/config/__init__.py
 -rw-r--r--  2.0 unx     2928 b- defN 23-Jun-10 04:30 bikeshare_model/config/core.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:16 bikeshare_model/datasets/__init__.py
 -rw-rw-r--  2.0 unx  1598454 b- defN 23-Jun-02 20:20 bikeshare_model/datasets/bike-sharing-dataset.csv
 -rw-rw-r--  2.0 unx   318833 b- defN 23-Jun-10 04:13 bikeshare_model/datasets/test.csv
 -rw-r--r--  2.0 unx        2 b- defN 23-Jun-02 13:16 bikeshare_model/processing/__init__.py
--rw-r--r--  2.0 unx     2967 b- defN 23-Jun-09 23:12 bikeshare_model/processing/data_manager.py
+-rw-r--r--  2.0 unx     2957 b- defN 23-Jun-17 03:46 bikeshare_model/processing/data_manager.py
 -rw-r--r--  2.0 unx     3241 b- defN 23-Jun-09 23:14 bikeshare_model/processing/features.py
 -rw-r--r--  2.0 unx     1266 b- defN 23-Jun-16 17:52 bikeshare_model/processing/validation.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:16 bikeshare_model/trained_models/__init__.py
 -rw-rw-r--  2.0 unx   659402 b- defN 23-Jun-10 04:30 bikeshare_model/trained_models/bikeshare__model_output_v0.0.1.pkl
--rw-r--r--  2.0 unx     1127 b- defN 23-Jun-16 18:12 bikeshare_model-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 18:12 bikeshare_model-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-16 18:12 bikeshare_model-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1965 b- defN 23-Jun-16 18:12 bikeshare_model-0.0.5.dist-info/RECORD
-22 files, 2604451 bytes uncompressed, 574494 bytes compressed:  78.0%
+-rw-r--r--  2.0 unx     1127 b- defN 23-Jun-17 03:47 bikeshare_model-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 03:47 bikeshare_model-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-17 03:47 bikeshare_model-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1965 b- defN 23-Jun-17 03:47 bikeshare_model-0.0.6.dist-info/RECORD
+22 files, 2604441 bytes uncompressed, 574482 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: bikeshare_model/trained_models/__init__.py
 Comment: 
 
 Filename: bikeshare_model/trained_models/bikeshare__model_output_v0.0.1.pkl
 Comment: 
 
-Filename: bikeshare_model-0.0.5.dist-info/METADATA
+Filename: bikeshare_model-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: bikeshare_model-0.0.5.dist-info/WHEEL
+Filename: bikeshare_model-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: bikeshare_model-0.0.5.dist-info/top_level.txt
+Filename: bikeshare_model-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: bikeshare_model-0.0.5.dist-info/RECORD
+Filename: bikeshare_model-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bikeshare_model/VERSION

```diff
@@ -1 +1 @@
-0.0.5
+0.0.6
```

## bikeshare_model/processing/data_manager.py

```diff
@@ -1,9 +1,9 @@
 import sys
-sys.path.append('C:/Users/mili/Desktop/IISC_AIMLOPs/Project')
+sys.path.append('/Users/ajaysingh/aimlops/Project')
 
 import typing as t
 from pathlib import Path
 import re
 
 import joblib
 import pandas as pd
```

## Comparing `bikeshare_model-0.0.5.dist-info/METADATA` & `bikeshare_model-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bikeshare-model
-Version: 0.0.5
+Version: 0.0.6
 Summary: Bikeshare dataset classification model package 
 Author: Ajay Singh
 Author-email: ajaytevatia@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `bikeshare_model-0.0.5.dist-info/RECORD` & `bikeshare_model-0.0.6.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 .DS_Store,sha256=JYjWrVq6wfd_yH8dN34ccrBeu88OKEKk75boDZo3c9M,6148
-bikeshare_model/VERSION,sha256=C4j3pj86QPw4Cq8hq8csyN7ZzSjX7pAbxzJ0l7toMRY,5
+bikeshare_model/VERSION,sha256=BMTxCtbXfYQbCdAxzrYbeUtTGcW5xch30vtlsup50GY,5
 bikeshare_model/__init__.py,sha256=FBsKr5BGRd1vc2e9OTnoCb4J8Nhb_RWLwuwdDinJYlc,253
 bikeshare_model/config.yml,sha256=ObXJC4ZYuTQXeBwmzNI0eTqhyqajQOo1fxV-ccKWkZg,2061
 bikeshare_model/pipeline.py,sha256=Iv5zp0Eo6aZB5rYo6GG_G5ikheeTdUYkDyb_6VFtWIs,2134
 bikeshare_model/predict.py,sha256=Emdw-4st-Me2WDJ54C4m7MGUv3Gm6xRuDSheFV_UJDs,1878
 bikeshare_model/train_pipeline.py,sha256=FT8b5Zn1i6c6DH_odV2xqeyBazLmZ_PvSEIIswjPlh8,1679
 bikeshare_model/config/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bikeshare_model/config/core.py,sha256=SIN1ruGN2QvueaySxmc--5-4OS5TeH4RTzTaQxywkPQ,2928
 bikeshare_model/datasets/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bikeshare_model/datasets/bike-sharing-dataset.csv,sha256=NyQ2F3BOHwh6JMkESfZL5hIrnecqwNFWQf4_uihALx4,1598454
 bikeshare_model/datasets/test.csv,sha256=qUBW4-MjYr_g-YqdY4wwl8_hNSYfPiAMjAo-TdG1Jhw,318833
 bikeshare_model/processing/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-bikeshare_model/processing/data_manager.py,sha256=ua314xx_3L6NWmPaEIJ2ybxGzVAfGgOmptYZKMlTUfM,2967
+bikeshare_model/processing/data_manager.py,sha256=v8_TvV1dmGTOlFP3JxhPXAss3_pRskA0_IwscKiiZ6s,2957
 bikeshare_model/processing/features.py,sha256=RUwJx34n45bcuwHIJuDoiIg-aX71Gf-fr30XGqYgcGc,3241
 bikeshare_model/processing/validation.py,sha256=flyKmoH3EGLpeGAt7TmcczsXumn29o8i_O0DRouxWa0,1266
 bikeshare_model/trained_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bikeshare_model/trained_models/bikeshare__model_output_v0.0.1.pkl,sha256=WCN9pbYeC4IKpjYdl-dX2m1BfQBP7SAagIjXngLg7sQ,659402
-bikeshare_model-0.0.5.dist-info/METADATA,sha256=-3S1rqhLwUnYTIDA30_7eTAR4MdofWzAeY7DZw4amZQ,1127
-bikeshare_model-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-bikeshare_model-0.0.5.dist-info/top_level.txt,sha256=ZKIHSbGTS6ZE2aLhfpCV8HFAqGuZmXzRWQVz-N03wPI,16
-bikeshare_model-0.0.5.dist-info/RECORD,,
+bikeshare_model-0.0.6.dist-info/METADATA,sha256=S5WubKNxILI9yeaEpUb1d5A-mKsqUKNXWQ5fZ99tlyE,1127
+bikeshare_model-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bikeshare_model-0.0.6.dist-info/top_level.txt,sha256=ZKIHSbGTS6ZE2aLhfpCV8HFAqGuZmXzRWQVz-N03wPI,16
+bikeshare_model-0.0.6.dist-info/RECORD,,
```

