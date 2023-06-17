# Comparing `tmp/django_short_links-0.1.4.tar.gz` & `tmp/django_short_links-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_short_links-0.1.4.tar", max compression
+gzip compressed data, was "django_short_links-0.1.5.tar", max compression
```

## Comparing `django_short_links-0.1.4.tar` & `django_short_links-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1095 2023-06-13 14:31:22.286365 django_short_links-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2023-06-13 14:31:22.287366 django_short_links-0.1.4/links/__init__.py
--rw-r--r--   0        0        0      167 2023-06-13 14:31:22.288380 django_short_links-0.1.4/links/admin.py
--rw-r--r--   0        0        0      218 2023-06-13 14:31:22.288380 django_short_links-0.1.4/links/apps.py
--rw-r--r--   0        0        0      849 2023-06-13 14:31:22.290365 django_short_links-0.1.4/links/migrations/0001_initial.py
--rw-r--r--   0        0        0     1057 2023-06-17 05:54:23.066017 django_short_links-0.1.4/links/migrations/0002_url_user_alter_url_token_alter_url_url.py
--rw-r--r--   0        0        0        0 2023-06-13 14:31:22.290365 django_short_links-0.1.4/links/migrations/__init__.py
--rw-r--r--   0        0        0      347 2023-06-16 15:03:04.978367 django_short_links-0.1.4/links/mixins.py
--rw-r--r--   0        0        0      841 2023-06-16 15:03:04.979367 django_short_links-0.1.4/links/models.py
--rw-r--r--   0        0        0      982 2023-06-13 14:31:22.292365 django_short_links-0.1.4/links/templates/links/base.html
--rw-r--r--   0        0        0     1466 2023-06-16 15:03:04.980889 django_short_links-0.1.4/links/templates/links/components/delete-modal.html
--rw-r--r--   0        0        0      426 2023-06-16 15:03:04.980889 django_short_links-0.1.4/links/templates/links/components/messages.html
--rw-r--r--   0        0        0     2550 2023-06-17 05:38:24.473941 django_short_links-0.1.4/links/templates/links/components/navbar.html
--rw-r--r--   0        0        0     3038 2023-06-16 15:03:04.986904 django_short_links-0.1.4/links/templates/links/components/url.html
--rw-r--r--   0        0        0     1094 2023-06-16 15:03:04.986904 django_short_links-0.1.4/links/templates/links/create.html
--rw-r--r--   0        0        0     1082 2023-06-16 15:03:04.987902 django_short_links-0.1.4/links/templates/links/delete.html
--rw-r--r--   0        0        0     3008 2023-06-16 15:03:04.989904 django_short_links-0.1.4/links/templates/links/detail.html
--rw-r--r--   0        0        0     3223 2023-06-16 15:03:04.990898 django_short_links-0.1.4/links/templates/links/index.html
--rw-r--r--   0        0        0     2241 2023-06-16 15:03:04.990898 django_short_links-0.1.4/links/templates/links/list.html
--rw-r--r--   0        0        0     1330 2023-06-16 15:03:04.991896 django_short_links-0.1.4/links/templates/links/update.html
--rw-r--r--   0        0        0      712 2023-06-16 15:03:04.991896 django_short_links-0.1.4/links/templates/registration/logged_out.html
--rw-r--r--   0        0        0     2214 2023-06-16 15:03:04.992898 django_short_links-0.1.4/links/templates/registration/login.html
--rw-r--r--   0        0        0       84 2023-06-13 14:31:22.293366 django_short_links-0.1.4/links/tests.py
--rw-r--r--   0        0        0      640 2023-06-16 15:03:04.992898 django_short_links-0.1.4/links/urls.py
--rw-r--r--   0        0        0     3222 2023-06-17 05:38:24.474928 django_short_links-0.1.4/links/views.py
--rw-r--r--   0        0        0      524 2023-06-17 05:56:38.204246 django_short_links-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      915 2023-06-17 05:38:24.471929 django_short_links-0.1.4/README.md
--rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 django_short_links-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-06-13 14:31:22.286365 django_short_links-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-13 14:31:22.287366 django_short_links-0.1.5/links/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-13 14:31:22.288380 django_short_links-0.1.5/links/admin.py
+-rw-r--r--   0        0        0      218 2023-06-13 14:31:22.288380 django_short_links-0.1.5/links/apps.py
+-rw-r--r--   0        0        0      849 2023-06-13 14:31:22.290365 django_short_links-0.1.5/links/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1057 2023-06-17 05:54:23.066017 django_short_links-0.1.5/links/migrations/0002_url_user_alter_url_token_alter_url_url.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:31:22.290365 django_short_links-0.1.5/links/migrations/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-16 15:03:04.978367 django_short_links-0.1.5/links/mixins.py
+-rw-r--r--   0        0        0      841 2023-06-16 15:03:04.979367 django_short_links-0.1.5/links/models.py
+-rw-r--r--   0        0        0      982 2023-06-13 14:31:22.292365 django_short_links-0.1.5/links/templates/links/base.html
+-rw-r--r--   0        0        0     1466 2023-06-16 15:03:04.980889 django_short_links-0.1.5/links/templates/links/components/delete-modal.html
+-rw-r--r--   0        0        0      426 2023-06-16 15:03:04.980889 django_short_links-0.1.5/links/templates/links/components/messages.html
+-rw-r--r--   0        0        0     2550 2023-06-17 05:38:24.473941 django_short_links-0.1.5/links/templates/links/components/navbar.html
+-rw-r--r--   0        0        0     3054 2023-06-17 06:12:16.687188 django_short_links-0.1.5/links/templates/links/components/url.html
+-rw-r--r--   0        0        0     1094 2023-06-16 15:03:04.986904 django_short_links-0.1.5/links/templates/links/create.html
+-rw-r--r--   0        0        0     1082 2023-06-16 15:03:04.987902 django_short_links-0.1.5/links/templates/links/delete.html
+-rw-r--r--   0        0        0     3075 2023-06-17 06:18:29.858148 django_short_links-0.1.5/links/templates/links/detail.html
+-rw-r--r--   0        0        0     3223 2023-06-16 15:03:04.990898 django_short_links-0.1.5/links/templates/links/index.html
+-rw-r--r--   0        0        0     2297 2023-06-17 06:15:07.597850 django_short_links-0.1.5/links/templates/links/list.html
+-rw-r--r--   0        0        0     1330 2023-06-16 15:03:04.991896 django_short_links-0.1.5/links/templates/links/update.html
+-rw-r--r--   0        0        0      712 2023-06-16 15:03:04.991896 django_short_links-0.1.5/links/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     2214 2023-06-16 15:03:04.992898 django_short_links-0.1.5/links/templates/registration/login.html
+-rw-r--r--   0        0        0       84 2023-06-13 14:31:22.293366 django_short_links-0.1.5/links/tests.py
+-rw-r--r--   0        0        0      640 2023-06-16 15:03:04.992898 django_short_links-0.1.5/links/urls.py
+-rw-r--r--   0        0        0     3222 2023-06-17 05:38:24.474928 django_short_links-0.1.5/links/views.py
+-rw-r--r--   0        0        0      524 2023-06-17 06:20:30.939590 django_short_links-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      915 2023-06-17 05:38:24.471929 django_short_links-0.1.5/README.md
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 django_short_links-0.1.5/PKG-INFO
```

### Comparing `django_short_links-0.1.4/LICENSE` & `django_short_links-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/migrations/0001_initial.py` & `django_short_links-0.1.5/links/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/migrations/0002_url_user_alter_url_token_alter_url_url.py` & `django_short_links-0.1.5/links/migrations/0002_url_user_alter_url_token_alter_url_url.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/models.py` & `django_short_links-0.1.5/links/models.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/templates/links/base.html` & `django_short_links-0.1.5/links/templates/links/base.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/templates/links/components/delete-modal.html` & `django_short_links-0.1.5/links/templates/links/components/delete-modal.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/templates/links/components/navbar.html` & `django_short_links-0.1.5/links/templates/links/components/navbar.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/templates/links/components/url.html` & `django_short_links-0.1.5/links/templates/links/components/url.html`

 * *Files 6% similar despite different names*

```diff
@@ -66,16 +66,17 @@
       <li>
         <small class="text-muted">
           {% translate 'Last update: ' %} {{ url.updated_at }}
         </small>
       </li>
     </ul>
   </div>
-  <div class="card card-body p-4 rounded-4 d-flex flex-row align-items-center justify-content-between gap-4 bg-light border-0">
+  <div class="card card-body p-4 rounded-4 justify-content-between gap-4 bg-light border-0 overflow-x-auto">
     <p class="mb-0">{{ site_url }}{% url 'links:redirect' url.token %}</p>
     <button id="copy-btn-{{ url.id }}" type="button" onclick="inform('copy-btn-{{ url.id }}')"
       class="btn btn-outline-dark shadow-sm rounded-3 fw-bold"
       data-clipboard-text="{{ site_url }}{% url 'links:redirect' url.token %}">
-      <i class="bi bi-clipboard"></i>
+      <i class="bi bi-clipboard me-3"></i>
+      {% translate 'Copy' %}
     </button>
   </div>
 </div>
```

#### html2text {}

```diff
@@ -6,8 +6,8 @@
     *   {%_translate_'Edit_link'_%}
     *   {%_translate_'Delete_link'_%}
 {{ url.url }}
     * {% translate 'Clicks: ' %} {{ url.clicks }}
     * {% translate 'Created: ' %} {{ url.created_at }}
     * {% translate 'Last update: ' %} {{ url.updated_at }}
 {{ site_url }}{% url 'links:redirect' url.token %}
-
+  {% translate 'Copy' %}
```

### Comparing `django_short_links-0.1.4/links/templates/links/create.html` & `django_short_links-0.1.5/links/templates/links/create.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/templates/links/delete.html` & `django_short_links-0.1.5/links/templates/links/delete.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/templates/links/detail.html` & `django_short_links-0.1.5/links/templates/links/detail.html`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 {% block title %}{% translate 'Links | URL details' %}{% endblock %}
 {% block content %}
 <h2 class="mb-4">
   {% translate 'Link Details' %}
 </h2>
 <div class="card card-body p-4 rounded-4 border-0">
   <h3 class="card-title mb-4">{{ url.url }}</h3>
-  <div
-    class="card card-body p-4 rounded-4 d-flex flex-row align-items-center justify-content-between gap-4 bg-light border-0 mb-4">
+  <div class="card card-body p-4 rounded-4 justify-content-between gap-4 bg-light border-0 mb-4 overflow-x-auto">
     <p class="mb-0">{{ site_url }}{% url 'links:redirect' url.token %}</p>
     <button id="copy-btn" type="button" onclick="inform()" class="btn btn-outline-dark shadow-sm rounded-3 fw-bold"
       data-clipboard-text="{{ site_url }}{% url 'links:redirect' url.token %}">
-      <i class="bi bi-clipboard"></i>
+      <i class="bi bi-clipboard me-3"></i>
+      {% translate 'Copy' %}
     </button>
   </div>
   <ul class="list-unstyled mb-4">
     <li>
       <small class="text-muted">
         {% translate 'Clicks: ' %} {{ url.clicks }}
       </small>
@@ -60,18 +60,18 @@
   crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script>
   const copyBtn = new ClipboardJS('#copy-btn')
 
   const btn = document.getElementById('copy-btn')
 
   const inform = () => {
-    btn.innerHTML = '<i class="bi bi-clipboard-check-fill text-success"></i>'
+    btn.innerHTML = '<i class="bi bi-clipboard-check-fill me-3 text-success"></i> <span class="text-success">Copied</span>'
 
     setTimeout(() => {
-      btn.innerHTML = '<i class="bi bi-clipboard"></i>'
+      btn.innerHTML = '<i class="bi bi-clipboard me-3"></i> Copy'
     }, 2000);
   }
 
   const onClick = (id) => {
     const form = document.getElementById('deleteForm')
     form.setAttribute('action', form.getAttribute('action').replace(form.getAttribute('data-last-id'), id))
     form.setAttribute('data-last-id', id)
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 {% extends 'links/index.html' %} {% load i18n %} {% block title %}{% translate
 'Links | URL details' %}{% endblock %} {% block content %}
 ***** {% translate 'Link Details' %} *****
 **** {{ url.url }} ****
 {{ site_url }}{% url 'links:redirect' url.token %}
-
+  {% translate 'Copy' %}
     * {% translate 'Clicks: ' %} {{ url.clicks }}
     * {% translate 'Created: ' %} {{ url.created_at }}
     * {% translate 'Last update: ' %} {{ url.updated_at }}
  {%_translate_'Verify'_%}
  {% if request.user == url.user %}
  {%_translate_'Change_token'_%}
    {% translate 'Delete' %}  {% endif %}
```

### Comparing `django_short_links-0.1.4/links/templates/links/index.html` & `django_short_links-0.1.5/links/templates/links/index.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/templates/links/list.html` & `django_short_links-0.1.5/links/templates/links/list.html`

 * *Files 9% similar despite different names*

```diff
@@ -42,18 +42,18 @@
   integrity="sha512-7O5pXpc0oCRrxk8RUfDYFgn0nO1t+jLuIOQdOMRp4APB7uZ4vSjspzp5y6YDtDs4VzUSTbWzBFZ/LKJhnyFOKw=="
   crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script>
   const inform = (id) => {
     const copyBtn = new ClipboardJS(`#${id}`)
 
     const btn = document.getElementById(id)
-    btn.innerHTML = '<i class="bi bi-clipboard-check-fill text-success"></i>'
+    btn.innerHTML = '<i class="bi bi-clipboard-check-fill me-3 text-success"></i> <span class="text-success">Copied</span>'
 
     setTimeout(() => {
-      btn.innerHTML = '<i class="bi bi-clipboard"></i>'
+      btn.innerHTML = '<i class="bi bi-clipboard me-3"></i> Copy'
     }, 2000);
   }
 
   const onClick = (id) => {
     const form = document.getElementById('deleteForm')
     form.setAttribute('action', form.getAttribute('action').replace(form.getAttribute('data-last-id'), id))
     form.setAttribute('data-last-id', id)
```

### Comparing `django_short_links-0.1.4/links/templates/links/update.html` & `django_short_links-0.1.5/links/templates/links/update.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/templates/registration/logged_out.html` & `django_short_links-0.1.5/links/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/templates/registration/login.html` & `django_short_links-0.1.5/links/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/urls.py` & `django_short_links-0.1.5/links/urls.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/links/views.py` & `django_short_links-0.1.5/links/views.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/pyproject.toml` & `django_short_links-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-short-links"
-version = "0.1.4"
+version = "0.1.5"
 description = "URL shortener Django app"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "links" }]
 homepage = "https://github.com/youzarsiph/django-short-links/"
 repository = "https://github.com/youzarsiph/django-short-links/"
```

### Comparing `django_short_links-0.1.4/README.md` & `django_short_links-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.4/PKG-INFO` & `django_short_links-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-short-links
-Version: 0.1.4
+Version: 0.1.5
 Summary: URL shortener Django app
 Home-page: https://github.com/youzarsiph/django-short-links/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

