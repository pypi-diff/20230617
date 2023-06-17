# Comparing `tmp/django-forbid-0.1.4.tar.gz` & `tmp/django-forbid-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forbid-0.1.4.tar", last modified: Sat Jun 10 14:11:24 2023, max compression
+gzip compressed data, was "django-forbid-0.1.5.tar", last modified: Sat Jun 17 16:59:34 2023, max compression
```

## Comparing `django-forbid-0.1.4.tar` & `django-forbid-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-10 14:11:16.000000 django-forbid-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-10 14:11:16.000000 django-forbid-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-10 14:11:24.587829 django-forbid-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-10 14:11:16.000000 django-forbid-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-10 14:11:16.000000 django-forbid-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-10 14:11:24.587829 django-forbid-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-10 14:11:16.000000 django-forbid-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/django_forbid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/django_forbid/skills/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/skills/forbid_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/skills/forbid_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/skills/forbid_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/django_forbid/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-10 14:11:16.000000 django-forbid-0.1.4/src/django_forbid/templates/timezone.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 14:11:24.587829 django-forbid-0.1.4/src/django_forbid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-10 14:11:24.000000 django-forbid-0.1.4/src/django_forbid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-17 16:59:24.000000 django-forbid-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 16:59:24.000000 django-forbid-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-17 16:59:34.531720 django-forbid-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-17 16:59:24.000000 django-forbid-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-17 16:59:24.000000 django-forbid-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-17 16:59:34.535720 django-forbid-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 16:59:24.000000 django-forbid-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/django_forbid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/django_forbid/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/skills/forbid_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/skills/forbid_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/skills/forbid_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/django_forbid/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/templates/timezone.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/django_forbid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/top_level.txt
```

### Comparing `django-forbid-0.1.4/LICENSE` & `django-forbid-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.4/PKG-INFO` & `django-forbid-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.1.4
+Version: 0.1.5
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
 Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
```

### Comparing `django-forbid-0.1.4/README.md` & `django-forbid-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.4/setup.cfg` & `django-forbid-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.4/src/django_forbid/middleware.py` & `django-forbid-0.1.5/src/django_forbid/middleware.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.4/src/django_forbid/skills/forbid_device.py` & `django-forbid-0.1.5/src/django_forbid/skills/forbid_device.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.4/src/django_forbid/skills/forbid_location.py` & `django-forbid-0.1.5/src/django_forbid/skills/forbid_location.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import itertools
+
 from django.conf import settings
 from django.contrib.gis.geoip2 import GeoIP2
 from django.http import HttpResponseForbidden
 from django.shortcuts import redirect
 from geoip2.errors import AddressNotFoundError
 
 from . import Access
 from . import Settings
+from . import continents_codes
 
 
 class ForbidLocationMiddleware:
     """Checks if the user location is forbidden."""
 
     def __init__(self, get_response):
         self.get_response = get_response
@@ -26,16 +29,27 @@
             return self.get_response(request)
 
         try:
             city = geoip.city(client_ip)
 
             countries = Settings.get("COUNTRIES", [])
             territories = Settings.get("TERRITORIES", [])
+            country_state_code = city.get("region")
+            country_identifier = city.get("country_code")
+
+            if territories:
+                # Adds the continent codes of the countries that are forbidden partially.
+                territories = list({*territories, *itertools.chain.from_iterable(
+                    map(continents_codes.__getitem__, filter(bool, map(Access.getattr, countries)))
+                )})
+
+            if country_state_code:
+                country_identifier += ":%s" % country_state_code
             granted = all([
-                Access(countries).grants(city.get("country_code")),
+                Access(countries).grants(country_identifier),
                 Access(territories).grants(city.get("continent_code")),
             ])
         except (AddressNotFoundError, Exception):
             # This happens when the IP address is not
             # in  the  GeoIP2 database. Usually, this
             # happens when the IP address is a local.
             granted = not any([
```

### Comparing `django-forbid-0.1.4/src/django_forbid/skills/forbid_network.py` & `django-forbid-0.1.5/src/django_forbid/skills/forbid_network.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.4/src/django_forbid/templates/timezone.html` & `django-forbid-0.1.5/src/django_forbid/templates/timezone.html`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.4/src/django_forbid.egg-info/PKG-INFO` & `django-forbid-0.1.5/src/django_forbid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.1.4
+Version: 0.1.5
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
 Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
```

### Comparing `django-forbid-0.1.4/src/django_forbid.egg-info/SOURCES.txt` & `django-forbid-0.1.5/src/django_forbid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

