# Comparing `tmp/goodmap-0.1.8.tar.gz` & `tmp/goodmap-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodmap-0.1.8.tar", max compression
+gzip compressed data, was "goodmap-0.1.9.tar", max compression
```

## Comparing `goodmap-0.1.8.tar` & `goodmap-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1067 2023-05-31 13:00:58.713740 goodmap-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     2763 2023-05-31 13:00:58.713740 goodmap-0.1.8/README.md
--rw-r--r--   0        0        0        1 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/__init__.py
--rw-r--r--   0        0        0     2697 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/config.py
--rw-r--r--   0        0        0      551 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/core.py
--rw-r--r--   0        0        0     1765 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/core_api.py
--rw-r--r--   0        0        0      545 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/formatter.py
--rw-r--r--   0        0        0     1428 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/goodmap.py
--rw-r--r--   0        0        0        0 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/__init__.py
--rw-r--r--   0        0        0     2794 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/blog/blog.py
--rw-r--r--   0        0        0      498 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/blog/comment_form.py
--rw-r--r--   0        0        0      354 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/blog/db.py
--rw-r--r--   0        0        0      476 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/blog/post_formatter.py
--rw-r--r--   0        0        0      909 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/db/google_json_db.py
--rw-r--r--   0        0        0     5108 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/db/graph_ql_db.py
--rw-r--r--   0        0        0     1356 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/db/json_db.py
--rw-r--r--   0        0        0      732 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/db/json_file_db.py
--rw-r--r--   0        0        0     3525 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/platzky.py
--rw-r--r--   0        0        0     1443 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/plugin_loader.py
--rw-r--r--   0        0        0     1205 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/plugins/redirections/entrypoint.py
--rw-r--r--   0        0        0      674 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/plugins/sendmail/entrypoint.py
--rw-r--r--   0        0        0     2615 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/seo/seo.py
--rw-r--r--   0        0        0     8079 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/static/blog.css
--rw-r--r--   0        0        0       78 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/404.html
--rw-r--r--   0        0        0     4165 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/base.html
--rw-r--r--   0        0        0     1286 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/blog.html
--rw-r--r--   0        0        0      756 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/body_meta.html
--rw-r--r--   0        0        0      859 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/feed.xml
--rw-r--r--   0        0        0     1796 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/head_meta.html
--rw-r--r--   0        0        0     3900 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/home.html
--rw-r--r--   0        0        0      647 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/page.html
--rw-r--r--   0        0        0     1921 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/post.html
--rw-r--r--   0        0        0      116 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/robots.txt
--rw-r--r--   0        0        0      578 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/templates/sitemap.xml
--rw-r--r--   0        0        0      771 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/platzky/www_handler.py
--rw-r--r--   0        0        0        0 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/templates/admin.html
--rw-r--r--   0        0        0      214 2023-05-31 13:00:58.713740 goodmap-0.1.8/goodmap/templates/map.html
--rw-r--r--   0        0        0     1551 2023-05-31 13:00:58.717740 goodmap-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3702 1970-01-01 00:00:00.000000 goodmap-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-17 20:24:56.939453 goodmap-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     2821 2023-06-17 20:24:56.939453 goodmap-0.1.9/README.md
+-rw-r--r--   0        0        0        1 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/__init__.py
+-rw-r--r--   0        0        0     2697 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/config.py
+-rw-r--r--   0        0        0      551 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/core.py
+-rw-r--r--   0        0        0     1765 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/core_api.py
+-rw-r--r--   0        0        0      585 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/formatter.py
+-rw-r--r--   0        0        0     1428 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/goodmap.py
+-rw-r--r--   0        0        0        0 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/__init__.py
+-rw-r--r--   0        0        0     2794 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/blog/blog.py
+-rw-r--r--   0        0        0      498 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/blog/comment_form.py
+-rw-r--r--   0        0        0      354 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/blog/db.py
+-rw-r--r--   0        0        0      476 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/blog/post_formatter.py
+-rw-r--r--   0        0        0      909 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/db/google_json_db.py
+-rw-r--r--   0        0        0     5108 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/db/graph_ql_db.py
+-rw-r--r--   0        0        0     1356 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/db/json_db.py
+-rw-r--r--   0        0        0      732 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/db/json_file_db.py
+-rw-r--r--   0        0        0     3525 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/platzky.py
+-rw-r--r--   0        0        0     1443 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/plugin_loader.py
+-rw-r--r--   0        0        0     1205 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/plugins/redirections/entrypoint.py
+-rw-r--r--   0        0        0      674 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/plugins/sendmail/entrypoint.py
+-rw-r--r--   0        0        0     2615 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/seo/seo.py
+-rw-r--r--   0        0        0     8079 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/static/blog.css
+-rw-r--r--   0        0        0       78 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/404.html
+-rw-r--r--   0        0        0     4165 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/base.html
+-rw-r--r--   0        0        0     1286 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/blog.html
+-rw-r--r--   0        0        0      756 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/body_meta.html
+-rw-r--r--   0        0        0      859 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/feed.xml
+-rw-r--r--   0        0        0     1796 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/head_meta.html
+-rw-r--r--   0        0        0     3900 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/home.html
+-rw-r--r--   0        0        0      647 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/page.html
+-rw-r--r--   0        0        0     1921 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/post.html
+-rw-r--r--   0        0        0      116 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/robots.txt
+-rw-r--r--   0        0        0      578 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/templates/sitemap.xml
+-rw-r--r--   0        0        0      771 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/platzky/www_handler.py
+-rw-r--r--   0        0        0        0 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/templates/admin.html
+-rw-r--r--   0        0        0      214 2023-06-17 20:24:56.939453 goodmap-0.1.9/goodmap/templates/map.html
+-rw-r--r--   0        0        0     1551 2023-06-17 20:24:56.943452 goodmap-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3760 1970-01-01 00:00:00.000000 goodmap-0.1.9/PKG-INFO
```

### Comparing `goodmap-0.1.8/LICENSE.md` & `goodmap-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/README.md` & `goodmap-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,18 @@
 - `e2e_test_config.yml`
 - `e2e_test_data.json`
 
 # Version History
 
 ### 0.1 - Initial Release - in development
 
-#### 0.1.8 - in development
+#### 0.1.9
+  * fix: App not displaying data if visible data is null (#53)
+
+#### 0.1.8
   * unified frontend
 
 #### 0.1.5
   * better looking frontend
 
 #### 0.1.4 - Makeover
   * frontend for mobile version
```

### Comparing `goodmap-0.1.8/goodmap/config.py` & `goodmap-0.1.9/goodmap/config.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/core.py` & `goodmap-0.1.9/goodmap/core.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/core_api.py` & `goodmap-0.1.9/goodmap/core_api.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/formatter.py` & `goodmap-0.1.9/goodmap/formatter.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,10 +11,12 @@
 
 
 def prepare_pin(place, visible_fields):
     pin_data = {
         "title": place["name"],
         "subtitle": lazy_gettext(place["type_of_place"]),
         "position": place["position"],
-        "data": {gettext(field): safe_gettext(place[field]) for field in visible_fields},
+        "data": {
+            gettext(field): safe_gettext(place[field]) for field in visible_fields if field in place
+        },
     }
     return pin_data
```

### Comparing `goodmap-0.1.8/goodmap/goodmap.py` & `goodmap-0.1.9/goodmap/goodmap.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/blog/blog.py` & `goodmap-0.1.9/goodmap/platzky/blog/blog.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/db/google_json_db.py` & `goodmap-0.1.9/goodmap/platzky/db/google_json_db.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/db/graph_ql_db.py` & `goodmap-0.1.9/goodmap/platzky/db/graph_ql_db.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/db/json_db.py` & `goodmap-0.1.9/goodmap/platzky/db/json_db.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/db/json_file_db.py` & `goodmap-0.1.9/goodmap/platzky/db/json_file_db.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/platzky.py` & `goodmap-0.1.9/goodmap/platzky/platzky.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/plugin_loader.py` & `goodmap-0.1.9/goodmap/platzky/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/plugins/redirections/entrypoint.py` & `goodmap-0.1.9/goodmap/platzky/plugins/redirections/entrypoint.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/plugins/sendmail/entrypoint.py` & `goodmap-0.1.9/goodmap/platzky/plugins/sendmail/entrypoint.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/seo/seo.py` & `goodmap-0.1.9/goodmap/platzky/seo/seo.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/static/blog.css` & `goodmap-0.1.9/goodmap/platzky/static/blog.css`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/templates/base.html` & `goodmap-0.1.9/goodmap/platzky/templates/base.html`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/templates/blog.html` & `goodmap-0.1.9/goodmap/platzky/templates/blog.html`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/templates/body_meta.html` & `goodmap-0.1.9/goodmap/platzky/templates/body_meta.html`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/templates/feed.xml` & `goodmap-0.1.9/goodmap/platzky/templates/feed.xml`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/templates/head_meta.html` & `goodmap-0.1.9/goodmap/platzky/templates/head_meta.html`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/templates/home.html` & `goodmap-0.1.9/goodmap/platzky/templates/home.html`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/templates/page.html` & `goodmap-0.1.9/goodmap/platzky/templates/page.html`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/templates/post.html` & `goodmap-0.1.9/goodmap/platzky/templates/post.html`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/templates/sitemap.xml` & `goodmap-0.1.9/goodmap/platzky/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/goodmap/platzky/www_handler.py` & `goodmap-0.1.9/goodmap/platzky/www_handler.py`

 * *Files identical despite different names*

### Comparing `goodmap-0.1.8/pyproject.toml` & `goodmap-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goodmap"
-version = "0.1.8"
+version = "0.1.9"
 description = "Map engine to serve all the people :)"
 authors = ["Krzysztof Kolodzinski <krzysztof.kolodzinski@problematy.pl>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Flask = "^2.2.2"
```

### Comparing `goodmap-0.1.8/PKG-INFO` & `goodmap-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodmap
-Version: 0.1.8
+Version: 0.1.9
 Summary: Map engine to serve all the people :)
 Author: Krzysztof Kolodzinski
 Author-email: krzysztof.kolodzinski@problematy.pl
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -85,15 +85,18 @@
 - `e2e_test_config.yml`
 - `e2e_test_data.json`
 
 # Version History
 
 ### 0.1 - Initial Release - in development
 
-#### 0.1.8 - in development
+#### 0.1.9
+  * fix: App not displaying data if visible data is null (#53)
+
+#### 0.1.8
   * unified frontend
 
 #### 0.1.5
   * better looking frontend
 
 #### 0.1.4 - Makeover
   * frontend for mobile version
```

