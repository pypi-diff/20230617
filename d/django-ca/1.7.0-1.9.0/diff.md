# Comparing `tmp/django-ca-1.7.0.tar.gz` & `tmp/django-ca-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-ca-1.7.0.tar", last modified: Sun Dec 17 18:18:31 2017, max compression
+gzip compressed data, was "dist/django-ca-1.9.0.tar", last modified: Sat Aug 25 10:03:20 2018, max compression
```

## Comparing `django-ca-1.7.0.tar` & `django-ca-1.9.0.tar`

### file list

```diff
@@ -1,89 +1,93 @@
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/
--rw-r--r--   0 mati      (1000) mati      (1000)     1678 2017-12-09 13:57:06.000000 django-ca-1.7.0/README.md
--rw-rw-r--   0 mati      (1000) mati      (1000)    35147 2007-07-01 22:55:35.000000 django-ca-1.7.0/LICENSE
--rw-r--r--   0 mati      (1000) mati      (1000)     2133 2017-12-17 18:18:31.000000 django-ca-1.7.0/PKG-INFO
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca.egg-info/
--rw-r--r--   0 mati      (1000) mati      (1000)     2853 2017-12-17 18:18:30.000000 django-ca-1.7.0/ca/django_ca.egg-info/SOURCES.txt
--rw-r--r--   0 mati      (1000) mati      (1000)     2133 2017-12-17 18:18:30.000000 django-ca-1.7.0/ca/django_ca.egg-info/PKG-INFO
--rw-r--r--   0 mati      (1000) mati      (1000)        1 2017-12-17 18:18:30.000000 django-ca-1.7.0/ca/django_ca.egg-info/dependency_links.txt
--rw-r--r--   0 mati      (1000) mati      (1000)       86 2017-12-17 18:18:30.000000 django-ca-1.7.0/ca/django_ca.egg-info/requires.txt
--rw-r--r--   0 mati      (1000) mati      (1000)       10 2017-12-17 18:18:30.000000 django-ca-1.7.0/ca/django_ca.egg-info/top_level.txt
--rw-r--r--   0 mati      (1000) mati      (1000)        1 2017-02-26 13:41:27.000000 django-ca-1.7.0/ca/django_ca.egg-info/not-zip-safe
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/
--rw-r--r--   0 mati      (1000) mati      (1000)     1620 2017-12-09 11:42:55.000000 django-ca-1.7.0/ca/django_ca/urls.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1734 2017-12-03 19:57:32.000000 django-ca-1.7.0/ca/django_ca/querysets.py
--rw-r--r--   0 mati      (1000) mati      (1000)     6844 2017-07-18 09:52:43.000000 django-ca-1.7.0/ca/django_ca/widgets.py
--rw-r--r--   0 mati      (1000) mati      (1000)     8791 2017-12-09 18:21:57.000000 django-ca-1.7.0/ca/django_ca/forms.py
--rw-r--r--   0 mati      (1000) mati      (1000)    11250 2017-12-13 21:15:58.000000 django-ca-1.7.0/ca/django_ca/views.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1682 2017-03-04 22:12:30.000000 django-ca-1.7.0/ca/django_ca/ocsp.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/templatetags/
--rw-r--r--   0 mati      (1000) mati      (1000)     1016 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/templatetags/django_ca.py
--rw-r--r--   0 mati      (1000) mati      (1000)        0 2016-01-24 13:54:17.000000 django-ca-1.7.0/ca/django_ca/templatetags/__init__.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/static/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/js/
--rw-r--r--   0 mati      (1000) mati      (1000)     2973 2016-03-04 21:36:53.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/js/profilewidget.js
--rw-r--r--   0 mati      (1000) mati      (1000)     5637 2016-01-29 20:25:19.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/js/sign.js
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/css/
--rw-r--r--   0 mati      (1000) mati      (1000)       75 2016-01-24 14:43:14.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/css/labeledtextinput.css
--rw-r--r--   0 mati      (1000) mati      (1000)     1354 2017-12-09 12:53:46.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/css/base.css
--rw-r--r--   0 mati      (1000) mati      (1000)       37 2016-02-28 13:23:31.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/css/certificateauthorityadmin.css
--rw-r--r--   0 mati      (1000) mati      (1000)      817 2016-01-24 13:54:17.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/css/labeledcheckboxinput.css
--rw-r--r--   0 mati      (1000) mati      (1000)     1175 2017-12-09 12:53:49.000000 django-ca-1.7.0/ca/django_ca/static/django_ca/admin/css/certificateadmin.css
--rw-r--r--   0 mati      (1000) mati      (1000)      921 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/apps.py
--rw-r--r--   0 mati      (1000) mati      (1000)     2854 2017-12-08 14:03:51.000000 django-ca-1.7.0/ca/django_ca/crl.py
--rw-r--r--   0 mati      (1000) mati      (1000)    19190 2017-12-14 20:31:10.000000 django-ca-1.7.0/ca/django_ca/utils.py
--rw-r--r--   0 mati      (1000) mati      (1000)       53 2015-12-26 14:14:39.000000 django-ca-1.7.0/ca/django_ca/__init__.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/templates/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/admin/
--rw-r--r--   0 mati      (1000) mati      (1000)     2077 2016-04-21 18:48:24.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/admin/certificate_revoke_form.html
--rw-r--r--   0 mati      (1000) mati      (1000)      607 2016-01-24 13:54:17.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/admin/submit_line.html
--rw-r--r--   0 mati      (1000) mati      (1000)      147 2016-01-24 13:54:17.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/admin/change_form.html
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/forms/
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/forms/widgets/
--rw-r--r--   0 mati      (1000) mati      (1000)      157 2017-04-19 20:57:37.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/forms/widgets/labeledcheckboxinput.html
--rw-r--r--   0 mati      (1000) mati      (1000)      146 2017-04-19 21:11:25.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/forms/widgets/subjecttextinput.html
--rw-r--r--   0 mati      (1000) mati      (1000)      116 2017-04-19 20:57:32.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/forms/widgets/custommultiwidget.html
--rw-r--r--   0 mati      (1000) mati      (1000)      237 2017-04-19 21:13:10.000000 django-ca-1.7.0/ca/django_ca/templates/django_ca/forms/widgets/labeledtextinput.html
--rw-r--r--   0 mati      (1000) mati      (1000)    15759 2017-12-14 19:24:40.000000 django-ca-1.7.0/ca/django_ca/managers.py
--rw-r--r--   0 mati      (1000) mati      (1000)    15086 2017-12-09 17:10:32.000000 django-ca-1.7.0/ca/django_ca/admin.py
--rw-r--r--   0 mati      (1000) mati      (1000)     4540 2017-12-09 11:14:06.000000 django-ca-1.7.0/ca/django_ca/ca_settings.py
--rw-r--r--   0 mati      (1000) mati      (1000)     3240 2017-11-19 16:04:25.000000 django-ca-1.7.0/ca/django_ca/fields.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/migrations/
--rw-r--r--   0 mati      (1000) mati      (1000)     4420 2017-07-18 10:08:02.000000 django-ca-1.7.0/ca/django_ca/migrations/0001_initial.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1024 2017-07-18 10:08:02.000000 django-ca-1.7.0/ca/django_ca/migrations/0005_auto_20170307_1839.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1299 2017-07-18 10:08:02.000000 django-ca-1.7.0/ca/django_ca/migrations/0003_auto_20170304_1434.py
--rw-r--r--   0 mati      (1000) mati      (1000)      470 2017-07-18 10:08:02.000000 django-ca-1.7.0/ca/django_ca/migrations/0006_auto_20170505_1251.py
--rw-r--r--   0 mati      (1000) mati      (1000)        0 2017-07-18 10:07:18.000000 django-ca-1.7.0/ca/django_ca/migrations/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1187 2017-07-18 10:08:02.000000 django-ca-1.7.0/ca/django_ca/migrations/0002_auto_20170304_1434.py
--rw-r--r--   0 mati      (1000) mati      (1000)      617 2017-11-19 10:00:08.000000 django-ca-1.7.0/ca/django_ca/migrations/0007_auto_20171119_1100.py
--rw-r--r--   0 mati      (1000) mati      (1000)      993 2017-07-18 10:08:02.000000 django-ca-1.7.0/ca/django_ca/migrations/0004_auto_20170304_1442.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1291 2017-12-03 19:01:57.000000 django-ca-1.7.0/ca/django_ca/migrations/0008_auto_20171203_2001.py
--rw-r--r--   0 mati      (1000) mati      (1000)    16116 2017-12-14 20:22:35.000000 django-ca-1.7.0/ca/django_ca/models.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/management/
--rw-r--r--   0 mati      (1000) mati      (1000)    13357 2017-12-09 17:32:53.000000 django-ca-1.7.0/ca/django_ca/management/base.py
--rw-r--r--   0 mati      (1000) mati      (1000)        0 2015-12-22 10:19:07.000000 django-ca-1.7.0/ca/django_ca/management/__init__.py
-drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2017-12-17 18:18:31.000000 django-ca-1.7.0/ca/django_ca/management/commands/
--rw-r--r--   0 mati      (1000) mati      (1000)     1104 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/management/commands/revoke_cert.py
--rw-r--r--   0 mati      (1000) mati      (1000)     2584 2017-12-02 14:26:58.000000 django-ca-1.7.0/ca/django_ca/management/commands/view_ca.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1135 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/management/commands/list_cas.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1865 2017-11-19 10:46:21.000000 django-ca-1.7.0/ca/django_ca/management/commands/import_cert.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1380 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/management/commands/dump_ocsp_index.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1957 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/management/commands/edit_ca.py
--rw-r--r--   0 mati      (1000) mati      (1000)     8075 2017-11-19 16:21:27.000000 django-ca-1.7.0/ca/django_ca/management/commands/sign_cert.py
--rw-r--r--   0 mati      (1000) mati      (1000)     4638 2017-11-19 10:46:40.000000 django-ca-1.7.0/ca/django_ca/management/commands/import_ca.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1616 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/management/commands/dump_ca.py
--rw-r--r--   0 mati      (1000) mati      (1000)        0 2015-12-22 10:24:56.000000 django-ca-1.7.0/ca/django_ca/management/commands/__init__.py
--rw-r--r--   0 mati      (1000) mati      (1000)     2086 2017-10-21 10:49:29.000000 django-ca-1.7.0/ca/django_ca/management/commands/list_certs.py
--rw-r--r--   0 mati      (1000) mati      (1000)     6864 2017-12-14 19:24:57.000000 django-ca-1.7.0/ca/django_ca/management/commands/init_ca.py
--rw-r--r--   0 mati      (1000) mati      (1000)     2765 2017-12-09 17:35:53.000000 django-ca-1.7.0/ca/django_ca/management/commands/view_cert.py
--rw-r--r--   0 mati      (1000) mati      (1000)     1591 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/management/commands/dump_cert.py
--rw-r--r--   0 mati      (1000) mati      (1000)     2388 2017-12-04 18:10:14.000000 django-ca-1.7.0/ca/django_ca/management/commands/dump_crl.py
--rw-r--r--   0 mati      (1000) mati      (1000)     2032 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/management/commands/notify_expiring_certs.py
--rw-r--r--   0 mati      (1000) mati      (1000)     2024 2017-03-04 21:58:48.000000 django-ca-1.7.0/ca/django_ca/management/commands/cert_watchers.py
--rw-r--r--   0 mati      (1000) mati      (1000)       67 2017-12-17 18:18:31.000000 django-ca-1.7.0/setup.cfg
--rw-r--r--   0 mati      (1000) mati      (1000)     7427 2017-12-14 19:37:41.000000 django-ca-1.7.0/setup.py
--rw-r--r--   0 mati      (1000) mati      (1000)      117 2016-01-24 13:54:17.000000 django-ca-1.7.0/MANIFEST.in
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/
+-rw-r--r--   0 mati      (1000) mati      (1000)     1683 2018-06-24 10:40:29.000000 django-ca-1.9.0/README.md
+-rw-rw-r--   0 mati      (1000) mati      (1000)    35147 2007-07-01 22:55:35.000000 django-ca-1.9.0/LICENSE
+-rw-r--r--   0 mati      (1000) mati      (1000)     2099 2018-08-25 10:03:20.000000 django-ca-1.9.0/PKG-INFO
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca.egg-info/
+-rw-r--r--   0 mati      (1000) mati      (1000)     3042 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca.egg-info/SOURCES.txt
+-rw-r--r--   0 mati      (1000) mati      (1000)     2099 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca.egg-info/PKG-INFO
+-rw-r--r--   0 mati      (1000) mati      (1000)        1 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca.egg-info/dependency_links.txt
+-rw-r--r--   0 mati      (1000) mati      (1000)       87 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca.egg-info/requires.txt
+-rw-r--r--   0 mati      (1000) mati      (1000)       10 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca.egg-info/top_level.txt
+-rw-r--r--   0 mati      (1000) mati      (1000)        1 2017-02-26 13:41:27.000000 django-ca-1.9.0/ca/django_ca.egg-info/not-zip-safe
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/
+-rw-r--r--   0 mati      (1000) mati      (1000)     1620 2017-12-09 11:42:55.000000 django-ca-1.9.0/ca/django_ca/urls.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1734 2017-12-03 19:57:32.000000 django-ca-1.9.0/ca/django_ca/querysets.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     7220 2018-08-04 15:53:29.000000 django-ca-1.9.0/ca/django_ca/widgets.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     9095 2018-08-25 08:30:41.000000 django-ca-1.9.0/ca/django_ca/forms.py
+-rw-r--r--   0 mati      (1000) mati      (1000)    11144 2018-06-24 10:42:25.000000 django-ca-1.9.0/ca/django_ca/views.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1682 2017-03-04 22:12:30.000000 django-ca-1.9.0/ca/django_ca/ocsp.py
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/templatetags/
+-rw-r--r--   0 mati      (1000) mati      (1000)     1016 2018-08-25 08:27:44.000000 django-ca-1.9.0/ca/django_ca/templatetags/django_ca.py
+-rw-r--r--   0 mati      (1000) mati      (1000)        0 2016-01-24 13:54:17.000000 django-ca-1.9.0/ca/django_ca/templatetags/__init__.py
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/static/
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/js/
+-rw-r--r--   0 mati      (1000) mati      (1000)     2973 2016-03-04 21:36:53.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/js/profilewidget.js
+-rw-r--r--   0 mati      (1000) mati      (1000)     5637 2016-01-29 20:25:19.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/js/sign.js
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/css/
+-rw-r--r--   0 mati      (1000) mati      (1000)       75 2016-01-24 14:43:14.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/css/labeledtextinput.css
+-rw-r--r--   0 mati      (1000) mati      (1000)     1354 2017-12-09 12:53:46.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/css/base.css
+-rw-r--r--   0 mati      (1000) mati      (1000)       37 2016-02-28 13:23:31.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/css/certificateauthorityadmin.css
+-rw-r--r--   0 mati      (1000) mati      (1000)      817 2016-01-24 13:54:17.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/css/labeledcheckboxinput.css
+-rw-r--r--   0 mati      (1000) mati      (1000)     1175 2017-12-09 12:53:49.000000 django-ca-1.9.0/ca/django_ca/static/django_ca/admin/css/certificateadmin.css
+-rw-r--r--   0 mati      (1000) mati      (1000)      921 2017-03-04 21:58:48.000000 django-ca-1.9.0/ca/django_ca/apps.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     2854 2017-12-08 14:03:51.000000 django-ca-1.9.0/ca/django_ca/crl.py
+-rw-r--r--   0 mati      (1000) mati      (1000)    19442 2018-08-04 18:45:06.000000 django-ca-1.9.0/ca/django_ca/utils.py
+-rw-r--r--   0 mati      (1000) mati      (1000)       53 2015-12-26 14:14:39.000000 django-ca-1.9.0/ca/django_ca/__init__.py
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/templates/
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/admin/
+-rw-r--r--   0 mati      (1000) mati      (1000)     2077 2016-04-21 18:48:24.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/admin/certificate_revoke_form.html
+-rw-r--r--   0 mati      (1000) mati      (1000)      607 2016-01-24 13:54:17.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/admin/submit_line.html
+-rw-r--r--   0 mati      (1000) mati      (1000)      147 2016-01-24 13:54:17.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/admin/change_form.html
+-rw-r--r--   0 mati      (1000) mati      (1000)      517 2018-08-11 13:45:33.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/admin/signedCertificateTimestampList.html
+-rw-r--r--   0 mati      (1000) mati      (1000)      168 2018-08-15 12:21:07.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/admin/unrecognizedextension.html
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/forms/
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/forms/widgets/
+-rw-r--r--   0 mati      (1000) mati      (1000)      157 2017-04-19 20:57:37.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/forms/widgets/labeledcheckboxinput.html
+-rw-r--r--   0 mati      (1000) mati      (1000)      146 2017-04-19 21:11:25.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/forms/widgets/subjecttextinput.html
+-rw-r--r--   0 mati      (1000) mati      (1000)      116 2017-04-19 20:57:32.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/forms/widgets/custommultiwidget.html
+-rw-r--r--   0 mati      (1000) mati      (1000)      237 2017-04-19 21:13:10.000000 django-ca-1.9.0/ca/django_ca/templates/django_ca/forms/widgets/labeledtextinput.html
+-rw-r--r--   0 mati      (1000) mati      (1000)    16571 2018-08-04 18:05:26.000000 django-ca-1.9.0/ca/django_ca/managers.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     5111 2018-08-04 17:13:05.000000 django-ca-1.9.0/ca/django_ca/subject.py
+-rw-r--r--   0 mati      (1000) mati      (1000)    19376 2018-08-25 09:52:47.000000 django-ca-1.9.0/ca/django_ca/admin.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     4873 2018-08-04 18:48:32.000000 django-ca-1.9.0/ca/django_ca/ca_settings.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     3210 2018-08-04 18:38:49.000000 django-ca-1.9.0/ca/django_ca/fields.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     2614 2018-06-23 11:01:33.000000 django-ca-1.9.0/ca/django_ca/signals.py
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/migrations/
+-rw-r--r--   0 mati      (1000) mati      (1000)     4420 2017-07-18 10:08:02.000000 django-ca-1.9.0/ca/django_ca/migrations/0001_initial.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1024 2017-07-18 10:08:02.000000 django-ca-1.9.0/ca/django_ca/migrations/0005_auto_20170307_1839.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1299 2017-07-18 10:08:02.000000 django-ca-1.9.0/ca/django_ca/migrations/0003_auto_20170304_1434.py
+-rw-r--r--   0 mati      (1000) mati      (1000)      470 2017-07-18 10:08:02.000000 django-ca-1.9.0/ca/django_ca/migrations/0006_auto_20170505_1251.py
+-rw-r--r--   0 mati      (1000) mati      (1000)        0 2017-07-18 10:07:18.000000 django-ca-1.9.0/ca/django_ca/migrations/__init__.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1187 2017-07-18 10:08:02.000000 django-ca-1.9.0/ca/django_ca/migrations/0002_auto_20170304_1434.py
+-rw-r--r--   0 mati      (1000) mati      (1000)      617 2017-11-19 10:00:08.000000 django-ca-1.9.0/ca/django_ca/migrations/0007_auto_20171119_1100.py
+-rw-r--r--   0 mati      (1000) mati      (1000)      993 2017-07-18 10:08:02.000000 django-ca-1.9.0/ca/django_ca/migrations/0004_auto_20170304_1442.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1291 2017-12-03 19:01:57.000000 django-ca-1.9.0/ca/django_ca/migrations/0008_auto_20171203_2001.py
+-rw-r--r--   0 mati      (1000) mati      (1000)    20519 2018-08-25 09:51:48.000000 django-ca-1.9.0/ca/django_ca/models.py
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/management/
+-rw-r--r--   0 mati      (1000) mati      (1000)    13035 2018-08-11 13:52:14.000000 django-ca-1.9.0/ca/django_ca/management/base.py
+-rw-r--r--   0 mati      (1000) mati      (1000)        0 2015-12-22 10:19:07.000000 django-ca-1.9.0/ca/django_ca/management/__init__.py
+drwxr-xr-x   0 mati      (1000) mati      (1000)        0 2018-08-25 10:03:20.000000 django-ca-1.9.0/ca/django_ca/management/commands/
+-rw-r--r--   0 mati      (1000) mati      (1000)     1104 2017-03-04 21:58:48.000000 django-ca-1.9.0/ca/django_ca/management/commands/revoke_cert.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     2584 2017-12-02 14:26:58.000000 django-ca-1.9.0/ca/django_ca/management/commands/view_ca.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1135 2017-03-04 21:58:48.000000 django-ca-1.9.0/ca/django_ca/management/commands/list_cas.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1865 2017-11-19 10:46:21.000000 django-ca-1.9.0/ca/django_ca/management/commands/import_cert.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1380 2017-03-04 21:58:48.000000 django-ca-1.9.0/ca/django_ca/management/commands/dump_ocsp_index.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1957 2017-03-04 21:58:48.000000 django-ca-1.9.0/ca/django_ca/management/commands/edit_ca.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     8352 2018-08-04 17:40:40.000000 django-ca-1.9.0/ca/django_ca/management/commands/sign_cert.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     4638 2017-11-19 10:46:40.000000 django-ca-1.9.0/ca/django_ca/management/commands/import_ca.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1616 2017-03-04 21:58:48.000000 django-ca-1.9.0/ca/django_ca/management/commands/dump_ca.py
+-rw-r--r--   0 mati      (1000) mati      (1000)        0 2015-12-22 10:24:56.000000 django-ca-1.9.0/ca/django_ca/management/commands/__init__.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     2086 2017-10-21 10:49:29.000000 django-ca-1.9.0/ca/django_ca/management/commands/list_certs.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     6982 2018-08-04 16:57:44.000000 django-ca-1.9.0/ca/django_ca/management/commands/init_ca.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     2765 2017-12-09 17:35:53.000000 django-ca-1.9.0/ca/django_ca/management/commands/view_cert.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     1591 2017-03-04 21:58:48.000000 django-ca-1.9.0/ca/django_ca/management/commands/dump_cert.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     2600 2018-08-04 18:40:48.000000 django-ca-1.9.0/ca/django_ca/management/commands/dump_crl.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     2032 2018-08-15 12:51:54.000000 django-ca-1.9.0/ca/django_ca/management/commands/notify_expiring_certs.py
+-rw-r--r--   0 mati      (1000) mati      (1000)     2024 2017-03-04 21:58:48.000000 django-ca-1.9.0/ca/django_ca/management/commands/cert_watchers.py
+-rw-r--r--   0 mati      (1000) mati      (1000)       67 2018-08-25 10:03:20.000000 django-ca-1.9.0/setup.cfg
+-rw-r--r--   0 mati      (1000) mati      (1000)     7417 2018-08-25 09:10:13.000000 django-ca-1.9.0/setup.py
+-rw-r--r--   0 mati      (1000) mati      (1000)      117 2016-01-24 13:54:17.000000 django-ca-1.9.0/MANIFEST.in
```

### Comparing `django-ca-1.7.0/README.md` & `django-ca-1.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 **django-ca** is a small project to manage TLS certificate authorities and easily issue
 certificates.  It is based on [cryptography](https://cryptography.io/) and
 [Django](https://www.djangoproject.com/>). It can be used as an app in an existing Django project
 or stand-alone with the basic project included.  Certificates can be managed through Djangos admin
 interface or via `manage.py` commands - so no webserver is needed, if you’re happy with the
 command-line.
 
-Documentation is available at http://django-ca.readthedocs.org/.
+Documentation is available at https://django-ca.readthedocs.org/.
 
 ## Features
 
 1. Set up a secure local certificate authority in just a few minutes.
-2. Written in Python2.7/Python3.4+, requires Django 1.8 or later.
+2. Written in Python2.7/Python3.4+, requires Django 1.11 or later.
 3. Manage your entire certificate authority from the command line and/or via
    Djangos admin interface.
 4. Get email notifications about certificates about to expire.
 5. Certificate validation using Certificate Revocation Lists (CRLs) and via an included OCSP
    responder.
 
 Please see https://django-ca.readthedocs.org for more extensive documentation.
 
 ## Documentation
 
-Documentation is available at http://django-ca.readthedocs.org/.
+Documentation is available at https://django-ca.readthedocs.org/.
 
 ## ChangeLog
 
-Please see http://django-ca.readthedocs.io/en/latest/changelog.html
+Please see https://django-ca.readthedocs.io/en/latest/changelog.html
 
 ## ToDo
 
 Ideas on what we could do for future releases:
 
 1. Add parameter to add generic CRL/OCSP URLs to CAs.
 2. Test CRL signing certificates.
 3. Only send out one notification if multiple certificates expire for a user.
 4. Add a "renew" button in the admin interface.
 5. Add ability to automatically regenerate CRLs when a certificate is revoked.
 
 ## License
 
-This project is free software licensed under the [GPLv3](http://www.gnu.org/licenses/gpl.txt).
+This project is free software licensed under the [GPLv3](https://www.gnu.org/licenses/gpl.txt).
```

### Comparing `django-ca-1.7.0/LICENSE` & `django-ca-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/PKG-INFO` & `django-ca-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 1.1
 Name: django-ca
-Version: 1.7.0
+Version: 1.9.0
 Summary: A Django app providing a SSL/TLS certificate authority.
 Home-page: https://github.com/mathiasertl/django-ca
 Author: Mathias Ertl
 Author-email: mati@er.tl
 License: UNKNOWN
-Description-Content-Type: UNKNOWN
 Description: django-ca is a tool to manage TLS certificate authorities and easily issue and revoke
         certificates. It is based `cryptography <https://cryptography.io/>`_ and `Django
         <https://www.djangoproject.com/>`_. It can be used as an app in an existing Django project or stand-alone with
         the basic project included.  Everything can be managed via the command line via `manage.py` commands - so no
         webserver is needed, if you’re happy with the command-line.
         
         Features:
         
         * Set up a secure local certificate authority in just a few minutes.
-        * Written in Python 2.7/Python3.4+, requires Django 1.8 or later.
+        * Written in Python 2.7/Python3.4+, requires Django 1.11 or later.
         * Manage your entire certificate authority from the command line and/or via Djangos admin
           interface.
         * Get email notifications about certificates about to expire.
         * Certificate validation using Certificate Revocation Lists (CRLs) and via an included OCSP
           responder.
         
         Please see https://django-ca.readthedocs.org for more extensive documentation.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
+Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-ca-1.7.0/ca/django_ca.egg-info/SOURCES.txt` & `django-ca-1.9.0/ca/django_ca.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 ca/django_ca/crl.py
 ca/django_ca/fields.py
 ca/django_ca/forms.py
 ca/django_ca/managers.py
 ca/django_ca/models.py
 ca/django_ca/ocsp.py
 ca/django_ca/querysets.py
+ca/django_ca/signals.py
+ca/django_ca/subject.py
 ca/django_ca/urls.py
 ca/django_ca/utils.py
 ca/django_ca/views.py
 ca/django_ca/widgets.py
 ca/django_ca.egg-info/PKG-INFO
 ca/django_ca.egg-info/SOURCES.txt
 ca/django_ca.egg-info/dependency_links.txt
@@ -57,14 +59,16 @@
 ca/django_ca/static/django_ca/admin/css/certificateauthorityadmin.css
 ca/django_ca/static/django_ca/admin/css/labeledcheckboxinput.css
 ca/django_ca/static/django_ca/admin/css/labeledtextinput.css
 ca/django_ca/static/django_ca/admin/js/profilewidget.js
 ca/django_ca/static/django_ca/admin/js/sign.js
 ca/django_ca/templates/django_ca/admin/certificate_revoke_form.html
 ca/django_ca/templates/django_ca/admin/change_form.html
+ca/django_ca/templates/django_ca/admin/signedCertificateTimestampList.html
 ca/django_ca/templates/django_ca/admin/submit_line.html
+ca/django_ca/templates/django_ca/admin/unrecognizedextension.html
 ca/django_ca/templates/django_ca/forms/widgets/custommultiwidget.html
 ca/django_ca/templates/django_ca/forms/widgets/labeledcheckboxinput.html
 ca/django_ca/templates/django_ca/forms/widgets/labeledtextinput.html
 ca/django_ca/templates/django_ca/forms/widgets/subjecttextinput.html
 ca/django_ca/templatetags/__init__.py
 ca/django_ca/templatetags/django_ca.py
```

### Comparing `django-ca-1.7.0/ca/django_ca.egg-info/PKG-INFO` & `django-ca-1.9.0/ca/django_ca.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 Metadata-Version: 1.1
 Name: django-ca
-Version: 1.7.0
+Version: 1.9.0
 Summary: A Django app providing a SSL/TLS certificate authority.
 Home-page: https://github.com/mathiasertl/django-ca
 Author: Mathias Ertl
 Author-email: mati@er.tl
 License: UNKNOWN
-Description-Content-Type: UNKNOWN
 Description: django-ca is a tool to manage TLS certificate authorities and easily issue and revoke
         certificates. It is based `cryptography <https://cryptography.io/>`_ and `Django
         <https://www.djangoproject.com/>`_. It can be used as an app in an existing Django project or stand-alone with
         the basic project included.  Everything can be managed via the command line via `manage.py` commands - so no
         webserver is needed, if you’re happy with the command-line.
         
         Features:
         
         * Set up a secure local certificate authority in just a few minutes.
-        * Written in Python 2.7/Python3.4+, requires Django 1.8 or later.
+        * Written in Python 2.7/Python3.4+, requires Django 1.11 or later.
         * Manage your entire certificate authority from the command line and/or via Djangos admin
           interface.
         * Get email notifications about certificates about to expire.
         * Certificate validation using Certificate Revocation Lists (CRLs) and via an included OCSP
           responder.
         
         Please see https://django-ca.readthedocs.org for more extensive documentation.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django :: 1.8
-Classifier: Framework :: Django :: 1.10
 Classifier: Framework :: Django :: 1.11
+Classifier: Framework :: Django :: 2.0
+Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-ca-1.7.0/ca/django_ca/urls.py` & `django-ca-1.9.0/ca/django_ca/urls.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/querysets.py` & `django-ca-1.9.0/ca/django_ca/querysets.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/widgets.py` & `django-ca-1.9.0/ca/django_ca/widgets.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         super(LabeledCheckboxInput, self).__init__(*args, **kwargs)
 
     def get_context(self, *args, **kwargs):
         ctx = super(LabeledCheckboxInput, self).get_context(*args, **kwargs)
         ctx['widget']['label'] = self.label
         return ctx
 
-    def render(self, name, value, attrs=None):  # pragma: no cover - <= Django 1.11
-        html = super(LabeledCheckboxInput, self).render(name, value, attrs=attrs)
+    def render(self, name, value, attrs=None, renderer=None):  # pragma: no cover - <= Django 1.11
+        html = super(LabeledCheckboxInput, self).render(name, value, attrs=attrs, renderer=renderer)
         label = '<label for="%s">%s</label>' % (attrs.get('id'), self.label)
         html = '<span class="critical-widget-wrapper">%s%s</span>' % (html, label)
         return html
 
     class Media:
         css = {
             'all': ('django_ca/admin/css/labeledcheckboxinput.css', ),
@@ -65,48 +65,48 @@
     def get_context(self, *args, **kwargs):
         ctx = super(LabeledTextInput, self).get_context(*args, **kwargs)
         ctx['widget']['label'] = self.label
         ctx['widget']['subrequired'] = self.attrs.get('required')
         ctx['widget']['cssid'] = self.label.lower().replace(' ', '-')
         return ctx
 
-    def render_wrapped(self, name, value, attrs):  # pragma: no cover - <= Django 1.11
-        html = super(LabeledTextInput, self).render(name, value, attrs=attrs)
+    def render_wrapped(self, name, value, attrs, renderer):  # pragma: no cover - <= Django 1.11
+        html = super(LabeledTextInput, self).render(name, value, attrs=attrs, renderer=renderer)
         required = ''
         if self.attrs.get('required', False):
             required = 'class="required" '
 
         html += '<label %sfor="%s">%s</label>' % (required, attrs.get('id'), self.label)
 
         return html
 
-    def render(self, name, value, attrs=None):  # pragma: no cover - <= Django 1.11
-        html = self.render_wrapped(name, value, attrs)
+    def render(self, name, value, attrs=None, renderer=None):  # pragma: no cover - <= Django 1.11
+        html = self.render_wrapped(name, value, attrs, renderer=renderer)
         cssid = self.label.lower().replace(' ', '-')
         html = '<span id="%s" class="labeled-text-multiwidget">%s</span>' % (cssid, html)
         return html
 
     class Media:
         css = {
             'all': ('django_ca/admin/css/labeledtextinput.css', ),
         }
 
 
 class SubjectTextInput(LabeledTextInput):
     template_name = 'django_ca/forms/widgets/subjecttextinput.html'
 
-    def render_wrapped(self, name, value, attrs):  # pragma: no cover - <= Django 1.11
-        html = super(SubjectTextInput, self).render_wrapped(name, value, attrs)
+    def render_wrapped(self, name, value, attrs, renderer):  # pragma: no cover - <= Django 1.11
+        html = super(SubjectTextInput, self).render_wrapped(name, value, attrs, renderer=renderer)
         html += '<span class="from-csr">%s <span></span></span>' % _('from CSR:')
         return html
 
 
 class ProfileWidget(widgets.Select):
-    def render(self, name, value, attrs=None):
-        html = super(ProfileWidget, self).render(name, value, attrs=attrs)
+    def render(self, name, value, attrs=None, renderer=None):  # pragma: no cover - <= Django 1.11
+        html = super(ProfileWidget, self).render(name, value, attrs=attrs, renderer=renderer)
         html += '''<script type="text/javascript">
             var ca_profiles = %s;
         </script>''' % json.dumps(ca_settings.CA_PROFILES, cls=LazyEncoder)
         html += '<p class="help profile-desc">%s</p>' % force_text(
             ca_settings.CA_PROFILES[ca_settings.CA_DEFAULT_PROFILE]['desc'])
         return html
 
@@ -140,14 +140,17 @@
             SubjectTextInput(label=_('E-Mail')),
         )
         super(SubjectWidget, self).__init__(_widgets, attrs)
 
     def decompress(self, value):
         if value is None:  # pragma: no cover
             return ('', '', '', '', '', '')
+
+        # NOTE: this appears to be only relevant on initial form load or when editing an existing form. The
+        # latter is never true, so this isn't relevant anywhere else.
         return [
             value.get('C', ''),
             value.get('ST', ''),
             value.get('L', ''),
             value.get('O', ''),
             value.get('OU', ''),
             value.get('CN', ''),
```

### Comparing `django-ca-1.7.0/ca/django_ca/forms.py` & `django-ca-1.9.0/ca/django_ca/forms.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,30 +18,26 @@
 from datetime import datetime
 from datetime import timedelta
 
 from cryptography.hazmat.primitives import hashes
 
 from django import forms
 from django.contrib.admin.widgets import AdminDateWidget
+from django.urls import reverse
 from django.utils.translation import ugettext_lazy as _
 
 from . import ca_settings
 from .fields import KeyUsageField
 from .fields import SubjectAltNameField
 from .fields import SubjectField
 from .models import Certificate
 from .utils import EXTENDED_KEY_USAGE_DESC
 from .utils import KEY_USAGE_DESC
 from .widgets import ProfileWidget
 
-try:
-    from django.urls import reverse
-except ImportError:  # pragma: only django<=1.8
-    from django.core.urlresolvers import reverse
-
 
 def _initial_expires():
     return datetime.today() + timedelta(days=ca_settings.CA_DEFAULT_EXPIRES)
 
 
 def _profile_choices():
     choices = [('', '----')] + [(p, p) for p in ca_settings.CA_PROFILES]
@@ -59,24 +55,31 @@
         * You cannot use the normal way of setting ``help_texts`` in the forms ``Meta`` class,
           because we cannot reference the object instance here.
         * We cannot access self.fields['pub'] in the constructor, because it is a readonly field
           and thus not present in the form.
         """
         super(X509CertMixinAdminForm, self).__init__(*args, **kwargs)
 
-        # help_texts is None if we have no Meta class defined here
-        if self._meta.help_texts is None:  # pragma: no branch
+        if not getattr(self._meta, 'help_texts', None):  # pragma: no cover
+            # help_texts is always set since we have a Meta class, but keeping this here as a precaution.
             self._meta.help_texts = {}
 
         info = self.instance._meta.app_label, self.instance._meta.model_name
         url = reverse('admin:%s_%s_download' % info, kwargs={'pk': self.instance.pk})
         self._meta.help_texts['pub'] = _(
             'Download: <a href="%s?format=PEM">as PEM</a> | <a href="%s?format=DER">as DER</a>.'
         ) % (url, url)
 
+    class Meta:
+        help_texts = {
+            'hpkp_pin': _('''SHA-256 HPKP pin of this certificate. See also
+<a href="https://en.wikipedia.org/wiki/HTTP_Public_Key_Pinning">HTTP Public Key Pinning</a>
+on Wikipedia.'''),
+        }
+
 
 class CreateCertificateForm(forms.ModelForm):
     def __init__(self, *args, **kwargs):
         super(CreateCertificateForm, self).__init__(*args, **kwargs)
 
         # Set choices so we can filter out CAs where the private key does not exist locally
         field = self.fields['ca']
@@ -95,15 +98,15 @@
         help_text=_('''Coma-separated list of alternative names for the certificate.''')
     )
     profile = forms.ChoiceField(
         required=False, widget=ProfileWidget,
         help_text=_('Select a suitable profile or manually select X509 extensions below.'),
         initial=ca_settings.CA_DEFAULT_PROFILE, choices=_profile_choices)
     algorithm = forms.ChoiceField(
-        label=_('Signature algorithm'), initial=ca_settings.CA_DIGEST_ALGORITHM, choices=[
+        label=_('Signature algorithm'), initial=ca_settings.CA_DIGEST_ALGORITHM.name, choices=[
             ('SHA512', 'SHA-512'),
             ('SHA256', 'SHA-256'),
             ('SHA1', 'SHA-1 (insecure!)'),
             ('MD5', 'MD5 (insecure!)'),
         ],
         help_text=_(
             'Algorithm used for signing the certificate. SHA-512 should be fine in most cases.'
@@ -124,25 +127,27 @@
         label='extendedKeyUsage', help_text=EXTENDED_KEY_USAGE_DESC, choices=(
             ('serverAuth', 'SSL/TLS Web Server Authentication'),
             ('clientAuth', 'SSL/TLS Web Client Authentication'),
             ('codeSigning', 'Code signing'),
             ('emailProtection', 'E-mail Protection (S/MIME)'),
             ('timeStamping', 'Trusted Timestamping'),
             ('OCSPSigning', 'OCSP Signing'),
+            ('smartcardLogon', 'Smart card logon'),
+            ('msKDC', 'Kerberos Domain Controller'),
         ))
     tlsFeature = KeyUsageField(
         label='TLS Features', choices=(
             ('OCSPMustStaple', 'OCSP Must-Staple'),
             ('MultipleCertStatusRequest', 'Multiple Certificate Status Request'),
         ))
 
     def clean_csr(self):
         data = self.cleaned_data['csr']
         lines = data.splitlines()
-        if lines[0] != '-----BEGIN CERTIFICATE REQUEST-----' \
+        if not lines or lines[0] != '-----BEGIN CERTIFICATE REQUEST-----' \
                 or lines[-1] != '-----END CERTIFICATE REQUEST-----':
             raise forms.ValidationError(_("Enter a valid CSR (in PEM format)."))
 
         return data
 
     def clean_algorithm(self):
         algo = self.cleaned_data['algorithm']
@@ -207,15 +212,15 @@
     class Meta:
         model = Certificate
         fields = ['csr', 'watchers', 'ca', ]
         help_texts = {
             'csr': _('''The Certificate Signing Request (CSR) in PEM format. To create a new one:
 <span class="shell">openssl genrsa -out hostname.key 4096
 openssl req -new -key hostname.key -out hostname.csr -utf8 -batch \\
-                     -subj '/CN=/hostname/emailAddress=root@hostname'
+                     -subj '/CN=hostname/emailAddress=root@hostname'
 </span>'''),
         }
 
 
 class RevokeCertificateForm(forms.ModelForm):
     class Meta:
         model = Certificate
```

### Comparing `django-ca-1.7.0/ca/django_ca/views.py` & `django-ca-1.9.0/ca/django_ca/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from oscrypto.asymmetric import load_certificate
 from oscrypto.asymmetric import load_private_key
 
 from django.core.cache import cache
 from django.core.exceptions import PermissionDenied
 from django.http import HttpResponse
 from django.http import HttpResponseServerError
+from django.urls import reverse
 from django.utils.decorators import method_decorator
 from django.utils.encoding import force_bytes
 from django.utils.encoding import force_text
 from django.views.decorators.csrf import csrf_exempt
 from django.views.generic.base import View
 from django.views.generic.detail import SingleObjectMixin
 from django.views.generic.edit import UpdateView
@@ -41,18 +42,14 @@
 from .crl import get_crl
 from .forms import RevokeCertificateForm
 from .models import Certificate
 from .models import CertificateAuthority
 from .utils import int_to_hex
 
 log = logging.getLogger(__name__)
-try:
-    from django.urls import reverse
-except ImportError:  # pragma: only django<=1.8
-    from django.core.urlresolvers import reverse
 
 
 class CertificateRevocationListView(View, SingleObjectMixin):
     """Generic view that provides Certificate Revocation Lists (CRLs)."""
 
     slug_field = 'serial'
     slug_url_kwarg = 'serial'
```

### Comparing `django-ca-1.7.0/ca/django_ca/ocsp.py` & `django-ca-1.9.0/ca/django_ca/ocsp.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/templatetags/django_ca.py` & `django-ca-1.9.0/ca/django_ca/templatetags/django_ca.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/static/django_ca/admin/js/profilewidget.js` & `django-ca-1.9.0/ca/django_ca/static/django_ca/admin/js/profilewidget.js`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/static/django_ca/admin/js/sign.js` & `django-ca-1.9.0/ca/django_ca/static/django_ca/admin/js/sign.js`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/static/django_ca/admin/css/base.css` & `django-ca-1.9.0/ca/django_ca/static/django_ca/admin/css/base.css`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/static/django_ca/admin/css/labeledcheckboxinput.css` & `django-ca-1.9.0/ca/django_ca/static/django_ca/admin/css/labeledcheckboxinput.css`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/static/django_ca/admin/css/certificateadmin.css` & `django-ca-1.9.0/ca/django_ca/static/django_ca/admin/css/certificateadmin.css`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/apps.py` & `django-ca-1.9.0/ca/django_ca/apps.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/crl.py` & `django-ca-1.9.0/ca/django_ca/crl.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/utils.py` & `django-ca-1.9.0/ca/django_ca/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 # You should have received a copy of the GNU General Public License along with django-ca.  If not,
 # see <http://www.gnu.org/licenses/>.
 
 """Central functions to load CA key and cert as PKey/X509 objects."""
 
 import re
 from collections import Iterable
-from collections import OrderedDict
 from copy import deepcopy
 from datetime import datetime
 from ipaddress import ip_address
 from ipaddress import ip_network
 
 import idna
 
+from asn1crypto.core import OctetString
 from cryptography import x509
 from cryptography.x509 import TLSFeatureType
 from cryptography.x509.oid import ExtendedKeyUsageOID
 from cryptography.x509.oid import NameOID
+from cryptography.x509.oid import ObjectIdentifier
 
 from django.core.serializers.json import DjangoJSONEncoder
 from django.core.validators import URLValidator
 from django.utils import six
 from django.utils.encoding import force_bytes
 from django.utils.encoding import force_text
 from django.utils.functional import Promise
@@ -76,14 +77,19 @@
     NameOID.COMMON_NAME: 'CN',
     NameOID.EMAIL_ADDRESS: 'emailAddress',
 }
 
 # same, but reversed
 NAME_OID_MAPPINGS = {v: k for k, v in OID_NAME_MAPPINGS.items()}
 
+# Some OIDs can occur multiple times
+MULTIPLE_OIDS = (
+    NameOID.ORGANIZATIONAL_UNIT_NAME,
+)
+
 # uppercase values as keys for normalizing case
 NAME_CASE_MAPPINGS = {v.upper(): v for v in OID_NAME_MAPPINGS.values()}
 
 KEY_USAGE_MAPPING = {
     'cRLSign': 'crl_sign',
     'dataEncipherment': 'data_encipherment',
     'decipherOnly': 'decipher_only',
@@ -99,14 +105,16 @@
 EXTENDED_KEY_USAGE_MAPPING = {
     'serverAuth': ExtendedKeyUsageOID.SERVER_AUTH,
     'clientAuth': ExtendedKeyUsageOID.CLIENT_AUTH,
     'codeSigning': ExtendedKeyUsageOID.CODE_SIGNING,
     'emailProtection': ExtendedKeyUsageOID.EMAIL_PROTECTION,
     'timeStamping': ExtendedKeyUsageOID.TIME_STAMPING,
     'OCSPSigning': ExtendedKeyUsageOID.OCSP_SIGNING,
+    'smartcardLogon': ObjectIdentifier("1.3.6.1.4.1.311.20.2.2"),
+    'msKDC': ObjectIdentifier("1.3.6.1.5.2.3.5"),
 }
 EXTENDED_KEY_USAGE_REVERSED = {v: k for k, v in EXTENDED_KEY_USAGE_MAPPING.items()}
 
 TLS_FEATURE_MAPPING = {
     # https://tools.ietf.org/html/rfc6066.html:
     'OCSPMustStaple': TLSFeatureType.status_request,
     # https://tools.ietf.org/html/rfc6961.html (not commonly used):
@@ -119,17 +127,17 @@
 
     def default(self, obj):
         if isinstance(obj, Promise):
             return force_text(obj)
         return super(LazyEncoder, self).default(obj)
 
 
-def sort_subject_dict(d):
-    """Returns an itemized dictionary in the correct order for a x509 subject."""
-    return sorted(d.items(), key=lambda e: SUBJECT_FIELDS.index(e[0]))
+def sort_name(subject):
+    """Returns the subject in the correct order for a x509 subject."""
+    return sorted(subject, key=lambda e: SUBJECT_FIELDS.index(e[0]))
 
 
 def format_name(subject):
     """Convert a subject into the canonical form for distinguished names.
 
     This function does not take care of sorting the subject in any meaningful order.
 
@@ -233,85 +241,78 @@
 
     The ``name`` is expected to be close to the subject format commonly used by OpenSSL, for example
     ``/C=AT/L=Vienna/CN=example.com/emailAddress=user@example.com``. The function does its best to be lenient
     on deviations from the format, object identifiers are case-insensitive (e.g. ``cn`` is the same as ``CN``,
     whitespace at the start and end is stripped and the subject does not have to start with a slash (``/``).
 
     >>> parse_name('/CN=example.com')
-    OrderedDict([('CN', 'example.com')])
+    [('CN', 'example.com')]
     >>> parse_name('c=AT/l= Vienna/o="ex org"/CN=example.com')
-    OrderedDict([('C', 'AT'), ('L', 'Vienna'), ('O', 'ex org'), ('CN', 'example.com')])
+    [('C', 'AT'), ('L', 'Vienna'), ('O', 'ex org'), ('CN', 'example.com')]
 
     Dictionary keys are normalized to the values of :py:const:`OID_NAME_MAPPINGS` and keys will be sorted
     based on x509 name specifications regardless of the given order:
 
     >>> parse_name('L="Vienna / District"/EMAILaddress=user@example.com')
-    OrderedDict([('L', 'Vienna / District'), ('emailAddress', 'user@example.com')])
+    [('L', 'Vienna / District'), ('emailAddress', 'user@example.com')]
     >>> parse_name('/C=AT/CN=example.com') == parse_name('/CN=example.com/C=AT')
     True
 
     Due to the magic of :py:const:`NAME_RE`, the function even supports quoting strings and including slashes,
     so strings like ``/OU="Org / Org Unit"/CN=example.com`` will work as expected.
 
     >>> parse_name('L="Vienna / District"/CN=example.com')
-    OrderedDict([('L', 'Vienna / District'), ('CN', 'example.com')])
+    [('L', 'Vienna / District'), ('CN', 'example.com')]
 
     But note that it's still easy to trick this function, if you really want to. The following example is
     *not* a valid subject, the location is just bogus, and whatever you were expecting as output, it's
     certainly different:
 
     >>> parse_name('L="Vienna " District"/CN=example.com')
-    OrderedDict([('L', 'Vienna'), ('CN', 'example.com')])
+    [('L', 'Vienna'), ('CN', 'example.com')]
 
     Examples of where this string is used are:
 
     .. code-block:: console
 
         # openssl req -new -key priv.key -out csr -utf8 -batch -sha256 -subj '/C=AT/CN=example.com'
         # openssl x509 -in cert.pem -noout -subject -nameopt compat
         /C=AT/L=Vienna/CN=example.com
     """
     name = name.strip()
     if not name:  # empty subjects are ok
-        return {}
+        return []
 
     try:
         items = [(NAME_CASE_MAPPINGS[t[0].upper()], force_text(t[2])) for t in NAME_RE.findall(name)]
     except KeyError as e:
         raise ValueError('Unknown x509 name field: %s' % e.args[0])
 
-    parsed = sorted(items, key=lambda e: SUBJECT_FIELDS.index(e[0]))
-    return OrderedDict(parsed)
+    # Check that no OIDs not in MULTIPLE_OIDS occur more then once
+    for key, oid in NAME_OID_MAPPINGS.items():
+        if sum(1 for t in items if t[0] == key) > 1 and oid not in MULTIPLE_OIDS:
+            raise ValueError('Subject contains multiple "%s" fields' % key)
+
+    return sort_name(items)
 
 
 def x509_name(name):
-    """Parses a subject string into a :py:class:`x509.Name <cryptography:cryptography.x509.Name>`.
+    """Parses a subject into a :py:class:`x509.Name <cryptography:cryptography.x509.Name>`.
 
-    If ``name`` is a string, :py:func:`parse_name` is used to parse it. A list of tuples or a ``dict``
-    (preferrably an :py:class:`~python:collections.OrderedDict`) is also supported.
+    If ``name`` is a string, :py:func:`parse_name` is used to parse it.
 
     >>> x509_name('/C=AT/CN=example.com')  # doctest: +NORMALIZE_WHITESPACE
     <Name([<NameAttribute(oid=<ObjectIdentifier(oid=2.5.4.6, name=countryName)>, value='AT')>,
            <NameAttribute(oid=<ObjectIdentifier(oid=2.5.4.3, name=commonName)>, value='example.com')>])>
     >>> x509_name([('C', 'AT'), ('CN', 'example.com')])  # doctest: +NORMALIZE_WHITESPACE
     <Name([<NameAttribute(oid=<ObjectIdentifier(oid=2.5.4.6, name=countryName)>, value='AT')>,
            <NameAttribute(oid=<ObjectIdentifier(oid=2.5.4.3, name=commonName)>, value='example.com')>])>
-    >>> x509_name(OrderedDict([('C', 'AT'), ('CN', 'example.com')]))  # doctest: +NORMALIZE_WHITESPACE
-    <Name([<NameAttribute(oid=<ObjectIdentifier(oid=2.5.4.6, name=countryName)>, value='AT')>,
-           <NameAttribute(oid=<ObjectIdentifier(oid=2.5.4.3, name=commonName)>, value='example.com')>])>
-    >>> x509_name(OrderedDict([('C', 'AT'), ('CN', 'example.com')]))  # doctest: +NORMALIZE_WHITESPACE
-    <Name([<NameAttribute(oid=<ObjectIdentifier(oid=2.5.4.6, name=countryName)>, value='AT')>,
-           <NameAttribute(oid=<ObjectIdentifier(oid=2.5.4.3, name=commonName)>, value='example.com')>])>
     """
     if isinstance(name, six.string_types):
-        name = parse_name(name).items()
-    elif isinstance(name, OrderedDict):
-        name = name.items()
-    elif isinstance(name, dict):
-        name = sort_subject_dict(name)
+        name = parse_name(name)
 
     return x509.Name([x509.NameAttribute(NAME_OID_MAPPINGS[typ], force_text(value)) for typ, value in name])
 
 
 def validate_email(addr):
     """Validate an email address.
 
@@ -342,14 +343,16 @@
 
     This function will do its best to detect the intended type of any value passed to it:
 
     >>> parse_general_name('example.com')
     <DNSName(value='example.com')>
     >>> parse_general_name('*.example.com')
     <DNSName(value='*.example.com')>
+    >>> parse_general_name('.example.com')  # Syntax used e.g. for NameConstraints: All levels of subdomains
+    <DNSName(value='.example.com')>
     >>> parse_general_name('user@example.com')
     <RFC822Name(value='user@example.com')>
     >>> parse_general_name('https://example.com')
     <UniformResourceIdentifier(value='https://example.com')>
     >>> parse_general_name('1.2.3.4')
     <IPAddress(value=1.2.3.4)>
     >>> parse_general_name('fd00::1')
@@ -380,15 +383,15 @@
     <DirectoryName(value=<Name([<NameAttribute(oid=<ObjectIdentifier(oid=2.5.4.3, name=commonName)>,
                                                value='example.com')>])>)>
 
     Some more exotic values can only be generated by using this prefix:
 
     >>> parse_general_name('rid:2.5.4.3')
     <RegisteredID(value=<ObjectIdentifier(oid=2.5.4.3, name=commonName)>)>
-    >>> parse_general_name('otherName:2.5.4.3,example.com')
+    >>> parse_general_name('otherName:2.5.4.3;UTF8:example.com')
     <OtherName(type_id=<ObjectIdentifier(oid=2.5.4.3, name=commonName)>, value=b'example.com')>
 
     If you give a prefixed value, this function is less forgiving of any typos and does not catch any
     exceptions:
 
     >>> parse_general_name('email:foo@bar com')
     Traceback (most recent call last):
@@ -425,18 +428,19 @@
         except ValueError:
             pass
         try:
             return x509.IPAddress(ip_network(name))
         except ValueError:
             pass
 
-        # Try to encode the domain name. DNSName() does not validate the domain name, but this
-        # check will fail.
+        # Try to encode as domain name. DNSName() does not validate the domain name, but this check will fail.
         if name.startswith('*.'):
             idna.encode(name[2:])
+        elif name.startswith('.'):
+            idna.encode(name[1:])
         else:
             idna.encode(name)
 
         # Almost anything passes as DNS name, so this is our default fallback
         return x509.DNSName(name)
 
     if typ == 'uri':
@@ -454,25 +458,38 @@
         except ValueError:
             pass
 
         raise ValueError('Could not parse IP address.')
     elif typ == 'rid':
         return x509.RegisteredID(x509.ObjectIdentifier(name))
     elif typ == 'othername':
-        type_id, value = name.split(',', 1)
-        type_id = x509.ObjectIdentifier(type_id)
-        value = force_bytes(value)
-        return x509.OtherName(type_id, value)
+        regex = "(.*);(.*):(.*)"
+        if re.match(regex, name) is not None:
+            oid, asn_typ, val = re.match(regex, name).groups()
+            oid = x509.ObjectIdentifier(oid)
+            if asn_typ == 'UTF8':
+                val = val.encode('utf-8')
+            elif asn_typ == 'OctetString':
+                val = bytes(bytearray.fromhex(val))
+                val = OctetString(val).dump()
+            else:
+                raise ValueError('Unsupported ASN type in otherName: %s' % asn_typ)
+            val = force_bytes(val)
+            return x509.OtherName(oid, val)
+        else:
+            raise ValueError('Incorrect otherName format: %s' % name)
     elif typ == 'dirname':
         return x509.DirectoryName(x509_name(name))
     else:
         # Try to encode the domain name. DNSName() does not validate the domain name, but this
         # check will fail.
         if name.startswith('*.'):
             idna.encode(name[2:])
+        elif name.startswith('.'):
+            idna.encode(name[1:])
         else:
             idna.encode(name)
 
         return x509.DNSName(name)
 
 
 def get_cert_builder(expires, now=None):
@@ -504,15 +521,15 @@
 
     if name is None:
         name = ca_settings.CA_DEFAULT_PROFILE
 
     profile = deepcopy(ca_settings.CA_PROFILES[name])
     kwargs = {
         'cn_in_san': profile['cn_in_san'],
-        'subject': OrderedDict(sort_subject_dict(profile['subject'])),
+        'subject': profile['subject'],
     }
     for arg in ['keyUsage', 'extendedKeyUsage']:
         config = profile.get(arg)
         if config is None or not config.get('value'):
             continue
 
         critical = config.get('critical', 'True')
```

### Comparing `django-ca-1.7.0/ca/django_ca/templates/django_ca/admin/certificate_revoke_form.html` & `django-ca-1.9.0/ca/django_ca/templates/django_ca/admin/certificate_revoke_form.html`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/templates/django_ca/admin/submit_line.html` & `django-ca-1.9.0/ca/django_ca/templates/django_ca/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/managers.py` & `django-ca-1.9.0/ca/django_ca/managers.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,25 @@
 
 from django.db import models
 from django.utils import six
 from django.utils.encoding import force_bytes
 from django.utils.encoding import force_text
 
 from . import ca_settings
+from .signals import post_create_ca
+from .signals import post_issue_cert
+from .signals import pre_create_ca
+from .signals import pre_issue_cert
+from .subject import Subject
 from .utils import EXTENDED_KEY_USAGE_MAPPING
 from .utils import KEY_USAGE_MAPPING
 from .utils import TLS_FEATURE_MAPPING
 from .utils import get_cert_builder
 from .utils import is_power2
 from .utils import parse_general_name
-from .utils import x509_name
 
 
 class CertificateManagerMixin(object):
     def get_common_extensions(self, issuer_url=None, crl_url=None, ocsp_url=None):
         extensions = []
         if crl_url:
             if isinstance(crl_url, six.string_types):
@@ -86,42 +90,49 @@
             :py:class:`~cryptography:cryptography.hazmat.primitives.hashes.HashAlgorithm`, e.g.
             :py:class:`~cryptography:cryptography.hazmat.primitives.hashes.SHA512`.
         expires : datetime
             Datetime for when this certificate expires.
         parent : :py:class:`~django_ca.models.CertificateAuthority`, optional
             Parent certificate authority for the new CA. This means that this CA will be an intermediate
             authority.
-        subject : str
-            Subject string, e.g. ``"/CN=example.com"``.
+        subject : :py:class:`~django_ca.subject.Subject`
+            Subject string, e.g. ``Subject("/CN=example.com")``.
         pathlen : int, optional
         password : bytes, optional
             Password to encrypt the private key with.
         parent_password : bytes, optional
             Password that the private key of the parent CA is encrypted with.
         """
         # NOTE: This is already verified by KeySizeAction, so none of these checks should ever be
         #       True in the real world. None the less they are here as a safety precaution.
         if not is_power2(key_size):
             raise RuntimeError("%s: Key size must be a power of two." % key_size)
         elif key_size < ca_settings.CA_MIN_KEY_SIZE:
             raise RuntimeError("%s: Key size must be least %s bits."
                                % (key_size, ca_settings.CA_MIN_KEY_SIZE))
 
+        pre_create_ca.send(
+            sender=self.model, name=name, key_size=key_size, key_type=key_type, algorithm=algorithm,
+            expires=expires, parent=parent, subject=subject, pathlen=pathlen, issuer_url=issuer_url,
+            issuer_alt_name=issuer_alt_name, crl_url=crl_url, ocsp_url=ocsp_url, ca_issuer_url=ca_issuer_url,
+            ca_crl_url=ca_crl_url, ca_ocsp_url=ca_ocsp_url, name_constraints=name_constraints,
+            password=password, parent_password=parent_password)
+
         if key_type == 'DSA':
             private_key = dsa.generate_private_key(key_size=key_size, backend=default_backend())
         else:
             private_key = rsa.generate_private_key(public_exponent=65537, key_size=key_size,
                                                    backend=default_backend())
         public_key = private_key.public_key()
-        subject = x509_name(subject)
 
         builder = get_cert_builder(expires)
         builder = builder.public_key(public_key)
-        builder = builder.subject_name(subject)
+        subject = subject.name
 
+        builder = builder.subject_name(subject)
         builder = builder.add_extension(x509.BasicConstraints(ca=True, path_length=pathlen), critical=True)
         builder = builder.add_extension(x509.KeyUsage(
             key_cert_sign=True, crl_sign=True, digital_signature=False, content_commitment=False,
             key_encipherment=False, data_encipherment=False, key_agreement=False, encipher_only=False,
             decipher_only=False), critical=True)
 
         subject_key_id = x509.SubjectKeyIdentifier.from_public_key(public_key)
@@ -140,15 +151,14 @@
                 ExtensionOID.AUTHORITY_KEY_IDENTIFIER).value
 
         builder = builder.add_extension(auth_key_id, critical=False)
 
         for critical, ext in self.get_common_extensions(ca_issuer_url, ca_crl_url, ca_ocsp_url):
             builder = builder.add_extension(ext, critical=critical)
 
-        # TODO: pass separate lists maybe?
         if name_constraints:
             excluded = []
             permitted = []
             for constraint in name_constraints:
                 typ, name = constraint.split(',', 1)
                 parsed = parse_general_name(name)
                 if typ == 'permitted':
@@ -181,14 +191,15 @@
         pem = private_key.private_bytes(encoding=Encoding.PEM,
                                         format=PrivateFormat.TraditionalOpenSSL,
                                         encryption_algorithm=encryption)
         with open(ca.private_key_path, 'wb') as key_file:
             key_file.write(pem)
         os.umask(oldmask)
 
+        post_create_ca.send(sender=self.model, ca=ca)
         return ca
 
 
 class CertificateManager(CertificateManagerMixin, models.Manager):
     def sign_cert(self, ca, csr, expires, algorithm, subject=None, cn_in_san=True, csr_format=Encoding.PEM,
                   subjectAltName=None, keyUsage=None, extendedKeyUsage=None, tls_features=None,
                   password=None):
@@ -240,26 +251,28 @@
         Returns
         -------
 
         cryptography.x509.Certificate
             The signed certificate.
         """
         if subject is None:
-            subject = {}
-        if not subject.get('CN') and not subjectAltName:
+            subject = Subject()
+
+        if 'CN' not in subject and not subjectAltName:
             raise ValueError("Must name at least a CN or a subjectAltName.")
 
         if subjectAltName:
             subjectAltName = [parse_general_name(san) for san in subjectAltName]
         else:
             subjectAltName = []  # so we can append the CN if requested
 
-        if not subject.get('CN'):  # use first SAN as CN if CN is not set
+        # use first SAN as CN if CN is not set
+        if 'CN' not in subject:
             subject['CN'] = subjectAltName[0].value
-        elif cn_in_san and subject.get('CN'):  # add CN to SAN if cn_in_san is True (default)
+        elif cn_in_san and 'CN' in subject:  # add CN to SAN if cn_in_san is True (default)
             try:
                 cn_name = parse_general_name(subject['CN'])
             except idna.IDNAError:
                 raise ValueError('%s: Could not parse CommonName as subjectAltName.' % subject['CN'])
             else:
                 if cn_name not in subjectAltName:
                     subjectAltName.insert(0, cn_name)
@@ -272,16 +285,15 @@
             raise ValueError('Unknown CSR format passed: %s' % csr_format)
 
         public_key = req.public_key()
 
         builder = get_cert_builder(expires)
         builder = builder.public_key(public_key)
         builder = builder.issuer_name(ca.x509.subject)
-
-        builder = builder.subject_name(x509_name(subject))
+        builder = builder.subject_name(subject.name)
 
         # Add extensions
         builder = builder.add_extension(x509.BasicConstraints(ca=False, path_length=None), critical=True)
         builder = builder.add_extension(
             x509.SubjectKeyIdentifier.from_public_key(public_key), critical=False)
 
         # Get authorityKeyIdentifier from subjectKeyIdentifier from signing CA
@@ -316,13 +328,17 @@
 
         if ca.issuer_alt_name:
             builder = builder.add_extension(x509.IssuerAlternativeName(
                 [parse_general_name(ca.issuer_alt_name)]), critical=False)
 
         return builder.sign(private_key=ca.key(password), algorithm=algorithm, backend=default_backend()), req
 
-    def init(self, ca, csr, *args, **kwargs):
+    def init(self, ca, csr, **kwargs):
+        pre_issue_cert.send(sender=self.model, ca=ca, csr=csr, **kwargs)
+
         c = self.model(ca=ca)
-        c.x509, csr = self.sign_cert(ca, csr, *args, **kwargs)
+        c.x509, csr = self.sign_cert(ca, csr, **kwargs)
         c.csr = csr.public_bytes(Encoding.PEM).decode('utf-8')
         c.save()
+
+        post_issue_cert.send(sender=self.model, cert=c)
         return c
```

### Comparing `django-ca-1.7.0/ca/django_ca/admin.py` & `django-ca-1.9.0/ca/django_ca/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,61 +9,61 @@
 # django-ca is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with django-ca.  If not,
 # see <http://www.gnu.org/licenses/>.
 
+import binascii
 import copy
 import json
 import os
 from datetime import datetime
+from functools import partial
 
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.serialization import Encoding
+from cryptography.x509.certificate_transparency import LogEntryType
+from cryptography.x509.extensions import UnrecognizedExtension
+from cryptography.x509.oid import ExtensionOID
 
 from django.conf.urls import url
 from django.contrib import admin
 from django.core.exceptions import PermissionDenied
 from django.http import Http404
 from django.http import HttpResponse
 from django.http import HttpResponseBadRequest
-from django.utils import six
+from django.template.loader import render_to_string
 from django.utils import timezone
 from django.utils.encoding import force_bytes
+from django.utils.html import escape
 from django.utils.html import mark_safe
 from django.utils.translation import ugettext_lazy as _
 
+from . import ca_settings
 from .forms import CreateCertificateForm
 from .forms import X509CertMixinAdminForm
 from .models import Certificate
 from .models import CertificateAuthority
 from .models import Watcher
+from .signals import post_issue_cert
+from .signals import pre_issue_cert
 from .utils import OID_NAME_MAPPINGS
 from .views import RevokeCertificateView
 
 
 @admin.register(Watcher)
 class WatcherAdmin(admin.ModelAdmin):
     pass
 
 
 class CertificateMixin(object):
     form = X509CertMixinAdminForm
 
-    def hpkp_pin(self, obj):
-        # TODO/Django 1.9: We replace newlines because Django 1.8 inserts HTML breaks for them
-
-        help_text = '''<p class="help">SHA-256 HPKP pin of this certificate. See also
-<a href="https://en.wikipedia.org/wiki/HTTP_Public_Key_Pinning">HTTP Public Key Pinning</a>
-on Wikipedia.</p>'''.replace('\n', ' ')
-        return mark_safe('%s%s' % (obj.hpkp_pin, help_text))
-    hpkp_pin.short_description = _('HPKP pin (SHA-256)')
-
     def get_urls(self):
         info = self.model._meta.app_label, self.model._meta.model_name
         urls = [
             url(r'^(?P<pk>\d+)/download/$', self.admin_site.admin_view(self.download_view),
                 name='%s_%s_download' % info),
         ]
         urls += super(CertificateMixin, self).get_urls()
@@ -106,34 +106,46 @@
         Otherwise the action is present even though has_delete_permission is False, it just doesn't
         work.
         """
         actions = super(CertificateMixin, self).get_actions(request)
         actions.pop('delete_selected', '')
         return actions
 
+    def hpkp_pin(self, obj):
+        return obj.hpkp_pin
+    hpkp_pin.short_description = _('HPKP pin')
+
+    def cn_display(self, obj):
+        if obj.cn:
+            return obj.cn
+        return _('<none>')
+    cn_display.short_description = _('CommonName')
+
     ##################################
     # Properties for x509 extensions #
     ##################################
 
     def output_extension(self, value):
         # shared function for formatting extension values
+        if value is None:
+            return '<none>'
 
         critical, value = value
         html = ''
         if critical is True:
             text = _('Critical')
             html = '<img src="/static/admin/img/icon-yes.svg" alt="%s"> %s' % (text, text)
 
-        if isinstance(value, six.string_types):
-            html += '<p>%s</p>' % value
-        else:  # list
+        if isinstance(value, list):
             html += '<ul class="x509-extension-value">'
             for val in value:
-                html += '<li>%s</li>' % val
+                html += '<li>%s</li>' % escape(val)
             html += '</ul>'
+        else:  # string or extension
+            html += '<p>%s<p>' % escape(value)
 
         return mark_safe(html)
 
     def basicConstraints(self, obj):
         return self.output_extension(obj.basicConstraints())
     basicConstraints.short_description = 'basicConstraints'
 
@@ -169,50 +181,125 @@
         return self.output_extension(obj.crlDistributionPoints())
     cRLDistributionPoints.short_description = _('CRL Distribution Points')
 
     def subjectAltName(self, obj):
         return self.output_extension(obj.subjectAltName())
     subjectAltName.short_description = _('subjectAltName')
 
+    def certificatePolicies(self, obj):
+        return self.output_extension(obj.certificatePolicies())
+    certificatePolicies.short_description = _('Certificate Policies')
+
+    def signedCertificateTimestampList(self, obj):
+        try:
+            ext = obj.x509.extensions.get_extension_for_oid(
+                ExtensionOID.PRECERT_SIGNED_CERTIFICATE_TIMESTAMPS)
+        except x509.ExtensionNotFound:  # pragma: no cover - method is only called when extension exists.
+            return ''
+
+        if isinstance(ext.value, UnrecognizedExtension):
+            return render_to_string('django_ca/admin/unrecognizedextension.html', {
+                'critical': ext.critical or True,
+                'entries': ext.value,
+            })
+
+        entries = []
+        for entry in ext.value:
+            if entry.entry_type == LogEntryType.PRE_CERTIFICATE:
+                entry_type = 'Precertificate'
+            elif entry.entry_type == LogEntryType.X509_CERTIFICATE:  # pragma: no cover - unseen in the wild
+                # NOTE: same pragma is also in django_ca.models.X509CertMixin.signedCertificateTimestampList
+                entry_type = 'X.509 certificate'
+            else:  # pragma: no cover - only the above two are part of the standard
+                # NOTE: same pragma is also in django_ca.models.X509CertMixin.signedCertificateTimestampList
+                entry_type = _('Unknown type')
+
+            entries.append([
+                entry_type,
+                entry.version.name,
+                entry.timestamp,
+                binascii.hexlify(entry.log_id).decode('utf-8'),  # sha256 hash
+            ])
+
+        return render_to_string('django_ca/admin/signedCertificateTimestampList.html', {
+            'critical': ext.critical or True,
+            'entries': entries,
+        })
+    signedCertificateTimestampList.short_description = _('Signed Certificate Timestamps')
+
+    def unknown_oid(self, oid, obj):
+        ext = obj.x509.extensions.get_extension_for_oid(oid)
+        return self.output_extension((ext.critical, ext.value))
+
+    def get_oid_name(self, oid):
+        return oid.dotted_string.replace('.', '_')
+
     def get_fieldsets(self, request, obj=None):
         fieldsets = super(CertificateMixin, self).get_fieldsets(request, obj=obj)
 
         if obj is None:
             return fieldsets
 
         fieldsets = copy.deepcopy(fieldsets)
-        for name, _value in sorted(obj.extensions()):
-            # TODO: we should handle unknown extensions here
-            fieldsets[self.x509_fieldset_index][1]['fields'].append(name)
+        extensions = list(sorted(obj.extensions()))
+        if extensions:
+            for name, _value in sorted(obj.extensions()):
+                if not hasattr(self, name):
+                    critical, value = _value
+                    attr_name = self.get_oid_name(value)
+                    func = partial(self.unknown_oid, value)
+                    if name == 'UnknownOID':
+                        func.short_description = 'Unkown OID (%s)' % value.dotted_string
+                    else:  # pragma: no cover
+                        # If this branch happens, it means that we encounter a known (to cryptography)
+                        # extension, that we do not yet support. This is usually fixed by us supporting the
+                        # extension, so it never happens.
+                        func.short_description = name
+                    setattr(self, attr_name, func)
+                else:
+                    attr_name = name
+
+                if attr_name == 'subjectAltName':  # already displayed in main section
+                    continue
+
+                fieldsets[self.x509_fieldset_index][1]['fields'].append(attr_name)
+        else:
+            fieldsets.pop(self.x509_fieldset_index)
 
         return fieldsets
 
     def get_readonly_fields(self, request, obj=None):
         fields = super(CertificateMixin, self).get_readonly_fields(request, obj=obj)
 
         if obj is None:  # pragma: no cover
             # This is never True because CertificateAdmin (the only case where objects are added) doesn't call
             # the superclass in this case.
             return fields
 
-        return list(fields) + list(dict(obj.extensions()).keys())
+        fields = list(fields)
+        for name, value in obj.extensions():
+            if not hasattr(self, name):
+                fields.append(self.get_oid_name(value[1]))
+            else:
+                fields.append(name)
+        return fields
 
     class Media:
         css = {
             'all': (
                 'django_ca/admin/css/base.css',
             ),
         }
 
 
 @admin.register(CertificateAuthority)
 class CertificateAuthorityAdmin(CertificateMixin, admin.ModelAdmin):
     fieldsets = (
         (None, {
-            'fields': ['name', 'enabled', 'cn', 'parent', 'hpkp_pin', ],
+            'fields': ['name', 'enabled', 'cn_display', 'parent', 'hpkp_pin', ],
         }),
         (_('Details'), {
             'description': _('Information to add to newly signed certificates.'),
             'fields': ['crl_url', 'issuer_url', 'ocsp_url', 'issuer_alt_name', ],
         }),
         (_('Certificate'), {
             'fields': ['serial', 'pub', 'expires'],
@@ -223,15 +310,15 @@
         (_('X509 extensions'), {
             'fields': [],  # dynamically added by add_fieldsets
         }),
     )
     list_display = ['enabled', 'name', 'serial', ]
     list_display_links = ['enabled', 'name', ]
     search_fields = ['cn', 'name', 'serial', ]
-    readonly_fields = ['serial', 'pub', 'parent', 'cn', 'expires', 'hpkp_pin', ]
+    readonly_fields = ['serial', 'pub', 'parent', 'cn_display', 'expires', 'hpkp_pin', ]
     x509_fieldset_index = 3
 
     def has_add_permission(self, request):
         return False
 
     class Media:
         css = {
@@ -262,27 +349,27 @@
             return queryset.revoked()
 
 
 @admin.register(Certificate)
 class CertificateAdmin(CertificateMixin, admin.ModelAdmin):
     actions = ['revoke', ]
     change_form_template = 'django_ca/admin/change_form.html'
-    list_display = ('cn', 'serial', 'status', 'expires_date')
+    list_display = ('cn_display', 'serial', 'status', 'expires_date')
     list_filter = (StatusListFilter, 'ca')
     readonly_fields = [
-        'expires', 'csr', 'pub', 'cn', 'serial', 'revoked', 'revoked_date', 'revoked_reason',
-        'distinguishedName', 'ca', 'hpkp_pin', ]
+        'expires', 'csr', 'pub', 'cn_display', 'serial', 'revoked', 'revoked_date', 'revoked_reason',
+        'distinguishedName', 'ca', 'hpkp_pin', 'subjectAltName']
     search_fields = ['cn', 'serial', ]
 
     fieldsets = [
         (None, {
-            'fields': ['cn', 'subjectAltName', 'distinguishedName', 'serial', 'ca', 'expires',
+            'fields': ['cn_display', 'subjectAltName', 'distinguishedName', 'serial', 'ca', 'expires',
                        'watchers', 'hpkp_pin'],
         }),
-        (_('X509 Extensions'), {
+        (_('X.509 Extensions'), {
             'fields': [],
             'classes': ('collapse', ),
         }),
         (_('Revocation'), {
             'fields': ('revoked', 'revoked_date', 'revoked_reason', ),
         }),
         (_('Certificate'), {
@@ -293,15 +380,15 @@
         }),
     ]
     add_fieldsets = [
         (None, {
             'fields': ['csr', ('ca', 'password'), 'profile', 'subject', 'subjectAltName', 'algorithm',
                        'expires', 'watchers', ],
         }),
-        (_('X509 Extensions'), {
+        (_('X.509 Extensions'), {
             'fields': ['keyUsage', 'extendedKeyUsage', 'tlsFeature', ]
         }),
     ]
     x509_fieldset_index = 1
 
     def has_add_permission(self, request):
         # Only grant add permissions if there is at least one useable CA
@@ -312,14 +399,19 @@
 
     def get_form(self, request, obj=None, **kwargs):
         if obj is None:
             return CreateCertificateForm
         else:
             return super(CertificateAdmin, self).get_form(request, obj=obj, **kwargs)
 
+    def get_changeform_initial_data(self, request):
+        data = super(CertificateAdmin, self).get_changeform_initial_data(request)
+        data['subject'] = ca_settings.CA_PROFILES[ca_settings.CA_DEFAULT_PROFILE].get('subject', {})
+        return data
+
     def csr_details_view(self, request):
         """Returns details of a CSR request."""
 
         if not request.user.is_staff or not self.has_change_permission(request):
             # NOTE: is_staff is already assured by ModelAdmin, but just to be sure
             raise PermissionDenied
 
@@ -391,29 +483,40 @@
     def save_model(self, request, obj, form, change):
         data = form.cleaned_data
 
         # If this is a new certificate, initialize it.
         if change is False:
             san, cn_in_san = data['subjectAltName']
             expires = datetime.combine(data['expires'], datetime.min.time())
+            subjectAltName = [e.strip() for e in san.split(',') if e.strip()]
 
-            obj.x509, req = self.model.objects.sign_cert(
-                ca=data['ca'],
-                csr=data['csr'],
-                expires=expires,
-                subject=data['subject'],
-                algorithm=data['algorithm'],
-                subjectAltName=[e.strip() for e in san.split(',') if e.strip()],
-                cn_in_san=cn_in_san,
-                keyUsage=data['keyUsage'],
-                extendedKeyUsage=data['extendedKeyUsage'],
-                tls_features=data['tlsFeature'],
-                password=data['password']
-            )
-        obj.save()
+            kwargs = {
+                'ca': data['ca'],
+                'csr': data['csr'],
+                'expires': expires,
+                'subject': data['subject'],
+                'algorithm': data['algorithm'],
+                'subjectAltName': subjectAltName,
+                'cn_in_san': cn_in_san,
+                'keyUsage': data['keyUsage'],
+                'extendedKeyUsage': data['extendedKeyUsage'],
+                'tls_features': data['tlsFeature'],
+                'password': data['password'],
+            }
+
+            pre_issue_cert.send(sender=self.model, **kwargs)
+
+            # Note: CSR is set by model form already
+            obj.x509, req = self.model.objects.sign_cert(**kwargs)
+            obj.save()
+
+            # call signals
+            post_issue_cert.send(sender=self.model, cert=obj)
+        else:
+            obj.save()
 
     class Media:
         css = {
             'all': (
                 'django_ca/admin/css/base.css',
                 'django_ca/admin/css/certificateadmin.css',
             ),
```

### Comparing `django-ca-1.7.0/ca/django_ca/ca_settings.py` & `django-ca-1.9.0/ca/django_ca/ca_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with django-ca.  If not,
 # see <http://www.gnu.org/licenses/>.
 
 import os
 
+from cryptography.hazmat.primitives import hashes
+
 from django.conf import settings
+from django.core.exceptions import ImproperlyConfigured
 from django.utils.translation import ugettext_lazy as _
 
 CA_DIR = getattr(settings, 'CA_DIR', os.path.join(settings.BASE_DIR, 'files'))
 
 CA_PROFILES = {
     'client': {
         # see: http://security.stackexchange.com/questions/68491/
@@ -130,13 +133,18 @@
     else:
         profile.setdefault('subject', _CA_DEFAULT_SUBJECT)
         profile.setdefault('cn_in_san', True)
         CA_PROFILES[name] = profile
 
 CA_DEFAULT_EXPIRES = getattr(settings, 'CA_DEFAULT_EXPIRES', 730)
 CA_DEFAULT_PROFILE = getattr(settings, 'CA_DEFAULT_PROFILE', 'webserver')
-CA_DIGEST_ALGORITHM = getattr(settings, 'CA_DIGEST_ALGORITHM', "sha512")
 CA_NOTIFICATION_DAYS = getattr(settings, 'CA_NOTIFICATION_DAYS', [14, 7, 3, 1, ])
 
 # Undocumented options, e.g. to share values between different parts of code
 CA_MIN_KEY_SIZE = getattr(settings, 'CA_MIN_KEY_SIZE', 2048)
 CA_PROVIDE_GENERIC_CRL = getattr(settings, 'CA_PROVIDE_GENERIC_CRL', True)
+
+CA_DIGEST_ALGORITHM = getattr(settings, 'CA_DIGEST_ALGORITHM', "sha512").strip().upper()
+try:
+    CA_DIGEST_ALGORITHM = getattr(hashes, CA_DIGEST_ALGORITHM)()
+except AttributeError:  # pragma: no cover
+    raise ImproperlyConfigured('Unkown CA_DIGEST_ALGORITHM: %s' % settings.CA_DIGEST_ALGORITHM)
```

### Comparing `django-ca-1.7.0/ca/django_ca/fields.py` & `django-ca-1.9.0/ca/django_ca/fields.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 # django-ca is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with django-ca.  If not,
 # see <http://www.gnu.org/licenses/>.
 
-from collections import OrderedDict
 
 from django import forms
 
 from . import ca_settings
+from .subject import Subject
 from .utils import SUBJECT_FIELDS
 from .widgets import KeyUsageWidget
 from .widgets import SubjectAltNameWidget
 from .widgets import SubjectWidget
 
 
 class SubjectField(forms.MultiValueField):
@@ -31,23 +31,24 @@
             forms.CharField(required=False),  # ST
             forms.CharField(required=False),  # L
             forms.CharField(required=False),  # O
             forms.CharField(required=False),  # OU
             forms.CharField(),  # CN
             forms.CharField(required=False),  # E
         )
-        initial = ca_settings.CA_PROFILES[ca_settings.CA_DEFAULT_PROFILE].get('subject', {})
-        kwargs.setdefault('initial', initial)
+
+        # NOTE: do not pass initial here as this is done on webserver invocation
+        #       This screws up tests.
         kwargs.setdefault('widget', SubjectWidget)
         super(SubjectField, self).__init__(fields=fields, require_all_fields=False,
                                            *args, **kwargs)
 
     def compress(self, values):
         # list comprehension is to filter empty fields
-        return OrderedDict([(k, v) for k, v in zip(SUBJECT_FIELDS, values) if v])
+        return Subject([(k, v) for k, v in zip(SUBJECT_FIELDS, values) if v])
 
 
 class SubjectAltNameField(forms.MultiValueField):
     def __init__(self, *args, **kwargs):
         fields = (
             forms.CharField(required=False),
             forms.BooleanField(required=False),
```

### Comparing `django-ca-1.7.0/ca/django_ca/migrations/0001_initial.py` & `django-ca-1.9.0/ca/django_ca/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/migrations/0005_auto_20170307_1839.py` & `django-ca-1.9.0/ca/django_ca/migrations/0005_auto_20170307_1839.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/migrations/0003_auto_20170304_1434.py` & `django-ca-1.9.0/ca/django_ca/migrations/0003_auto_20170304_1434.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/migrations/0002_auto_20170304_1434.py` & `django-ca-1.9.0/ca/django_ca/migrations/0002_auto_20170304_1434.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/migrations/0007_auto_20171119_1100.py` & `django-ca-1.9.0/ca/django_ca/migrations/0007_auto_20171119_1100.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/migrations/0004_auto_20170304_1442.py` & `django-ca-1.9.0/ca/django_ca/migrations/0004_auto_20170304_1442.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/migrations/0008_auto_20171203_2001.py` & `django-ca-1.9.0/ca/django_ca/migrations/0008_auto_20171203_2001.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/models.py` & `django-ca-1.9.0/ca/django_ca/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,42 +13,48 @@
 # You should have received a copy of the GNU General Public License along with django-ca.  If not,
 # see <http://www.gnu.org/licenses/>.
 
 import base64
 import binascii
 import hashlib
 import re
-from collections import OrderedDict
+from datetime import datetime
+from datetime import timedelta
 
 import pytz
 
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.serialization import Encoding
 from cryptography.hazmat.primitives.serialization import PublicFormat
 from cryptography.hazmat.primitives.serialization import load_pem_private_key
 from cryptography.x509 import TLSFeatureType
+from cryptography.x509.certificate_transparency import LogEntryType
+from cryptography.x509.extensions import UnrecognizedExtension
 from cryptography.x509.oid import AuthorityInformationAccessOID
 from cryptography.x509.oid import ExtensionOID
 
 from django.conf import settings
 from django.db import models
 from django.utils import timezone
 from django.utils.encoding import force_bytes
 from django.utils.encoding import force_str
 from django.utils.translation import ugettext_lazy as _
 
+from . import ca_settings
 from .managers import CertificateAuthorityManager
 from .managers import CertificateManager
 from .querysets import CertificateAuthorityQuerySet
 from .querysets import CertificateQuerySet
+from .signals import post_revoke_cert
+from .signals import pre_revoke_cert
+from .subject import Subject
 from .utils import EXTENDED_KEY_USAGE_REVERSED
 from .utils import KEY_USAGE_MAPPING
-from .utils import OID_NAME_MAPPINGS
 from .utils import add_colons
 from .utils import format_general_name
 from .utils import format_general_names
 from .utils import format_name
 from .utils import int_to_hex
 from .utils import multiline_url_validator
 
@@ -121,46 +127,46 @@
             self._x509 = x509.load_pem_x509_certificate(force_bytes(self.pub), backend)
         return self._x509
 
     @x509.setter
     def x509(self, value):
         self._x509 = value
         self.pub = force_str(self.dump_certificate(Encoding.PEM))
-        self.cn = self.subject['CN']
+        self.cn = self.subject.get('CN', '')
         self.expires = self.not_after
         if settings.USE_TZ:
             self.expires = timezone.make_aware(self.expires, timezone=pytz.utc)
 
         self.serial = int_to_hex(value.serial_number)
 
     @property
     def subject(self):
-        return OrderedDict([(OID_NAME_MAPPINGS[s.oid], s.value) for s in self.x509.subject])
+        return Subject([(s.oid, s.value) for s in self.x509.subject])
 
     @property
     def issuer(self):
-        return OrderedDict([(OID_NAME_MAPPINGS[s.oid], s.value) for s in self.x509.issuer])
+        return Subject([(s.oid, s.value) for s in self.x509.issuer])
 
     @property
     def not_before(self):
         return self.x509.not_valid_before
 
     @property
     def not_after(self):
         return self.x509.not_valid_after
 
     def extensions(self):
         for ext in sorted(self.x509.extensions, key=lambda e: e.oid._name):
-            name = ext.oid._name
+            name = ext.oid._name.replace(' ', '')
             if hasattr(self, name):
                 yield name, getattr(self, name)()
             elif name == 'cRLDistributionPoints':
                 yield name, self.crlDistributionPoints()
             else:  # pragma: no cover  - we have a function for everything we support
-                yield name, str(ext.value)
+                yield name, (ext.critical, ext.oid)
 
     def distinguishedName(self):
         return format_name(self.x509.subject)
     distinguishedName.short_description = 'Distinguished Name'
 
     def subjectAltName(self):
         try:
@@ -184,32 +190,32 @@
                 value.append('Relative Name: %s' % format_name(dp.relative_name.value))
 
         return ext.critical, value
 
     def authorityInfoAccess(self):
         try:
             ext = self.x509.extensions.get_extension_for_oid(ExtensionOID.AUTHORITY_INFORMATION_ACCESS)
-        except x509.ExtensionNotFound:  # pragma: no cover - extension should always be present
+        except x509.ExtensionNotFound:
             return None
 
         output = []
         for desc in ext.value:
             if desc.access_method == AuthorityInformationAccessOID.OCSP:
                 output.append('OCSP - %s' % format_general_name(desc.access_location))
             elif desc.access_method == AuthorityInformationAccessOID.CA_ISSUERS:
                 output.append('CA Issuers - %s' % format_general_name(desc.access_location))
-            else:  # pragma: no cover - nothing else is known currently.
+            else:  # pragma: no cover - we don't know any other access methods
                 output.append('Unknown')
 
         return ext.critical, output
 
     def basicConstraints(self):
         try:
             ext = self.x509.extensions.get_extension_for_oid(ExtensionOID.BASIC_CONSTRAINTS)
-        except x509.ExtensionNotFound:  # pragma: no cover - extension should always be present
+        except x509.ExtensionNotFound:
             return None
 
         if ext.value.ca is True:
             value = 'CA:TRUE'
         else:
             value = 'CA:FALSE'
         if ext.value.path_length is not None:
@@ -240,15 +246,15 @@
             return None
 
         return ext.critical, [EXTENDED_KEY_USAGE_REVERSED[u] for u in ext.value]
 
     def subjectKeyIdentifier(self):
         try:
             ext = self.x509.extensions.get_extension_for_oid(ExtensionOID.SUBJECT_KEY_IDENTIFIER)
-        except x509.ExtensionNotFound:  # pragma: no cover - extension should always be present
+        except x509.ExtensionNotFound:
             return None
 
         hexlified = binascii.hexlify(ext.value.digest).upper().decode('utf-8')
         return ext.critical, add_colons(hexlified)
 
     def issuerAltName(self):
         try:
@@ -257,15 +263,15 @@
             return None
 
         return ext.critical, format_general_names(ext.value)
 
     def authorityKeyIdentifier(self):
         try:
             ext = self.x509.extensions.get_extension_for_oid(ExtensionOID.AUTHORITY_KEY_IDENTIFIER)
-        except x509.ExtensionNotFound:  # pragma: no cover - extension should always be present
+        except x509.ExtensionNotFound:
             return None
 
         hexlified = binascii.hexlify(ext.value.key_identifier).upper().decode('utf-8')
         return ext.critical, 'keyid:%s' % add_colons(hexlified)
 
     def TLSFeature(self):
         try:
@@ -280,14 +286,80 @@
             elif feature == TLSFeatureType.status_request_v2:
                 features.append('Multiple Certificate Status Request')
             else:  # pragma: no cover - all features of cryptography 2.1 are covered
                 features.append('Unknown TLS Feature')
 
         return ext.critical, features
 
+    def _parse_policy_qualifier(self, qualifier):
+        if isinstance(qualifier, x509.extensions.UserNotice):
+            # https://tools.ietf.org/html/rfc5280#section-4.2.1.4
+            notice_ref = qualifier.notice_reference
+            text = qualifier.explicit_text
+            if notice_ref is None:
+                return text
+            else:  # pragma: no cover - unseen in the wild
+                org = notice_ref.organization
+                numbers = notice_ref.notice_numbers
+                if not numbers:
+                    return '%s (Reference: %s)' % (text, org)
+                elif len(numbers) == 1:
+                    return '%s (Reference: %s, number %s)' % (text, org, numbers[0])
+                else:
+                    return '%s (Reference: %s, numbers %s)' % (text, org, ', '.join(numbers))
+
+        return qualifier
+
+    def certificatePolicies(self):
+        try:
+            ext = self.x509.extensions.get_extension_for_oid(ExtensionOID.CERTIFICATE_POLICIES)
+        except x509.ExtensionNotFound:
+            return None
+
+        policies = []
+        for value in ext.value:
+            output = 'OID %s: ' % value.policy_identifier.dotted_string
+            if value.policy_qualifiers is None:
+                output += "None"
+            else:
+                output += ', '.join([self._parse_policy_qualifier(p) for p in value.policy_qualifiers])
+            policies.append(output)
+
+        return ext.critical, policies
+
+    def signedCertificateTimestampList(self):
+        try:
+            ext = self.x509.extensions.get_extension_for_oid(
+                ExtensionOID.PRECERT_SIGNED_CERTIFICATE_TIMESTAMPS)
+        except x509.ExtensionNotFound:
+            return None
+
+        if isinstance(ext.value, UnrecognizedExtension):
+            # Older versions of OpenSSL (and LibreSSL) cannot parse this extension
+            # see https://github.com/pyca/cryptography/blob/master/tests/x509/test_x509_ext.py#L4455-L4459
+            return ext.critical, ['Parsing requires OpenSSL 1.1.0f+']
+
+        timestamps = []
+        for entry in ext.value:
+            if entry.entry_type == LogEntryType.PRE_CERTIFICATE:
+                entry_type = 'Precertificate'
+            elif entry.entry_type == LogEntryType.X509_CERTIFICATE:  # pragma: no cover - unseen in the wild
+                # NOTE: same pragma is also in django_ca.admin.CertificateMixin.signedCertificateTimestampList
+                entry_type = 'x509 certificate'
+            else:  # pragma: no cover - only the above two are part of the standard
+                # NOTE: same pragma is also in django_ca.admin.CertificateMixin.signedCertificateTimestampList
+                entry_type = 'unknown'
+
+            timestamps.append('%s (%s): %s\n%s' % (
+                entry_type, entry.version.name, entry.timestamp,
+                '\n%s' % binascii.hexlify(entry.log_id).decode('utf-8')
+            ))
+
+        return ext.critical, timestamps
+
     def get_digest(self, algo):
         algo = getattr(hashes, algo.upper())()
         return add_colons(binascii.hexlify(self.x509.fingerprint(algo)).upper().decode('utf-8'))
 
     @property
     def hpkp_pin(self):
         # taken from https://github.com/luisgf/hpkp-python/blob/master/hpkp.py
@@ -297,27 +369,31 @@
         public_key_hash = hashlib.sha256(public_key_raw).digest()
         return base64.b64encode(public_key_hash).decode('utf-8')
 
     def dump_certificate(self, encoding=Encoding.PEM):
         return self.x509.public_bytes(encoding=encoding)
 
     def revoke(self, reason=None):
+        pre_revoke_cert.send(sender=self.__class__, cert=self, reason=reason)
+
         self.revoked = True
         self.revoked_date = timezone.now()
         self.revoked_reason = reason
         self.save()
 
+        post_revoke_cert.send(sender=self.__class__, cert=self)
+
     def get_revocation(self):
         """Get a crypto.Revoked object or None if the cert is not revoked."""
 
         if self.revoked is False:
             raise ValueError('Certificate is not revoked.')
 
-        revoked_cert = x509.RevokedCertificateBuilder().serial_number(self.x509.serial).revocation_date(
-            self.revoked_date)
+        revoked_cert = x509.RevokedCertificateBuilder().serial_number(
+            self.x509.serial_number).revocation_date(self.revoked_date)
 
         if self.revoked_reason:
             reason_flag = getattr(x509.ReasonFlags, self.revoked_reason)
             revoked_cert = revoked_cert.add_extension(x509.CRLReason(reason_flag), critical=False)
 
         return revoked_cert.build(default_backend())
 
@@ -334,15 +410,14 @@
 
 
 class CertificateAuthority(X509CertMixin):
     objects = CertificateAuthorityManager.from_queryset(CertificateAuthorityQuerySet)()
 
     name = models.CharField(max_length=32, help_text=_('A human-readable name'), unique=True)
     enabled = models.BooleanField(default=True)
-    # WARNING: on_delete MUST be a keyword argument in Django 1.8.
     parent = models.ForeignKey('self', on_delete=models.SET_NULL, null=True, blank=True,
                                related_name='children')
     private_key_path = models.CharField(max_length=256, help_text=_('Path to the private key.'))
 
     # various details used when signing certs
     crl_url = models.TextField(blank=True, null=True, validators=[multiline_url_validator],
                                verbose_name=_('CRL URLs'),
@@ -355,15 +430,17 @@
                                       help_text=_("URL for your CA."))
 
     _key = None
 
     def key(self, password):
         if self._key is None:
             with open(self.private_key_path, 'rb') as f:
-                self._key = load_pem_private_key(f.read(), password, default_backend())
+                key_data = f.read()
+
+            self._key = load_pem_private_key(key_data, password, default_backend())
         return self._key
 
     @property
     def pathlen(self):
         try:
             ext = self.x509.extensions.get_extension_for_oid(ExtensionOID.BASIC_CONSTRAINTS)
         except x509.ExtensionNotFound:  # pragma: no cover - extension should always be present
@@ -418,14 +495,43 @@
 
 
 class Certificate(X509CertMixin):
     objects = CertificateManager.from_queryset(CertificateQuerySet)()
 
     watchers = models.ManyToManyField(Watcher, related_name='certificates', blank=True)
 
-    # WARNING: on_delete MUST be a keyword argument in Django 1.8.
     ca = models.ForeignKey(CertificateAuthority, on_delete=models.CASCADE,
                            verbose_name=_('Certificate Authority'))
     csr = models.TextField(verbose_name=_('CSR'), blank=True)
 
+    def resign(self, **kwargs):  # pragma: no cover - not used yet
+        kwargs.setdefault('algorithm', ca_settings.CA_DIGEST_ALGORITHM)
+        kwargs.setdefault('subject', self.subject)
+        kwargs.setdefault('cn_in_san', False)  # this should already be the case
+        kwargs.setdefault('subjectAltName', self.subjectAltName()[1])
+
+        now = datetime.utcnow().replace(hour=0, minute=0, second=0, microsecond=0)
+        expires = now + timedelta(days=ca_settings.CA_DEFAULT_EXPIRES)
+        kwargs.setdefault('expires', expires)
+
+        try:
+            ext_key_usage = self.x509.extensions.get_extension_for_oid(ExtensionOID.EXTENDED_KEY_USAGE)
+            kwargs.setdefault('extendedKeyUsage', (ext_key_usage.critical, ext_key_usage.value))
+        except x509.ExtensionNotFound:
+            pass
+
+        try:
+            key_usage = self.x509.extensions.get_extension_for_oid(ExtensionOID.KEY_USAGE)
+            kwargs.setdefault('keyUsage', (key_usage.critical, key_usage.value))
+        except x509.ExtensionNotFound:
+            pass
+
+        try:
+            tls_features = self.x509.extensions.get_extension_for_oid(ExtensionOID.TLS_FEATURE)
+            kwargs.setdefault('tls_features', (tls_features.critical, tls_features.value))
+        except x509.ExtensionNotFound:
+            pass
+
+        return Certificate.objects.init(self.ca, self.csr, **kwargs)
+
     def __str__(self):
         return self.cn
```

### Comparing `django-ca-1.7.0/ca/django_ca/management/base.py` & `django-ca-1.9.0/ca/django_ca/management/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,35 @@
 from datetime import timedelta
 
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.serialization import Encoding
 
 from django.conf import settings
 from django.core.management.base import BaseCommand as _BaseCommand
+from django.core.management.base import CommandError
 from django.core.management.base import OutputWrapper
 from django.core.management.color import no_style
 from django.core.validators import URLValidator
 from django.utils import six
 from django.utils import timezone
 from django.utils.encoding import force_bytes
+from django.utils.encoding import force_text
 
 from django_ca import ca_settings
 from django_ca.models import Certificate
 from django_ca.models import CertificateAuthority
+from django_ca.subject import Subject
 from django_ca.utils import SUBJECT_FIELDS
 from django_ca.utils import is_power2
-from django_ca.utils import parse_name
 
 
 class SubjectAction(argparse.Action):
     def __call__(self, parser, namespace, value, option_string=None):
         try:
-            value = parse_name(value)
+            value = Subject(value)
         except ValueError as e:
             parser.error(e)
         setattr(namespace, self.dest, value)
 
 
 class FormatAction(argparse.Action):
     def __call__(self, parser, namespace, value, option_string=None):
@@ -62,18 +64,16 @@
             parser.error('Unknown format "%s".' % value)
 
         setattr(namespace, self.dest, value)
 
 
 class AlgorithmAction(argparse.Action):
     def __call__(self, parser, namespace, value, option_string=None):
-        value = value.strip().upper()
-
         try:
-            value = getattr(hashes, value)()
+            value = getattr(hashes, value.upper().strip())()
         except AttributeError:
             parser.error('Unknown hash algorithm: %s' % value)
 
         setattr(namespace, self.dest, value)
 
 
 class KeySizeAction(argparse.Action):
@@ -138,21 +138,14 @@
         except CertificateAuthority.MultipleObjectsReturned:
             parser.error('%s: Multiple Certificate authorities match.' % value)
 
         # verify that the private key exists
         if not os.path.exists(value.private_key_path):
             parser.error('%s: %s: Private key does not exist.' % (value, value.private_key_path))
 
-        # try to parse the private key
-        # TODO: Must be moved into a the Command implementation itself, since any password is available here.
-        try:
-            value.key(None)
-        except Exception as e:
-            raise parser.error('%s: %s: Could not read private key: %s' % (value, value.private_key_path, e))
-
         setattr(namespace, self.dest, value)
 
 
 class URLAction(argparse.Action):
     def __call__(self, parser, namespace, value, option_string=None):
         validator = URLValidator()
         try:
@@ -217,17 +210,14 @@
             msg += ending
         self._out.write(msg)
 
 
 class BaseCommand(_BaseCommand):
     binary_output = False
 
-    # TODO/Django1.9: Only necessary in Django 1.8
-    requires_system_checks = True
-
     def __init__(self, stdout=None, stderr=None, no_color=False):
         if self.binary_output is True and six.PY3 is True:
             self.stdout = BinaryOutputWrapper(stdout or sys.stdout.buffer)
             self.stderr = BinaryOutputWrapper(stderr or sys.stderr.buffer)
             self.style = no_style()
         else:
             super(BaseCommand, self).__init__(stdout, stderr, no_color=no_color)
@@ -241,26 +231,20 @@
             options['no_color'] = True
 
         super(BaseCommand, self).execute(*args, **options)
 
     def add_algorithm(self, parser):
         """Add the --algorithm option."""
 
-        default = ca_settings.CA_DIGEST_ALGORITHM
-
-        try:
-            default = getattr(hashes, default.upper())()
-        except AttributeError:
-            parser.error('Unknown hash algorithm: %s' % default)
-
         help = 'The HashAlgorithm that will be used to generate the signature (default: %(default)s).' % {
-            'default': default.name, }
+            'default': ca_settings.CA_DIGEST_ALGORITHM.name, }
 
         parser.add_argument(
-            '--algorithm', metavar='{sha512,sha256,...}', default=default, action=AlgorithmAction, help=help)
+            '--algorithm', metavar='{sha512,sha256,...}', default=ca_settings.CA_DIGEST_ALGORITHM,
+            action=AlgorithmAction, help=help)
 
     @property
     def valid_subject_keys(self):
         fields = ['"%s"' % f for f in SUBJECT_FIELDS]
         return '%s and %s' % (', '.join(fields[:-1]), fields[-1])
 
     def add_subject(self, parser, arg='subject', metavar=None, help=None):
@@ -294,19 +278,19 @@
             help = 'Password used for accessing the private key of the CA.'
         parser.add_argument('-p', '--password', nargs='?', action=PasswordAction, help=help)
 
     def indent(self, s, prefix='    '):
         if isinstance(s, list):
             return ''.join(['%s* %s\n' % (prefix, l) for l in s])
         elif six.PY3:
-            return textwrap.indent(s, prefix)
+            return textwrap.indent(force_text(s), prefix)
         else:  # pragma: no cover
             # copied from py3.4 version of textwrap.indent
             def prefixed_lines():
-                for line in s.splitlines(True):
+                for line in force_text(s).splitlines(True):
                     yield prefix + line
 
             return ''.join(prefixed_lines())
 
     def print_extension(self, name, value):
         critical, value = value
         if critical:
@@ -316,14 +300,20 @@
 
         self.stdout.write(self.indent(value))
 
     def print_extensions(self, cert):
         for name, value in sorted(dict(cert.extensions()).items()):
             self.print_extension(name, value)
 
+    def test_private_key(self, ca, password):
+        try:
+            ca.key(password)
+        except Exception as e:
+            raise CommandError(str(e))
+
 
 class CertCommand(BaseCommand):
     allow_revoked = False
 
     def add_arguments(self, parser):
         parser.add_argument(
             'cert', action=CertificateAction, allow_revoked=self.allow_revoked,
```

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/revoke_cert.py` & `django-ca-1.9.0/ca/django_ca/management/commands/revoke_cert.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/view_ca.py` & `django-ca-1.9.0/ca/django_ca/management/commands/view_ca.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/list_cas.py` & `django-ca-1.9.0/ca/django_ca/management/commands/list_cas.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/import_cert.py` & `django-ca-1.9.0/ca/django_ca/management/commands/import_cert.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/dump_ocsp_index.py` & `django-ca-1.9.0/ca/django_ca/management/commands/dump_ocsp_index.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/edit_ca.py` & `django-ca-1.9.0/ca/django_ca/management/commands/edit_ca.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/sign_cert.py` & `django-ca-1.9.0/ca/django_ca/management/commands/sign_cert.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 # django-ca is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without
 # even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with django-ca.  If not,
 # see <http://www.gnu.org/licenses/>.
 
-from collections import OrderedDict
-
 from django.core.management.base import CommandError
 from django.utils import six
 from django.utils import timezone
 
 from ... import ca_settings
 from ...management.base import BaseCommand
 from ...models import Certificate
 from ...models import Watcher
+from ...subject import Subject
 from ...utils import get_cert_profile_kwargs
 from ..base import ExpiresAction
 
 
 class Command(BaseCommand):
     help = """Sign a CSR and output signed certificate. The defaults depend on the configured
 default profile, currently %s.""" % ca_settings.CA_DEFAULT_PROFILE
@@ -88,21 +87,26 @@
         parser.add_argument(
             '--watch', metavar='EMAIL', action='append', default=[],
             help='Email EMAIL when this certificate expires (may be given multiple times)')
         parser.add_argument(
             '--out', metavar='FILE',
             help='Save signed certificate to FILE. If omitted, print to stdout.')
 
-        group = parser.add_argument_group('X509 v3 certificate extensions')
+        group = parser.add_argument_group(
+            'X509 v3 certificate extensions',
+            'Values for more complex x509 extensions. This is for advanced usage only, the profiles already '
+            'set the correct values for the most common use cases. See '
+            '   https://django-ca.readthedocs.io/en/latest/extensions.html for more information.'
+        )
         group.add_argument(
             '--key-usage', metavar='VALUES',
-            help='Override the keyUsage extension, e.g. "critical,keyCertSign".')
+            help='The keyUsage extension, e.g. "critical,keyCertSign".')
         group.add_argument(
             '--ext-key-usage', metavar='VALUES',
-            help='Override the extendedKeyUsage extension, e.g. "serverAuth,clientAuth".')
+            help='The extendedKeyUsage extension, e.g. "serverAuth,clientAuth".')
         group.add_argument(
             '--tls-features', metavar='VALUES', help='TLS Feature extensions.')
 
         group = parser.add_argument_group(
             'profiles', """Sign certificate based on the given profile. A profile only sets the
 the default values, options like --key-usage still override the profile.""")
         group = group.add_mutually_exclusive_group()
@@ -118,41 +122,41 @@
     def handle(self, *args, **options):
         ca = options['ca']
         if ca.expires < options['expires']:
             max_days = (ca.expires - timezone.now()).days
             raise CommandError(
                 'Certificate would outlive CA, maximum expiry for this CA is %s days.' % max_days)
 
+        # See if we can work with the private key
+        self.test_private_key(ca, options['password'])
+
         # get list of watchers
         watchers = [Watcher.from_addr(addr) for addr in options['watch']]
 
         # get keyUsage and extendedKeyUsage flags based on profiles
         kwargs = get_cert_profile_kwargs(options['profile'])
+        kwargs['subject'] = Subject(kwargs.get('subject'))
         kwargs['password'] = options['password']
         kwargs['csr_format'] = options['csr_format']
         if options['cn_in_san'] is not None:
             kwargs['cn_in_san'] = options['cn_in_san']
         if options['key_usage']:
             kwargs['keyUsage'] = self.parse_extension(options['key_usage'])
         if options['ext_key_usage']:
             kwargs['extendedKeyUsage'] = self.parse_extension(options['ext_key_usage'])
         if options['tls_features']:
             kwargs['tls_features'] = self.parse_extension(options['tls_features'])
 
         # update subject with arguments from the command line
-        kwargs.setdefault('subject', OrderedDict())
         if options.get('subject'):
-            kwargs['subject'].update(options['subject'])  # update from command line
-
-        # filter empty values
-        kwargs['subject'] = OrderedDict([(k, v) for k, v in kwargs['subject'].items() if v])
+            # TODO: Update value
+            kwargs['subject'] = options['subject']  # update from command line
 
-        if not kwargs['subject'].get('CN') and not options['alt']:
-            raise CommandError(
-                "Must give at least a CN in --subject or one or more --alt arguments.")
+        if 'CN' not in kwargs['subject'] and not options['alt']:
+            raise CommandError("Must give at least a CN in --subject or one or more --alt arguments.")
 
         # Read the CSR
         if options['csr'] is None:
             self.stdout.write('Please paste the CSR:')
             csr = ''
             while not csr.endswith('-----END CERTIFICATE REQUEST-----\n'):
                 csr += '%s\n' % six.moves.input()
```

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/import_ca.py` & `django-ca-1.9.0/ca/django_ca/management/commands/import_ca.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/dump_ca.py` & `django-ca-1.9.0/ca/django_ca/management/commands/dump_ca.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/list_certs.py` & `django-ca-1.9.0/ca/django_ca/management/commands/list_certs.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/init_ca.py` & `django-ca-1.9.0/ca/django_ca/management/commands/init_ca.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,17 +114,21 @@
         if parent and not parent.allows_intermediate_ca:
             raise CommandError("Parent CA cannot create intermediate CA due to pathlen restrictions.")
         if not parent and options['ca_crl_url']:
             raise CommandError("CRLs cannot be used to revoke root CAs.")
         if not parent and options['ca_ocsp_url']:
             raise CommandError("OCSP cannot be used to revoke root CAs.")
 
-        # filter empty values in the subject
-        subject.setdefault('CN', name)
-        subject = {k: v for k, v in subject.items() if v}
+        # See if we can work with the private key
+        if parent:
+            self.test_private_key(parent, options['parent_password'])
+
+        # Set CommonName to name if not set in subject
+        if 'CN' not in subject:
+            subject['CN'] = name
 
         try:
             CertificateAuthority.objects.init(
                 key_size=options['key_size'], key_type=options['key_type'],
                 algorithm=options['algorithm'],
                 expires=options['expires'],
                 parent=parent,
```

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/view_cert.py` & `django-ca-1.9.0/ca/django_ca/management/commands/view_cert.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/dump_cert.py` & `django-ca-1.9.0/ca/django_ca/management/commands/dump_cert.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/dump_crl.py` & `django-ca-1.9.0/ca/django_ca/management/commands/dump_crl.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,17 +42,21 @@
             'encoding': options['format'],
             'expires': options['expires'],
             'algorithm': options['algorithm'],
             'password': options['password'],
             'ca_crl': options['ca_crl'],
         }
 
+        # See if we can work with the private key
+        self.test_private_key(options['ca'], options['password'])
+
         try:
             crl = get_crl(ca=options['ca'], **kwargs)
-        except Exception as e:
+        except Exception as e:  # pragma: no cover
+            # Note: all parameters are already sanitized by parser actions
             raise CommandError(str(e))
 
         if path == '-':
             self.stdout.write(crl, ending=b'')
         else:
             try:
                 with open(path, 'wb') as stream:
```

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/notify_expiring_certs.py` & `django-ca-1.9.0/ca/django_ca/management/commands/notify_expiring_certs.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/ca/django_ca/management/commands/cert_watchers.py` & `django-ca-1.9.0/ca/django_ca/management/commands/cert_watchers.py`

 * *Files identical despite different names*

### Comparing `django-ca-1.7.0/setup.py` & `django-ca-1.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,53 +13,53 @@
 #
 # You should have received a copy of the GNU General Public License along with django-ca.  If not,
 # see <http://www.gnu.org/licenses/>.
 
 import os
 import subprocess
 import sys
-from distutils.cmd import Command
 
+from setuptools import Command
 from setuptools import setup
 
 long_description = """django-ca is a tool to manage TLS certificate authorities and easily issue and revoke
 certificates. It is based `cryptography <https://cryptography.io/>`_ and `Django
 <https://www.djangoproject.com/>`_. It can be used as an app in an existing Django project or stand-alone with
 the basic project included.  Everything can be managed via the command line via `manage.py` commands - so no
 webserver is needed, if you’re happy with the command-line.
 
 Features:
 
 * Set up a secure local certificate authority in just a few minutes.
-* Written in Python 2.7/Python3.4+, requires Django 1.8 or later.
+* Written in Python 2.7/Python3.4+, requires Django 1.11 or later.
 * Manage your entire certificate authority from the command line and/or via Djangos admin
   interface.
 * Get email notifications about certificates about to expire.
 * Certificate validation using Certificate Revocation Lists (CRLs) and via an included OCSP
   responder.
 
 Please see https://django-ca.readthedocs.org for more extensive documentation.
 """
 
 PY2 = sys.version_info[0] == 2
 PY3 = sys.version_info[0] == 3
 _rootdir = os.path.dirname(os.path.realpath(__file__))
 
 install_requires = [
-    'asn1crypto>=0.22.0',
+    'asn1crypto>=0.24.0',
     'cryptography>=2.1',
     'ocspbuilder>=0.10.2',
-    'oscrypto>=0.18.0',
+    'oscrypto>=0.19.0',
 ]
 
 if PY2:
     install_requires.append('ipaddress>=1.0.18')
-    install_requires.append('Django>=1.8,<2.0')
+    install_requires.append('Django>=1.11,<2.0')
 else:
-    install_requires.append('Django>=1.8')
+    install_requires.append('Django>=1.11')
 
 
 class BaseCommand(Command):
     user_options = [
         ('suite=', None, 'Testsuite to run', )
     ]
 
@@ -112,15 +112,15 @@
         # exclude version-specific code
         if PY2:
             cov.exclude('only py3')
         else:
             cov.exclude('only py2')
 
         from django import VERSION
-        django_versions = [(1, 8), (1, 9), (1, 10), (1, 11), (2, 0), (2, 1)]
+        django_versions = [(1, 11), (2, 0), (2, 1), (2, 2), (2, 3)]
         this_version = VERSION[:2]
 
         for version in django_versions:
             version_str = '.'.join([str(v) for v in version])
 
             if version != this_version:
                 cov.exclude(r'(pragma|PRAGMA)[:\s]?\s*only django==%s' % version_str)
@@ -184,15 +184,15 @@
     return data
 
 
 package_data = find_package_data('static') + find_package_data('templates')
 
 setup(
     name='django-ca',
-    version='1.7.0',
+    version='1.9.0',
     description='A Django app providing a SSL/TLS certificate authority.',
     long_description=long_description,
     author='Mathias Ertl',
     author_email='mati@er.tl',
     url='https://github.com/mathiasertl/django-ca',
     packages=[
         'django_ca',
@@ -208,17 +208,17 @@
     cmdclass={
         'coverage': CoverageCommand,
         'test': TestCommand,
         'code_quality': QualityCommand,
     },
     classifiers=[
         'Development Status :: 4 - Beta',
-        'Framework :: Django :: 1.8',
-        'Framework :: Django :: 1.10',
         'Framework :: Django :: 1.11',
+        'Framework :: Django :: 2.0',
+        'Framework :: Django :: 2.1',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
```

