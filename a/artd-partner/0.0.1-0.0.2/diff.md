# Comparing `tmp/artd-partner-0.0.1.tar.gz` & `tmp/artd-partner-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-partner-0.0.1.tar", last modified: Sat Jun 17 01:03:49 2023, max compression
+gzip compressed data, was "artd-partner-0.0.2.tar", last modified: Sat Jun 17 14:21:28 2023, max compression
```

## Comparing `artd-partner-0.0.1.tar` & `artd-partner-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:49.149326 artd-partner-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 01:03:40.000000 artd-partner-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-17 01:03:40.000000 artd-partner-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-17 01:03:49.149326 artd-partner-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-17 01:03:40.000000 artd-partner-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:49.145326 artd-partner-0.0.1/artd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:49.145326 artd-partner-0.0.1/artd_partner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:49.149326 artd-partner-0.0.1/artd_partner/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/__pycache__/admin.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/__pycache__/apps.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/__pycache__/models.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/__pycache__/tests.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:49.149326 artd-partner-0.0.1/artd_partner/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:49.149326 artd-partner-0.0.1/artd_partner/migrations/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:49.149326 artd-partner-0.0.1/artd_partner/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:49.149326 artd-partner-0.0.1/artd_partner/utils/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/utils/__pycache__/generators.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/utils/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 01:03:40.000000 artd-partner-0.0.1/artd_partner/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 01:03:49.149326 artd-partner-0.0.1/artd_partner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-17 01:03:49.000000 artd-partner-0.0.1/artd_partner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-17 01:03:49.000000 artd-partner-0.0.1/artd_partner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 01:03:49.000000 artd-partner-0.0.1/artd_partner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 01:03:49.000000 artd-partner-0.0.1/artd_partner.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 01:03:49.149326 artd-partner-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-17 01:03:46.000000 artd-partner-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:28.743434 artd-partner-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 14:21:22.000000 artd-partner-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-17 14:21:22.000000 artd-partner-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-17 14:21:28.743434 artd-partner-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-17 14:21:22.000000 artd-partner-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:28.739434 artd-partner-0.0.2/artd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:28.739434 artd-partner-0.0.2/artd_partner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:28.739434 artd-partner-0.0.2/artd_partner/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/__pycache__/admin.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/__pycache__/apps.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/__pycache__/models.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/__pycache__/tests.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:28.743434 artd-partner-0.0.2/artd_partner/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:28.743434 artd-partner-0.0.2/artd_partner/migrations/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:28.743434 artd-partner-0.0.2/artd_partner/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:28.743434 artd-partner-0.0.2/artd_partner/utils/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/utils/__pycache__/generators.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/utils/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 14:21:22.000000 artd-partner-0.0.2/artd_partner/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:21:28.739434 artd-partner-0.0.2/artd_partner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-17 14:21:28.000000 artd-partner-0.0.2/artd_partner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-17 14:21:28.000000 artd-partner-0.0.2/artd_partner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:21:28.000000 artd-partner-0.0.2/artd_partner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 14:21:28.000000 artd-partner-0.0.2/artd_partner.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:21:28.743434 artd-partner-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-17 14:21:27.000000 artd-partner-0.0.2/setup.py
```

### Comparing `artd-partner-0.0.1/LICENSE` & `artd-partner-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/PKG-INFO` & `artd-partner-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-partner
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to administrate partner
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -32,27 +32,19 @@
 Quick start
 -----------
 1. Install artd_location and add to your INSTALLED_APPS like this:
     
         INSTALLED_APPS = [
             ...
             'artd_location',
+            'artd_partner',
         ]
 
-2. Run ``python manage.py migrate`` to create the cities models.
+2. Run ``python manage.py migrate`` to create the models.
 
 3. run ``python manage.py create_countries`` to create the countries.
 
 4. run ``python manage.py create_regions`` to create the regions.
 
 5. run ``python manage.py create_cities`` to create the cities.
 
-6. Add "artd_partner" to your INSTALLED_APPS setting like this:
-    
-        INSTALLED_APPS = [
-            ...
-            'artd_partner',
-        ]
-
-7. Run ``python manage.py migrate`` to create the Partner models.
-
-3. Start the development server and visit http://127.0.0.1:8000/admin/
+6. Start the development server and visit http://127.0.0.1:8000/admin/
```

### Comparing `artd-partner-0.0.1/README.rst` & `artd-partner-0.0.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -8,27 +8,19 @@
 Quick start
 -----------
 1. Install artd_location and add to your INSTALLED_APPS like this:
     
         INSTALLED_APPS = [
             ...
             'artd_location',
+            'artd_partner',
         ]
 
-2. Run ``python manage.py migrate`` to create the cities models.
+2. Run ``python manage.py migrate`` to create the models.
 
 3. run ``python manage.py create_countries`` to create the countries.
 
 4. run ``python manage.py create_regions`` to create the regions.
 
 5. run ``python manage.py create_cities`` to create the cities.
 
-6. Add "artd_partner" to your INSTALLED_APPS setting like this:
-    
-        INSTALLED_APPS = [
-            ...
-            'artd_partner',
-        ]
-
-7. Run ``python manage.py migrate`` to create the Partner models.
-
-3. Start the development server and visit http://127.0.0.1:8000/admin/
+6. Start the development server and visit http://127.0.0.1:8000/admin/
```

### Comparing `artd-partner-0.0.1/artd/settings.py` & `artd-partner-0.0.2/artd/settings.py`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd/urls.py` & `artd-partner-0.0.2/artd/urls.py`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/__pycache__/admin.cpython-310.pyc` & `artd-partner-0.0.2/artd_partner/__pycache__/admin.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/__pycache__/apps.cpython-310.pyc` & `artd-partner-0.0.2/artd_partner/__pycache__/apps.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/__pycache__/models.cpython-310.pyc` & `artd-partner-0.0.2/artd_partner/__pycache__/models.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/__pycache__/tests.cpython-310.pyc` & `artd-partner-0.0.2/artd_partner/__pycache__/tests.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/admin.py` & `artd-partner-0.0.2/artd_partner/admin.py`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/migrations/0001_initial.py` & `artd-partner-0.0.2/artd_partner/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/migrations/__pycache__/0001_initial.cpython-310.pyc` & `artd-partner-0.0.2/artd_partner/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/models.py` & `artd-partner-0.0.2/artd_partner/models.py`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/tests.py` & `artd-partner-0.0.2/artd_partner/tests.py`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/utils/__pycache__/generators.cpython-310.pyc` & `artd-partner-0.0.2/artd_partner/utils/__pycache__/generators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner/utils/generators.py` & `artd-partner-0.0.2/artd_partner/utils/generators.py`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/artd_partner.egg-info/PKG-INFO` & `artd-partner-0.0.2/artd_partner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-partner
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Django app to administrate partner
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -32,27 +32,19 @@
 Quick start
 -----------
 1. Install artd_location and add to your INSTALLED_APPS like this:
     
         INSTALLED_APPS = [
             ...
             'artd_location',
+            'artd_partner',
         ]
 
-2. Run ``python manage.py migrate`` to create the cities models.
+2. Run ``python manage.py migrate`` to create the models.
 
 3. run ``python manage.py create_countries`` to create the countries.
 
 4. run ``python manage.py create_regions`` to create the regions.
 
 5. run ``python manage.py create_cities`` to create the cities.
 
-6. Add "artd_partner" to your INSTALLED_APPS setting like this:
-    
-        INSTALLED_APPS = [
-            ...
-            'artd_partner',
-        ]
-
-7. Run ``python manage.py migrate`` to create the Partner models.
-
-3. Start the development server and visit http://127.0.0.1:8000/admin/
+6. Start the development server and visit http://127.0.0.1:8000/admin/
```

### Comparing `artd-partner-0.0.1/artd_partner.egg-info/SOURCES.txt` & `artd-partner-0.0.2/artd_partner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd-partner-0.0.1/setup.py` & `artd-partner-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="artd-partner",
-    version="0.0.1",
+    version="0.0.2",
     include_package_data=True,
     author="Jonathan Urzola Maladonado",
     author_email="jonathan@artd.com.co",
     description="A Django app to administrate partner",
     long_description_content_type="text/markdown",
     url="https://www.artd.com.co/",
     long_description=long_description,
```

