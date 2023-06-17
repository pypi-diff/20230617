# Comparing `tmp/django_short_links-0.1.2.tar.gz` & `tmp/django_short_links-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_short_links-0.1.2.tar", max compression
+gzip compressed data, was "django_short_links-0.1.3.tar", max compression
```

## Comparing `django_short_links-0.1.2.tar` & `django_short_links-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,27 @@
--rw-r--r--   0        0        0     1095 2022-08-21 12:14:58.898018 django_short_links-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2022-08-21 12:10:59.901587 django_short_links-0.1.2/links/__init__.py
--rw-r--r--   0        0        0      167 2023-06-12 11:03:25.902464 django_short_links-0.1.2/links/admin.py
--rw-r--r--   0        0        0      218 2023-06-12 13:20:44.527009 django_short_links-0.1.2/links/apps.py
--rw-r--r--   0        0        0      228 2023-06-12 11:03:47.298696 django_short_links-0.1.2/links/forms.py
--rw-r--r--   0        0        0      849 2023-06-13 10:30:17.657675 django_short_links-0.1.2/links/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-12 10:57:28.904816 django_short_links-0.1.2/links/migrations/__init__.py
--rw-r--r--   0        0        0      654 2023-06-13 10:25:49.830518 django_short_links-0.1.2/links/models.py
--rw-r--r--   0        0        0      982 2023-06-12 12:33:21.684915 django_short_links-0.1.2/links/templates/links/base.html
--rw-r--r--   0        0        0     1719 2023-06-13 10:46:10.589864 django_short_links-0.1.2/links/templates/links/detail.html
--rw-r--r--   0        0        0     1879 2023-06-13 14:23:34.656752 django_short_links-0.1.2/links/templates/links/index.html
--rw-r--r--   0        0        0       84 2023-02-06 09:50:24.122941 django_short_links-0.1.2/links/tests.py
--rw-r--r--   0        0        0      416 2023-06-12 13:18:46.120022 django_short_links-0.1.2/links/urls.py
--rw-r--r--   0        0        0     1974 2023-06-13 10:44:53.464487 django_short_links-0.1.2/links/views.py
--rw-r--r--   0        0        0      524 2023-06-13 12:23:10.526038 django_short_links-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      753 2023-06-13 12:22:40.155650 django_short_links-0.1.2/README.md
--rw-r--r--   0        0        0     1372 1970-01-01 00:00:00.000000 django_short_links-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-06-13 14:31:22.286365 django_short_links-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-13 14:31:22.287366 django_short_links-0.1.3/links/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-13 14:31:22.288380 django_short_links-0.1.3/links/admin.py
+-rw-r--r--   0        0        0      218 2023-06-13 14:31:22.288380 django_short_links-0.1.3/links/apps.py
+-rw-r--r--   0        0        0      849 2023-06-13 14:31:22.290365 django_short_links-0.1.3/links/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-13 14:31:22.290365 django_short_links-0.1.3/links/migrations/__init__.py
+-rw-r--r--   0        0        0      347 2023-06-16 15:03:04.978367 django_short_links-0.1.3/links/mixins.py
+-rw-r--r--   0        0        0      841 2023-06-16 15:03:04.979367 django_short_links-0.1.3/links/models.py
+-rw-r--r--   0        0        0      982 2023-06-13 14:31:22.292365 django_short_links-0.1.3/links/templates/links/base.html
+-rw-r--r--   0        0        0     1466 2023-06-16 15:03:04.980889 django_short_links-0.1.3/links/templates/links/components/delete-modal.html
+-rw-r--r--   0        0        0      426 2023-06-16 15:03:04.980889 django_short_links-0.1.3/links/templates/links/components/messages.html
+-rw-r--r--   0        0        0     2550 2023-06-17 05:38:24.473941 django_short_links-0.1.3/links/templates/links/components/navbar.html
+-rw-r--r--   0        0        0     3038 2023-06-16 15:03:04.986904 django_short_links-0.1.3/links/templates/links/components/url.html
+-rw-r--r--   0        0        0     1094 2023-06-16 15:03:04.986904 django_short_links-0.1.3/links/templates/links/create.html
+-rw-r--r--   0        0        0     1082 2023-06-16 15:03:04.987902 django_short_links-0.1.3/links/templates/links/delete.html
+-rw-r--r--   0        0        0     3008 2023-06-16 15:03:04.989904 django_short_links-0.1.3/links/templates/links/detail.html
+-rw-r--r--   0        0        0     3223 2023-06-16 15:03:04.990898 django_short_links-0.1.3/links/templates/links/index.html
+-rw-r--r--   0        0        0     2241 2023-06-16 15:03:04.990898 django_short_links-0.1.3/links/templates/links/list.html
+-rw-r--r--   0        0        0     1330 2023-06-16 15:03:04.991896 django_short_links-0.1.3/links/templates/links/update.html
+-rw-r--r--   0        0        0      712 2023-06-16 15:03:04.991896 django_short_links-0.1.3/links/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     2214 2023-06-16 15:03:04.992898 django_short_links-0.1.3/links/templates/registration/login.html
+-rw-r--r--   0        0        0       84 2023-06-13 14:31:22.293366 django_short_links-0.1.3/links/tests.py
+-rw-r--r--   0        0        0      640 2023-06-16 15:03:04.992898 django_short_links-0.1.3/links/urls.py
+-rw-r--r--   0        0        0     3222 2023-06-17 05:38:24.474928 django_short_links-0.1.3/links/views.py
+-rw-r--r--   0        0        0      524 2023-06-17 05:41:08.726089 django_short_links-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      915 2023-06-17 05:38:24.471929 django_short_links-0.1.3/README.md
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 django_short_links-0.1.3/PKG-INFO
```

### Comparing `django_short_links-0.1.2/LICENSE` & `django_short_links-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.2/links/migrations/0001_initial.py` & `django_short_links-0.1.3/links/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.2/links/templates/links/base.html` & `django_short_links-0.1.3/links/templates/links/base.html`

 * *Files identical despite different names*

### Comparing `django_short_links-0.1.2/links/templates/links/detail.html` & `django_short_links-0.1.3/links/templates/links/detail.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,80 @@
 {% extends 'links/index.html' %}
 {% load i18n %}
 {% block title %}{% translate 'Links | URL details' %}{% endblock %}
 {% block content %}
 <h2 class="mb-4">
-  {% translate 'Success!' %}
+  {% translate 'Link Details' %}
 </h2>
-<p class="lead">
-  {% translate 'Your URL shortened' %}
-</p>
-<div class="card card-body p-4 rounded-4 shadow">
-  <h3 class="card-title">Shortened URL</h3>
-  <p class="card-text lead">
-    {{ site_url }}{% url 'links:redirect' url.token %}
-  </p>
-  <div class="d-grid d-md-flex align-items-center justify-content-lg-around gap-4">
-    <button id="copy-btn" type="button" onclick="inform()" class="btn btn-lg btn-primary w-100"
+<div class="card card-body p-4 rounded-4 border-0">
+  <h3 class="card-title mb-4">{{ url.url }}</h3>
+  <div
+    class="card card-body p-4 rounded-4 d-flex flex-row align-items-center justify-content-between gap-4 bg-light border-0 mb-4">
+    <p class="mb-0">{{ site_url }}{% url 'links:redirect' url.token %}</p>
+    <button id="copy-btn" type="button" onclick="inform()" class="btn btn-outline-dark shadow-sm rounded-3 fw-bold"
       data-clipboard-text="{{ site_url }}{% url 'links:redirect' url.token %}">
-      <i class="bi bi-clipboard me-3"></i>
-      {% translate 'Copy' %}
+      <i class="bi bi-clipboard"></i>
     </button>
-    <a class="btn btn-lg btn-success w-100" href="{% url 'links:redirect' url.token %}" target="_blank">
+  </div>
+  <ul class="list-unstyled mb-4">
+    <li>
+      <small class="text-muted">
+        {% translate 'Clicks: ' %} {{ url.clicks }}
+      </small>
+    </li>
+    <li>
+      <small class="text-muted">
+        {% translate 'Created: ' %} {{ url.created_at }}
+      </small>
+    </li>
+    <li>
+      <small class="text-muted">
+        {% translate 'Last update: ' %} {{ url.updated_at }}
+      </small>
+    </li>
+  </ul>
+  <div class="d-grid d-md-flex align-items-center justify-content-lg-around gap-4">
+    <a class="btn btn-lg btn-success w-100 shadow-sm rounded-3 fw-bold" target="_blank"
+      href="{% url 'links:redirect' url.token %}">
       <i class="bi bi-check-lg me-3"></i>
       {% translate 'Verify' %}
     </a>
-    <a class="btn btn-lg btn-dark w-100" href="{% url 'links:index' %}">
-      <i class="bi bi-house me-3"></i>
-      {% translate 'Home' %}
+    {% if request.user == url.user %}
+    <a class="btn btn-lg btn-light w-100 shadow-sm rounded-3 fw-bold" href="{% url 'links:update_url' url.id %}">
+      <i class="bi bi-pencil me-3"></i>
+      {% translate 'Change token' %}
     </a>
+    <button class="btn btn-lg btn-danger w-100 shadow-sm rounded-3 fw-bold" data-bs-toggle="modal"
+      data-bs-target="#deleteModal" onclick="onClick('{{ url.id }}')">
+      <i class="bi bi-trash me-3"></i>
+      {% translate 'Delete' %}
+    </button>
+    {% endif %}
   </div>
 </div>
+
+{% include 'links/components/delete-modal.html' %}
 {% endblock %}
 {% block footer %}
 <script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.11/clipboard.min.js"
   integrity="sha512-7O5pXpc0oCRrxk8RUfDYFgn0nO1t+jLuIOQdOMRp4APB7uZ4vSjspzp5y6YDtDs4VzUSTbWzBFZ/LKJhnyFOKw=="
   crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 <script>
   const copyBtn = new ClipboardJS('#copy-btn')
 
   const btn = document.getElementById('copy-btn')
 
-  const inform = () => btn.innerHTML = '<i class="bi bi-clipboard-check me-4"></i> {% translate "Copied" %}'
+  const inform = () => {
+    btn.innerHTML = '<i class="bi bi-clipboard-check-fill text-success"></i>'
+
+    setTimeout(() => {
+      btn.innerHTML = '<i class="bi bi-clipboard"></i>'
+    }, 2000);
+  }
+
+  const onClick = (id) => {
+    const form = document.getElementById('deleteForm')
+    form.setAttribute('action', form.getAttribute('action').replace(form.getAttribute('data-last-id'), id))
+    form.setAttribute('data-last-id', id)
+  }
 </script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,12 +1,16 @@
 {% extends 'links/index.html' %} {% load i18n %} {% block title %}{% translate
 'Links | URL details' %}{% endblock %} {% block content %}
-***** {% translate 'Success!' %} *****
-{% translate 'Your URL shortened' %}
-**** Shortened URL ****
+***** {% translate 'Link Details' %} *****
+**** {{ url.url }} ****
 {{ site_url }}{% url 'links:redirect' url.token %}
-  {% translate 'Copy' %}
- {%_translate_'Verify'_%}
 
- {%_translate_'Home'_%}
-{% endblock %} {% block footer %}
+    * {% translate 'Clicks: ' %} {{ url.clicks }}
+    * {% translate 'Created: ' %} {{ url.created_at }}
+    * {% translate 'Last update: ' %} {{ url.updated_at }}
+ {%_translate_'Verify'_%}
+ {% if request.user == url.user %}
+ {%_translate_'Change_token'_%}
+   {% translate 'Delete' %}  {% endif %}
+{% include 'links/components/delete-modal.html' %} {% endblock %} {% block
+footer %}
  {% endblock %}
```

### Comparing `django_short_links-0.1.2/links/templates/links/index.html` & `django_short_links-0.1.3/links/templates/registration/login.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,63 @@
-{% extends 'links/base.html' %} {% load i18n %}
-{% block title %}{% translate 'Links | URL shortener' %}{% endblock %}
-{% block body_attrs %}class="overflow-hidden"{% endblock %}
-{% block main %}
-<div class="container d-flex align-items-center justify-content-between overflow-hidden" style="height: 100vh">
-  <div class="w-100">
-    <h1 class="display-1 fw-bold mb-4">
-      <a href="{% url 'links:index' %}" class="text-decoration-none">
-        {% translate 'Links' %}
-      </a>
+{% extends 'links/index.html' %}
+{% load i18n %}
+{% block title %}{% translate 'Links | Login' %}{% endblock %}
+{% block content %}
+<div class="d-flex align-items-center justify-content-center">
+  <div class="col-12 col-md-6 col-lg-4">
+    <h1 class="display-1 mb-4">
+      {% translate 'Links' %}
     </h1>
-    {% block content %}
-    <p class="lead mb-4">
+    {% if next %}
+    {% if user.is_authenticated %}
+    <p>
       {% blocktranslate %}
-      A Django app that allows users to shorten long urls.
+      Your account doesn't have access to this page. To proceed,
+      please login with an account that has access.
       {% endblocktranslate %}
     </p>
-    {% if form.errors %}
-    <div class="text-white p-3 border rounded-3" role="alert">
-      {{ form.errors }}
-    </div>
+    {% else %}
+    <p>
+      {% translate 'Please login to see this page.' %}
+    </p>
+    {% endif %}
     {% endif %}
-    <div class="card card-body p-4 rounded-4 shadow mb-5">
-      <h2 class="mb-4">Shorten URL</h2>
-      <form method="post" action="{% url 'links:create_url' %}">
+    <div class="card card-body p-4 border-0 rounded-4">
+      <h2 class="mb-4">{% translate 'Login' %}</h2>
+      <p class="lead mb-4 text-center">
+        {% translate 'Login to start using Links' %}
+      </p>
+      {% if form.errors %}
+      <div class="alert alert-danger rounded-4 shadow-sm" role="alert">
+        <div class="badge bg-danger">{% translate 'Error' %}</div>
+        {% translate 'Please enter a correct username and password. Note that both fields may be case-sensitive.' %}
+      </div>
+      {% endif %}
+      <form method="post">
         {% csrf_token %}
+        <input type="hidden" name="next" value="{{ next }}">
+        <div class="form-floating mb-4">
+          {{ form.username }}
+          {{ form.username.label_tag }}
+          <small class="text-muted">
+            {{ form.username.help_text }}
+          </small>
+        </div>
         <div class="form-floating mb-4">
-          <input type="url" name="url" maxlength="200" required id="id_url" placeholder="{% translate 'URL' %}"
-            class="form-control" value="{{ url.value }}">
-          <label for="id_url" class="form-label">
-            {% translate 'URL' %}
-          </label>
-          <small>
-            {% translate 'The URL to be shortened' %}
+          {{ form.password }}
+          {{ form.password.label_tag }}
+          <small class="text-muted">
+            {{ form.password.help_text }}
           </small>
         </div>
-        <button type="submit" class="btn btn-lg btn-primary w-100">
-          <i class="bi bi-scissors me-3"></i>
-          {% translate 'Cut' %}
+        <button type="submit" class="btn btn-lg btn-dark shadow-sm rounded-3 fw-bold w-100">
+          {% translate 'Submit' %}
         </button>
       </form>
     </div>
-    <a class="btn btn-lg btn-dark w-100" href="https://github.com/youzarsiph/django-links.git">
-      <i class="bi bi-github me-3"></i>
-      {% translate 'Github' %}
-    </a>
-    {% endblock %}
   </div>
 </div>
+<script>
+  document.querySelectorAll('form label').forEach(i => i.classList.add('form-label'))
+  document.querySelectorAll('form input').forEach(i => i.classList.add('form-control'))
+</script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,18 +1,21 @@
-{% extends 'links/base.html' %} {% load i18n %} {% block title %}{% translate
-'Links | URL shortener' %}{% endblock %} {% block body_attrs %}class="overflow-
-hidden"{% endblock %} {% block main %}
-****** {%_translate_'Links'_%} ******
-{% block content %}
-{% blocktranslate %} A Django app that allows users to shorten long urls. {%
-endblocktranslate %}
+{% extends 'links/index.html' %} {% load i18n %} {% block title %}{% translate
+'Links | Login' %}{% endblock %} {% block content %}
+****** {% translate 'Links' %} ******
+{% if next %} {% if user.is_authenticated %}
+{% blocktranslate %} Your account doesn't have access to this page. To proceed,
+please login with an account that has access. {% endblocktranslate %}
+{% else %}
+{% translate 'Please login to see this page.' %}
+{% endif %} {% endif %}
+***** {% translate 'Login' %} *****
+{% translate 'Login to start using Links' %}
 {% if form.errors %}
-{{ form.errors }}
+{% translate 'Error' %}
+{% translate 'Please enter a correct username and password. Note that both
+fields may be case-sensitive.' %}
 {% endif %}
-***** Shorten URL *****
 {% csrf_token %}
-[Unknown INPUT type]  {% translate 'URL' %}  {% translate 'The URL to be
-shortened' %}
-  {% translate 'Cut' %}
- {%_translate_'Github'_%}
+{{ form.username }} {{ form.username.label_tag }} {{ form.username.help_text }}
+{{ form.password }} {{ form.password.label_tag }} {{ form.password.help_text }}
+ {% translate 'Submit' %}
  {% endblock %}
-{% endblock %}
```

### Comparing `django_short_links-0.1.2/links/views.py` & `django_short_links-0.1.3/links/views.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,106 @@
 """ Views """
 
 
 import secrets
+from typing import Any
 
 from django.conf import settings
+from django.views import generic
 from django.urls import reverse_lazy
 from django.shortcuts import redirect
-from django.views.generic import TemplateView, CreateView, DetailView
+from django.forms.forms import BaseForm
+from django.http import HttpRequest, HttpResponse
+from django.contrib.auth.mixins import LoginRequiredMixin
+from django.contrib.messages.views import SuccessMessageMixin
 
-from links.forms import URLForm
 from links.models import URL
+from links.mixins import UserFilterMixin
 
 
 # Create your views here.
-class Index(TemplateView):
+class Index(generic.TemplateView):
     """ Index page """
 
     template_name = 'links/index.html'
-    extra_context = {'form': URLForm()}
 
 
-class URLCreateView(CreateView):
+class URLCreateView(LoginRequiredMixin, SuccessMessageMixin, generic.CreateView):
     """ URL CreateView """
 
     model = URL
-    form_class = URLForm
-    template_name = "links/index.html"
-    success_url = reverse_lazy('links:index')
+    fields = ['url']
+    template_name = "links/create.html"
+    success_url = reverse_lazy('links:url_list')
+    success_message = 'Link was created successfully'
 
-    def post(self, request, *args, **kwargs):
+    def post(self, request: HttpRequest, *args: str, **kwargs: Any) -> HttpResponse:
         """ Redirect to details or create new instance """
 
         try:
             url = URL.objects.get(url=request.POST['url'])
-            return redirect(reverse_lazy('links:url_detail', args=[url.id]))
+            return redirect(reverse_lazy('links:url_detail', args=[url.pk]))
 
         except URL.DoesNotExist:
             return super().post(request, *args, **kwargs)
 
-    def form_valid(self, form):
+    def form_valid(self, form: BaseForm) -> HttpResponse:
         """ Compute the shortened url """
 
         # Create a url object
-        instance = form.save(commit=False)
+        instance: URL = form.save(commit=False)
 
-        # Set url token
+        # Set the owner and url token
+        instance.user = self.request.user
         instance.token = secrets.token_urlsafe(7)
 
         # Save the object
         instance.save()
         return super().form_valid(form)
 
-    def get_success_url(self) -> str:
-        return reverse_lazy('links:url_detail', args=[self.object.id])
 
+class URLListView(LoginRequiredMixin, UserFilterMixin, generic.ListView):
+    """ URL List view """
 
-class URLDetailView(DetailView):
+    model = URL
+    template_name = 'links/list.html'
+    extra_context = {'site_url': settings.LINKS_SITE_URL}
+
+
+class URLDetailView(LoginRequiredMixin, UserFilterMixin, generic.DetailView):
     """ URL Details """
 
     model = URL
     pk_url_kwarg = 'id'
     template_name = 'links/detail.html'
     extra_context = {'site_url': settings.LINKS_SITE_URL}
 
 
-class ServeURL(DetailView):
+class URLUpdateView(LoginRequiredMixin, UserFilterMixin, SuccessMessageMixin, generic.UpdateView):
+    """ URL Update View """
+
+    model = URL
+    pk_url_kwarg = 'id'
+    fields = ['token', 'url']
+    template_name = 'links/update.html'
+    success_url = reverse_lazy('links:url_list')
+    success_message = 'Link was updated successfully'
+
+
+class URLDeleteView(LoginRequiredMixin, UserFilterMixin, SuccessMessageMixin, generic.DeleteView):
+    """ URL Delete View """
+
+    model = URL
+    pk_url_kwarg = 'id'
+    template_name = 'links/delete.html'
+    success_url = reverse_lazy('links:url_list')
+    success_message = 'Link was deleted successfully'
+
+
+class ServeURL(generic.DetailView):
     """ Redirect URLs """
 
     model = URL
     slug_field = 'token'
 
     def get(self, request, *args, **kwargs):
         """ Redirect urls """
```

### Comparing `django_short_links-0.1.2/pyproject.toml` & `django_short_links-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-short-links"
-version = "0.1.2"
+version = "0.1.3"
 description = "URL shortener Django app"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "links" }]
 homepage = "https://github.com/youzarsiph/django-short-links/"
 repository = "https://github.com/youzarsiph/django-short-links/"
```

### Comparing `django_short_links-0.1.2/README.md` & `django_short_links-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,37 +6,39 @@
 
 Install `links`:
 
 ```shell
 pip install django-short-links
 ```
 
-Add `links` to `INSTALLED_APPS` and add a new setting `LINKS_SITE_NAME`, in `settings.py`:
+Add `links` to `INSTALLED_APPS`. Make sure that `django.contrib.auth` installed, then add a new setting `LINKS_SITE_NAME`, in `settings.py`:
 
 ```python
 # settings.py
 
 INSTALLED_APPS = [
     ...
     'links',
+    'django.contrib.auth',
     ...
 ]
 
 # Your server's IP address without trailing slash
 LINKS_SITE_URL = 'https://your.domain.com'
 ```
 
-Include `links` URLConf, in project's `urls.py`:
+Include `links` and `django.contrib.auth.urls`, in project's `urls.py`:
 
 ```python
 # urls.py
 
 urlpatterns = [
     ...
     path('l/', include('links.urls')),
+    path('accounts/', include('django.contrib.auth.urls')),
     ...
 ]
 ```
 
 Run `migrate`:
 
 ```shell
```

### Comparing `django_short_links-0.1.2/PKG-INFO` & `django_short_links-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-short-links
-Version: 0.1.2
+Version: 0.1.3
 Summary: URL shortener Django app
 Home-page: https://github.com/youzarsiph/django-short-links/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -24,37 +24,39 @@
 
 Install `links`:
 
 ```shell
 pip install django-short-links
 ```
 
-Add `links` to `INSTALLED_APPS` and add a new setting `LINKS_SITE_NAME`, in `settings.py`:
+Add `links` to `INSTALLED_APPS`. Make sure that `django.contrib.auth` installed, then add a new setting `LINKS_SITE_NAME`, in `settings.py`:
 
 ```python
 # settings.py
 
 INSTALLED_APPS = [
     ...
     'links',
+    'django.contrib.auth',
     ...
 ]
 
 # Your server's IP address without trailing slash
 LINKS_SITE_URL = 'https://your.domain.com'
 ```
 
-Include `links` URLConf, in project's `urls.py`:
+Include `links` and `django.contrib.auth.urls`, in project's `urls.py`:
 
 ```python
 # urls.py
 
 urlpatterns = [
     ...
     path('l/', include('links.urls')),
+    path('accounts/', include('django.contrib.auth.urls')),
     ...
 ]
 ```
 
 Run `migrate`:
 
 ```shell
```

