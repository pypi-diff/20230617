# Comparing `tmp/artd-location-0.0.1.tar.gz` & `tmp/artd-location-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-location-0.0.1.tar", last modified: Fri Jun 16 02:56:09 2023, max compression
+gzip compressed data, was "artd-location-0.0.2.tar", last modified: Sat Jun 17 15:56:05 2023, max compression
```

## Comparing `artd-location-0.0.1.tar` & `artd-location-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:09.935336 artd-location-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-16 02:56:05.000000 artd-location-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 02:56:05.000000 artd-location-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-16 02:56:09.935336 artd-location-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-16 02:56:05.000000 artd-location-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:09.935336 artd-location-0.0.1/artd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:09.935336 artd-location-0.0.1/artd_location/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:09.935336 artd-location-0.0.1/artd_location/data/
--rw-r--r--   0 runner    (1001) docker     (123)   108426 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/data/cities.py
--rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/data/countries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/data/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:09.935336 artd-location-0.0.1/artd_location/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/generators/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:09.931336 artd-location-0.0.1/artd_location/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:09.935336 artd-location-0.0.1/artd_location/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/management/commands/create_colombian_cities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/management/commands/create_colombian_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/management/commands/create_countries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:09.935336 artd-location-0.0.1/artd_location/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-16 02:56:05.000000 artd-location-0.0.1/artd_location/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 02:56:09.935336 artd-location-0.0.1/artd_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-16 02:56:09.000000 artd-location-0.0.1/artd_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-16 02:56:09.000000 artd-location-0.0.1/artd_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 02:56:09.000000 artd-location-0.0.1/artd_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-16 02:56:09.000000 artd-location-0.0.1/artd_location.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 02:56:09.935336 artd-location-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-16 02:56:07.000000 artd-location-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:56:05.591457 artd-location-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 15:55:58.000000 artd-location-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-17 15:55:58.000000 artd-location-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-17 15:56:05.591457 artd-location-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-17 15:55:58.000000 artd-location-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:56:05.591457 artd-location-0.0.2/artd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:56:05.591457 artd-location-0.0.2/artd_location/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:56:05.591457 artd-location-0.0.2/artd_location/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   108426 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/data/cities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33716 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/data/countries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/data/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:56:05.591457 artd-location-0.0.2/artd_location/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/generators/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:56:05.587457 artd-location-0.0.2/artd_location/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:56:05.591457 artd-location-0.0.2/artd_location/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/management/commands/create_colombian_cities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/management/commands/create_colombian_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/management/commands/create_countries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:56:05.591457 artd-location-0.0.2/artd_location/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 15:55:58.000000 artd-location-0.0.2/artd_location/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:56:05.591457 artd-location-0.0.2/artd_location.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-17 15:56:05.000000 artd-location-0.0.2/artd_location.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-17 15:56:05.000000 artd-location-0.0.2/artd_location.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:56:05.000000 artd-location-0.0.2/artd_location.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 15:56:05.000000 artd-location-0.0.2/artd_location.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:56:05.591457 artd-location-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-17 15:56:03.000000 artd-location-0.0.2/setup.py
```

### Comparing `artd-location-0.0.1/LICENSE` & `artd-location-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/PKG-INFO` & `artd-location-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-location
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to administrate location
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `artd-location-0.0.1/README.rst` & `artd-location-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd/settings.py` & `artd-location-0.0.2/artd/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 For more information on this file, see
 https://docs.djangoproject.com/en/4.2/topics/settings/
 
 For the full list of settings and their values, see
 https://docs.djangoproject.com/en/4.2/ref/settings/
 """
-
+import os
 from pathlib import Path
 
 # Build paths inside the project like this: BASE_DIR / 'subdir'.
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 
 # Quick-start development settings - unsuitable for production
@@ -100,15 +100,15 @@
     },
 ]
 
 
 # Internationalization
 # https://docs.djangoproject.com/en/4.2/topics/i18n/
 
-LANGUAGE_CODE = "en-us"
+LANGUAGE_CODE = "en"
 
 TIME_ZONE = "UTC"
 
 USE_I18N = True
 
 USE_TZ = True
 
@@ -118,7 +118,9 @@
 
 STATIC_URL = "static/"
 
 # Default primary key field type
 # https://docs.djangoproject.com/en/4.2/ref/settings/#default-auto-field
 
 DEFAULT_AUTO_FIELD = "django.db.models.BigAutoField"
+
+LOCALE_PATHS = [os.path.join(BASE_DIR, "locale")]
```

### Comparing `artd-location-0.0.1/artd/urls.py` & `artd-location-0.0.2/artd/urls.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/admin.py` & `artd-location-0.0.2/artd_location/admin.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/data/cities.py` & `artd-location-0.0.2/artd_location/data/cities.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/data/countries.py` & `artd-location-0.0.2/artd_location/data/countries.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/data/regions.py` & `artd-location-0.0.2/artd_location/data/regions.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/generators/generators.py` & `artd-location-0.0.2/artd_location/generators/generators.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/management/commands/create_colombian_cities.py` & `artd-location-0.0.2/artd_location/management/commands/create_colombian_cities.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/management/commands/create_colombian_regions.py` & `artd-location-0.0.2/artd_location/management/commands/create_colombian_regions.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/management/commands/create_countries.py` & `artd-location-0.0.2/artd_location/management/commands/create_countries.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/migrations/0001_initial.py` & `artd-location-0.0.2/artd_location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/models.py` & `artd-location-0.0.2/artd_location/models.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location/tests.py` & `artd-location-0.0.2/artd_location/tests.py`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/artd_location.egg-info/PKG-INFO` & `artd-location-0.0.2/artd_location.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-location
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to administrate location
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `artd-location-0.0.1/artd_location.egg-info/SOURCES.txt` & `artd-location-0.0.2/artd_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd-location-0.0.1/setup.py` & `artd-location-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="artd-location",
-    version="0.0.1",
+    version="0.0.2",
     include_package_data=True,
     author="Jonathan Urzola Maladonado",
     author_email="jonathan@artd.com.co",
     description="A Django app to administrate location",
     long_description_content_type="text/markdown",
     url="https://www.artd.com.co/",
     long_description=long_description,
```

