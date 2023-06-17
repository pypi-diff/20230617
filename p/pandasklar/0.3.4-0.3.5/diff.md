# Comparing `tmp/pandasklar-0.3.4.tar.gz` & `tmp/pandasklar-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasklar-0.3.4.tar", last modified: Fri Jun 16 08:34:52 2023, max compression
+gzip compressed data, was "pandasklar-0.3.5.tar", last modified: Sat Jun 17 20:47:35 2023, max compression
```

## Comparing `pandasklar-0.3.4.tar` & `pandasklar-0.3.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-16 08:34:52.223574 pandasklar-0.3.4/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.3.4/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)     9805 2023-06-16 08:34:52.223574 pandasklar-0.3.4/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     9297 2023-06-16 08:34:16.000000 pandasklar-0.3.4/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1301 2023-06-16 08:34:00.000000 pandasklar-0.3.4/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-16 08:34:52.223574 pandasklar-0.3.4/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-16 08:34:52.215574 pandasklar-0.3.4/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-16 08:34:52.223574 pandasklar-0.3.4/src/pandasklar/
--rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.3.4/src/pandasklar/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.3.4/src/pandasklar/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)    19899 2023-05-12 20:23:55.000000 pandasklar-0.3.4/src/pandasklar/aggregate.py
--rw-r--r--   0 me        (1000) me        (1000)    27921 2023-06-16 07:57:01.000000 pandasklar-0.3.4/src/pandasklar/analyse.py
--rw-r--r--   0 me        (1000) me        (1000)    10330 2023-02-12 20:17:03.000000 pandasklar-0.3.4/src/pandasklar/compare.py
--rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.3.4/src/pandasklar/config.py
--rw-r--r--   0 me        (1000) me        (1000)    27326 2023-06-16 08:25:57.000000 pandasklar-0.3.4/src/pandasklar/content.py
--rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.3.4/src/pandasklar/develop.py
--rw-r--r--   0 me        (1000) me        (1000)    32239 2023-03-16 08:54:51.000000 pandasklar-0.3.4/src/pandasklar/pandas.py
--rw-r--r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.3.4/src/pandasklar/plot.py
--rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.3.4/src/pandasklar/rank.py
--rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.3.4/src/pandasklar/scale.py
--rw-r--r--   0 me        (1000) me        (1000)     8975 2023-04-10 20:10:39.000000 pandasklar-0.3.4/src/pandasklar/string.py
--rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.3.4/src/pandasklar/subsets.py
--rw-r--r--   0 me        (1000) me        (1000)     5665 2023-06-09 20:00:34.000000 pandasklar-0.3.4/src/pandasklar/type_info.py
--rw-r--r--   0 me        (1000) me        (1000)     5467 2022-11-09 07:00:35.000000 pandasklar-0.3.4/src/pandasklar/values_info.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-16 08:34:52.223574 pandasklar-0.3.4/src/pandasklar.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     9805 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      677 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       56 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       47 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)       11 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 20:47:35.803096 pandasklar-0.3.5/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.3.5/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)     9805 2023-06-17 20:47:35.803096 pandasklar-0.3.5/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     9297 2023-06-17 20:46:52.000000 pandasklar-0.3.5/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1301 2023-06-17 20:46:44.000000 pandasklar-0.3.5/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-17 20:47:35.803096 pandasklar-0.3.5/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 20:47:35.407100 pandasklar-0.3.5/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 20:47:35.783096 pandasklar-0.3.5/src/pandasklar/
+-rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.3.5/src/pandasklar/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.3.5/src/pandasklar/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)    19899 2023-05-12 20:23:55.000000 pandasklar-0.3.5/src/pandasklar/aggregate.py
+-rw-r--r--   0 me        (1000) me        (1000)    28272 2023-06-16 15:41:42.000000 pandasklar-0.3.5/src/pandasklar/analyse.py
+-rw-r--r--   0 me        (1000) me        (1000)    10330 2023-02-12 20:17:03.000000 pandasklar-0.3.5/src/pandasklar/compare.py
+-rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.3.5/src/pandasklar/config.py
+-rw-r--r--   0 me        (1000) me        (1000)    27326 2023-06-16 08:25:57.000000 pandasklar-0.3.5/src/pandasklar/content.py
+-rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.3.5/src/pandasklar/develop.py
+-rw-r--r--   0 me        (1000) me        (1000)    32239 2023-03-16 08:54:51.000000 pandasklar-0.3.5/src/pandasklar/pandas.py
+-rw-rw-r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.3.5/src/pandasklar/plot.py
+-rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.3.5/src/pandasklar/rank.py
+-rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.3.5/src/pandasklar/scale.py
+-rw-r--r--   0 me        (1000) me        (1000)     9244 2023-06-16 08:47:39.000000 pandasklar-0.3.5/src/pandasklar/string.py
+-rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.3.5/src/pandasklar/subsets.py
+-rw-r--r--   0 me        (1000) me        (1000)     5665 2023-06-09 20:00:34.000000 pandasklar-0.3.5/src/pandasklar/type_info.py
+-rw-r--r--   0 me        (1000) me        (1000)     7796 2023-06-16 19:15:33.000000 pandasklar-0.3.5/src/pandasklar/values_info.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-17 20:47:35.803096 pandasklar-0.3.5/src/pandasklar.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)     9805 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      677 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       56 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       47 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)       11 2023-06-17 20:47:35.000000 pandasklar-0.3.5/src/pandasklar.egg-info/top_level.txt
```

### Comparing `pandasklar-0.3.4/LICENSE` & `pandasklar-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/PKG-INFO` & `pandasklar-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.3.4
+Version: 0.3.5
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandasklar-0.3.4/README.md` & `pandasklar-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/pyproject.toml` & `pandasklar-0.3.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyproject.toml
 
 
 [project]
 name            = "pandasklar"
-version         = "0.3.4"    
+version         = "0.3.5"    
 
 requires-python = ">=3.8"
 dependencies    = ['pandas','numpy','perlin_noise','termcolor','bpyth','blab',]
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
 description     = "Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL."
 readme          = "README.md"
```

### Comparing `pandasklar-0.3.4/src/pandasklar/__init__.py` & `pandasklar-0.3.5/src/pandasklar/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/aggregate.py` & `pandasklar-0.3.5/src/pandasklar/aggregate.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/analyse.py` & `pandasklar-0.3.5/src/pandasklar/analyse.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,89 +90,86 @@
 # ...............................................................................
 # Spalten auf datatype untersuchen
 # ...............................................................................
 #################################################################################    
     
 
     
-def mem_usage(data):
+def mem_usage(data, human_readable=True):
     """Returns the memory consumption of a Series or a DataFrame"""
     
     if isinstance(data, pd.Series): 
         result = data.memory_usage(index=False, deep=True)
-        return bpy.human_readable_bytes(result)    
+        if human_readable:
+            return bpy.human_readable_bytes(result) 
+        else:
+            return result
     
     elif isinstance(data, pd.DataFrame):
         result = data.memory_usage(index=False, deep=True).sum()
-        return bpy.human_readable_bytes(result)    
+        if human_readable:
+            return bpy.human_readable_bytes(result) 
+        else:
+            return result 
         
     else:
         assert 'ERROR'    
 
 
 
 
 # Alle class_info einer Series oder eines Index   
-def analyse_datatype(data):
+def analyse_datatype(data, human_readable=True):
     """ 
     Returns a dict with info about the datatypes of a Series or Index and it's content
     """
-
-
-    def is_datetime_series(series):
-        try:
-            pd.to_datetime(series)
-            return pd.api.types.is_datetime64_any_dtype(series)
-        except ValueError:
-            return False
-
     
     if isinstance(data, pd.DataFrame): 
-        return dataframe( analyse_datatypes(data) ) 
+        return dataframe( analyse_datatypes(data, human_readable=human_readable) ) 
         
     # Aufruf mit Index
     if isinstance(data, pd.Index): 
         series = data.to_series()
         series.name = '__index__'
-        return analyse_datatype(series)    
+        return analyse_datatype(series, human_readable=human_readable)    
 
     info = type_info(data)
     result = {
         'col_name': data.name,
         'datatype_instance': info.name_instance,  
         'datatype': info.name,        
         'datatype_short': info.name_short,        
         'is_numeric': is_numeric_dtype(data),                
         'is_string': is_string_dtype(data),  
         'is_datetime': pd.api.types.is_datetime64_any_dtype(data),         
         'is_hashable': info.is_hashable,
         'nan_allowed': info.nan_allowed,   
-        'mem_usage': mem_usage(data),        
+        'mem_usage': mem_usage(data, human_readable=human_readable),        
     }
         
     return result
 
 
 
 # Alle class_info eines DataFrame
-def analyse_datatypes(df, with_index=True):
+def analyse_datatypes(df, with_index=True, human_readable=True):
     """
     Returns info about the datatypes and the mem_usage of the columns of a DataFrame.  
     """
     if isinstance(df, pd.Series): 
-        return dataframe( analyse_datatype(df), verbose=False ) 
+        return dataframe( analyse_datatype(df, human_readable=human_readable), verbose=False ) 
     
     # Kleine Probe reicht
     if df.shape[0] > 10:
-        return analyse_datatypes(quicksample(df, 10), with_index=with_index)
+        return analyse_datatypes(quicksample(df, 10), with_index=with_index, human_readable=human_readable)
     
     data  = [] 
     if with_index:
-        data += [ analyse_datatype(df.index)]
-    data     += [ analyse_datatype(df[col]) for col in df ]
+        data += [ analyse_datatype( df.index, human_readable=human_readable) ]
+    data     += [ analyse_datatype( df[col],  human_readable=human_readable) for col in df ]
 
     result = dataframe(data, verbose=False)
 
     # Zeilen-, Spalten- und Tabellenname
     result = result.rename_axis('col_no')    
     result = result.rename_axis('', axis='columns')
     return result
@@ -326,23 +323,24 @@
         info.n,   
         info.vmin,      
         info.vmean,        
         info.vmedian,
         info.vmax,      
         info.vsum,            
         info.datatype_suggest,
+        info.datatype_identified,
     ]
     
     # Rückgabe als Liste
     if as_list:
         return result
     
     # In DataFrame wandeln
     result = pd.DataFrame(result)
-    result['analyse'] = pd.Series(['col_name','ntypes', 'nunique','nnan','ndups','n','vmin','vmean','vmedian','vmax','vsum','datatype_suggest'])
+    result['analyse'] = pd.Series(['col_name','ntypes', 'nunique','nnan','ndups','n','vmin','vmean','vmedian','vmax','vsum','datatype_suggest','datatype_identified'])
     result = result.set_index('analyse')
     
     # Rückgabe als dict
     if as_dict:
         result = result.to_dict()[0]
         del result['col_name']
         return result    
@@ -353,24 +351,24 @@
     
     
 
 # ==================================================================================================
 # analyse_cols
 # ==================================================================================================
 
-def analyse_cols(df, sort=False, with_index=True):
+def analyse_cols(df, sort=False, with_index=True, human_readable=True):
     """ 
     Describes the datatypes and the content of a DataFrame.
     Merged info from analyse_datatypes and analyse_values.
     """   
         
-    info1  = analyse_datatypes(df, with_index=with_index)
+    info1  = analyse_datatypes(df, with_index=with_index, human_readable=human_readable)
     info2  = analyse_values(   df, with_index=with_index)
     result = pd.merge(info1, info2)    
-    result = move_cols(result, ['col_name','datatype_instance','datatype','datatype_short','datatype_suggest'])
+    result = move_cols(result, ['col_name','datatype_instance','datatype','datatype_short','datatype_suggest','datatype_identified'])
 
     if sort:
         result = result.sort_values(['nunique','col_name'], ascending=[False,True])    
     return result    
 
             
         
@@ -611,14 +609,17 @@
     '''
     return series[series.notna()].map(type).nunique()
 
 
 
 
 
+
+
+
 ##############################################################################################
 # ............................................................................................
 # DataFrames 
 # ............................................................................................
 ##############################################################################################
```

### Comparing `pandasklar-0.3.4/src/pandasklar/compare.py` & `pandasklar-0.3.5/src/pandasklar/compare.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/config.py` & `pandasklar-0.3.5/src/pandasklar/config.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/content.py` & `pandasklar-0.3.5/src/pandasklar/content.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/develop.py` & `pandasklar-0.3.5/src/pandasklar/develop.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/pandas.py` & `pandasklar-0.3.5/src/pandasklar/pandas.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/plot.py` & `pandasklar-0.3.5/src/pandasklar/plot.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/rank.py` & `pandasklar-0.3.5/src/pandasklar/rank.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/scale.py` & `pandasklar-0.3.5/src/pandasklar/scale.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/string.py` & `pandasklar-0.3.5/src/pandasklar/string.py`

 * *Files 5% similar despite different names*

```diff
@@ -240,7 +240,31 @@
 
 
 
 def preprocess_strings( dirty, how=''):
     raise('preprocess_strings ist jetzt in bj_nlp')
 
 
+
+def force_string(s):
+    ''' Forces a Series to String'''
+    t = pd.get_option('display.max_colwidth')
+    pd.set_option('display.max_colwidth', 100000)
+    s = s.to_string(index=False)
+    pd.set_option('display.max_colwidth', t)   
+    return s
+
+
+
+
+
+
+
+
+
+
+
+
+
+    
+
+
```

### Comparing `pandasklar-0.3.4/src/pandasklar/subsets.py` & `pandasklar-0.3.5/src/pandasklar/subsets.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/type_info.py` & `pandasklar-0.3.5/src/pandasklar/type_info.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.4/src/pandasklar/values_info.py` & `pandasklar-0.3.5/src/pandasklar/values_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-
+import warnings
 import numpy  as np
 import pandas as pd
 
 from pandas.api.types import is_string_dtype, is_numeric_dtype
 
 from .config       import Config
+from .type_info    import type_info
 
 
 
  
 
     
 #############################################################################################
@@ -114,19 +115,87 @@
                     i = type_info(versuch)            
                     if i.xmin <= self.vmin   and   i.xmax >= self.vmax:
                         self.datatype_suggest = versuch
                         break   
                                             
             # wieder löschen wenn schon erfüllt
             if self.datatype_suggest == self.type_info.name:
-                self.datatype_suggest = ''
+                self.datatype_suggest = ''                
         # Ende if (self.ntypes == 1)
-        
+
+        # datatype_identified
+        self.datatype_identified = identify_datatype(data) 
+        if self.datatype_identified == '' and self.datatype_suggest.endswith('string'):
+            self.datatype_identified = 'string'
+        if self.datatype_identified.startswith('float'):
+            self.datatype_identified = 'float'  
+        if self.datatype_identified.startswith('int'):
+            self.datatype_identified = 'int'                 
         
     def info(self):
         """Returns all attributes"""
         result = dict(self.__dict__) # Kopie ziehen
         #del result['data']
         return result    
-    
+
+
+
+def identify_datatype(series):
+    '''    
+    # Example usage
+    data = pd.Series([1, 2, '3', pd.Timestamp('2022-01-01'), 'text'])
+    data_type = identify_data_type(data)
+    print(data_type)
+    '''
+    result = type_info(series).name_short 
+    if result == 'object':
+        result = ''
+
+    filtered_series = series.dropna()
+    str_series = filtered_series.astype(str)
+
+    try:
+        # Try converting to float
+        float_series = pd.to_numeric(str_series, errors='raise').astype(float)
+        if (float_series == filtered_series).all():
+            result = 'float'
+    except:
+        pass
+        
+    try:
+        # Try converting to int
+        int_series = pd.to_numeric(str_series, errors='raise').astype(int)
+        diff_sum = (int_series - filtered_series).abs().sum()
+        if diff_sum < 0.00001:
+            result = 'int'    
+    except:
+        pass
+
+    try:
+        # Try converting to datetime
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore")
+            datetime_series = pd.to_datetime(str_series, errors='raise')
+        if (datetime_series == filtered_series).all():
+            result = 'datetime'
+    except:
+        pass
+
+    try:
+        # Count comma
+        if result in ['','string']:
+            kommas = str_series.str.count(',').sum()
+            alle = str_series.str.len().sum() 
+            duplicate_count = series.duplicated().sum()
+            total_count = len(series)
+            if kommas / alle > 0.05:
+                result = 'list'
+            if duplicate_count / total_count > 0.2   and kommas / alle > 0.02:
+                result = 'list'
+            if duplicate_count / total_count > 0.4   and kommas / alle > 0.01:
+                result = 'list'                
+    except:
+        pass        
+
+    return result
```

### Comparing `pandasklar-0.3.4/src/pandasklar.egg-info/PKG-INFO` & `pandasklar-0.3.5/src/pandasklar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.3.4
+Version: 0.3.5
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandasklar-0.3.4/src/pandasklar.egg-info/SOURCES.txt` & `pandasklar-0.3.5/src/pandasklar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

