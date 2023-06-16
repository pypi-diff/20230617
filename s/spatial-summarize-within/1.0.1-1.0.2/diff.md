# Comparing `tmp/spatial_summarize_within-1.0.1.tar.gz` & `tmp/spatial_summarize_within-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatial_summarize_within-1.0.1.tar", last modified: Mon Jun 12 00:20:38 2023, max compression
+gzip compressed data, was "spatial_summarize_within-1.0.2.tar", last modified: Fri Jun 16 23:36:36 2023, max compression
```

## Comparing `spatial_summarize_within-1.0.1.tar` & `spatial_summarize_within-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-06-12 00:20:38.048242 spatial_summarize_within-1.0.1/
--rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-1.0.1/LICENSE
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-06-12 00:20:38.048125 spatial_summarize_within-1.0.1/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)     6664 2023-05-28 20:50:21.000000 spatial_summarize_within-1.0.1/README.md
--rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-06-12 00:20:38.048288 spatial_summarize_within-1.0.1/setup.cfg
--rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-06-12 00:15:07.000000 spatial_summarize_within-1.0.1/setup.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-06-12 00:20:38.047412 spatial_summarize_within-1.0.1/spatial_summarize_within/
--rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-1.0.1/spatial_summarize_within/__init__.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2593 2023-06-12 00:12:28.000000 spatial_summarize_within-1.0.1/spatial_summarize_within/max_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2791 2023-06-12 00:12:28.000000 spatial_summarize_within-1.0.1/spatial_summarize_within/mean_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2594 2023-06-12 00:12:28.000000 spatial_summarize_within-1.0.1/spatial_summarize_within/min_within.py
--rw-r--r--   0 Kenne      (501) staff       (20)     2575 2023-06-12 00:08:32.000000 spatial_summarize_within-1.0.1/spatial_summarize_within/sum_within.py
-drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-06-12 00:20:38.047948 spatial_summarize_within-1.0.1/spatial_summarize_within.egg-info/
--rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-06-12 00:20:38.000000 spatial_summarize_within-1.0.1/spatial_summarize_within.egg-info/PKG-INFO
--rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-06-12 00:20:38.000000 spatial_summarize_within-1.0.1/spatial_summarize_within.egg-info/SOURCES.txt
--rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-06-12 00:20:38.000000 spatial_summarize_within-1.0.1/spatial_summarize_within.egg-info/dependency_links.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-06-12 00:20:38.000000 spatial_summarize_within-1.0.1/spatial_summarize_within.egg-info/requires.txt
--rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-06-12 00:20:38.000000 spatial_summarize_within-1.0.1/spatial_summarize_within.egg-info/top_level.txt
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-06-16 23:36:36.043167 spatial_summarize_within-1.0.2/
+-rw-r--r--   0 Kenne      (501) staff       (20)     1076 2023-05-06 22:57:53.000000 spatial_summarize_within-1.0.2/LICENSE
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-06-16 23:36:36.043056 spatial_summarize_within-1.0.2/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)     6664 2023-05-28 20:50:21.000000 spatial_summarize_within-1.0.2/README.md
+-rw-r--r--   0 Kenne      (501) staff       (20)       38 2023-06-16 23:36:36.043202 spatial_summarize_within-1.0.2/setup.cfg
+-rw-r--r--   0 Kenne      (501) staff       (20)      329 2023-06-16 23:29:51.000000 spatial_summarize_within-1.0.2/setup.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-06-16 23:36:36.042360 spatial_summarize_within-1.0.2/spatial_summarize_within/
+-rw-r--r--   0 Kenne      (501) staff       (20)      141 2023-05-12 03:23:32.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/__init__.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2348 2023-06-16 23:34:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/max_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2376 2023-06-16 23:34:08.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/mean_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2348 2023-06-16 23:35:44.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/min_within.py
+-rw-r--r--   0 Kenne      (501) staff       (20)     2335 2023-06-16 23:35:44.000000 spatial_summarize_within-1.0.2/spatial_summarize_within/sum_within.py
+drwxr-xr-x   0 Kenne      (501) staff       (20)        0 2023-06-16 23:36:36.042901 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/
+-rw-r--r--   0 Kenne      (501) staff       (20)       90 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/PKG-INFO
+-rw-r--r--   0 Kenne      (501) staff       (20)      459 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/SOURCES.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)        1 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/dependency_links.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       37 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/requires.txt
+-rw-r--r--   0 Kenne      (501) staff       (20)       25 2023-06-16 23:36:36.000000 spatial_summarize_within-1.0.2/spatial_summarize_within.egg-info/top_level.txt
```

### Comparing `spatial_summarize_within-1.0.1/LICENSE` & `spatial_summarize_within-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-1.0.1/README.md` & `spatial_summarize_within-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `spatial_summarize_within-1.0.1/spatial_summarize_within/max_within.py` & `spatial_summarize_within-1.0.2/spatial_summarize_within/min_within.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,46 +4,44 @@
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
 # Function
-def max_within(input_shapefile, input_summary_features, columns, key):
+def min_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
+    # Intersect the input geodataframe with the entire overlay shapefile
+    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection')
+    # Calculate the area of each polygon in intersect dataframe
+    intersected["intersect_area"] = intersected.area
+    # Calculate the percentage overlap of each polygon
+    intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
     # Loop through each polygon in the overlay geodataframe
-    for index, row in input_shapefile.iterrows():
-        # Create a temporary geodataframe with just the current overlay polygon
-        temp_overlay = gpd.GeoDataFrame([row], columns=input_shapefile.columns)
-        # Set the CRS of temp_overlay to match input_summary_features
-        temp_overlay.set_crs(input_summary_features.crs, inplace=True)
-        # Intersect the input geodataframe with the current overlay polygon
-        temp_intersect = gpd.overlay(input_summary_features, temp_overlay, how='intersection')
-        # Calculate the area of each polygon in intersect dataframe
-        temp_intersect["intersect_area"] = temp_intersect.area
-        # Calculate the percentage overlap of each polygon in the input geodataframe with the current overlay polygon
-        temp_intersect["overlap_pct"] = temp_intersect["intersect_area"] / temp_intersect["area"]
+    for polygon in input_shapefile.itertuples():
+        # Select intersected parts that belong to the current polygon
+        temp_intersect = intersected.loc[intersected[key] == getattr(polygon, key)]
         # Calculate the weighted value for each column
         for column in columns:
-            temp_intersect[column] = temp_intersect[column] * temp_intersect["overlap_pct"]
+            temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).min()
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
-        # Group the results and calculate the maximum of weighted values
-        temp_result = temp_intersect.groupby(key)[columns].max().reset_index()
+        # Group the results
+        temp_result = temp_intersect.groupby(key).min(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
-    result_gdf = input_shapefile.merge(result_gdf, on=key)
+    result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
 
-    # Remove the added area column from input geodataframe
+    # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
-    return result_gdf
+    return result_gdf
```

### Comparing `spatial_summarize_within-1.0.1/spatial_summarize_within/mean_within.py` & `spatial_summarize_within-1.0.2/spatial_summarize_within/mean_within.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,50 +4,44 @@
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
 # Function
-def mean_within(input_shapefile, input_summary_features, columns, key):
+def mean_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
+    # Intersect the input geodataframe with the entire overlay shapefile
+    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection')
+    # Calculate the area of each polygon in intersect dataframe
+    intersected["intersect_area"] = intersected.area
+    # Calculate the percentage overlap of each polygon
+    intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
     # Loop through each polygon in the overlay geodataframe
-    for index, row in input_shapefile.iterrows():
-        # Create a temporary geodataframe with just the current overlay polygon
-        temp_overlay = gpd.GeoDataFrame([row], columns=input_shapefile.columns)
-        # Set the CRS of temp_overlay to match input_summary_features
-        temp_overlay.set_crs(input_summary_features.crs, inplace=True)
-        # Intersect the input geodataframe with the current overlay polygon
-        temp_intersect = gpd.overlay(input_summary_features, temp_overlay, how='intersection')
-        # Calculate the area of each polygon in intersect dataframe
-        temp_intersect["intersect_area"] = temp_intersect.area
-        # Calculate the percentage overlap of each polygon in the input geodataframe with the current overlay polygon
-        temp_intersect["overlap_pct"] = temp_intersect["intersect_area"] / temp_intersect["area"]
+    for polygon in input_shapefile.itertuples():
+        # Select intersected parts that belong to the current polygon
+        temp_intersect = intersected.loc[intersected[key] == getattr(polygon, key)]
         # Calculate the weighted mean
-        columns = columns
         for column in columns:
-            temp_intersect[column] = temp_intersect[column] * temp_intersect["intersect_area"]
+            temp_intersect[column] = (temp_intersect[column] * temp_intersect["intersect_area"]).sum() / temp_intersect["intersect_area"].sum()
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
-        # Group the results by key and calculate the sum of each group
-        temp_sum = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
-        # Calculate the mean by dividing the sum by the total intersect area
-        for column in columns:
-            temp_sum[column] = temp_sum[column] / temp_sum['intersect_area']
+        # Group the results
+        temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
         # Append the results to the result gdf
-        result_gdf = pd.concat([result_gdf, temp_sum], ignore_index=True)
+        result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
-    result_gdf = input_shapefile.merge(result_gdf, on=key)
+    result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
 
-    # Remove the added area column from input geodataframe
+    # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
-    return result_gdf
+    return result_gdf
```

### Comparing `spatial_summarize_within-1.0.1/spatial_summarize_within/min_within.py` & `spatial_summarize_within-1.0.2/spatial_summarize_within/sum_within.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,47 +3,44 @@
 import shapely
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
-# Function
-def min_within(input_shapefile, input_summary_features, columns, key):
+# function
+def sum_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
+    # Intersect the input geodataframe with the entire overlay shapefile
+    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection')
+    # Calculate the area of each polygon in intersect dataframe
+    intersected["intersect_area"] = intersected.area
+    # Calculate the percentage overlap of each polygon
+    intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
     # Loop through each polygon in the overlay geodataframe
-    for index, row in input_shapefile.iterrows():
-        # Create a temporary geodataframe with just the current overlay polygon
-        temp_overlay = gpd.GeoDataFrame([row], columns=input_shapefile.columns)
-        # Set the CRS of temp_overlay to match input_summary_features
-        temp_overlay.set_crs(input_summary_features.crs, inplace=True)
-        # Intersect the input geodataframe with the current overlay polygon
-        temp_intersect = gpd.overlay(input_summary_features, temp_overlay, how='intersection')
-        # Calculate the area of each polygon in intersect dataframe
-        temp_intersect["intersect_area"] = temp_intersect.area
-        # Calculate the percentage overlap of each polygon in the input geodataframe with the current overlay polygon
-        temp_intersect["overlap_pct"] = temp_intersect["intersect_area"] / temp_intersect["area"]
-        # Calculate the weighted value for each column
+    for polygon in input_shapefile.itertuples():
+        # Select intersected parts that belong to current polygon
+        temp_intersect = intersected.loc[intersected[key] == getattr(polygon, key)]
+        # Calculate the weighted sum
         for column in columns:
-            temp_intersect[column] = temp_intersect[column] * temp_intersect["overlap_pct"]
+            temp_intersect.loc[:, column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
-        # Group the results and calculate the minimum of weighted values
-        temp_result = temp_intersect.groupby(key)[columns].min().reset_index()
+        # Group the results
+        temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
-    result_gdf = input_shapefile.merge(result_gdf, on=key)
-
-    # Remove the added area column from input geodataframe
+    result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
+    # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
     return result_gdf
```

### Comparing `spatial_summarize_within-1.0.1/spatial_summarize_within/sum_within.py` & `spatial_summarize_within-1.0.2/spatial_summarize_within/max_within.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,48 +3,45 @@
 import shapely
 from shapely import wkt
 import shapely.ops
 from shapely.geometry import Polygon, MultiPolygon, shape, Point
 import geopandas as gpd
 import mapclassify
 
-# function
-def sum_within(input_shapefile, input_summary_features, columns, key):
+# Function
+def max_within(input_shapefile, input_summary_features, columns, key, join_type='inner'):
     # Check if key exists in both dataframes
     if key in input_shapefile.columns and key in input_summary_features.columns:
         # Append suffix to key in input_summary_features
         input_summary_features = input_summary_features.rename(columns={key: key+"_summary"})
     # Add area column to input geodataframe
     input_summary_features["area"] = input_summary_features.geometry.area
+    # Intersect the input geodataframe with the entire overlay shapefile
+    intersected = gpd.overlay(input_summary_features, input_shapefile, how='intersection')
+    # Calculate the area of each polygon in intersect dataframe
+    intersected["intersect_area"] = intersected.area
+    # Calculate the percentage overlap of each polygon
+    intersected["overlap_pct"] = intersected["intersect_area"] / intersected["area"]
     # Create an empty geodataframe to store the results
     result_gdf = gpd.GeoDataFrame()
 
     # Loop through each polygon in the overlay geodataframe
-    for index, row in input_shapefile.iterrows():
-        # Create a temporary geodataframe with just the current overlay polygon
-        temp_overlay = gpd.GeoDataFrame([row], columns=input_shapefile.columns)
-        # Set the CRS of temp_overlay to match input_summary_features
-        temp_overlay.set_crs(input_summary_features.crs, inplace=True)
-        # Intersect the input geodataframe with the current overlay polygon
-        temp_intersect = gpd.overlay(input_summary_features, temp_overlay, how='intersection')
-        # Calculate the area of each polygon in intersect dataframe
-        temp_intersect["intersect_area"] = temp_intersect.area
-        # Calculate the percentage overlap of each polygon in the input geodataframe with the current overlay polygon
-        temp_intersect["overlap_pct"] = temp_intersect["intersect_area"] / temp_intersect["area"]
-        # Calculate the weighted sum
-        columns = columns
+    for polygon in input_shapefile.itertuples():
+        # Select intersected parts that belong to the current polygon
+        temp_intersect = intersected.loc[intersected[key] == getattr(polygon, key)]
+        # Calculate the weighted value for each column
         for column in columns:
-            temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).round(0)
+            temp_intersect[column] = (temp_intersect[column] * temp_intersect["overlap_pct"]).max()
         # Keep only the relevant columns in the temp_intersect dataframe
         temp_intersect = temp_intersect[[key] + columns + ['intersect_area', 'overlap_pct']]
         # Group the results
-        temp_result = temp_intersect.groupby(key).sum(numeric_only=True).reset_index()
+        temp_result = temp_intersect.groupby(key).max(numeric_only=True).reset_index()
         # Append the results to the result gdf
         result_gdf = pd.concat([result_gdf, temp_result], ignore_index=True)
 
     # Merge the result with the overlay geodataframe
-    result_gdf = input_shapefile.merge(result_gdf, on=key)
+    result_gdf = input_shapefile.merge(result_gdf, on=key, how=join_type)
 
-    # Remove the added area column from input geodataframe
+    # Remove the area column from input geodataframe
     input_summary_features = input_summary_features.drop("area", axis=1)
 
-    return result_gdf
+    return result_gdf
```

