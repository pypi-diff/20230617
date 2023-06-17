# Comparing `tmp/django_short_links-0.1.3.tar.gz` & `tmp/django_short_links-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_short_links-0.1.3.tar", max compression
+gzip compressed data, was "django_short_links-0.1.4.tar", max compression
```

## Comparing `django_short_links-0.1.3.tar` & `django_short_links-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1095 2023-06-13 14:31:22.286365 django_short_links-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2023-06-13 14:31:22.287366 django_short_links-0.1.3/links/__init__.py
--rw-r--r--   0        0        0      167 2023-06-13 14:31:22.288380 django_short_links-0.1.3/links/admin.py
--rw-r--r--   0        0        0      218 2023-06-13 14:31:22.288380 django_short_links-0.1.3/links/apps.py
--rw-r--r--   0        0        0      849 2023-06-13 14:31:22.290365 django_short_links-0.1.3/links/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-13 14:31:22.290365 django_short_links-0.1.3/links/migrations/__init__.py
--rw-r--r--   0        0        0      347 2023-06-16 15:03:04.978367 django_short_links-0.1.3/links/mixins.py
--rw-r--r--   0        0        0      841 2023-06-16 15:03:04.979367 django_short_links-0.1.3/links/models.py
--rw-r--r--   0        0        0      982 2023-06-13 14:31:22.292365 django_short_links-0.1.3/links/templates/links/base.html
--rw-r--r--   0        0        0     1466 2023-06-16 15:03:04.980889 django_short_links-0.1.3/links/templates/links/components/delete-modal.html
--rw-r--r--   0        0        0      426 2023-06-16 15:03:04.980889 django_short_links-0.1.3/links/templates/links/components/messages.html
--rw-r--r--   0        0        0     2550 2023-06-17 05:38:24.473941 django_short_links-0.1.3/links/templates/links/components/navbar.html
--rw-r--r--   0        0        0     3038 2023-06-16 15:03:04.986904 django_short_links-0.1.3/links/templates/links/components/url.html
--rw-r--r--   0        0        0     1094 2023-06-16 15:03:04.986904 django_short_links-0.1.3/links/templates/links/create.html
--rw-r--r--   0        0        0     1082 2023-06-16 15:03:04.987902 django_short_links-0.1.3/links/templates/links/delete.html
--rw-r--r--   0        0        0     3008 2023-06-16 15:03:04.989904 django_short_links-0.1.3/links/templates/links/detail.html
--rw-r--r--   0        0        0     3223 2023-06-16 15:03:04.990898 django_short_links-0.1.3/links/templates/links/index.html
--rw-r--r--   0        0        0     2241 2023-06-16 15:03:04.990898 django_short_links-0.1.3/links/templates/links/list.html
--rw-r--r--   0        0        0     1330 2023-06-16 15:03:04.991896 django_short_links-0.1.3/links/templates/links/update.html
--rw-r--r--   0        0        0      712 2023-06-16 15:03:04.991896 django_short_links-0.1.3/links/templates/registration/logged_out.html
--rw-r--r--   0        0        0     2214 2023-06-16 15:03:04.992898 django_short_links-0.1.3/links/templates/registration/login.html
--rw-r--r--   0        0        0       84 2023-06-13 14:31:22.293366 django_short_links-0.1.3/links/tests.py
--rw-r--r--   0        0        0      640 2023-06-16 15:03:04.992898 django_short_links-0.1.3/links/urls.py
--rw-r--r--   0        0        0     3222 2023-06-17 05:38:24.474928 django_short_links-0.1.3/links/views.py
--rw-r--r--   0        0        0      524 2023-06-17 05:41:08.726089 django_short_links-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      915 2023-06-17 05:38:24.471929 django_short_links-0.1.3/README.md
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 django_short_links-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-06-13 14:31:22.286365 django_short_links-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-13 14:31:22.287366 django_short_links-0.1.4/links/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-13 14:31:22.288380 django_short_links-0.1.4/links/admin.py
+-rw-r--r--   0        0        0      218 2023-06-13 14:31:22.288380 django_short_links-0.1.4/links/apps.py
+-rw-r--r--   0        0        0      849 2023-06-13 14:31:22.290365 django_short_links-0.1.4/links/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1057 2023-06-17 05:54:23.066017 django_short_links-0.1.4/links/migrations/0002_url_user_alter_url_token_alter_url_url.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:31:22.290365 django_short_links-0.1.4/links/migrations/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-16 15:03:04.978367 django_short_links-0.1.4/links/mixins.py
+-rw-r--r--   0        0        0      841 2023-06-16 15:03:04.979367 django_short_links-0.1.4/links/models.py
+-rw-r--r--   0        0        0      982 2023-06-13 14:31:22.292365 django_short_links-0.1.4/links/templates/links/base.html
+-rw-r--r--   0        0        0     1466 2023-06-16 15:03:04.980889 django_short_links-0.1.4/links/templates/links/components/delete-modal.html
+-rw-r--r--   0        0        0      426 2023-06-16 15:03:04.980889 django_short_links-0.1.4/links/templates/links/components/messages.html
+-rw-r--r--   0        0        0     2550 2023-06-17 05:38:24.473941 django_short_links-0.1.4/links/templates/links/components/navbar.html
+-rw-r--r--   0        0        0     3038 2023-06-16 15:03:04.986904 django_short_links-0.1.4/links/templates/links/components/url.html
+-rw-r--r--   0        0        0     1094 2023-06-16 15:03:04.986904 django_short_links-0.1.4/links/templates/links/create.html
+-rw-r--r--   0        0        0     1082 2023-06-16 15:03:04.987902 django_short_links-0.1.4/links/templates/links/delete.html
+-rw-r--r--   0        0        0     3008 2023-06-16 15:03:04.989904 django_short_links-0.1.4/links/templates/links/detail.html
+-rw-r--r--   0        0        0     3223 2023-06-16 15:03:04.990898 django_short_links-0.1.4/links/templates/links/index.html
+-rw-r--r--   0        0        0     2241 2023-06-16 15:03:04.990898 django_short_links-0.1.4/links/templates/links/list.html
+-rw-r--r--   0        0        0     1330 2023-06-16 15:03:04.991896 django_short_links-0.1.4/links/templates/links/update.html
+-rw-r--r--   0        0        0      712 2023-06-16 15:03:04.991896 django_short_links-0.1.4/links/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     2214 2023-06-16 15:03:04.992898 django_short_links-0.1.4/links/templates/registration/login.html
+-rw-r--r--   0        0        0       84 2023-06-13 14:31:22.293366 django_short_links-0.1.4/links/tests.py
+-rw-r--r--   0        0        0      640 2023-06-16 15:03:04.992898 django_short_links-0.1.4/links/urls.py
+-rw-r--r--   0        0        0     3222 2023-06-17 05:38:24.474928 django_short_links-0.1.4/links/views.py
+-rw-r--r--   0        0        0      524 2023-06-17 05:56:38.204246 django_short_links-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      915 2023-06-17 05:38:24.471929 django_short_links-0.1.4/README.md
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 django_short_links-0.1.4/PKG-INFO
```

### Comparing `django_short_links-0.1.3/LICENSE` & `django_short_links-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/migrations/0001_initial.py` & `django_short_links-0.1.4/links/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/models.py` & `django_short_links-0.1.4/links/models.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/base.html` & `django_short_links-0.1.4/links/templates/links/base.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/components/delete-modal.html` & `django_short_links-0.1.4/links/templates/links/components/delete-modal.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/components/navbar.html` & `django_short_links-0.1.4/links/templates/links/components/navbar.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/components/url.html` & `django_short_links-0.1.4/links/templates/links/components/url.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/create.html` & `django_short_links-0.1.4/links/templates/links/create.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/delete.html` & `django_short_links-0.1.4/links/templates/links/delete.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/detail.html` & `django_short_links-0.1.4/links/templates/links/detail.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/index.html` & `django_short_links-0.1.4/links/templates/links/index.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/list.html` & `django_short_links-0.1.4/links/templates/links/list.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/links/update.html` & `django_short_links-0.1.4/links/templates/links/update.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/registration/logged_out.html` & `django_short_links-0.1.4/links/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/templates/registration/login.html` & `django_short_links-0.1.4/links/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/urls.py` & `django_short_links-0.1.4/links/urls.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/links/views.py` & `django_short_links-0.1.4/links/views.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/pyproject.toml` & `django_short_links-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-short-links"
-version = "0.1.3"
+version = "0.1.4"
 description = "URL shortener Django app"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "links" }]
 homepage = "https://github.com/youzarsiph/django-short-links/"
 repository = "https://github.com/youzarsiph/django-short-links/"
```

### Comparing `django_short_links-0.1.3/README.md` & `django_short_links-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.3/PKG-INFO` & `django_short_links-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-short-links
-Version: 0.1.3
+Version: 0.1.4
 Summary: URL shortener Django app
 Home-page: https://github.com/youzarsiph/django-short-links/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

