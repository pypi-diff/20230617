# Comparing `tmp/bikeshare_model-0.0.8-py3-none-any.whl.zip` & `tmp/bikeshare_model-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 577753 bytes, number of entries: 22
+Zip file size: 577750 bytes, number of entries: 22
 -rw-r--r--  2.0 unx     6148 b- defN 23-Jun-16 16:18 .DS_Store
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-17 04:39 bikeshare_model/VERSION
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-17 04:45 bikeshare_model/VERSION
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
--rw-r--r--  2.0 unx     3058 b- defN 23-Jun-17 04:32 bikeshare_model/processing/data_manager.py
+-rw-r--r--  2.0 unx     3057 b- defN 23-Jun-17 04:45 bikeshare_model/processing/data_manager.py
 -rw-r--r--  2.0 unx     3241 b- defN 23-Jun-09 23:14 bikeshare_model/processing/features.py
 -rw-r--r--  2.0 unx     1266 b- defN 23-Jun-16 17:52 bikeshare_model/processing/validation.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-02 13:16 bikeshare_model/trained_models/__init__.py
 -rw-rw-r--  2.0 unx   659402 b- defN 23-Jun-10 04:30 bikeshare_model/trained_models/bikeshare__model_output_v0.0.1.pkl
--rw-r--r--  2.0 unx     1127 b- defN 23-Jun-17 04:40 bikeshare_model-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 04:40 bikeshare_model-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-17 04:40 bikeshare_model-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1965 b- defN 23-Jun-17 04:40 bikeshare_model-0.0.8.dist-info/RECORD
-22 files, 2604542 bytes uncompressed, 574503 bytes compressed:  78.0%
+-rw-r--r--  2.0 unx     1127 b- defN 23-Jun-17 04:45 bikeshare_model-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-17 04:45 bikeshare_model-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-17 04:45 bikeshare_model-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1965 b- defN 23-Jun-17 04:45 bikeshare_model-0.0.9.dist-info/RECORD
+22 files, 2604541 bytes uncompressed, 574500 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: bikeshare_model/trained_models/__init__.py
 Comment: 
 
 Filename: bikeshare_model/trained_models/bikeshare__model_output_v0.0.1.pkl
 Comment: 
 
-Filename: bikeshare_model-0.0.8.dist-info/METADATA
+Filename: bikeshare_model-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: bikeshare_model-0.0.8.dist-info/WHEEL
+Filename: bikeshare_model-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: bikeshare_model-0.0.8.dist-info/top_level.txt
+Filename: bikeshare_model-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bikeshare_model-0.0.8.dist-info/RECORD
+Filename: bikeshare_model-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bikeshare_model/VERSION

```diff
@@ -1 +1 @@
-0.0.8
+0.0.9
```

## bikeshare_model/processing/data_manager.py

```diff
@@ -14,15 +14,15 @@
 
 
 ##  Pre-Pipeline Preparation
 
 def get_year_and_month(dataframe):
 
     df = dataframe.copy()
-    print("get_year_and_month:"+dataframe)
+    print("get_year_and_month:",dataframe)
     # convert 'dteday' column to Datetime datatype
     df['dteday'] = pd.to_datetime(df['dteday'], format='%Y-%m-%d')
     
     #df['dteday'] = pd.to_datetime(df['dteday'], format='%d-%m-%Y')
     df['dteday']=df['dteday']
     # Add new features 'yr' and 'mnth
     df['yr'] = df['dteday'].dt.year.astype(str)
@@ -32,15 +32,15 @@
  
 # 2. processing cabin
 
 #f1=lambda x: 0 if type(x) == float else 1  ## Ternary Expression
   
 
 def pre_pipeline_preparation(*, data_frame: pd.DataFrame) -> pd.DataFrame:
-    print("pre_pipeline_preparation:" + data_frame)
+    print("pre_pipeline_preparation:", data_frame)
     data_frame = get_year_and_month(data_frame)
     #print("yr and month column")
     # drop unnecessary variables
     data_frame.drop(labels=config.model_config.unused_fields, axis=1, inplace=True)
     #print(data_frame.head)
     return data_frame
```

## Comparing `bikeshare_model-0.0.8.dist-info/METADATA` & `bikeshare_model-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bikeshare-model
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bikeshare dataset classification model package 
 Author: Ajay Singh
 Author-email: ajaytevatia@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

## Comparing `bikeshare_model-0.0.8.dist-info/RECORD` & `bikeshare_model-0.0.9.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 .DS_Store,sha256=JYjWrVq6wfd_yH8dN34ccrBeu88OKEKk75boDZo3c9M,6148
-bikeshare_model/VERSION,sha256=CM2QiEICclYGiuUIJbKSOagcqGl9WSXDl2ub1bBely4,5
+bikeshare_model/VERSION,sha256=8FnrHOC_APq3TqYxmKhYhiUrt0ws9oGS8F-Zd6kADbQ,5
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
-bikeshare_model/processing/data_manager.py,sha256=5u80GirVyppuOzMjw3N7whiZa_YmsFBkRqXil1bwAww,3058
+bikeshare_model/processing/data_manager.py,sha256=NHDHmvkAwYQeUXcOjp6oWvHK13YI_8OPsG-pyiJsU1w,3057
 bikeshare_model/processing/features.py,sha256=RUwJx34n45bcuwHIJuDoiIg-aX71Gf-fr30XGqYgcGc,3241
 bikeshare_model/processing/validation.py,sha256=flyKmoH3EGLpeGAt7TmcczsXumn29o8i_O0DRouxWa0,1266
 bikeshare_model/trained_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 bikeshare_model/trained_models/bikeshare__model_output_v0.0.1.pkl,sha256=WCN9pbYeC4IKpjYdl-dX2m1BfQBP7SAagIjXngLg7sQ,659402
-bikeshare_model-0.0.8.dist-info/METADATA,sha256=XaM1QOBo_wR1Gti-zYGdb_UJUgJoBgr0UoXJxyS1Dms,1127
-bikeshare_model-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-bikeshare_model-0.0.8.dist-info/top_level.txt,sha256=ZKIHSbGTS6ZE2aLhfpCV8HFAqGuZmXzRWQVz-N03wPI,16
-bikeshare_model-0.0.8.dist-info/RECORD,,
+bikeshare_model-0.0.9.dist-info/METADATA,sha256=ynvPOKnOlB7d0OioumYx0fNZZL8WmN4GnpkX5Y1QRfk,1127
+bikeshare_model-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bikeshare_model-0.0.9.dist-info/top_level.txt,sha256=ZKIHSbGTS6ZE2aLhfpCV8HFAqGuZmXzRWQVz-N03wPI,16
+bikeshare_model-0.0.9.dist-info/RECORD,,
```

