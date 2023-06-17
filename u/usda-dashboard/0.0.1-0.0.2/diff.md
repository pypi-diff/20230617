# Comparing `tmp/usda_dashboard-0.0.1.tar.gz` & `tmp/usda_dashboard-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usda_dashboard-0.0.1.tar", last modified: Sat Jun 17 01:17:09 2023, max compression
+gzip compressed data, was "usda_dashboard-0.0.2.tar", last modified: Sat Jun 17 01:50:30 2023, max compression
```

## Comparing `usda_dashboard-0.0.1.tar` & `usda_dashboard-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-17 01:17:09.754948 usda_dashboard-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-05-28 12:37:09.000000 usda_dashboard-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      225 2023-06-17 01:17:09.754948 usda_dashboard-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-05-28 12:37:09.000000 usda_dashboard-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-17 01:17:09.754948 usda_dashboard-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-17 01:15:09.000000 usda_dashboard-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-17 01:17:09.671270 usda_dashboard-0.0.1/usda_dashboard/
--rw-rw-rw-   0        0        0      354 2023-06-17 01:08:53.000000 usda_dashboard-0.0.1/usda_dashboard/__init__.py
--rw-rw-rw-   0        0        0    14642 2023-06-17 00:59:25.000000 usda_dashboard-0.0.1/usda_dashboard/_dash_USDA_dataIndex.py
--rw-rw-rw-   0        0        0      664 2023-06-16 23:36:44.000000 usda_dashboard-0.0.1/usda_dashboard/_dash_USDA_dataIndex_run.py
--rw-rw-rw-   0        0        0     7728 2023-06-17 01:11:20.000000 usda_dashboard-0.0.1/usda_dashboard/_dash_fossil_CO2_emissions_2022.py
--rw-rw-rw-   0        0        0      697 2023-06-17 01:09:56.000000 usda_dashboard-0.0.1/usda_dashboard/_dash_fossil_CO2_emissions_2022_run.py
--rw-rw-rw-   0        0        0     3992 2023-02-24 02:02:45.000000 usda_dashboard-0.0.1/usda_dashboard/_gadgets.py
-drwxrwxrwx   0        0        0        0 2023-06-17 01:17:09.702521 usda_dashboard-0.0.1/usda_dashboard/data/
--rw-rw-rw-   0        0        0  1151590 2023-05-27 13:42:46.000000 usda_dashboard-0.0.1/usda_dashboard/data/EDGARv7.0_FT2021_fossil_CO2_booklet_2022.xlsx
--rw-rw-rw-   0        0        0  7864320 2023-06-16 15:28:02.000000 usda_dashboard-0.0.1/usda_dashboard/data/USDA_dataIndex.accdb
--rw-rw-rw-   0        0        0  1757184 2023-06-12 15:23:35.000000 usda_dashboard-0.0.1/usda_dashboard/data/USDA_dataIndex_Backup.accdb
--rw-rw-rw-   0        0        0      125 2023-06-17 00:57:48.000000 usda_dashboard-0.0.1/usda_dashboard/data/__init__.py
--rw-rw-rw-   0        0        0 24090863 2023-05-29 06:44:21.000000 usda_dashboard-0.0.1/usda_dashboard/data/countries.geojson
-drwxrwxrwx   0        0        0        0 2023-06-17 01:17:09.686896 usda_dashboard-0.0.1/usda_dashboard.egg-info/
--rw-rw-rw-   0        0        0      225 2023-06-17 01:17:09.000000 usda_dashboard-0.0.1/usda_dashboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      643 2023-06-17 01:17:09.000000 usda_dashboard-0.0.1/usda_dashboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-17 01:17:09.000000 usda_dashboard-0.0.1/usda_dashboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-17 01:17:09.000000 usda_dashboard-0.0.1/usda_dashboard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-17 01:50:30.871736 usda_dashboard-0.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-05-28 12:37:09.000000 usda_dashboard-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      225 2023-06-17 01:50:30.871736 usda_dashboard-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-05-28 12:37:09.000000 usda_dashboard-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-17 01:50:30.871736 usda_dashboard-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      941 2023-06-17 01:48:04.000000 usda_dashboard-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-17 01:50:30.777455 usda_dashboard-0.0.2/usda_dashboard/
+-rw-rw-rw-   0        0        0      354 2023-06-17 01:50:10.000000 usda_dashboard-0.0.2/usda_dashboard/__init__.py
+-rw-rw-rw-   0        0        0    14642 2023-06-17 00:59:25.000000 usda_dashboard-0.0.2/usda_dashboard/_dash_USDA_dataIndex.py
+-rw-rw-rw-   0        0        0      664 2023-06-16 23:36:44.000000 usda_dashboard-0.0.2/usda_dashboard/_dash_USDA_dataIndex_run.py
+-rw-rw-rw-   0        0        0     7728 2023-06-17 01:11:20.000000 usda_dashboard-0.0.2/usda_dashboard/_dash_fossil_CO2_emissions_2022.py
+-rw-rw-rw-   0        0        0      697 2023-06-17 01:09:56.000000 usda_dashboard-0.0.2/usda_dashboard/_dash_fossil_CO2_emissions_2022_run.py
+-rw-rw-rw-   0        0        0     3992 2023-02-24 02:02:45.000000 usda_dashboard-0.0.2/usda_dashboard/_gadgets.py
+drwxrwxrwx   0        0        0        0 2023-06-17 01:50:30.824382 usda_dashboard-0.0.2/usda_dashboard/data/
+-rw-rw-rw-   0        0        0  1151590 2023-05-27 13:42:46.000000 usda_dashboard-0.0.2/usda_dashboard/data/EDGARv7.0_FT2021_fossil_CO2_booklet_2022.xlsx
+-rw-rw-rw-   0        0        0  7864320 2023-06-16 15:28:02.000000 usda_dashboard-0.0.2/usda_dashboard/data/USDA_dataIndex.accdb
+-rw-rw-rw-   0        0        0  1757184 2023-06-12 15:23:35.000000 usda_dashboard-0.0.2/usda_dashboard/data/USDA_dataIndex_Backup.accdb
+-rw-rw-rw-   0        0        0      125 2023-06-17 00:57:48.000000 usda_dashboard-0.0.2/usda_dashboard/data/__init__.py
+-rw-rw-rw-   0        0        0 24090863 2023-05-29 06:44:21.000000 usda_dashboard-0.0.2/usda_dashboard/data/countries.geojson
+drwxrwxrwx   0        0        0        0 2023-06-17 01:50:30.793096 usda_dashboard-0.0.2/usda_dashboard.egg-info/
+-rw-rw-rw-   0        0        0      225 2023-06-17 01:50:30.000000 usda_dashboard-0.0.2/usda_dashboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      680 2023-06-17 01:50:30.000000 usda_dashboard-0.0.2/usda_dashboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-17 01:50:30.000000 usda_dashboard-0.0.2/usda_dashboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-17 01:50:30.000000 usda_dashboard-0.0.2/usda_dashboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-17 01:50:30.000000 usda_dashboard-0.0.2/usda_dashboard.egg-info/top_level.txt
```

### Comparing `usda_dashboard-0.0.1/LICENSE` & `usda_dashboard-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard/_dash_USDA_dataIndex.py` & `usda_dashboard-0.0.2/usda_dashboard/_dash_USDA_dataIndex.py`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard/_dash_USDA_dataIndex_run.py` & `usda_dashboard-0.0.2/usda_dashboard/_dash_USDA_dataIndex_run.py`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard/_dash_fossil_CO2_emissions_2022.py` & `usda_dashboard-0.0.2/usda_dashboard/_dash_fossil_CO2_emissions_2022.py`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard/_dash_fossil_CO2_emissions_2022_run.py` & `usda_dashboard-0.0.2/usda_dashboard/_dash_fossil_CO2_emissions_2022_run.py`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard/_gadgets.py` & `usda_dashboard-0.0.2/usda_dashboard/_gadgets.py`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard/data/EDGARv7.0_FT2021_fossil_CO2_booklet_2022.xlsx` & `usda_dashboard-0.0.2/usda_dashboard/data/EDGARv7.0_FT2021_fossil_CO2_booklet_2022.xlsx`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard/data/USDA_dataIndex.accdb` & `usda_dashboard-0.0.2/usda_dashboard/data/USDA_dataIndex.accdb`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard/data/USDA_dataIndex_Backup.accdb` & `usda_dashboard-0.0.2/usda_dashboard/data/USDA_dataIndex_Backup.accdb`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard/data/countries.geojson` & `usda_dashboard-0.0.2/usda_dashboard/data/countries.geojson`

 * *Files identical despite different names*

### Comparing `usda_dashboard-0.0.1/usda_dashboard.egg-info/SOURCES.txt` & `usda_dashboard-0.0.2/usda_dashboard.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,13 +6,14 @@
 usda_dashboard/_dash_USDA_dataIndex_run.py
 usda_dashboard/_dash_fossil_CO2_emissions_2022.py
 usda_dashboard/_dash_fossil_CO2_emissions_2022_run.py
 usda_dashboard/_gadgets.py
 usda_dashboard.egg-info/PKG-INFO
 usda_dashboard.egg-info/SOURCES.txt
 usda_dashboard.egg-info/dependency_links.txt
+usda_dashboard.egg-info/requires.txt
 usda_dashboard.egg-info/top_level.txt
 usda_dashboard/data/EDGARv7.0_FT2021_fossil_CO2_booklet_2022.xlsx
 usda_dashboard/data/USDA_dataIndex.accdb
 usda_dashboard/data/USDA_dataIndex_Backup.accdb
 usda_dashboard/data/__init__.py
 usda_dashboard/data/countries.geojson
```

