# Comparing `tmp/netbox_sb_dc_accessdata-1.0.tar.gz` & `tmp/netbox_sb_dc_accessdata-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_sb_dc_accessdata-1.0.tar", last modified: Sat Jun 17 01:21:39 2023, max compression
+gzip compressed data, was "netbox_sb_dc_accessdata-1.1.tar", last modified: Sat Jun 17 01:47:46 2023, max compression
```

## Comparing `netbox_sb_dc_accessdata-1.0.tar` & `netbox_sb_dc_accessdata-1.1.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:39.689081 netbox_sb_dc_accessdata-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-17 01:21:39.689081 netbox_sb_dc_accessdata-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:39.689081 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:39.689081 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:39.689081 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:21:39.689081 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-17 01:21:39.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-17 01:21:39.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:21:39.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:21:39.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-17 01:21:39.000000 netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:21:39.689081 netbox_sb_dc_accessdata-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 01:21:30.000000 netbox_sb_dc_accessdata-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:47:46.328915 netbox_sb_dc_accessdata-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-17 01:47:46.328915 netbox_sb_dc_accessdata-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:47:46.328915 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:47:46.328915 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:47:46.328915 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:47:46.324915 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:47:46.328915 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/templates/netbox_sb_dc_accessdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/templates/netbox_sb_dc_accessdata/key.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/templates/netbox_sb_dc_accessdata/keycard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:47:46.328915 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-17 01:47:46.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-17 01:47:46.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:47:46.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:47:46.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-17 01:47:46.000000 netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:47:46.328915 netbox_sb_dc_accessdata-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-17 01:47:34.000000 netbox_sb_dc_accessdata-1.1/setup.py
```

### Comparing `netbox_sb_dc_accessdata-1.0/LICENSE` & `netbox_sb_dc_accessdata-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/api/serializers.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/api/views.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/forms.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/graphql.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/migrations/0001_initial.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/models.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/models.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/navigation.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/tables.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/urls.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata/views.py` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata/views.py`

 * *Files identical despite different names*

### Comparing `netbox_sb_dc_accessdata-1.0/netbox_sb_dc_accessdata.egg-info/SOURCES.txt` & `netbox_sb_dc_accessdata-1.1/netbox_sb_dc_accessdata.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 setup.py
 netbox_sb_dc_accessdata/__init__.py
 netbox_sb_dc_accessdata/filtersets.py
 netbox_sb_dc_accessdata/forms.py
 netbox_sb_dc_accessdata/graphql.py
 netbox_sb_dc_accessdata/models.py
@@ -16,8 +17,10 @@
 netbox_sb_dc_accessdata.egg-info/not-zip-safe
 netbox_sb_dc_accessdata.egg-info/top_level.txt
 netbox_sb_dc_accessdata/api/__init__.py
 netbox_sb_dc_accessdata/api/serializers.py
 netbox_sb_dc_accessdata/api/urls.py
 netbox_sb_dc_accessdata/api/views.py
 netbox_sb_dc_accessdata/migrations/0001_initial.py
-netbox_sb_dc_accessdata/migrations/__init__.py
+netbox_sb_dc_accessdata/migrations/__init__.py
+netbox_sb_dc_accessdata/templates/netbox_sb_dc_accessdata/key.html
+netbox_sb_dc_accessdata/templates/netbox_sb_dc_accessdata/keycard.html
```

### Comparing `netbox_sb_dc_accessdata-1.0/setup.py` & `netbox_sb_dc_accessdata-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='netbox_sb_dc_accessdata',
-    version='1.0',
+    version='1.1',
     description='SB DC Accessdata',
     long_description='Speedbone Datacenter Accessdata integration for netbox via plugin',
     install_requires=[],
     packages=find_packages(),
     include_package_data=True,
     zip_safe=False,
     author='Marco Krajniak',
```

