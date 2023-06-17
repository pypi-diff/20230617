# Comparing `tmp/django-api-admin-1.1.2.tar.gz` & `tmp/django-api-admin-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-api-admin-1.1.2.tar", last modified: Sat Jun 17 04:04:54 2023, max compression
+gzip compressed data, was "django-api-admin-1.1.3.tar", last modified: Sat Jun 17 11:58:18 2023, max compression
```

## Comparing `django-api-admin-1.1.2.tar` & `django-api-admin-1.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.829963 django-api-admin-1.1.2/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1071 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/LICENSE
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       90 2023-06-17 03:55:51.000000 django-api-admin-1.1.2/MANIFEST.in
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2982 2023-06-17 04:04:54.826630 django-api-admin-1.1.2/PKG-INFO
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2291 2023-06-17 03:55:51.000000 django-api-admin-1.1.2/README.md
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.823297 django-api-admin-1.1.2/django_api_admin/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/__init__.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1771 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/actions.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.826630 django-api-admin-1.1.2/django_api_admin/declarations/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/declarations/__init__.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1324 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/declarations/classes.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13151 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/declarations/functions.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3726 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/field_attributes.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11294 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/options.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      548 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/pagination.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      335 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/permissions.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     5255 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/serializers.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    12948 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/sites.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.826630 django-api-admin-1.1.2/django_api_admin/views/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/views/__init__.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    26075 2023-06-17 03:55:51.000000 django-api-admin-1.1.2/django_api_admin/views/admin_views.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11410 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/views/fields_test_views.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8315 2023-06-17 03:55:51.000000 django-api-admin-1.1.2/django_api_admin/views/site_views.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.826630 django-api-admin-1.1.2/django_api_admin.egg-info/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2982 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/PKG-INFO
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      760 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/SOURCES.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        1 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/dependency_links.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       27 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/requires.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       17 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/top_level.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       38 2023-06-17 04:04:54.829963 django-api-admin-1.1.2/setup.cfg
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1111 2023-06-17 03:59:45.000000 django-api-admin-1.1.2/setup.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.216513 django-api-admin-1.1.3/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1071 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/LICENSE
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       90 2023-06-17 11:37:37.000000 django-api-admin-1.1.3/MANIFEST.in
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2982 2023-06-17 11:58:18.216513 django-api-admin-1.1.3/PKG-INFO
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2291 2023-06-17 11:38:23.000000 django-api-admin-1.1.3/README.md
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.213180 django-api-admin-1.1.3/django_api_admin/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/__init__.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1771 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/actions.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.213180 django-api-admin-1.1.3/django_api_admin/declarations/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/declarations/__init__.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1324 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/declarations/classes.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13151 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/declarations/functions.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3726 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/field_attributes.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11294 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/options.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      548 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/pagination.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      335 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/permissions.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     5255 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/serializers.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    12948 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/sites.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.216513 django-api-admin-1.1.3/django_api_admin/views/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/views/__init__.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    26075 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/views/admin_views.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11410 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/views/fields_test_views.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8327 2023-06-17 11:36:49.000000 django-api-admin-1.1.3/django_api_admin/views/site_views.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.213180 django-api-admin-1.1.3/django_api_admin.egg-info/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2982 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/PKG-INFO
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      760 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        1 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       27 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/requires.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       17 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/top_level.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       38 2023-06-17 11:58:18.216513 django-api-admin-1.1.3/setup.cfg
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1111 2023-06-17 11:57:33.000000 django-api-admin-1.1.3/setup.py
```

### Comparing `django-api-admin-1.1.2/LICENSE` & `django-api-admin-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/PKG-INFO` & `django-api-admin-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.2
+Version: 1.1.3
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-api-admin-1.1.2/README.md` & `django-api-admin-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/actions.py` & `django-api-admin-1.1.3/django_api_admin/actions.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/declarations/classes.py` & `django-api-admin-1.1.3/django_api_admin/declarations/classes.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/declarations/functions.py` & `django-api-admin-1.1.3/django_api_admin/declarations/functions.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/field_attributes.py` & `django-api-admin-1.1.3/django_api_admin/field_attributes.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/options.py` & `django-api-admin-1.1.3/django_api_admin/options.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/pagination.py` & `django-api-admin-1.1.3/django_api_admin/pagination.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/serializers.py` & `django-api-admin-1.1.3/django_api_admin/serializers.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/sites.py` & `django-api-admin-1.1.3/django_api_admin/sites.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/views/admin_views.py` & `django-api-admin-1.1.3/django_api_admin/views/admin_views.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/views/fields_test_views.py` & `django-api-admin-1.1.3/django_api_admin/views/fields_test_views.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/django_api_admin/views/site_views.py` & `django-api-admin-1.1.3/django_api_admin/views/site_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def get(self, request, admin_site):
         serializer = self.serializer_class()
         form_fields = get_form_fields(serializer)
         return Response({'fields': form_fields}, status=status.HTTP_200_OK)
 
     def post(self, request, admin_site):
         serializer = self.serializer_class(
-            data=request.data, context={'request': request})
+            data=request.data.get('data'), context={'request': request})
         if serializer.is_valid():
             user = serializer.get_user()
             login(request, user)
             user_serializer = admin_site.user_serializer(user)
             data = {
                 'detail': _('you are logged in successfully'),
                 'user': user_serializer.data
```

### Comparing `django-api-admin-1.1.2/django_api_admin.egg-info/PKG-INFO` & `django-api-admin-1.1.3/django_api_admin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.2
+Version: 1.1.3
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-api-admin-1.1.2/django_api_admin.egg-info/SOURCES.txt` & `django-api-admin-1.1.3/django_api_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.2/setup.py` & `django-api-admin-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="django-api-admin",
-    version="1.1.2",
+    version="1.1.3",
     description="Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MuhammadSalahAli/django-api-admin",
     author="Muhammad Salah",
     author_email="msmainacc0unt@gmail.com",
     license="MIT",
```

