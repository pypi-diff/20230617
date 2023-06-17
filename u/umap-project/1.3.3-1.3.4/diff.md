# Comparing `tmp/umap-project-1.3.3.tar.gz` & `tmp/umap_project-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umap-project-1.3.3.tar", last modified: Wed Jun  7 08:50:21 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `umap-project-1.3.3.tar` & `umap_project-1.3.4.tar`

### file list

```diff
@@ -1,535 +1,341 @@
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.605311 umap-project-1.3.3/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      482 2016-04-23 07:38:39.000000 umap-project-1.3.3/LICENSE
--rw-r--r--   0 ybon      (1000) ybon      (1000)      196 2018-07-14 08:06:10.000000 umap-project-1.3.3/MANIFEST.in
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2026 2023-06-07 08:50:21.605311 umap-project-1.3.3/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1022 2023-06-02 15:29:26.000000 umap-project-1.3.3/README.md
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1438 2023-06-07 08:50:21.605311 umap-project-1.3.3/setup.cfg
--rw-r--r--   0 ybon      (1000) ybon      (1000)       37 2023-05-23 16:48:43.000000 umap-project-1.3.3/setup.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.458642 umap-project-1.3.3/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      178 2023-05-23 16:48:43.000000 umap-project-1.3.3/umap/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      541 2023-06-02 15:27:32.000000 umap-project-1.3.3/umap/admin.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      109 2023-06-02 15:27:32.000000 umap-project-1.3.3/umap/apps.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      535 2023-02-22 09:51:22.000000 umap-project-1.3.3/umap/autocomplete.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.458642 umap-project-1.3.3/umap/bin/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      256 2016-09-17 20:05:31.000000 umap-project-1.3.3/umap/bin/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/context_processors.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2021 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/decorators.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      869 2023-06-02 15:27:32.000000 umap-project-1.3.3/umap/fields.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2731 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/forms.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.438641 umap-project-1.3.3/umap/locale/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/am_ET/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.458642 umap-project-1.3.3/umap/locale/am_ET/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6107 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/am_ET/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10304 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/am_ET/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/ar/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.458642 umap-project-1.3.3/umap/locale/ar/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3749 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9124 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/ast/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.458642 umap-project-1.3.3/umap/locale/ast/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      432 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/locale/ast/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8007 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/locale/ast/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/bg/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.461975 umap-project-1.3.3/umap/locale/bg/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6647 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10835 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/ca/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.461975 umap-project-1.3.3/umap/locale/ca/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6826 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10085 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/cs_CZ/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.461975 umap-project-1.3.3/umap/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6979 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10374 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/cs_CZ/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/da/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.461975 umap-project-1.3.3/umap/locale/da/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6636 2023-06-06 21:16:20.000000 umap-project-1.3.3/umap/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10037 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/da/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/de/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.461975 umap-project-1.3.3/umap/locale/de/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6960 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10432 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/el/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.465309 umap-project-1.3.3/umap/locale/el/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10713 2023-06-06 21:16:20.000000 umap-project-1.3.3/umap/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13678 2023-06-06 20:33:04.000000 umap-project-1.3.3/umap/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.428641 umap-project-1.3.3/umap/locale/en/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.465309 umap-project-1.3.3/umap/locale/en/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      337 2023-06-07 07:12:27.000000 umap-project-1.3.3/umap/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7453 2023-06-06 21:16:39.000000 umap-project-1.3.3/umap/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/es/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.465309 umap-project-1.3.3/umap/locale/es/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6880 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10502 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/et/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.465309 umap-project-1.3.3/umap/locale/et/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5780 2023-06-06 21:16:20.000000 umap-project-1.3.3/umap/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9375 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/et/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/fa_IR/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.465309 umap-project-1.3.3/umap/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8468 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11765 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/fa_IR/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/fi/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.468642 umap-project-1.3.3/umap/locale/fi/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5407 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9762 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/fr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.468642 umap-project-1.3.3/umap/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7811 2023-06-07 07:12:27.000000 umap-project-1.3.3/umap/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10992 2023-06-07 07:11:14.000000 umap-project-1.3.3/umap/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/gl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.468642 umap-project-1.3.3/umap/locale/gl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6842 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10170 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/gl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/he/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.468642 umap-project-1.3.3/umap/locale/he/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7594 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10828 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/he/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/hr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.468642 umap-project-1.3.3/umap/locale/hr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1777 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8477 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/locale/hr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/hu/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.471975 umap-project-1.3.3/umap/locale/hu/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7235 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10494 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/hu/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.431975 umap-project-1.3.3/umap/locale/id/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.471975 umap-project-1.3.3/umap/locale/id/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      425 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8000 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/locale/id/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/is/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.471975 umap-project-1.3.3/umap/locale/is/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7179 2023-06-06 21:16:20.000000 umap-project-1.3.3/umap/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10409 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/it/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.475309 umap-project-1.3.3/umap/locale/it/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6941 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10630 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/ja/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.475309 umap-project-1.3.3/umap/locale/ja/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7273 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10564 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/ko/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.475309 umap-project-1.3.3/umap/locale/ko/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7228 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10458 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/lt/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.475309 umap-project-1.3.3/umap/locale/lt/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6453 2023-06-06 21:16:20.000000 umap-project-1.3.3/umap/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10006 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/ms/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.475309 umap-project-1.3.3/umap/locale/ms/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7690 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ms/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10565 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ms/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/nl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.478642 umap-project-1.3.3/umap/locale/nl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6640 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9964 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/no/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.478642 umap-project-1.3.3/umap/locale/no/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      423 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/locale/no/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7998 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/locale/no/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/pl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.478642 umap-project-1.3.3/umap/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6960 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10403 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/pt/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.478642 umap-project-1.3.3/umap/locale/pt/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6922 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10217 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/pt/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/pt_BR/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.478642 umap-project-1.3.3/umap/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6909 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10258 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/pt_PT/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.481976 umap-project-1.3.3/umap/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6937 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10232 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/ro/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.488643 umap-project-1.3.3/umap/locale/ro/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1383 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7904 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ro/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/ru/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.488643 umap-project-1.3.3/umap/locale/ru/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8782 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12229 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/si_LK/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.491976 umap-project-1.3.3/umap/locale/si_LK/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      447 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/locale/si_LK/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8022 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/locale/si_LK/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/sk_SK/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.491976 umap-project-1.3.3/umap/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6509 2023-06-06 21:16:20.000000 umap-project-1.3.3/umap/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10087 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/sk_SK/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/sl/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.491976 umap-project-1.3.3/umap/locale/sl/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6500 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9979 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/sl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.435308 umap-project-1.3.3/umap/locale/sr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.495309 umap-project-1.3.3/umap/locale/sr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8384 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11629 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/sr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.438641 umap-project-1.3.3/umap/locale/sv/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.495309 umap-project-1.3.3/umap/locale/sv/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6620 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9944 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.438641 umap-project-1.3.3/umap/locale/th_TH/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.495309 umap-project-1.3.3/umap/locale/th_TH/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9739 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/th_TH/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12950 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/th_TH/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.438641 umap-project-1.3.3/umap/locale/tr/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.495309 umap-project-1.3.3/umap/locale/tr/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6971 2023-06-06 21:16:20.000000 umap-project-1.3.3/umap/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    10296 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.438641 umap-project-1.3.3/umap/locale/uk_UA/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.498643 umap-project-1.3.3/umap/locale/uk_UA/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9009 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/uk_UA/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12296 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/uk_UA/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.438641 umap-project-1.3.3/umap/locale/vi/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.498643 umap-project-1.3.3/umap/locale/vi/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5616 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9835 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.438641 umap-project-1.3.3/umap/locale/zh/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.498643 umap-project-1.3.3/umap/locale/zh/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4059 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8751 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/zh/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.438641 umap-project-1.3.3/umap/locale/zh_TW/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.498643 umap-project-1.3.3/umap/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6440 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9968 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.498643 umap-project-1.3.3/umap/management/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.3/umap/management/__init__.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.501976 umap-project-1.3.3/umap/management/commands/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-09-17 20:05:31.000000 umap-project-1.3.3/umap/management/commands/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      786 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/management/commands/anonymous_edit_url.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1298 2019-04-07 14:33:20.000000 umap-project-1.3.3/umap/management/commands/generate_js_locale.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1902 2019-04-07 14:28:38.000000 umap-project-1.3.3/umap/management/commands/import_pictograms.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      207 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/managers.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/middleware.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.505309 umap-project-1.3.3/umap/migrations/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5563 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/migrations/0001_initial.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      373 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/migrations/0002_tilelayer_tms.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      812 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/migrations/0003_add_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      530 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/migrations/0004_add_licence.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2018-07-14 11:58:47.000000 umap-project-1.3.3/umap/migrations/0005_remove_map_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      497 2019-04-07 08:09:35.000000 umap-project-1.3.3/umap/migrations/0006_auto_20190407_0719.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      515 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/migrations/0007_auto_20190416_1757.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      459 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/migrations/0008_alter_map_settings.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/migrations/0009_star.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-11-26 16:02:45.000000 umap-project-1.3.3/umap/migrations/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11496 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/models.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.505309 umap-project-1.3.3/umap/settings/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1641 2023-06-05 15:00:46.000000 umap-project-1.3.3/umap/settings/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9356 2023-06-05 15:00:46.000000 umap-project-1.3.3/umap/settings/base.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      386 2018-05-19 15:10:46.000000 umap-project-1.3.3/umap/settings/dev.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.505309 umap-project-1.3.3/umap/static/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/static/.gitignore
--rw-r--r--   0 ybon      (1000) ybon      (1000)      638 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/static/favicon.ico
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.508643 umap-project-1.3.3/umap/static/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18168 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/static/umap/base.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9125 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/static/umap/bitbucket.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5858 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/content.css
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.511976 umap-project-1.3.3/umap/static/umap/font/
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   182984 2018-05-17 09:59:39.000000 umap-project-1.3.3/umap/static/umap/font/FiraSans-Light.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   129180 2018-05-17 09:59:39.000000 umap-project-1.3.3/umap/static/umap/font/FiraSans-Light.woff2
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   191400 2018-05-17 09:59:39.000000 umap-project-1.3.3/umap/static/umap/font/FiraSans-LightItalic.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   135744 2018-05-17 09:59:39.000000 umap-project-1.3.3/umap/static/umap/font/FiraSans-LightItalic.woff2
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   198128 2018-05-17 09:59:39.000000 umap-project-1.3.3/umap/static/umap/font/FiraSans-SemiBold.woff
--rwxr-xr-x   0 ybon      (1000) ybon      (1000)   140168 2018-05-17 09:59:39.000000 umap-project-1.3.3/umap/static/umap/font/FiraSans-SemiBold.woff2
--rw-r--r--   0 ybon      (1000) ybon      (1000)      832 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/static/umap/font.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1564 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/static/umap/github.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.515310 umap-project-1.3.3/umap/static/umap/img/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12648 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/static/umap/img/16-white.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    58857 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/static/umap/img/16-white.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11308 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/static/umap/img/16.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38140 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/static/umap/img/16.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19711 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/img/24-white.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38377 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/img/24-white.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16878 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/img/24.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)    36478 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/img/24.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)      430 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/static/umap/img/edit-16.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      554 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/static/umap/img/edit.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)      190 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/static/umap/img/icon-bg.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      327 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/static/umap/img/logo.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5537 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/static/umap/img/logo_filigree.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      375 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/static/umap/img/marker.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      473 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/static/umap/img/opensource.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1997 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/static/umap/img/osm.svg
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1472 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/static/umap/img/search.gif
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.518643 umap-project-1.3.3/umap/static/umap/js/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7937 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.autocomplete.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    38965 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.controls.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19966 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.core.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31642 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.features.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27320 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.forms.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5762 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.icon.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    71362 2023-06-07 08:11:23.000000 umap-project-1.3.3/umap/static/umap/js/umap.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33580 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.layer.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5809 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.permissions.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6802 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.popup.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4421 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.slideshow.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4191 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.tableeditor.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7099 2023-06-07 08:11:23.000000 umap-project-1.3.3/umap/static/umap/js/umap.ui.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8711 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/js/umap.xhr.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.555311 umap-project-1.3.3/umap/static/umap/locale/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27680 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/am_ET.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27609 2023-06-07 07:11:13.000000 umap-project-1.3.3/umap/static/umap/locale/am_ET.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23520 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/ar.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23455 2023-06-07 07:11:13.000000 umap-project-1.3.3/umap/static/umap/locale/ar.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23053 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/ast.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22986 2023-06-07 07:11:13.000000 umap-project-1.3.3/umap/static/umap/locale/ast.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26806 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/bg.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26741 2023-06-07 07:11:13.000000 umap-project-1.3.3/umap/static/umap/locale/bg.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23902 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/ca.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23837 2023-06-07 07:11:15.000000 umap-project-1.3.3/umap/static/umap/locale/ca.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24872 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/cs_CZ.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24801 2023-06-07 07:11:15.000000 umap-project-1.3.3/umap/static/umap/locale/cs_CZ.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23490 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/da.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23425 2023-06-07 07:11:15.000000 umap-project-1.3.3/umap/static/umap/locale/da.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24978 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/de.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24913 2023-06-07 07:11:15.000000 umap-project-1.3.3/umap/static/umap/locale/de.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33900 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/el.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33835 2023-06-07 07:11:15.000000 umap-project-1.3.3/umap/static/umap/locale/el.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23053 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/en.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22988 2023-06-06 21:16:39.000000 umap-project-1.3.3/umap/static/umap/locale/en.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22698 2023-06-07 07:11:16.000000 umap-project-1.3.3/umap/static/umap/locale/en_US.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25208 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/es.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25143 2023-06-07 07:11:16.000000 umap-project-1.3.3/umap/static/umap/locale/es.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23306 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/et.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23241 2023-06-07 07:11:16.000000 umap-project-1.3.3/umap/static/umap/locale/et.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30419 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/fa_IR.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30348 2023-06-07 07:11:16.000000 umap-project-1.3.3/umap/static/umap/locale/fa_IR.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24094 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/fi.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24029 2023-06-07 07:11:16.000000 umap-project-1.3.3/umap/static/umap/locale/fi.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25266 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/fr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25201 2023-06-07 07:11:17.000000 umap-project-1.3.3/umap/static/umap/locale/fr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24704 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/gl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24639 2023-06-07 07:11:17.000000 umap-project-1.3.3/umap/static/umap/locale/gl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27116 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/he.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27051 2023-06-07 07:11:17.000000 umap-project-1.3.3/umap/static/umap/locale/he.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23261 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/hr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23196 2023-06-07 07:11:17.000000 umap-project-1.3.3/umap/static/umap/locale/hr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26055 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/hu.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    25990 2023-06-07 07:11:18.000000 umap-project-1.3.3/umap/static/umap/locale/hu.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23051 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/id.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22986 2023-06-07 07:11:19.000000 umap-project-1.3.3/umap/static/umap/locale/id.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24625 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/is.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24560 2023-06-07 07:11:19.000000 umap-project-1.3.3/umap/static/umap/locale/is.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24731 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/it.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24666 2023-06-07 07:11:19.000000 umap-project-1.3.3/umap/static/umap/locale/it.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26151 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/ja.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    26086 2023-06-07 07:11:19.000000 umap-project-1.3.3/umap/static/umap/locale/ja.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23279 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/ko.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23214 2023-06-07 07:11:19.000000 umap-project-1.3.3/umap/static/umap/locale/ko.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24002 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/lt.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23937 2023-06-07 07:11:20.000000 umap-project-1.3.3/umap/static/umap/locale/lt.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24216 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/ms.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24151 2023-06-07 07:11:20.000000 umap-project-1.3.3/umap/static/umap/locale/ms.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24656 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/nl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24591 2023-06-07 07:11:20.000000 umap-project-1.3.3/umap/static/umap/locale/nl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23330 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/no.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23265 2023-06-07 07:11:20.000000 umap-project-1.3.3/umap/static/umap/locale/no.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24524 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/pl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24459 2023-06-07 07:11:21.000000 umap-project-1.3.3/umap/static/umap/locale/pl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22986 2023-06-07 07:11:21.000000 umap-project-1.3.3/umap/static/umap/locale/pl_PL.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24696 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/pt.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24631 2023-06-07 07:11:21.000000 umap-project-1.3.3/umap/static/umap/locale/pt.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24685 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/pt_BR.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24614 2023-06-07 07:11:22.000000 umap-project-1.3.3/umap/static/umap/locale/pt_BR.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24695 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/pt_PT.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24624 2023-06-07 07:11:22.000000 umap-project-1.3.3/umap/static/umap/locale/pt_PT.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23112 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/ro.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23047 2023-06-07 07:11:22.000000 umap-project-1.3.3/umap/static/umap/locale/ro.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31691 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/ru.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31626 2023-06-07 07:11:23.000000 umap-project-1.3.3/umap/static/umap/locale/ru.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23057 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/si_LK.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22986 2023-06-07 07:11:23.000000 umap-project-1.3.3/umap/static/umap/locale/si_LK.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24555 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/sk_SK.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24484 2023-06-07 07:11:23.000000 umap-project-1.3.3/umap/static/umap/locale/sk_SK.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24398 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/sl.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24333 2023-06-07 07:11:23.000000 umap-project-1.3.3/umap/static/umap/locale/sl.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27813 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/sr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27748 2023-06-07 07:11:23.000000 umap-project-1.3.3/umap/static/umap/locale/sr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24277 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/sv.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24212 2023-06-07 07:11:24.000000 umap-project-1.3.3/umap/static/umap/locale/sv.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23057 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/th_TH.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22986 2023-06-07 07:11:24.000000 umap-project-1.3.3/umap/static/umap/locale/th_TH.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24905 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/tr.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    24840 2023-06-07 07:11:24.000000 umap-project-1.3.3/umap/static/umap/locale/tr.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31284 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/uk_UA.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    31213 2023-06-07 07:11:24.000000 umap-project-1.3.3/umap/static/umap/locale/uk_UA.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23430 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/vi.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23365 2023-06-07 07:11:25.000000 umap-project-1.3.3/umap/static/umap/locale/vi.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22986 2023-06-07 07:11:25.000000 umap-project-1.3.3/umap/static/umap/locale/vi_VN.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22677 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/zh.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22612 2023-06-07 07:11:25.000000 umap-project-1.3.3/umap/static/umap/locale/zh.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22986 2023-06-07 07:11:26.000000 umap-project-1.3.3/umap/static/umap/locale/zh_CN.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22986 2023-06-07 07:11:26.000000 umap-project-1.3.3/umap/static/umap/locale/zh_TW.Big5.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22659 2023-06-07 08:50:20.000000 umap-project-1.3.3/umap/static/umap/locale/zh_TW.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    22588 2023-06-07 07:11:26.000000 umap-project-1.3.3/umap/static/umap/locale/zh_TW.json
--rw-r--r--   0 ybon      (1000) ybon      (1000)    32282 2023-06-06 20:32:57.000000 umap-project-1.3.3/umap/static/umap/map.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1531 2023-06-06 20:32:57.000000 umap-project-1.3.3/umap/static/umap/nav.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    19408 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/static/umap/openstreetmap.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.558644 umap-project-1.3.3/umap/static/umap/test/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      464 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/static/umap/test/.eslintrc
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1665 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/Controls.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11544 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/DataLayer.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9423 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/Feature.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16802 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/Map.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3318 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/Marker.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2314 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/Permissions.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12614 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/Polygon.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    13986 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/Polyline.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3216 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/TableEditor.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14080 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/Util.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9840 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/_pre.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5318 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/static/umap/test/index.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)       49 2018-06-02 13:09:22.000000 umap-project-1.3.3/umap/static/umap/theme.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3225 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/static/umap/twitter.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.441975 umap-project-1.3.3/umap/static/umap/vendors/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.558644 umap-project-1.3.3/umap/static/umap/vendors/contextmenu/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1231 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    16343 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      990 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8994 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/contextmenu/leaflet.contextmenu.min.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.558644 umap-project-1.3.3/umap/static/umap/vendors/csv2geojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    15029 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/csv2geojson/csv2geojson.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6994 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/csv2geojson/index.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.558644 umap-project-1.3.3/umap/static/umap/vendors/dompurify/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    62738 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/dompurify/purify.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.561977 umap-project-1.3.3/umap/static/umap/vendors/editable/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    74768 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/editable/Leaflet.Editable.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3898 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/editable/Path.Drag.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.561977 umap-project-1.3.3/umap/static/umap/vendors/editinosm/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1263 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9141 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/editinosm/Leaflet.EditInOSM.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3340 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/editinosm/edit-in-osm.png
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.561977 umap-project-1.3.3/umap/static/umap/vendors/formbuilder/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12235 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/formbuilder/Leaflet.FormBuilder.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.561977 umap-project-1.3.3/umap/static/umap/vendors/fullscreen/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5041 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3654 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/fullscreen/Leaflet.fullscreen.min.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/fullscreen/fullscreen.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      420 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/fullscreen/fullscreen@2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      994 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/fullscreen/leaflet.fullscreen.css
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.561977 umap-project-1.3.3/umap/static/umap/vendors/georsstogeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3202 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/georsstogeojson/GeoRSSToGeoJSON.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.561977 umap-project-1.3.3/umap/static/umap/vendors/hash/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3462 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/hash/leaflet-hash.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.565311 umap-project-1.3.3/umap/static/umap/vendors/heat/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5158 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/heat/leaflet-heat.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.565311 umap-project-1.3.3/umap/static/umap/vendors/i18n/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1305 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/i18n/Leaflet.i18n.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.581978 umap-project-1.3.3/umap/static/umap/vendors/leaflet/
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.585311 umap-project-1.3.3/umap/static/umap/vendors/leaflet/images/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1259 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/images/layers-2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      696 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/images/layers.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2464 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/images/marker-icon-2x.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/images/marker-icon.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)      618 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/images/marker-shadow.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)   398517 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/leaflet-src.esm.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   759894 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/leaflet-src.esm.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)   400242 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/leaflet-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   759986 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/leaflet-src.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14106 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/leaflet.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)   140468 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/leaflet.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   191112 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/leaflet/leaflet.js.map
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.585311 umap-project-1.3.3/umap/static/umap/vendors/loading/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3252 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/loading/Control.Loading.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14143 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/loading/Control.Loading.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.585311 umap-project-1.3.3/umap/static/umap/vendors/locatecontrol/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2471 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/locatecontrol/L.Control.Locate.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    30907 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/locatecontrol/L.Control.Locate.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.588645 umap-project-1.3.3/umap/static/umap/vendors/markercluster/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1346 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/markercluster/MarkerCluster.Default.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)      886 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/markercluster/MarkerCluster.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)      318 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/markercluster/WhereAreTheJavascriptFiles.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)    80271 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)   157229 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/markercluster/leaflet.markercluster-src.js.map
--rw-r--r--   0 ybon      (1000) ybon      (1000)    33679 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/markercluster/leaflet.markercluster.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    27566 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/markercluster/leaflet.markercluster.js.map
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.588645 umap-project-1.3.3/umap/static/umap/vendors/measurable/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      937 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/measurable/Leaflet.Measurable.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7256 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/measurable/Leaflet.Measurable.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.591978 umap-project-1.3.3/umap/static/umap/vendors/minimap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1998 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/minimap/Control.MiniMap.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)    12129 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/minimap/Control.MiniMap.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.591978 umap-project-1.3.3/umap/static/umap/vendors/minimap/images/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      219 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/minimap/images/toggle.png
--rw-r--r--   0 ybon      (1000) ybon      (1000)     8057 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/minimap/images/toggle.svg
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.591978 umap-project-1.3.3/umap/static/umap/vendors/osmtogeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    35642 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/osmtogeojson/osmtogeojson.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.591978 umap-project-1.3.3/umap/static/umap/vendors/photon/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14433 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/photon/leaflet.photon.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.591978 umap-project-1.3.3/umap/static/umap/vendors/print/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    44559 2021-09-12 08:45:21.000000 umap-project-1.3.3/umap/static/umap/vendors/print/leaflet.browser.print.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)    23442 2021-09-12 08:45:21.000000 umap-project-1.3.3/umap/static/umap/vendors/print/leaflet.browser.print.min.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.591978 umap-project-1.3.3/umap/static/umap/vendors/togeojson/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    18098 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/togeojson/togeojson.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.591978 umap-project-1.3.3/umap/static/umap/vendors/togpx/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    17936 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/togpx/togpx.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.591978 umap-project-1.3.3/umap/static/umap/vendors/tokml/
--rw-r--r--   0 ybon      (1000) ybon      (1000)    11521 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/tokml/tokml.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.595311 umap-project-1.3.3/umap/static/umap/vendors/toolbar/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2890 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     9060 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/toolbar/leaflet.toolbar-src.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2244 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/toolbar/leaflet.toolbar.css
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5326 2023-06-05 10:39:54.000000 umap-project-1.3.3/umap/static/umap/vendors/toolbar/leaflet.toolbar.js
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.595311 umap-project-1.3.3/umap/templates/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      305 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/templates/404.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4904 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/templates/500.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.595311 umap-project-1.3.3/umap/templates/auth/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      467 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/templates/auth/user_detail.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      487 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/templates/auth/user_stars.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      702 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/templates/base.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.595311 umap-project-1.3.3/umap/templates/registration/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1157 2023-03-01 18:10:17.000000 umap-project-1.3.3/umap/templates/registration/login.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.598645 umap-project-1.3.3/umap/templates/umap/
--rw-r--r--   0 ybon      (1000) ybon      (1000)      128 2018-05-18 20:43:08.000000 umap-project-1.3.3/umap/templates/umap/about.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1897 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/templates/umap/about_summary.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2857 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/templates/umap/content.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      752 2023-06-06 20:32:57.000000 umap-project-1.3.3/umap/templates/umap/content_footer.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1309 2023-05-30 13:55:57.000000 umap-project-1.3.3/umap/templates/umap/css.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-05-18 20:43:08.000000 umap-project-1.3.3/umap/templates/umap/footer.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      631 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/templates/umap/home.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3155 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/templates/umap/js.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      112 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/templates/umap/locale.js
--rw-r--r--   0 ybon      (1000) ybon      (1000)      629 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/templates/umap/login_popup_end.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      595 2021-09-12 08:45:40.000000 umap-project-1.3.3/umap/templates/umap/map_detail.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      200 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/templates/umap/map_fragment.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      165 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/templates/umap/map_init.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      597 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/templates/umap/map_list.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      299 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/templates/umap/map_messages.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1125 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/templates/umap/navigation.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      878 2018-05-18 20:43:08.000000 umap-project-1.3.3/umap/templates/umap/password_change.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      258 2018-05-18 20:43:08.000000 umap-project-1.3.3/umap/templates/umap/password_change_done.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      390 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/templates/umap/search.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)      448 2018-05-18 20:43:08.000000 umap-project-1.3.3/umap/templates/umap/search_bar.html
--rw-r--r--   0 ybon      (1000) ybon      (1000)        2 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/templates/umap/success.html
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.598645 umap-project-1.3.3/umap/templatetags/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2016-04-23 07:38:39.000000 umap-project-1.3.3/umap/templatetags/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2405 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/templatetags/umap_tags.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.601978 umap-project-1.3.3/umap/tests/
--rw-r--r--   0 ybon      (1000) ybon      (1000)        0 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/tests/__init__.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2945 2023-05-05 17:42:43.000000 umap-project-1.3.3/umap/tests/base.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1466 2023-06-02 15:29:26.000000 umap-project-1.3.3/umap/tests/conftest.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      453 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/tests/settings.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2870 2023-02-27 10:29:01.000000 umap-project-1.3.3/umap/tests/test_datalayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     7173 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/tests/test_datalayer_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      339 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/tests/test_licence.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     3149 2018-07-14 13:10:40.000000 umap-project-1.3.3/umap/tests/test_map.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    21739 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/tests/test_map_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      605 2018-07-14 08:06:10.000000 umap-project-1.3.3/umap/tests/test_tilelayer.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)      407 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/tests/test_utils.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     6177 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/tests/test_views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     5538 2023-06-05 15:00:43.000000 umap-project-1.3.3/umap/urls.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     4381 2023-06-02 15:27:33.000000 umap-project-1.3.3/umap/utils.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)    29363 2023-06-06 20:32:57.000000 umap-project-1.3.3/umap/views.py
--rw-r--r--   0 ybon      (1000) ybon      (1000)     1152 2018-05-19 15:10:36.000000 umap-project-1.3.3/umap/wsgi.py
-drwxr-xr-x   0 ybon      (1000) ybon      (1000)        0 2023-06-07 08:50:21.605311 umap-project-1.3.3/umap_project.egg-info/
--rw-r--r--   0 ybon      (1000) ybon      (1000)     2026 2023-06-07 08:50:21.000000 umap-project-1.3.3/umap_project.egg-info/PKG-INFO
--rw-r--r--   0 ybon      (1000) ybon      (1000)    14363 2023-06-07 08:50:21.000000 umap-project-1.3.3/umap_project.egg-info/SOURCES.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        1 2023-06-07 08:50:21.000000 umap-project-1.3.3/umap_project.egg-info/dependency_links.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)       39 2023-06-07 08:50:21.000000 umap-project-1.3.3/umap_project.egg-info/entry_points.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)      310 2023-06-07 08:50:21.000000 umap-project-1.3.3/umap_project.egg-info/requires.txt
--rw-r--r--   0 ybon      (1000) ybon      (1000)        5 2023-06-07 08:50:21.000000 umap-project-1.3.3/umap_project.egg-info/top_level.txt
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/.DS_Store
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/__init__.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/admin.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/apps.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/autocomplete.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/context_processors.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/decorators.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/fields.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/forms.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/managers.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/middleware.py
+-rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/models.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/urls.py
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/utils.py
+-rw-r--r--   0        0        0    29191 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/views.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/wsgi.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/bin/__init__.py
+-rw-r--r--   0        0        0     6107 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/am_ET/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10304 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/am_ET/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ast/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ast/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/bg/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10085 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10374 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/cs_CZ/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6960 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10713 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13678 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/et/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8468 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/fa_IR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9762 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10992 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10170 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/gl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10828 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/hr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/hu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7179 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/is/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10564 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7228 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10458 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ms/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10565 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ms/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/no/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7998 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/no/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6960 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10217 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6909 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10232 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7904 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8782 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12229 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/si_LK/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/si_LK/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10087 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/sk_SK/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6500 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9979 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/sl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11629 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/sr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9944 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/th_TH/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/th_TH/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/uk_UA/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/uk_UA/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9835 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/vi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/zh/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/management/commands/__init__.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/management/commands/anonymous_edit_url.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/management/commands/generate_js_locale.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/management/commands/import_pictograms.py
+-rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/0001_initial.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/0002_tilelayer_tms.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/0003_add_tilelayer.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/0004_add_licence.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/0005_remove_map_tilelayer.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/0006_auto_20190407_0719.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/0007_auto_20190416_1757.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/0008_alter_map_settings.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/0009_star.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/migrations/__init__.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/settings/__init__.py
+-rw-r--r--   0        0        0     9418 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/settings/base.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/settings/dev.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/settings/local.py.sample
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/.gitignore
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/favicon.ico
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/.DS_Store
+-rw-r--r--   0        0        0    18144 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/base.css
+-rw-r--r--   0        0        0     9125 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/bitbucket.png
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/content.css
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/font.css
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/github.png
+-rw-r--r--   0        0        0    32282 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/map.css
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/nav.css
+-rw-r--r--   0        0        0    19408 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/openstreetmap.png
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/theme.css
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/twitter.png
+-rwxr-xr-x   0        0        0   182984 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/font/FiraSans-Light.woff
+-rwxr-xr-x   0        0        0   129180 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/font/FiraSans-Light.woff2
+-rwxr-xr-x   0        0        0   191400 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/font/FiraSans-LightItalic.woff
+-rwxr-xr-x   0        0        0   135744 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/font/FiraSans-LightItalic.woff2
+-rwxr-xr-x   0        0        0   198128 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/font/FiraSans-SemiBold.woff
+-rwxr-xr-x   0        0        0   140168 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/font/FiraSans-SemiBold.woff2
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/fonts/.DS_Store
+-rw-r--r--   0        0        0    12648 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/16-white.png
+-rw-r--r--   0        0        0    58857 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/16-white.svg
+-rw-r--r--   0        0        0    11308 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/16.png
+-rw-r--r--   0        0        0    38140 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/16.svg
+-rw-r--r--   0        0        0    19711 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/24-white.png
+-rw-r--r--   0        0        0    38377 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/24-white.svg
+-rw-r--r--   0        0        0    16878 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/24.png
+-rw-r--r--   0        0        0    36478 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/24.svg
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/edit-16.png
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/edit.svg
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/icon-bg.png
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/logo.svg
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/logo_filigree.png
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/marker.png
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/opensource.svg
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/osm.svg
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/img/search.gif
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.autocomplete.js
+-rw-r--r--   0        0        0    38965 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.controls.js
+-rw-r--r--   0        0        0    20305 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.core.js
+-rw-r--r--   0        0        0    31688 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.features.js
+-rw-r--r--   0        0        0    27476 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.forms.js
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.icon.js
+-rw-r--r--   0        0        0    71436 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.js
+-rw-r--r--   0        0        0    33609 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.layer.js
+-rw-r--r--   0        0        0     5809 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.permissions.js
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.popup.js
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.slideshow.js
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.tableeditor.js
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.ui.js
+-rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/js/umap.xhr.js
+-rw-r--r--   0        0        0    27680 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/am_ET.js
+-rw-r--r--   0        0        0    27609 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/am_ET.json
+-rw-r--r--   0        0        0    23520 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ar.js
+-rw-r--r--   0        0        0    23455 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ar.json
+-rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ast.js
+-rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ast.json
+-rw-r--r--   0        0        0    26806 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/bg.js
+-rw-r--r--   0        0        0    26741 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/bg.json
+-rw-r--r--   0        0        0    23902 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ca.js
+-rw-r--r--   0        0        0    23837 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ca.json
+-rw-r--r--   0        0        0    24872 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/cs_CZ.js
+-rw-r--r--   0        0        0    24801 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/cs_CZ.json
+-rw-r--r--   0        0        0    23490 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/da.js
+-rw-r--r--   0        0        0    23425 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/da.json
+-rw-r--r--   0        0        0    24978 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/de.js
+-rw-r--r--   0        0        0    24913 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/de.json
+-rw-r--r--   0        0        0    33900 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/el.js
+-rw-r--r--   0        0        0    33835 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/el.json
+-rw-r--r--   0        0        0    23053 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/en.js
+-rw-r--r--   0        0        0    22988 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/en.json
+-rw-r--r--   0        0        0    22698 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/en_US.json
+-rw-r--r--   0        0        0    25208 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/es.js
+-rw-r--r--   0        0        0    25143 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/es.json
+-rw-r--r--   0        0        0    23306 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/et.js
+-rw-r--r--   0        0        0    23241 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/et.json
+-rw-r--r--   0        0        0    30419 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/fa_IR.js
+-rw-r--r--   0        0        0    30348 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/fa_IR.json
+-rw-r--r--   0        0        0    24094 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/fi.js
+-rw-r--r--   0        0        0    24029 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/fi.json
+-rw-r--r--   0        0        0    25266 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/fr.js
+-rw-r--r--   0        0        0    25201 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/fr.json
+-rw-r--r--   0        0        0    24704 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/gl.js
+-rw-r--r--   0        0        0    24639 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/gl.json
+-rw-r--r--   0        0        0    27116 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/he.js
+-rw-r--r--   0        0        0    27051 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/he.json
+-rw-r--r--   0        0        0    23261 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/hr.js
+-rw-r--r--   0        0        0    23196 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/hr.json
+-rw-r--r--   0        0        0    26055 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/hu.js
+-rw-r--r--   0        0        0    25990 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/hu.json
+-rw-r--r--   0        0        0    23051 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/id.js
+-rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/id.json
+-rw-r--r--   0        0        0    24625 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/is.js
+-rw-r--r--   0        0        0    24560 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/is.json
+-rw-r--r--   0        0        0    24731 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/it.js
+-rw-r--r--   0        0        0    24666 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/it.json
+-rw-r--r--   0        0        0    26151 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ja.js
+-rw-r--r--   0        0        0    26086 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ja.json
+-rw-r--r--   0        0        0    23279 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ko.js
+-rw-r--r--   0        0        0    23214 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ko.json
+-rw-r--r--   0        0        0    24002 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/lt.js
+-rw-r--r--   0        0        0    23937 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/lt.json
+-rw-r--r--   0        0        0    24216 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ms.js
+-rw-r--r--   0        0        0    24151 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ms.json
+-rw-r--r--   0        0        0    24656 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/nl.js
+-rw-r--r--   0        0        0    24591 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/nl.json
+-rw-r--r--   0        0        0    23330 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/no.js
+-rw-r--r--   0        0        0    23265 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/no.json
+-rw-r--r--   0        0        0    24524 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/pl.js
+-rw-r--r--   0        0        0    24459 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/pl.json
+-rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/pl_PL.json
+-rw-r--r--   0        0        0    24696 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/pt.js
+-rw-r--r--   0        0        0    24631 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/pt.json
+-rw-r--r--   0        0        0    24685 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/pt_BR.js
+-rw-r--r--   0        0        0    24614 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/pt_BR.json
+-rw-r--r--   0        0        0    24695 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/pt_PT.js
+-rw-r--r--   0        0        0    24624 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/pt_PT.json
+-rw-r--r--   0        0        0    23112 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ro.js
+-rw-r--r--   0        0        0    23047 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ro.json
+-rw-r--r--   0        0        0    31691 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ru.js
+-rw-r--r--   0        0        0    31626 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/ru.json
+-rw-r--r--   0        0        0    23057 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/si_LK.js
+-rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/si_LK.json
+-rw-r--r--   0        0        0    24555 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/sk_SK.js
+-rw-r--r--   0        0        0    24484 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/sk_SK.json
+-rw-r--r--   0        0        0    24398 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/sl.js
+-rw-r--r--   0        0        0    24333 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/sl.json
+-rw-r--r--   0        0        0    27813 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/sr.js
+-rw-r--r--   0        0        0    27748 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/sr.json
+-rw-r--r--   0        0        0    24277 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/sv.js
+-rw-r--r--   0        0        0    24212 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/sv.json
+-rw-r--r--   0        0        0    23057 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/th_TH.js
+-rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/th_TH.json
+-rw-r--r--   0        0        0    24905 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/tr.js
+-rw-r--r--   0        0        0    24840 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/tr.json
+-rw-r--r--   0        0        0    31284 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/uk_UA.js
+-rw-r--r--   0        0        0    31213 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/uk_UA.json
+-rw-r--r--   0        0        0    23430 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/vi.js
+-rw-r--r--   0        0        0    23365 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/vi.json
+-rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/vi_VN.json
+-rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/zh.js
+-rw-r--r--   0        0        0    22612 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/zh.json
+-rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/zh_CN.json
+-rw-r--r--   0        0        0    22986 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/zh_TW.Big5.json
+-rw-r--r--   0        0        0    22659 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/zh_TW.js
+-rw-r--r--   0        0        0    22588 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/locale/zh_TW.json
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/.eslintrc
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/Controls.js
+-rw-r--r--   0        0        0    11544 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/DataLayer.js
+-rw-r--r--   0        0        0     9423 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/Feature.js
+-rw-r--r--   0        0        0    16802 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/Map.js
+-rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/Marker.js
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/Permissions.js
+-rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/Polygon.js
+-rw-r--r--   0        0        0    13986 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/Polyline.js
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/TableEditor.js
+-rw-r--r--   0        0        0    14255 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/Util.js
+-rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/_pre.js
+-rw-r--r--   0        0        0     5318 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/static/umap/test/index.html
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/404.html
+-rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/500.html
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/base.html
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/auth/user_detail.html
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/auth/user_stars.html
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/registration/login.html
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/about.html
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/about_summary.html
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/content.html
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/content_footer.html
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/css.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/footer.html
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/home.html
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/js.html
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/locale.js
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/login_popup_end.html
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/map_detail.html
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/map_fragment.html
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/map_init.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/map_list.html
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/map_messages.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/messages.html
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/navigation.html
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/password_change.html
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/password_change_done.html
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/search.html
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/search_bar.html
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templates/umap/success.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templatetags/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/templatetags/umap_tags.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/__init__.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/base.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/conftest.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/settings.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/test_datalayer.py
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/test_datalayer_views.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/test_licence.py
+-rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/test_map.py
+-rw-r--r--   0        0        0    21739 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/test_map_views.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/test_tilelayer.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/test_utils.py
+-rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/test_views.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/fixtures/test_upload_data.csv
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/fixtures/test_upload_data.gpx
+-rw-r--r--   0        0        0     5650 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/fixtures/test_upload_data.json
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/fixtures/test_upload_data.kml
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/fixtures/test_upload_empty_coordinates.json
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/fixtures/test_upload_missing_name.json
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/fixtures/test_upload_non_linear_ring.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 umap_project-1.3.4/umap/tests/integration/.DS_Store
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 umap_project-1.3.4/.gitignore
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 umap_project-1.3.4/LICENSE
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 umap_project-1.3.4/README.md
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 umap_project-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 umap_project-1.3.4/PKG-INFO
```

### Comparing `umap-project-1.3.3/PKG-INFO` & `umap_project-1.3.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,49 @@
 Metadata-Version: 2.1
 Name: umap-project
-Version: 1.3.3
+Version: 1.3.4
 Summary: Create maps with OpenStreetMap layers in a minute and embed them in your site.
-Author: Yohan Boniface
-Keywords: django leaflet geodjango openstreetmap map
+Author-email: Yohan Boniface <yb@enix.org>
+Maintainer-email: David Larlet <david@larlet.fr>
+License-File: LICENSE
+Keywords: django,geodjango,leaflet,map,openstreetmap
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Requires-Dist: django-agnocomplete==2.2.0
+Requires-Dist: django-compressor==4.3.1
+Requires-Dist: django-environ==0.10.0
+Requires-Dist: django>=4.1
+Requires-Dist: pillow==9.5.0
+Requires-Dist: psycopg2==2.9.6
+Requires-Dist: requests==2.30.0
+Requires-Dist: social-auth-app-django==5.2.0
+Requires-Dist: social-auth-core==4.4.2
 Provides-Extra: dev
-Provides-Extra: test
+Requires-Dist: black==21.10b0; extra == 'dev'
+Requires-Dist: hatch==1.7.0; extra == 'dev'
+Requires-Dist: mkdocs==1.2.3; extra == 'dev'
 Provides-Extra: docker
-License-File: LICENSE
+Requires-Dist: uwsgi==2.0.21; extra == 'docker'
+Provides-Extra: test
+Requires-Dist: factory-boy==3.2.1; extra == 'test'
+Requires-Dist: pytest-django==4.5.2; extra == 'test'
+Requires-Dist: pytest==6.2.5; extra == 'test'
+Description-Content-Type: text/markdown
 
 
 # uMap project
 
 [![Requirements Status](https://requires.io/github/umap-project/umap/requirements.svg?branch=master)](https://requires.io/github/umap-project/umap/requirements/?branch=master)
 [![Join the chat at https://gitter.im/umap-project/umap](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/umap-project/umap?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Documentation Status](https://readthedocs.org/projects/umap-project/badge/?version=latest)](http://umap-project.readthedocs.io/en/latest/?badge=latest)[![Build Status](https://travis-ci.org/umap-project/umap.svg?branch=master)](https://travis-ci.org/umap-project/umap)
```

### Comparing `umap-project-1.3.3/README.md` & `umap_project-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/admin.py` & `umap_project-1.3.4/umap/admin.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/decorators.py` & `umap_project-1.3.4/umap/decorators.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/fields.py` & `umap_project-1.3.4/umap/fields.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/forms.py` & `umap_project-1.3.4/umap/forms.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/am_ET/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/am_ET/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/am_ET/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/am_ET/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ar/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ar/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ast/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/ast/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/bg/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/bg/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ca/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ca/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/cs_CZ/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/cs_CZ/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/da/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/da/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/de/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/de/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/el/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/el/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/en/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/es/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/es/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/et/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/et/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/fa_IR/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/fa_IR/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/fi/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/fi/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/fr/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/fr/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/gl/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/gl/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/he/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/he/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/hr/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/hr/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/hu/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/hu/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/id/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/is/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/is/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/it/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/it/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ja/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ja/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ko/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ko/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/lt/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/lt/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ms/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/ms/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ms/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/ms/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/nl/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/nl/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/no/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/no/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/pl/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/pl/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/pt/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/pt/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/pt_BR/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/pt_BR/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/pt_PT/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/pt_PT/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ro/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ro/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ru/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/ru/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/si_LK/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/si_LK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/sk_SK/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/sk_SK/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/sl/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/sl/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/sr/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/sr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/sr/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/sv/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/sv/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/th_TH/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/th_TH/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/th_TH/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/th_TH/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/tr/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/tr/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/uk_UA/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/uk_UA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/uk_UA/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/uk_UA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/vi/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/vi/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/zh/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/zh/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/zh_TW/LC_MESSAGES/django.mo` & `umap_project-1.3.4/umap/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/locale/zh_TW/LC_MESSAGES/django.po` & `umap_project-1.3.4/umap/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/management/commands/anonymous_edit_url.py` & `umap_project-1.3.4/umap/management/commands/anonymous_edit_url.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/management/commands/generate_js_locale.py` & `umap_project-1.3.4/umap/management/commands/generate_js_locale.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/management/commands/import_pictograms.py` & `umap_project-1.3.4/umap/management/commands/import_pictograms.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/middleware.py` & `umap_project-1.3.4/umap/middleware.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/migrations/0001_initial.py` & `umap_project-1.3.4/umap/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/migrations/0003_add_tilelayer.py` & `umap_project-1.3.4/umap/migrations/0003_add_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/migrations/0004_add_licence.py` & `umap_project-1.3.4/umap/migrations/0004_add_licence.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/migrations/0007_auto_20190416_1757.py` & `umap_project-1.3.4/umap/migrations/0007_auto_20190416_1757.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/migrations/0009_star.py` & `umap_project-1.3.4/umap/migrations/0009_star.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/models.py` & `umap_project-1.3.4/umap/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,45 @@
 import os
 import time
 
+from django.contrib.auth.models import User
 from django.contrib.gis.db import models
 from django.conf import settings
 from django.urls import reverse
 from django.utils.translation import gettext_lazy as _
 from django.core.signing import Signer
 from django.template.defaultfilters import slugify
 from django.core.files.base import File
 
 from .managers import PublicManager
 
 
+# Did not find a clean way to do this in Django
+# - creating a Proxy model would mean replacing get_user_model by this proxy model
+#   in every template
+# - extending User model woulc mean a non trivial migration
+def display_name(self):
+    return settings.USER_DISPLAY_NAME.format(**self.__dict__)
+
+
+def get_user_url(self):
+    identifier = getattr(self, settings.USER_URL_FIELD)
+    return reverse(settings.USER_MAPS_URL, kwargs={"identifier": identifier})
+
+
+def get_user_stars_url(self):
+    identifier = getattr(self, settings.USER_URL_FIELD)
+    return reverse("user_stars", kwargs={"identifier": identifier})
+
+
+User.add_to_class("__str__", display_name)
+User.add_to_class("get_url", get_user_url)
+User.add_to_class("get_stars_url", get_user_stars_url)
+
+
 class NamedModel(models.Model):
     name = models.CharField(max_length=200, verbose_name=_("name"))
 
     class Meta:
         abstract = True
         ordering = ("name",)
```

### Comparing `umap-project-1.3.3/umap/settings/__init__.py` & `umap_project-1.3.4/umap/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/settings/base.py` & `umap_project-1.3.4/umap/settings/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,17 +165,14 @@
 # Templates
 # =============================================================================
 
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'APP_DIRS': True,
-        'DIRS': [
-            os.path.join(PROJECT_DIR, 'templates'),
-        ],
         'OPTIONS': {
             'context_processors': (
                 'django.contrib.auth.context_processors.auth',
                 'django.template.context_processors.debug',
                 'django.template.context_processors.i18n',
                 'django.template.context_processors.request',
                 'django.template.context_processors.media',
@@ -210,14 +207,19 @@
 # =============================================================================
 # Auth / security
 # =============================================================================
 
 # Set to True if login into django account should be possible. Default is to
 # only use OAuth flow.
 ENABLE_ACCOUNT_LOGIN = env.bool("ENABLE_ACCOUNT_LOGIN", default=False)
+USER_DISPLAY_NAME = "{username}"
+# For use by Agnocomplete
+# See https://django-agnocomplete.readthedocs.io/en/latest/autocomplete-definition.html#agnocompletemode
+USER_AUTOCOMPLETE_FIELDS = ["^username"]
+USER_URL_FIELD = "username"
 
 # =============================================================================
 # Miscellaneous project settings
 # =============================================================================
 UMAP_ALLOW_ANONYMOUS = env.bool("UMAP_ALLOW_ANONYMOUS", default=False)
 
 UMAP_EXTRA_URLS = {
@@ -251,16 +253,14 @@
 
 # =============================================================================
 # Third party app settings
 # =============================================================================
 COMPRESS_ENABLED = True
 COMPRESS_OFFLINE = True
 
-SOCIAL_AUTH_DEFAULT_USERNAME = lambda u: slugify(u)
-SOCIAL_AUTH_ASSOCIATE_BY_EMAIL = True
 SOCIAL_AUTH_NO_DEFAULT_PROTECTED_USER_FIELDS = True
 SOCIAL_AUTH_PROTECTED_USER_FIELDS = ("id", )
 LOGIN_URL = "login"
 SOCIAL_AUTH_LOGIN_REDIRECT_URL = "/login/popup/end/"
 
 AUTHENTICATION_BACKENDS = ()
```

### Comparing `umap-project-1.3.3/umap/static/favicon.ico` & `umap_project-1.3.4/umap/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/base.css` & `umap_project-1.3.4/umap/static/umap/base.css`

 * *Files 0% similar despite different names*

```diff
@@ -502,15 +502,14 @@
 }
 .permissions-panel,
 .umap-upload,
 .umap-share,
 .umap-edit-container,
 .umap-datalayer-container,
 .umap-layer-properties-container,
-.umap-footer-container,
 .umap-browse-data,
 .umap-filter-data,
 .umap-browse-datalayers {
     padding: 0 10px;
 }
 .umap-field-datalist {
     display: flex;
```

### Comparing `umap-project-1.3.3/umap/static/umap/bitbucket.png` & `umap_project-1.3.4/umap/static/umap/bitbucket.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/content.css` & `umap_project-1.3.4/umap/static/umap/content.css`

 * *Files 6% similar despite different names*

```diff
@@ -255,14 +255,35 @@
 }
 .umap-singleresult div .close,
 .umap-multiresult li .close {
     float: right;
     cursor: pointer;
 }
 
+/* **************************** */
+/*           Messages           */
+/* **************************** */
+.messages li {
+    border-radius: 1px;
+    color: white;
+    margin-bottom: 20px;
+    padding: 20px;
+    text-align: center;
+    width: 100%;
+    background-color: #444;
+    font-weight: bold;
+}
+
+.messages .success {
+    background-color: #16a085;
+}
+
+.messages .error {
+    background-color: #c60f13;
+}
 
 
 /* **************************** */
 /*   Override Leaflet.Storage   */
 /* **************************** */
 #id_editors + br + span.helptext {
     display: none;
```

### Comparing `umap-project-1.3.3/umap/static/umap/font/FiraSans-Light.woff` & `umap_project-1.3.4/umap/static/umap/font/FiraSans-Light.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/font/FiraSans-Light.woff2` & `umap_project-1.3.4/umap/static/umap/font/FiraSans-Light.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/font/FiraSans-LightItalic.woff` & `umap_project-1.3.4/umap/static/umap/font/FiraSans-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/font/FiraSans-LightItalic.woff2` & `umap_project-1.3.4/umap/static/umap/font/FiraSans-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/font/FiraSans-SemiBold.woff` & `umap_project-1.3.4/umap/static/umap/font/FiraSans-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/font/FiraSans-SemiBold.woff2` & `umap_project-1.3.4/umap/static/umap/font/FiraSans-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/font.css` & `umap_project-1.3.4/umap/static/umap/font.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/github.png` & `umap_project-1.3.4/umap/static/umap/github.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/16-white.png` & `umap_project-1.3.4/umap/static/umap/img/16-white.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/16-white.svg` & `umap_project-1.3.4/umap/static/umap/img/16-white.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/16.png` & `umap_project-1.3.4/umap/static/umap/img/16.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/16.svg` & `umap_project-1.3.4/umap/static/umap/img/16.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/24-white.png` & `umap_project-1.3.4/umap/static/umap/img/24-white.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/24-white.svg` & `umap_project-1.3.4/umap/static/umap/img/24-white.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/24.png` & `umap_project-1.3.4/umap/static/umap/img/24.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/24.svg` & `umap_project-1.3.4/umap/static/umap/img/24.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/edit.svg` & `umap_project-1.3.4/umap/static/umap/img/edit.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/logo_filigree.png` & `umap_project-1.3.4/umap/static/umap/img/logo_filigree.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/osm.svg` & `umap_project-1.3.4/umap/static/umap/img/osm.svg`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/img/search.gif` & `umap_project-1.3.4/umap/static/umap/img/search.gif`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.autocomplete.js` & `umap_project-1.3.4/umap/static/umap/js/umap.autocomplete.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.controls.js` & `umap_project-1.3.4/umap/static/umap/js/umap.controls.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.core.js` & `umap_project-1.3.4/umap/static/umap/js/umap.core.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -62,14 +62,19 @@
             'div',
             'iframe',
             'img',
             'br',
         ],
         ADD_ATTR: ['target', 'allow', 'allowfullscreen', 'frameborder', 'scrolling'],
         ALLOWED_ATTR: ['href', 'src', 'width', 'height'],
+        // Added: `geo:` URL scheme as defined in RFC5870:
+        // https://www.rfc-editor.org/rfc/rfc5870.html
+        // The base RegExp comes from:
+        // https://github.com/cure53/DOMPurify/blob/main/src/regexp.js#L10
+        ALLOWED_URI_REGEXP: /^(?:(?:(?:f|ht)tps?|mailto|tel|callto|sms|cid|xmpp|geo):|[^a-z]|[a-z+.\-]+(?:[^a-z+.\-:]|$))/i,
     })
     return s
 }
 L.Util.toHTML = (r) => {
     if (!r) return ''
     let ii
```

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.features.js` & `umap_project-1.3.4/umap/static/umap/js/umap.features.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -594,14 +594,15 @@
     },
 
     getShapeOptions: function() {
         return [
             'properties._umap_options.color',
             'properties._umap_options.iconClass',
             'properties._umap_options.iconUrl',
+            'properties._umap_options.iconOpacity',
         ]
     },
 
     getAdvancedOptions: function() {
         return ['properties._umap_options.zoomTo']
     },
```

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.forms.js` & `umap_project-1.3.4/umap/static/umap/js/umap.forms.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -911,14 +911,22 @@
         },
         color: {
             handler: 'ColorPicker',
             label: L._('color'),
             helpEntries: 'colorValue',
             inheritable: true,
         },
+        iconOpacity: {
+            handler: 'Range',
+            min: 0.1,
+            max: 1,
+            step: 0.1,
+            label: L._('icon opacity'),
+            inheritable: true,
+        },
         opacity: {
             handler: 'Range',
             min: 0.1,
             max: 1,
             step: 0.1,
             label: L._('opacity'),
             inheritable: true,
```

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.icon.js` & `umap_project-1.3.4/umap/static/umap/js/umap.icon.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -26,14 +26,19 @@
         let color
         if (this.feature) color = this.feature.getOption('color')
         else if (this.options.color) color = this.options.color
         else color = this.map.getDefaultOption('color')
         return color
     },
 
+    _getOpacity: function() {
+        if (this.feature) return this.feature.getOption('iconOpacity')
+        return this.map.getDefaultOption('iconOpacity')
+    },
+
     formatUrl: function(url, feature) {
         return L.Util.greedyTemplate(url || '', feature ? feature.extendedProperties() : {})
     },
 })
 
 L.U.Icon.Default = L.U.Icon.extend({
     default_options: {
@@ -44,18 +49,22 @@
     },
 
     initialize: function(map, options) {
         options = L.Util.extend({}, this.default_options, options)
         L.U.Icon.prototype.initialize.call(this, map, options)
     },
 
-    _setColor: function() {
-        const color = this._getColor()
+    _setIconStyles: function(img, name) {
+        L.U.Icon.prototype._setIconStyles.call(this, img, name)
+        const color = this._getColor(),
+            opacity = this._getOpacity()
         this.elements.container.style.backgroundColor = color
         this.elements.arrow.style.borderTopColor = color
+        this.elements.container.style.opacity = opacity
+        this.elements.arrow.style.opacity = opacity
     },
 
     createIcon: function() {
         this.elements = {}
         this.elements.main = L.DomUtil.create('div')
         this.elements.container = L.DomUtil.create(
             'div',
@@ -74,15 +83,14 @@
                 this.elements.img = L.DomUtil.create('img', null, this.elements.container)
                 this.elements.img.src = src
             } else {
                 this.elements.span = L.DomUtil.create('span', null, this.elements.container)
                 this.elements.span.textContent = src
             }
         }
-        this._setColor()
         this._setIconStyles(this.elements.main, 'icon')
         return this.elements.main
     },
 })
 
 L.U.Icon.Circle = L.U.Icon.extend({
     initialize: function(map, options) {
@@ -92,23 +100,24 @@
             tooltipAnchor: new L.Point(6, 0),
             className: 'umap-circle-icon',
         }
         options = L.Util.extend({}, default_options, options)
         L.U.Icon.prototype.initialize.call(this, map, options)
     },
 
-    _setColor: function() {
+    _setIconStyles: function(img, name) {
+        L.U.Icon.prototype._setIconStyles.call(this, img, name)
         this.elements.main.style.backgroundColor = this._getColor()
+        this.elements.main.style.opacity = this._getOpacity()
     },
 
     createIcon: function() {
         this.elements = {}
         this.elements.main = L.DomUtil.create('div')
         this.elements.main.innerHTML = '&nbsp;'
-        this._setColor()
         this._setIconStyles(this.elements.main, 'icon')
         return this.elements.main
     },
 })
 
 L.U.Icon.Drop = L.U.Icon.Default.extend({
     default_options: {
@@ -132,30 +141,31 @@
         this.elements.main = L.DomUtil.create('div')
         this.elements.container = L.DomUtil.create(
             'div',
             'icon_container',
             this.elements.main
         )
         this.elements.arrow = L.DomUtil.create('div', 'icon_arrow', this.elements.main)
-        this._setColor()
         this._setIconStyles(this.elements.main, 'icon')
         return this.elements.main
     },
 
-    _setColor: function() {
+    _setIconStyles: function(img, name) {
+        L.U.Icon.prototype._setIconStyles.call(this, img, name)
         const color = this._getColor('color')
         let background
         if (L.Browser.ielt9) {
             background = color
         } else if (L.Browser.webkit) {
             background = `-webkit-gradient( radial, 6 38%, 0, 6 38%, 8, from(white), to(${color}) )`
         } else {
             background = `radial-gradient(circle at 6px 38% , white -4px, ${color} 8px) repeat scroll 0 0 transparent`
         }
         this.elements.container.style.background = background
+        this.elements.container.style.opacity = this._getOpacity()
     },
 })
 
 const _CACHE_COLOR = {}
 L.U.Icon.Cluster = L.DivIcon.extend({
     options: {
         iconSize: [40, 40],
```

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.js` & `umap_project-1.3.4/umap/static/umap/js/umap.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,14 +7,15 @@
     default_color: 'DarkBlue',
     default_smoothFactor: 1.0,
     default_opacity: 0.5,
     default_fillOpacity: 0.3,
     default_stroke: true,
     default_fill: true,
     default_weight: 3,
+    default_iconOpacity: 1,
     default_iconClass: 'Default',
     default_popupContentTemplate: '# {name}\n{description}',
     default_interactive: true,
     default_labelDirection: 'auto',
     attributionControl: false,
     allowEdit: true,
     embedControl: true,
@@ -1320,14 +1321,15 @@
         'tilelayer',
         'overlay',
         'limitBounds',
         'color',
         'iconClass',
         'iconUrl',
         'smoothFactor',
+        'iconOpacity',
         'opacity',
         'weight',
         'fill',
         'fillColor',
         'fillOpacity',
         'dashArray',
         'popupShape',
@@ -1612,14 +1614,15 @@
     },
 
     _editShapeProperties: function(container) {
         const shapeOptions = [
             'options.color',
             'options.iconClass',
             'options.iconUrl',
+            'options.iconOpacity',
             'options.opacity',
             'options.weight',
             'options.fill',
             'options.fillColor',
             'options.fillOpacity',
         ]
```

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.layer.js` & `umap_project-1.3.4/umap/static/umap/js/umap.layer.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -827,14 +827,15 @@
         })
         container.appendChild(builder.build())
 
         let shapeOptions = [
             'options.color',
             'options.iconClass',
             'options.iconUrl',
+            'options.iconOpacity',
             'options.opacity',
             'options.stroke',
             'options.weight',
             'options.fill',
             'options.fillColor',
             'options.fillOpacity',
         ]
```

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.permissions.js` & `umap_project-1.3.4/umap/static/umap/js/umap.permissions.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.popup.js` & `umap_project-1.3.4/umap/static/umap/js/umap.popup.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -114,20 +114,15 @@
         content = L.Util.toHTML(content)
         container.innerHTML = content
         return container
     },
 
     renderFooter: function() {
         if (this.feature.hasPopupFooter()) {
-            const footerContainer = L.DomUtil.create(
-                    'div',
-                    'umap-footer-container',
-                    this.container
-                ),
-                footer = L.DomUtil.create('ul', 'umap-popup-footer', footerContainer),
+            const footer = L.DomUtil.create('ul', 'umap-popup-footer', this.container),
                 previousLi = L.DomUtil.create('li', 'previous', footer),
                 zoomLi = L.DomUtil.create('li', 'zoom', footer),
                 nextLi = L.DomUtil.create('li', 'next', footer),
                 next = this.feature.getNext(),
                 prev = this.feature.getPrevious()
             if (next)
                 nextLi.title = L._('Go to «{feature}»', {
```

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.slideshow.js` & `umap_project-1.3.4/umap/static/umap/js/umap.slideshow.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.tableeditor.js` & `umap_project-1.3.4/umap/static/umap/js/umap.tableeditor.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.ui.js` & `umap_project-1.3.4/umap/static/umap/js/umap.ui.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -122,15 +122,20 @@
                 el = L.DomUtil.element('a', {
                     className: 'umap-action'
                 }, this._alert)
                 el.href = '#'
                 el.textContent = action.label
                 L.DomEvent.on(el, 'click', L.DomEvent.stop)
                 if (action.callback) {
-                    L.DomEvent.on(el, 'click', action.callback, action.callbackContext || this.map)
+                    L.DomEvent.on(
+                        el,
+                        'click',
+                        action.callback,
+                        action.callbackContext || this.map
+                    )
                 }
                 L.DomEvent.on(el, 'click', close, this)
             }
         }
         if (e.duration !== Infinity) {
             this.ALERT_ID = timeoutID = window.setTimeout(
                 L.bind(close, this),
```

### Comparing `umap-project-1.3.3/umap/static/umap/js/umap.xhr.js` & `umap_project-1.3.4/umap/static/umap/js/umap.xhr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/am_ET.js` & `umap_project-1.3.4/umap/static/umap/locale/am_ET.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/am_ET.json` & `umap_project-1.3.4/umap/static/umap/locale/am_ET.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ar.js` & `umap_project-1.3.4/umap/static/umap/locale/ar.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ar.json` & `umap_project-1.3.4/umap/static/umap/locale/ar.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ast.js` & `umap_project-1.3.4/umap/static/umap/locale/ast.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ast.json` & `umap_project-1.3.4/umap/static/umap/locale/ast.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/bg.js` & `umap_project-1.3.4/umap/static/umap/locale/bg.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/bg.json` & `umap_project-1.3.4/umap/static/umap/locale/bg.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ca.js` & `umap_project-1.3.4/umap/static/umap/locale/ca.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ca.json` & `umap_project-1.3.4/umap/static/umap/locale/ca.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/cs_CZ.js` & `umap_project-1.3.4/umap/static/umap/locale/cs_CZ.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/cs_CZ.json` & `umap_project-1.3.4/umap/static/umap/locale/cs_CZ.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/da.js` & `umap_project-1.3.4/umap/static/umap/locale/da.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/da.json` & `umap_project-1.3.4/umap/static/umap/locale/da.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/de.js` & `umap_project-1.3.4/umap/static/umap/locale/de.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/de.json` & `umap_project-1.3.4/umap/static/umap/locale/de.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/el.js` & `umap_project-1.3.4/umap/static/umap/locale/el.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/el.json` & `umap_project-1.3.4/umap/static/umap/locale/el.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/en.js` & `umap_project-1.3.4/umap/static/umap/locale/en.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/en.json` & `umap_project-1.3.4/umap/static/umap/locale/en.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/en_US.json` & `umap_project-1.3.4/umap/static/umap/locale/en_US.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/es.js` & `umap_project-1.3.4/umap/static/umap/locale/es.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/es.json` & `umap_project-1.3.4/umap/static/umap/locale/es.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/et.js` & `umap_project-1.3.4/umap/static/umap/locale/et.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/et.json` & `umap_project-1.3.4/umap/static/umap/locale/et.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/fa_IR.js` & `umap_project-1.3.4/umap/static/umap/locale/fa_IR.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/fa_IR.json` & `umap_project-1.3.4/umap/static/umap/locale/fa_IR.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/fi.js` & `umap_project-1.3.4/umap/static/umap/locale/fi.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/fi.json` & `umap_project-1.3.4/umap/static/umap/locale/fi.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/fr.js` & `umap_project-1.3.4/umap/static/umap/locale/fr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/fr.json` & `umap_project-1.3.4/umap/static/umap/locale/fr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/gl.js` & `umap_project-1.3.4/umap/static/umap/locale/gl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/gl.json` & `umap_project-1.3.4/umap/static/umap/locale/gl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/he.js` & `umap_project-1.3.4/umap/static/umap/locale/he.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/he.json` & `umap_project-1.3.4/umap/static/umap/locale/he.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/hr.js` & `umap_project-1.3.4/umap/static/umap/locale/hr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/hr.json` & `umap_project-1.3.4/umap/static/umap/locale/hr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/hu.js` & `umap_project-1.3.4/umap/static/umap/locale/hu.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/hu.json` & `umap_project-1.3.4/umap/static/umap/locale/hu.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/id.js` & `umap_project-1.3.4/umap/static/umap/locale/id.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/id.json` & `umap_project-1.3.4/umap/static/umap/locale/id.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/is.js` & `umap_project-1.3.4/umap/static/umap/locale/is.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/is.json` & `umap_project-1.3.4/umap/static/umap/locale/is.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/it.js` & `umap_project-1.3.4/umap/static/umap/locale/it.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/it.json` & `umap_project-1.3.4/umap/static/umap/locale/it.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ja.js` & `umap_project-1.3.4/umap/static/umap/locale/ja.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ja.json` & `umap_project-1.3.4/umap/static/umap/locale/ja.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ko.js` & `umap_project-1.3.4/umap/static/umap/locale/ko.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ko.json` & `umap_project-1.3.4/umap/static/umap/locale/ko.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/lt.js` & `umap_project-1.3.4/umap/static/umap/locale/lt.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/lt.json` & `umap_project-1.3.4/umap/static/umap/locale/lt.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ms.js` & `umap_project-1.3.4/umap/static/umap/locale/ms.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ms.json` & `umap_project-1.3.4/umap/static/umap/locale/ms.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/nl.js` & `umap_project-1.3.4/umap/static/umap/locale/nl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/nl.json` & `umap_project-1.3.4/umap/static/umap/locale/nl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/no.js` & `umap_project-1.3.4/umap/static/umap/locale/no.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/no.json` & `umap_project-1.3.4/umap/static/umap/locale/no.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/pl.js` & `umap_project-1.3.4/umap/static/umap/locale/pl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/pl.json` & `umap_project-1.3.4/umap/static/umap/locale/pl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/pl_PL.json` & `umap_project-1.3.4/umap/static/umap/locale/pl_PL.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/pt.js` & `umap_project-1.3.4/umap/static/umap/locale/pt.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/pt.json` & `umap_project-1.3.4/umap/static/umap/locale/pt.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/pt_BR.js` & `umap_project-1.3.4/umap/static/umap/locale/pt_BR.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/pt_BR.json` & `umap_project-1.3.4/umap/static/umap/locale/pt_BR.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/pt_PT.js` & `umap_project-1.3.4/umap/static/umap/locale/pt_PT.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/pt_PT.json` & `umap_project-1.3.4/umap/static/umap/locale/pt_PT.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ro.js` & `umap_project-1.3.4/umap/static/umap/locale/ro.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ro.json` & `umap_project-1.3.4/umap/static/umap/locale/ro.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ru.js` & `umap_project-1.3.4/umap/static/umap/locale/ru.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/ru.json` & `umap_project-1.3.4/umap/static/umap/locale/ru.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/si_LK.js` & `umap_project-1.3.4/umap/static/umap/locale/si_LK.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/si_LK.json` & `umap_project-1.3.4/umap/static/umap/locale/si_LK.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/sk_SK.js` & `umap_project-1.3.4/umap/static/umap/locale/sk_SK.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/sk_SK.json` & `umap_project-1.3.4/umap/static/umap/locale/sk_SK.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/sl.js` & `umap_project-1.3.4/umap/static/umap/locale/sl.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/sl.json` & `umap_project-1.3.4/umap/static/umap/locale/sl.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/sr.js` & `umap_project-1.3.4/umap/static/umap/locale/sr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/sr.json` & `umap_project-1.3.4/umap/static/umap/locale/sr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/sv.js` & `umap_project-1.3.4/umap/static/umap/locale/sv.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/sv.json` & `umap_project-1.3.4/umap/static/umap/locale/sv.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/th_TH.js` & `umap_project-1.3.4/umap/static/umap/locale/th_TH.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/th_TH.json` & `umap_project-1.3.4/umap/static/umap/locale/th_TH.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/tr.js` & `umap_project-1.3.4/umap/static/umap/locale/tr.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/tr.json` & `umap_project-1.3.4/umap/static/umap/locale/tr.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/uk_UA.js` & `umap_project-1.3.4/umap/static/umap/locale/uk_UA.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/uk_UA.json` & `umap_project-1.3.4/umap/static/umap/locale/uk_UA.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/vi.js` & `umap_project-1.3.4/umap/static/umap/locale/vi.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/vi.json` & `umap_project-1.3.4/umap/static/umap/locale/vi.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/vi_VN.json` & `umap_project-1.3.4/umap/static/umap/locale/vi_VN.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/zh.js` & `umap_project-1.3.4/umap/static/umap/locale/zh.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/zh.json` & `umap_project-1.3.4/umap/static/umap/locale/zh.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/zh_CN.json` & `umap_project-1.3.4/umap/static/umap/locale/zh_CN.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/zh_TW.Big5.json` & `umap_project-1.3.4/umap/static/umap/locale/zh_TW.Big5.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/zh_TW.js` & `umap_project-1.3.4/umap/static/umap/locale/zh_TW.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/locale/zh_TW.json` & `umap_project-1.3.4/umap/static/umap/locale/zh_TW.json`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/map.css` & `umap_project-1.3.4/umap/static/umap/map.css`

 * *Files 0% similar despite different names*

```diff
@@ -583,15 +583,15 @@
     background-color: #fff;
     padding: 10px;
     display: none;
     line-height: 24px;
     border-radius: 2px;
 }
 .leaflet-control-browse .umap-browse-datalayers {
-    max-height: 10em;
+    max-height: 15em;
     overflow-y: auto;
 }
 .search-result-tools i,
 .leaflet-inplace-toolbar a,
 .umap-browse-features i,
 .umap-caption i,
 .umap-browse-datalayers i {
@@ -1312,22 +1312,22 @@
     line-height: inherit;
 }
 .leaflet-popup-content-wrapper, .leaflet-popup-tip {
     box-shadow: 0 1px 6px rgba(0, 0, 0, 0.4);
 }
 .leaflet-popup-content-wrapper {
     border-radius: 4px;
-    overflow-y: scroll;
 }
 .umap-popup-content {
     max-height: 500px;
     flex-grow: 1;
     margin-bottom: 4px;
     display: flex;
     flex-direction: column;
+    overflow-y: scroll;
 }
 .umap-popup-content iframe {
     min-width: 310px;
     max-width: 100%;
 }
 .umap-popup-content tr:nth-child(odd) {
    background-color: #f6f6f6;
```

### Comparing `umap-project-1.3.3/umap/static/umap/nav.css` & `umap_project-1.3.4/umap/static/umap/nav.css`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/openstreetmap.png` & `umap_project-1.3.4/umap/static/umap/openstreetmap.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/Controls.js` & `umap_project-1.3.4/umap/static/umap/test/Controls.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/DataLayer.js` & `umap_project-1.3.4/umap/static/umap/test/DataLayer.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/Feature.js` & `umap_project-1.3.4/umap/static/umap/test/Feature.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/Map.js` & `umap_project-1.3.4/umap/static/umap/test/Map.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/Marker.js` & `umap_project-1.3.4/umap/static/umap/test/Marker.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/Permissions.js` & `umap_project-1.3.4/umap/static/umap/test/Permissions.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/Polygon.js` & `umap_project-1.3.4/umap/static/umap/test/Polygon.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/Polyline.js` & `umap_project-1.3.4/umap/static/umap/test/Polyline.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/TableEditor.js` & `umap_project-1.3.4/umap/static/umap/test/TableEditor.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/Util.js` & `umap_project-1.3.4/umap/static/umap/test/Util.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -162,14 +162,21 @@
     })
 
     describe('#escapeHTML', function() {
         it('should escape HTML tags', function() {
             assert.equal(L.Util.escapeHTML('<span onload="alert(oups)">'), '<span></span>')
         })
 
+        it('should not escape geo: links', function() {
+            assert.equal(
+                L.Util.escapeHTML('<a href="geo:1,2"></a>'),
+                '<a href="geo:1,2"></a>'
+            )
+        })
+
         it('should not fail with int value', function() {
             assert.equal(L.Util.escapeHTML(25), '25')
         })
 
         it('should not fail with null value', function() {
             assert.equal(L.Util.escapeHTML(null), '')
         })
```

### Comparing `umap-project-1.3.3/umap/static/umap/test/_pre.js` & `umap_project-1.3.4/umap/static/umap/test/_pre.js`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/test/index.html` & `umap_project-1.3.4/umap/static/umap/test/index.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/static/umap/twitter.png` & `umap_project-1.3.4/umap/static/umap/twitter.png`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/500.html` & `umap_project-1.3.4/umap/templates/500.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/base.html` & `umap_project-1.3.4/umap/templates/base.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/registration/login.html` & `umap_project-1.3.4/umap/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/umap/about_summary.html` & `umap_project-1.3.4/umap/templates/umap/about_summary.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/umap/content.html` & `umap_project-1.3.4/umap/templates/umap/content.html`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     {% umap_js %}
 {% endblock %}
 
 {% block header %}
   <header class="wrapper row">
     {% include 'umap/navigation.html' with title=SITE_NAME %}
   </header>
+    {% include 'umap/messages.html' with title=SITE_NAME %}
 {% endblock %}
 
 {% block content %}
   {% if UMAP_READONLY %}
     <div class="wrapper demo-instance-warning">
       <div class="row">
         <p>
```

### Comparing `umap-project-1.3.3/umap/templates/umap/content_footer.html` & `umap_project-1.3.4/umap/templates/umap/content_footer.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/umap/css.html` & `umap_project-1.3.4/umap/templates/umap/css.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/umap/home.html` & `umap_project-1.3.4/umap/templates/umap/home.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/umap/js.html` & `umap_project-1.3.4/umap/templates/umap/js.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/umap/map_detail.html` & `umap_project-1.3.4/umap/templates/umap/map_detail.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templates/umap/map_list.html` & `umap_project-1.3.4/umap/templates/umap/map_list.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load umap_tags umap_tags i18n %}
 
 {% for map_inst in maps %}
 <hr />
 <div class="col wide">
     {% map_fragment map_inst prefix=prefix page=request.GET.p %}
-    <div class="legend"><a href="{{ map_inst.get_absolute_url }}">{{ map_inst.name }}</a>{% if map_inst.owner %} <em>{% trans "by" %} <a href="{% url 'user_maps' map_inst.owner.username %}">{{ map_inst.owner }}</a></em>{% endif %}</div>
+    <div class="legend"><a href="{{ map_inst.get_absolute_url }}">{{ map_inst.name }}</a>{% if map_inst.owner %} <em>{% trans "by" %} <a href="{{ map_inst.owner.get_url }}">{{ map_inst.owner }}</a></em>{% endif %}</div>
 </div>
 {% endfor %}
 {% if maps.has_next %}
 <div class="col wide"><a href="?{% paginate_querystring maps.next_page_number %}" class="button more_button neutral">{% trans "More" %}</a></div>
 {% endif %}
```

### Comparing `umap-project-1.3.3/umap/templates/umap/navigation.html` & `umap_project-1.3.4/umap/templates/umap/navigation.html`

 * *Files 25% similar despite different names*

```diff
@@ -3,16 +3,16 @@
   <section>
     <h1><a href="/">{{ title }}</a></h1>
   </section>
 
   <section>
     <ul>
       {% if user.is_authenticated %}
-        <li><a href="{% url 'user_maps' user.username %}">{% trans "My maps" %} ({{ user }})</a></li>
-        <li><a href="{% url 'user_stars' user.username %}">{% trans "Starred maps" %}</a></li>
+        <li><a href="{{ user.get_url }}">{% trans "My maps" %} ({{ user }})</a></li>
+        <li><a href="{{ user.get_stars_url %}">{% trans "Starred maps" %}</a></li>
       {% else %}
         <li><a href="{% url 'login' %}" class="login">{% trans "Log in" %} / {% trans "Sign in" %}</a></li>
       {% endif %}
       <li><a href="{% url 'about' %}">{% trans "About" %}</a></li>
       <li><a href="{{ UMAP_FEEDBACK_LINK }}">{% trans "Help" %}</a></li>
       {% if user.is_authenticated %}
         {% if user.has_usable_password %}
```

### Comparing `umap-project-1.3.3/umap/templates/umap/password_change.html` & `umap_project-1.3.4/umap/templates/umap/password_change.html`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/templatetags/umap_tags.py` & `umap_project-1.3.4/umap/templatetags/umap_tags.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/tests/base.py` & `umap_project-1.3.4/umap/tests/base.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/tests/conftest.py` & `umap_project-1.3.4/umap/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/tests/test_datalayer.py` & `umap_project-1.3.4/umap/tests/test_datalayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/tests/test_datalayer_views.py` & `umap_project-1.3.4/umap/tests/test_datalayer_views.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/tests/test_map.py` & `umap_project-1.3.4/umap/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/tests/test_map_views.py` & `umap_project-1.3.4/umap/tests/test_map_views.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/tests/test_tilelayer.py` & `umap_project-1.3.4/umap/tests/test_tilelayer.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/tests/test_views.py` & `umap_project-1.3.4/umap/tests/test_views.py`

 * *Files 8% similar despite different names*

```diff
@@ -203,7 +203,37 @@
 
 
 @pytest.mark.django_db
 def test_read_only_shows_create_buttons_if_disabled(client, settings):
     settings.UMAP_READONLY = False
     response = client.get(reverse("home"))
     assert "Create a map" in response.content.decode()
+
+
+@pytest.mark.django_db
+def test_change_user_display_name(client, user, settings):
+    username = "MyUserFooName"
+    first_name = "Ezekiel"
+    user.username = username
+    user.first_name = first_name
+    user.save()
+    client.login(username=username, password="123123")
+    response = client.get(reverse("home"))
+    assert username in response.content.decode()
+    assert first_name not in response.content.decode()
+    settings.USER_DISPLAY_NAME = "{first_name}"
+    response = client.get(reverse("home"))
+    assert first_name in response.content.decode()
+    # username will still be in the contant as it's in the "my maps" URL path.
+
+
+@pytest.mark.django_db
+def test_change_user_slug(client, user, settings):
+    username = "MyUserFooName"
+    user.username = username
+    user.save()
+    client.login(username=username, password="123123")
+    response = client.get(reverse("home"))
+    assert f"/en/user/{username}/" in response.content.decode()
+    settings.USER_URL_FIELD = "pk"
+    response = client.get(reverse("home"))
+    assert f"/en/user/{user.pk}/" in response.content.decode()
```

### Comparing `umap-project-1.3.3/umap/urls.py` & `umap_project-1.3.4/umap/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,16 +153,16 @@
 urlpatterns += i18n_patterns(
     re_path(r"^$", views.home, name="home"),
     re_path(
         r"^showcase/$", cache_page(24 * 60 * 60)(views.showcase), name="maps_showcase"
     ),
     re_path(r"^search/$", views.search, name="search"),
     re_path(r"^about/$", views.about, name="about"),
-    re_path(r"^user/(?P<username>.+)/stars/$", views.user_stars, name="user_stars"),
-    re_path(r"^user/(?P<username>.+)/$", views.user_maps, name="user_maps"),
+    re_path(r"^user/(?P<identifier>.+)/stars/$", views.user_stars, name="user_stars"),
+    re_path(r"^user/(?P<identifier>.+)/$", views.user_maps, name="user_maps"),
     re_path(r"", include(i18n_urls)),
 )
 urlpatterns += (path("stats/", cache_page(60 * 60)(views.stats), name="stats"),)
 
 if settings.DEBUG and settings.MEDIA_ROOT:
     urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
 urlpatterns += staticfiles_urlpatterns()
```

### Comparing `umap-project-1.3.3/umap/utils.py` & `umap_project-1.3.4/umap/utils.py`

 * *Files identical despite different names*

### Comparing `umap-project-1.3.3/umap/views.py` & `umap_project-1.3.4/umap/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,16 @@
 
 
 about = About.as_view()
 
 
 class UserMaps(DetailView, PaginatorMixin):
     model = User
-    slug_url_kwarg = "username"
-    slug_field = "username"
+    slug_url_kwarg = "identifier"
+    slug_field = settings.USER_URL_FIELD
     list_template_name = "umap/map_list.html"
     context_object_name = "current_user"
 
     def is_owner(self):
         return self.request.user == self.object
 
     @property
@@ -208,24 +208,26 @@
 
 class Search(TemplateView, PaginatorMixin):
     template_name = "umap/search.html"
     list_template_name = "umap/map_list.html"
 
     def get_context_data(self, **kwargs):
         q = self.request.GET.get("q")
+        qs_count = 0
         results = []
         if q:
             vector = SearchVector("name", config=settings.UMAP_SEARCH_CONFIGURATION)
             query = SearchQuery(
                 q, config=settings.UMAP_SEARCH_CONFIGURATION, search_type="websearch"
             )
             qs = Map.objects.annotate(search=vector).filter(search=query)
             qs = qs.filter(share_status=Map.PUBLIC).order_by("-modified_at")
+            qs_count = qs.count()
             results = self.paginate(qs)
-        kwargs.update({"maps": results, "q": q})
+        kwargs.update({"maps": results, "count": qs_count, "q": q})
         return kwargs
 
     def get_template_names(self):
         """
         Dispatch template according to the kind of request: ajax or normal.
         """
         if is_ajax(self.request):
@@ -244,15 +246,15 @@
 
         def make(m):
             description = m.description or ""
             if m.owner:
                 description = "{description}\n{by} [[{url}|{name}]]".format(
                     description=description,
                     by=_("by"),
-                    url=reverse("user_maps", kwargs={"username": m.owner.username}),
+                    url=m.owner.get_url(),
                     name=m.owner,
                 )
             description = "{}\n[[{}|{}]]".format(
                 description, m.get_absolute_url(), _("View the map")
             )
             geometry = m.settings.get("geometry", json.loads(m.center.geojson))
             return {
@@ -412,16 +414,16 @@
             locale = to_locale(locale)
             properties["locale"] = locale
             context["locale"] = locale
         user = self.request.user
         if not user.is_anonymous:
             properties["user"] = {
                 "id": user.pk,
-                "name": user.get_username(),
-                "url": reverse(settings.USER_MAPS_URL, args=(user.get_username(),)),
+                "name": str(user),
+                "url": user.get_url(),
             }
         map_settings = self.get_geojson()
         if "properties" not in map_settings:
             map_settings["properties"] = {}
         map_settings["properties"].update(properties)
         map_settings["properties"]["datalayers"] = self.get_datalayers()
         context["map_settings"] = json.dumps(map_settings, indent=settings.DEBUG)
@@ -459,24 +461,19 @@
     def get_permissions(self):
         permissions = {}
         permissions["edit_status"] = self.object.edit_status
         permissions["share_status"] = self.object.share_status
         if self.object.owner:
             permissions["owner"] = {
                 "id": self.object.owner.pk,
-                "name": self.object.owner.get_username(),
-                "url": reverse(
-                    settings.USER_MAPS_URL, args=(self.object.owner.get_username(),)
-                ),
+                "name": str(self.object.owner),
+                "url": self.object.owner.get_url(),
             }
             permissions["editors"] = [
-                {
-                    "id": editor.pk,
-                    "name": editor.get_username(),
-                }
+                {"id": editor.pk, "name": str(editor)}
                 for editor in self.object.editors.all()
             ]
         if not self.object.owner and self.object.is_anonymous_owner(self.request):
             permissions["anonymous_edit_url"] = self.object.get_anonymous_edit_url()
         return permissions
```

### Comparing `umap-project-1.3.3/umap/wsgi.py` & `umap_project-1.3.4/umap/wsgi.py`

 * *Files identical despite different names*

