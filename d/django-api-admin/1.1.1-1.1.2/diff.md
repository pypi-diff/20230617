# Comparing `tmp/django-api-admin-1.1.1.tar.gz` & `tmp/django-api-admin-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-api-admin-1.1.1.tar", last modified: Sat Apr 15 21:03:51 2023, max compression
+gzip compressed data, was "django-api-admin-1.1.2.tar", last modified: Sat Jun 17 04:04:54 2023, max compression
```

## Comparing `django-api-admin-1.1.1.tar` & `django-api-admin-1.1.2.tar`

### file list

```diff
@@ -1,40 +1,31 @@
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.434317 django-api-admin-1.1.1/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1071 2023-03-15 22:10:39.000000 django-api-admin-1.1.1/LICENSE
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       90 2023-04-15 20:58:20.000000 django-api-admin-1.1.1/MANIFEST.in
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2761 2023-04-15 21:03:51.434317 django-api-admin-1.1.1/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2070 2023-04-15 20:39:35.000000 django-api-admin-1.1.1/README.md
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.414317 django-api-admin-1.1.1/django_api_admin/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        0 2023-03-15 22:10:39.000000 django-api-admin-1.1.1/django_api_admin/__init__.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1771 2023-03-24 20:07:54.000000 django-api-admin-1.1.1/django_api_admin/actions.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.422317 django-api-admin-1.1.1/django_api_admin/declarations/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 20:39:49.000000 django-api-admin-1.1.1/django_api_admin/declarations/__init__.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.426317 django-api-admin-1.1.1/django_api_admin/declarations/__pycache__/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      186 2023-04-15 19:12:35.000000 django-api-admin-1.1.1/django_api_admin/declarations/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2319 2023-04-13 19:27:34.000000 django-api-admin-1.1.1/django_api_admin/declarations/__pycache__/classes.cpython-310.pyc
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     6903 2023-04-15 13:54:24.000000 django-api-admin-1.1.1/django_api_admin/declarations/__pycache__/functions.cpython-310.pyc
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1324 2023-04-13 10:53:41.000000 django-api-admin-1.1.1/django_api_admin/declarations/classes.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    13151 2023-04-15 13:54:21.000000 django-api-admin-1.1.1/django_api_admin/declarations/functions.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     3726 2023-03-24 20:00:01.000000 django-api-admin-1.1.1/django_api_admin/field_attributes.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    11294 2023-04-15 20:39:49.000000 django-api-admin-1.1.1/django_api_admin/options.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      548 2023-03-24 20:11:26.000000 django-api-admin-1.1.1/django_api_admin/pagination.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      335 2023-03-15 22:10:39.000000 django-api-admin-1.1.1/django_api_admin/permissions.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     5255 2023-04-12 08:25:20.000000 django-api-admin-1.1.1/django_api_admin/serializers.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    12948 2023-04-15 20:39:49.000000 django-api-admin-1.1.1/django_api_admin/sites.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.430317 django-api-admin-1.1.1/django_api_admin/views/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 20:39:49.000000 django-api-admin-1.1.1/django_api_admin/views/__init__.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.434317 django-api-admin-1.1.1/django_api_admin/views/__pycache__/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)      179 2023-04-15 18:52:38.000000 django-api-admin-1.1.1/django_api_admin/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    17641 2023-04-15 16:51:31.000000 django-api-admin-1.1.1/django_api_admin/views/__pycache__/admin_views.cpython-310.pyc
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     7747 2023-04-14 11:41:03.000000 django-api-admin-1.1.1/django_api_admin/views/__pycache__/fields_test_views.cpython-310.pyc
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     8325 2023-04-14 11:40:18.000000 django-api-admin-1.1.1/django_api_admin/views/__pycache__/site_views.cpython-310.pyc
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    25791 2023-04-15 16:51:29.000000 django-api-admin-1.1.1/django_api_admin/views/admin_views.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)    11410 2023-04-14 11:40:59.000000 django-api-admin-1.1.1/django_api_admin/views/fields_test_views.py
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     8166 2023-04-14 11:40:16.000000 django-api-admin-1.1.1/django_api_admin/views/site_views.py
-drwxrwxr-x   0 muhammad  (1000) muhammad  (1000)        0 2023-04-15 21:03:51.418317 django-api-admin-1.1.1/django_api_admin.egg-info/
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     2761 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/PKG-INFO
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1215 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/SOURCES.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)        1 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/dependency_links.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       27 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/requires.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       17 2023-04-15 21:03:51.000000 django-api-admin-1.1.1/django_api_admin.egg-info/top_level.txt
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)       38 2023-04-15 21:03:51.434317 django-api-admin-1.1.1/setup.cfg
--rw-rw-r--   0 muhammad  (1000) muhammad  (1000)     1111 2023-04-15 21:03:11.000000 django-api-admin-1.1.1/setup.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.829963 django-api-admin-1.1.2/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1071 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/LICENSE
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       90 2023-06-17 03:55:51.000000 django-api-admin-1.1.2/MANIFEST.in
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2982 2023-06-17 04:04:54.826630 django-api-admin-1.1.2/PKG-INFO
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2291 2023-06-17 03:55:51.000000 django-api-admin-1.1.2/README.md
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.823297 django-api-admin-1.1.2/django_api_admin/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/__init__.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1771 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/actions.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.826630 django-api-admin-1.1.2/django_api_admin/declarations/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/declarations/__init__.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1324 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/declarations/classes.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13151 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/declarations/functions.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3726 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/field_attributes.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11294 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/options.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      548 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/pagination.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      335 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/permissions.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     5255 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/serializers.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    12948 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/sites.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.826630 django-api-admin-1.1.2/django_api_admin/views/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/views/__init__.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    26075 2023-06-17 03:55:51.000000 django-api-admin-1.1.2/django_api_admin/views/admin_views.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11410 2023-06-17 02:42:22.000000 django-api-admin-1.1.2/django_api_admin/views/fields_test_views.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8315 2023-06-17 03:55:51.000000 django-api-admin-1.1.2/django_api_admin/views/site_views.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 04:04:54.826630 django-api-admin-1.1.2/django_api_admin.egg-info/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2982 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/PKG-INFO
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      760 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        1 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       27 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/requires.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       17 2023-06-17 04:04:54.000000 django-api-admin-1.1.2/django_api_admin.egg-info/top_level.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       38 2023-06-17 04:04:54.829963 django-api-admin-1.1.2/setup.cfg
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1111 2023-06-17 03:59:45.000000 django-api-admin-1.1.2/setup.py
```

### Comparing `django-api-admin-1.1.1/LICENSE` & `django-api-admin-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/PKG-INFO` & `django-api-admin-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.1
+Version: 1.1.2
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,20 @@
 - [x] Expose all django.contrib.admin views as a restful api.
 - [x] Similar to django.contrib.admin.
 - [x] Customizable AdminSite and ModelAdmin.
 - [x] Supports InlineModelAdmins and bulk edits.
 - [x] Provides data to dynamically create forms on clients from serializers.
 - [x] Extensively tested
 
+## Demo 🚀
+
+You can also test it in this <a href="https://django-api-admin.demon-bixia.repl.co/" target="_blank">demo</a> that is hosted on replit. use these credentials to login
+
+* username: admin
+* password: password
 
 ## Requirements 📄
 
 <p>Python 3.9+</p>
 <p>This package depends on</p>
 <ul>
     <li><a href="https://github.com/encode/django-rest-framework">django-rest-framework</a></li>
```

### Comparing `django-api-admin-1.1.1/README.md` & `django-api-admin-1.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 - [x] Expose all django.contrib.admin views as a restful api.
 - [x] Similar to django.contrib.admin.
 - [x] Customizable AdminSite and ModelAdmin.
 - [x] Supports InlineModelAdmins and bulk edits.
 - [x] Provides data to dynamically create forms on clients from serializers.
 - [x] Extensively tested
 
+## Demo 🚀
+
+You can also test it in this <a href="https://django-api-admin.demon-bixia.repl.co/" target="_blank">demo</a> that is hosted on replit. use these credentials to login
+
+* username: admin
+* password: password
 
 ## Requirements 📄
 
 <p>Python 3.9+</p>
 <p>This package depends on</p>
 <ul>
     <li><a href="https://github.com/encode/django-rest-framework">django-rest-framework</a></li>
```

### Comparing `django-api-admin-1.1.1/django_api_admin/actions.py` & `django-api-admin-1.1.2/django_api_admin/actions.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/django_api_admin/declarations/classes.py` & `django-api-admin-1.1.2/django_api_admin/declarations/classes.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/django_api_admin/declarations/functions.py` & `django-api-admin-1.1.2/django_api_admin/declarations/functions.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/django_api_admin/field_attributes.py` & `django-api-admin-1.1.2/django_api_admin/field_attributes.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/django_api_admin/options.py` & `django-api-admin-1.1.2/django_api_admin/options.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/django_api_admin/pagination.py` & `django-api-admin-1.1.2/django_api_admin/pagination.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/django_api_admin/serializers.py` & `django-api-admin-1.1.2/django_api_admin/serializers.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/django_api_admin/sites.py` & `django-api-admin-1.1.2/django_api_admin/sites.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/django_api_admin/views/admin_views.py` & `django-api-admin-1.1.2/django_api_admin/views/admin_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,20 @@
         info = (
             admin.admin_site.name,
             admin.model._meta.app_label,
             admin.model._meta.model_name
         )
         pattern = '%s:%s_%s_detail'
 
+        domain = request.get_host()
+        scheme = 'https://' if request.is_secure() else 'http://'
         for item in data:
-            item['detail_url'] = reverse(pattern % info, kwargs={
+            path = reverse(pattern % info, kwargs={
                 'object_id': int(item['pk'])}, request=request)
+            item['detail_url'] = scheme + domain + path
         return Response(data, status=status.HTTP_200_OK)
 
 
 class DetailView(APIView):
     """
     GET one instance of this model using pk and to_fields.
     """
@@ -79,28 +82,25 @@
         # add admin urls.
         info = (
             admin.admin_site.name,
             admin.model._meta.app_label,
             admin.model._meta.model_name,
         )
         pattern = '%s:%s_%s_'
-        data['history_url'] = reverse((pattern + 'history') % info, kwargs={'object_id': data['pk']},
-                                      request=request)
+        domain = request.get_host()
+        scheme = 'https://' if request.is_secure() else 'http://'
         if admin.view_on_site:
             model_type = ContentType.objects.get_for_model(
-                model=admin.model)
-            data['view_on_site'] = reverse('%s:view_on_site' % admin.admin_site.name,
-                                           kwargs={
-                                               'content_type_id': model_type.pk, 'object_id': obj.pk},
-                                           request=request)
-
-        data['list_url'] = reverse((pattern + 'list') % info, request=request)
-        data['delete_url'] = reverse(
+                model=admin.model)    
+        data['view_on_site'] = scheme + domain + reverse('%s:view_on_site' % admin.admin_site.name, kwargs={ 'content_type_id': model_type.pk, 'object_id': obj.pk}, request=request)
+        data['list_url'] = scheme + domain + reverse((pattern + 'list') % info, request=request)
+        data['history_url'] = scheme + domain + reverse((pattern + 'history') % info, kwargs={'object_id': data['pk']}, request=request)
+        data['delete_url'] = scheme + domain + reverse(
             (pattern + 'delete') % info, kwargs={'object_id': data['pk']}, request=request)
-        data['change_url'] = reverse(
+        data['change_url'] = scheme + domain + reverse(
             (pattern + 'change') % info, kwargs={'object_id': data['pk']}, request=request)
         return Response(data, status=status.HTTP_200_OK)
 
 
 class AddView(APIView):
     """
     Add new instances of this model. if this model has inline models associated with it 
@@ -482,19 +482,21 @@
         """
         Return changelist rows actual list of data.
         """
         rows = []
         # generate changelist attributes (e.g result_list, paginator, result_count)
         cl.get_results(request)
         empty_value_display = cl.model_admin.get_empty_value_display()
+        domain = request.get_host()
+        scheme = 'https://' if request.is_secure() else 'http://'
         for result in cl.result_list:
             model_info = (cl.model_admin.admin_site.name, type(
                 result)._meta.app_label, type(result)._meta.model_name)
             row = {
-                'change_url': reverse('%s:%s_%s_change' % model_info, kwargs={'object_id': result.pk}, request=request),
+                'change_url': scheme + domain + reverse('%s:%s_%s_change' % model_info, kwargs={'object_id': result.pk}, request=request),
                 'id': result.pk,
                 'cells': {}
             }
 
             for field_name in self.get_fields_list(request, cl):
                 try:
                     _, _, value = lookup_field(
```

### Comparing `django-api-admin-1.1.1/django_api_admin/views/fields_test_views.py` & `django-api-admin-1.1.2/django_api_admin/views/fields_test_views.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.1/django_api_admin/views/site_views.py` & `django-api-admin-1.1.2/django_api_admin/views/site_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 import json
 
 from django.contrib.admin.views.autocomplete import AutocompleteJsonView
 from django.contrib.auth import login, logout
 from django.middleware.csrf import get_token
 from django.utils.translation import gettext_lazy as _
 from django.views.i18n import JSONCatalog
+from django.urls import reverse
 
 from rest_framework import status
 from rest_framework.response import Response
-from rest_framework.reverse import reverse
 from rest_framework.views import APIView
 
 from django_api_admin.declarations.functions import get_form_fields
-
 # todo split the views file.
 # todo add more comments.
 # todo add support for bulk edits.
 
 
 class CsrfTokenView(APIView):
     serializer_class = None
@@ -106,19 +105,20 @@
     Return json object that lists all the installed
     apps that have been registered by the admin site.
     """
     permission_classes = []
 
     def get(self, request, admin_site):
         app_list = admin_site.get_app_list(request)
+
         # add an url to app_index in every app in app_list
+        domain = request.get_host()
+        scheme = 'https://' if request.is_secure() else 'http://'
         for app in app_list:
-            url = reverse(f'{admin_site.name}:app_list', kwargs={
-                'app_label': app['app_label']}, request=request)
-            app['url'] = url
+            app['url'] = scheme + domain + reverse(f'{admin_site.name}:app_list', kwargs={ 'app_label': app['app_label']})
         data = {
             'app_list': app_list,
         }
         request.current_app = admin_site.name
         return Response(data, status=status.HTTP_200_OK)
 
 
@@ -247,11 +247,13 @@
         data = dict()
 
         for url in self.root_urls:
             if request.user.is_authenticated and url.name == 'login':
                 continue
             elif not request.user.is_authenticated and url.name in ('logout', 'password_change'):
                 continue
-            data[url.name] = reverse(
-                namespace + ':' + url.name, request=request, args=args, kwargs=kwargs)
+
+            domain = request.get_host()
+            scheme = 'https://' if request.is_secure() else 'http://'
+            data[url.name] = scheme + domain + reverse(namespace + ':' + url.name, args=args, kwargs=kwargs)
 
         return Response(data or {}, status=status.HTTP_200_OK)
```

### Comparing `django-api-admin-1.1.1/django_api_admin.egg-info/PKG-INFO` & `django-api-admin-1.1.2/django_api_admin.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.1
+Version: 1.1.2
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,20 @@
 - [x] Expose all django.contrib.admin views as a restful api.
 - [x] Similar to django.contrib.admin.
 - [x] Customizable AdminSite and ModelAdmin.
 - [x] Supports InlineModelAdmins and bulk edits.
 - [x] Provides data to dynamically create forms on clients from serializers.
 - [x] Extensively tested
 
+## Demo 🚀
+
+You can also test it in this <a href="https://django-api-admin.demon-bixia.repl.co/" target="_blank">demo</a> that is hosted on replit. use these credentials to login
+
+* username: admin
+* password: password
 
 ## Requirements 📄
 
 <p>Python 3.9+</p>
 <p>This package depends on</p>
 <ul>
     <li><a href="https://github.com/encode/django-rest-framework">django-rest-framework</a></li>
```

### Comparing `django-api-admin-1.1.1/setup.py` & `django-api-admin-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="django-api-admin",
-    version="1.1.1",
+    version="1.1.2",
     description="Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MuhammadSalahAli/django-api-admin",
     author="Muhammad Salah",
     author_email="msmainacc0unt@gmail.com",
     license="MIT",
```

