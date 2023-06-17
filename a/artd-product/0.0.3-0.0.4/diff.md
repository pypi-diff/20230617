# Comparing `tmp/artd-product-0.0.3.tar.gz` & `tmp/artd-product-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-product-0.0.3.tar", last modified: Thu Jun 15 13:32:51 2023, max compression
+gzip compressed data, was "artd-product-0.0.4.tar", last modified: Sat Jun 17 15:37:39 2023, max compression
```

## Comparing `artd-product-0.0.3.tar` & `artd-product-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-15 13:32:47.000000 artd-product-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 13:32:47.000000 artd-product-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-15 13:32:51.366399 artd-product-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-15 13:32:47.000000 artd-product-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.362399 artd-product-0.0.3/artd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product/data/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/data/taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.362399 artd-product-0.0.3/artd_product/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/management/commands/create_taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/migrations/0002_alter_product_special_price_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-15 13:32:47.000000 artd-product-0.0.3/artd_product/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 13:32:51.366399 artd-product-0.0.3/artd_product.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-15 13:32:51.000000 artd-product-0.0.3/artd_product.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-15 13:32:51.000000 artd-product-0.0.3/artd_product.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 13:32:51.000000 artd-product-0.0.3/artd_product.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 13:32:51.000000 artd-product-0.0.3/artd_product.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 13:32:51.366399 artd-product-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-15 13:32:49.000000 artd-product-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.440183 artd-product-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 15:37:35.000000 artd-product-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 15:37:35.000000 artd-product-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-17 15:37:39.436183 artd-product-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-17 15:37:35.000000 artd-product-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/data/taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/management/commands/create_taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/migrations/0002_alter_product_special_price_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-17 15:37:39.000000 artd-product-0.0.4/artd_product.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-17 15:37:39.000000 artd-product-0.0.4/artd_product.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:37:39.000000 artd-product-0.0.4/artd_product.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 15:37:39.000000 artd-product-0.0.4/artd_product.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:37:39.440183 artd-product-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 15:37:37.000000 artd-product-0.0.4/setup.py
```

### Comparing `artd-product-0.0.3/LICENSE` & `artd-product-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.3/PKG-INFO` & `artd-product-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-product
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Django app to administrate products
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -35,12 +35,12 @@
 1. Add "artd_product" to your INSTALLED_APPS setting like this:
     
         INSTALLED_APPS = [
             ...
             'artd_product',
         ]
 
-2. Run ``python manage.py migrate`` to create the polls models.
+2. Run ``python manage.py migrate`` to create the product models.
 
 3. Run ``python manage.py create_taxes`` to create tax types.
 
 4. Start the development server and visit http://127.0.0.1:8000/admin/
```

### Comparing `artd-product-0.0.3/artd/settings.py` & `artd-product-0.0.4/artd/settings.py`

 * *Files 3% similar despite different names*

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

### Comparing `artd-product-0.0.3/artd/urls.py` & `artd-product-0.0.4/artd/urls.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.3/artd_product/admin.py` & `artd-product-0.0.4/artd_product/admin.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.3/artd_product/migrations/0001_initial.py` & `artd-product-0.0.4/artd_product/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.3/artd_product/migrations/0002_alter_product_special_price_and_more.py` & `artd-product-0.0.4/artd_product/migrations/0002_alter_product_special_price_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.3/artd_product/models.py` & `artd-product-0.0.4/artd_product/models.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.3/artd_product/tests.py` & `artd-product-0.0.4/artd_product/tests.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.3/artd_product.egg-info/PKG-INFO` & `artd-product-0.0.4/artd_product.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-product
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Django app to administrate products
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -35,12 +35,12 @@
 1. Add "artd_product" to your INSTALLED_APPS setting like this:
     
         INSTALLED_APPS = [
             ...
             'artd_product',
         ]
 
-2. Run ``python manage.py migrate`` to create the polls models.
+2. Run ``python manage.py migrate`` to create the product models.
 
 3. Run ``python manage.py create_taxes`` to create tax types.
 
 4. Start the development server and visit http://127.0.0.1:8000/admin/
```

### Comparing `artd-product-0.0.3/artd_product.egg-info/SOURCES.txt` & `artd-product-0.0.4/artd_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.3/setup.py` & `artd-product-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="artd-product",
-    version="0.0.3",
+    version="0.0.4",
     include_package_data=True,
     author="Jonathan Urzola Maladonado",
     author_email="jonathan@artd.com.co",
     description="A Django app to administrate products",
     long_description_content_type="text/markdown",
     url="https://www.artd.com.co/",
     long_description=long_description,
```

