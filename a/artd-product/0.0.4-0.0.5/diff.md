# Comparing `tmp/artd-product-0.0.4.tar.gz` & `tmp/artd-product-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artd-product-0.0.4.tar", last modified: Sat Jun 17 15:37:39 2023, max compression
+gzip compressed data, was "artd-product-0.0.5.tar", last modified: Sat Jun 17 16:01:02 2023, max compression
```

## Comparing `artd-product-0.0.4.tar` & `artd-product-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.440183 artd-product-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 15:37:35.000000 artd-product-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 15:37:35.000000 artd-product-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-17 15:37:39.436183 artd-product-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-17 15:37:35.000000 artd-product-0.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/data/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/data/taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/management/commands/create_taxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/migrations/0002_alter_product_special_price_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 15:37:35.000000 artd-product-0.0.4/artd_product/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 15:37:39.436183 artd-product-0.0.4/artd_product.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-17 15:37:39.000000 artd-product-0.0.4/artd_product.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-17 15:37:39.000000 artd-product-0.0.4/artd_product.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 15:37:39.000000 artd-product-0.0.4/artd_product.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 15:37:39.000000 artd-product-0.0.4/artd_product.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 15:37:39.440183 artd-product-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 15:37:37.000000 artd-product-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:01:02.653362 artd-product-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-06-17 16:00:58.000000 artd-product-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 16:00:58.000000 artd-product-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-17 16:01:02.653362 artd-product-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-17 16:00:58.000000 artd-product-0.0.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:01:02.653362 artd-product-0.0.5/artd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:01:02.653362 artd-product-0.0.5/artd_product/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:01:02.653362 artd-product-0.0.5/artd_product/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/data/taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:01:02.649362 artd-product-0.0.5/artd_product/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:01:02.653362 artd-product-0.0.5/artd_product/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/management/commands/create_taxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:01:02.653362 artd-product-0.0.5/artd_product/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    22033 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/migrations/0002_alter_product_special_price_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8993 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 16:00:58.000000 artd-product-0.0.5/artd_product/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:01:02.653362 artd-product-0.0.5/artd_product.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-17 16:01:02.000000 artd-product-0.0.5/artd_product.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-17 16:01:02.000000 artd-product-0.0.5/artd_product.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:01:02.000000 artd-product-0.0.5/artd_product.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-17 16:01:02.000000 artd-product-0.0.5/artd_product.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 16:01:02.653362 artd-product-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-17 16:01:00.000000 artd-product-0.0.5/setup.py
```

### Comparing `artd-product-0.0.4/LICENSE` & `artd-product-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.4/PKG-INFO` & `artd-product-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-product
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django app to administrate products
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `artd-product-0.0.4/artd/settings.py` & `artd-product-0.0.5/artd/settings.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.4/artd/urls.py` & `artd-product-0.0.5/artd/urls.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.4/artd_product/admin.py` & `artd-product-0.0.5/artd_product/admin.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.4/artd_product/migrations/0001_initial.py` & `artd-product-0.0.5/artd_product/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.4/artd_product/migrations/0002_alter_product_special_price_and_more.py` & `artd-product-0.0.5/artd_product/migrations/0002_alter_product_special_price_and_more.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.4/artd_product/models.py` & `artd-product-0.0.5/artd_product/models.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.4/artd_product/tests.py` & `artd-product-0.0.5/artd_product/tests.py`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.4/artd_product.egg-info/PKG-INFO` & `artd-product-0.0.5/artd_product.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artd-product
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Django app to administrate products
 Home-page: https://www.artd.com.co/
 Author: Jonathan Urzola Maladonado
 Author-email: jonathan@artd.com.co
 Keywords: pypi,cicd,python
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `artd-product-0.0.4/artd_product.egg-info/SOURCES.txt` & `artd-product-0.0.5/artd_product.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `artd-product-0.0.4/setup.py` & `artd-product-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="artd-product",
-    version="0.0.4",
+    version="0.0.5",
     include_package_data=True,
     author="Jonathan Urzola Maladonado",
     author_email="jonathan@artd.com.co",
     description="A Django app to administrate products",
     long_description_content_type="text/markdown",
     url="https://www.artd.com.co/",
     long_description=long_description,
```

